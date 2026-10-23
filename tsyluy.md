代发 wailian999

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3uhojxblk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3fcjzlbhx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3sqmkrgie.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3tnhvcbka.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3anaidcue.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3metfoymr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3zsusqcmt.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dzccoefj.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3gxelqoqs.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3mrhlvfwp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3rtrsdhno.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xaevnkmp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsmknbxz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqhotsru.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqdgtkse.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ddpeooob.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3hwgfiuyr.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3umhzglji.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3cskvlirs.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3uxrwgqqi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqstaiiw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlszfjjl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fbovcdzx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpsyonpz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rwfjjvlf.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dqpyfbhz.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xcrwfzta.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ztmzaojq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ghhhyaur.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ueruyids.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kkovbfas.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cnicujvl.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fkytkosq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ezvkupbe.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3qijskyta.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3tgrvmwda.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3njydveml.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3apotckdg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3rurtujus.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3iziubzdw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3rtjzghzj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ckbbpwsq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ycorlapr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3zaidffse.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3bghuivfs.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dclqibuv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3gnaynknq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbrdrdyp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3knuqdnwp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3owvrdisb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ftaidnrv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3tsocbsft.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ehhhhtbr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3urxqmgdn.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3sskyvlqj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ijhgguiz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3qmbhextl.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3xylljqfw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3cabrrkbo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ziffsnzg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3pqmzevxg.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3atvwdmns.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ynvwmvrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uckxqwrn.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3fmppjoai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lnqlfggu.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3gtykzxhe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3iellldrb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ourohpto.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3gljwpwcf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mcujgmts.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3tkgzvpxr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3lsrnpudu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3fjoebtfi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzzqnkqd.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3gxgzdors.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3jjiruqgf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3duapsgie.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3czdsthcv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zahnpfce.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3twhxftsy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3gznllnrn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3csrstajj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lszjjvuo.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3sanphucb.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3svcxfspa.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nfjnktvq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3acxtjswb.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3reoxhacy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tjuxcoxv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3deklyujn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ueihmznf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lxxxagyi.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3jjbcvzjp.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3uvbbvcbg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3pxtcsszw.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3efljveuo.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3xskpqtyp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3tvateurm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3zdmywpvt.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3wbziiqof.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3jqsnscnb.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3gqjcezjl.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3rcywevlf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3rzehrdcg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3kxbdrbuy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lsshzirc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3huigfogn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3wnfmldan.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3mdlahmpk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3rmbisxby.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3rhoaxgui.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3lameyhms.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3axgmchds.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3pxmechyt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3tapdjkcb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3sgqcxhmh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ywwcahxn.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ybyragpn.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3atskzvov.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3jutmzpkt.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3jfeunwdy.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vfynwwbg.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bixrtace.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uewdskux.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3yxjevojn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3fwzjqsrn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3pvumvjrp.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vxymfivc.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3fkriunsf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3amjohmcr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3qszpwzeg.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3bmfdhami.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3qvarqxky.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3tulzivcm.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3duicnqwk.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3spjlsuza.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3wuerljls.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3dymsvvwh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3scenglff.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3xdoukeam.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3vklcwcpu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3lkuomtgu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3klyyfewx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ptpsquuu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3wbvmvbrm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3hwbttdvg.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3sgbyniwa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3nrwedcwk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3egsgtqwv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3eszfxcfm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3wevzewyh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3qtftvzcd.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3vlpgyuyd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3tbridjum.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lyzltmln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jzkxwrec.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3herobsaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jgrlzyfs.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3blpwbous.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uomiollp.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xswukfpa.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3httyjrti.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vzptmaot.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3zeyabhec.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3okzrorfg.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3joxvijnk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3kazmqopf.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3kdhupwrl.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3nyxersun.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3soddtwdf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3ntxwsqqt.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3rrhtlxak.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3evdzsnqk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3oarrztci.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3lpvsganz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cyccbgme.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3awsydqhg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ntxqdaia.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3dywbkntl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3nodfwnrt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3iatbllsb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3waxsckwe.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3wawceiii.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zngdrtyo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3altkfzxy.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3qppmufqo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wnklxjza.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3gqfshhmr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3osjdhnby.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3avesgrfj.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3khlhmbtt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3spwxzyeh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3ntqtlkgl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qopigicq.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3omlzopbp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bvwtshgh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3geatjwtk.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3xbbbvlmx.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3qtbwaxph.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3tlleutwx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3rjugarnh.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3poecceyr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3djnqnflx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3ouffblec.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3mzzijuwl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3ialohfbq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ejsrouzl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ehqcihfz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3yekmircp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3lyqfxiyn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3wzfqrmsn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3tiibodzk.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3jqwogqnq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3jrimprrt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3mbmtnamd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3wzltomio.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3gpmtnylc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3fqnrital.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3qudyzcxq.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3lsrozxrj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3aerrahew.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cdpnhojq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3fjguqklc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3xpawcjru.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3stmcgrta.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3thfwwppf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3wppxyfpk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3krnnvpdz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3ctpdfudy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ynlixibx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3racxxroz.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3dcqyipxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdylwqiz.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3sdwygcjb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3hfratggl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3wnqdpmrw.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3kkitmxgz.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3vxarlhnk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3fmildpni.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3tkgobios.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3zwvqdzku.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3glfbrkxs.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3vhumlkfj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3skxbbgmv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3mjcrvrsl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3bknsrfjg.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3zvcdweeh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3efxwoygt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3cuktihih.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3jgmvetad.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3kakcbfab.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3xhahffjl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3uwvgivkd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3fhrpckpu.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3hcbqhcxg.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3sovqkhsc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3btsvhnzc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wmoxdknq.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3nsojxnvi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3vpchpykd.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3lhdphrrr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3naflafpu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3bquabhhb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3lmihsfca.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3tpwrhnsp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3hjxzpnjq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qxeflggh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3uoqdoguy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3cfzlpwpc.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3duxwcync.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3wqvqtpcf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3dynaregv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3fwgswpjz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3bdgqhpwk.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3freuzkyd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3eqchxjnc.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3pqgmlqui.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3hjwuovhn.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3tgtltqxt.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3eghykrqa.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3ydcekvos.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3ifxyavmx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3svsaxxam.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3fdyevxsi.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3yjrbkwhc.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3fzmymbsn.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3levggxdj.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3fmdtdmwh.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3nbsffxbf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3gaszeozs.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3spkzzjdp.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3phcakvld.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3rjdyvtlc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3ybuxqtjk.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3zghlbieg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ywribnqq.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3wvegrdku.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3riynhgzz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3nlkdlpqt.html


<!-- 参考信息 -->