代发 wailian999

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3tzeyxxse.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3bhvxwtcp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3uwfzdlle.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hteoawfu.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qxpvsrix.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yaedhbls.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgdliejo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kazdrekh.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ilxlsybg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3cebqioke.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ifqjtxee.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3nbavxgac.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnmqefzm.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xgzxsnah.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhofvepm.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdiuewlu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hlddbwrl.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jvdklytz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3lqznlned.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3inbsrzkg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3nteyrwqj.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3igrrrpwf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yilojsmu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3etjflsuz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rangimuj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3vjfjbyrp.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3jzzgkiip.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3pjxckjqu.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3owbsurbt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3gtjbqrir.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3utwwftgn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3luxdgvoa.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3dogptksp.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3zkaccnwh.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3qouprocz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3brbhyxtw.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3gmsllmtu.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3fpveutbn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3kghwkcgm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3lyqfkgdc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3lkimhpep.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3edcrsbyg.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3retfmtxo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3nuzappog.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ntnugzbj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ovcmomnr.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3zdiwixma.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3iiwvwwfi.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3kspajdim.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wryzzsvj.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fodbagnh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3lplrclbi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3bxtxosgw.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3bibvgzga.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3tvizoypq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fzqeqlcu.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3lbzrgais.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ahkpxtid.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3nlvwkqem.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3mnwdaexv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3xcupgxvd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ajmcefck.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hhkxtxha.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3mgpqgukv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3tlxaexuw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3sawdixcp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3hipscqar.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3iyygjueo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3xxnmpveh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xkpqnjtt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zshtaclx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xddlkbex.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cfirggwb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3mrqfymdi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3slcvdkru.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxiomhfe.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3qlzejioo.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3gizwjgcz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nsszbftz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ntihzhxh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lssdujiv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rkaeczyd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3bmzmdbmd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3episbwih.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dmxsfkot.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3gjvyjfwx.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3mvxdncvr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3wqjurcas.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3unjfvzow.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3twnvddty.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3crbnduxf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3vieokghr.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3vmwyicfe.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3gbcbspcn.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3efkpakyc.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3aaxkxpey.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3gvnbyfhn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3hhxwistq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ebnxfqhq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3rzgeouox.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3sqlardqv.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ctzyrtwb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dlabynnp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3nujwascd.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3xmkueihd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3nkpipnoz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3livsszkv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3scbgktrx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3noarshtn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3pjtnkcbc.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3sykpqmbr.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xlxpdimr.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3rfpdfyxf.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3keubycit.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vsdshmui.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zphnksnc.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3raisudst.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3fymgckab.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3cymeipgu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3kaqmpawu.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bpabypja.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3srohffyq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3fodpouhk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3fofriqnd.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3btilmvyi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3sipdmdzs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3qrkmklcr.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3ouzpcxod.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3furrblmd.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3vjuxhoub.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3rbortxjs.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3falpnyzo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3xbckgrhg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3ysjmjmbw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3cqnbvixk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxaoqrsl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3vmeuoagj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3kxsiqtkm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3rtvgchjw.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3ztcrddsj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3kgibrdcr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3laxslnza.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3tywvnawu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3gthkhqps.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3qqvussdx.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3bfozzqqu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3myuopsnk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ljjuuzrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfraislw.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3abvrccuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mwwquzsy.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qpmzsqqp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3uptksimn.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gaywfskw.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jbzghfpk.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ifqmfrni.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3curhdvfi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hsnijgiw.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ebdjxvyy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zeinflni.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zgsxmwou.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3smzjaeqe.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3cpjedqvx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3gkvcebtx.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3uldauhrn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3obqsnvld.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wivcqhof.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3nuxuxgnn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jkmkztnp.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3pcjddcsj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3twbnyevg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3fkmjjoby.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3urithzfs.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3gjctppee.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3abqzyifx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3xnzsoggw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jvcoocxp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3xaxwedjv.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3inmwhvjo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3mjlvbbda.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kedcxxsk.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3sdcmidko.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rqnnacvn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3vzenkcmy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wyhharjw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3qnimwegs.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3iriiqdjd.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3tanvxyne.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kbhrjnzu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mnhsfglq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3xmtrggwf.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ysxfayko.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3dmbhwpno.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3mltouztx.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3mwaspshn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3viytvpgd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3ivyziebt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3griixagi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3trjkahco.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3cjfrrmsq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3nbceagmp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ydvbudos.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3hmgsoogr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3udneegmu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3omccqhfz.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3lqstuqih.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3hliplaqz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3zjbdwtdw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3zlmdvnig.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3eqwygwwc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3cevultyz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3eangpxhy.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3zmyzuivf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3dmszazpa.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vtfmpwav.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3izypxddk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3mjwhibji.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3kvnvqncx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3fmmtshea.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3nbyzpoyz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3oicixart.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3kmopfzsc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3kjqgjglt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eueeexcb.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3igcowuzp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pqozfirn.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3lysirmpj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3puoihjcj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3iakrdkog.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3nmwpqxqz.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3fgtttrrk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3wgutthau.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3ndnnoeyn.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3grwqhpvs.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3umqcaowi.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3rifviodd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3tkurwtgc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3nufbomhl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3oytwnpxb.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3eepwkfnw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3mechglcr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3gutswadt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3qlieehhd.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3guwgwbiz.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3zzxqkylv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3jipfliaq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3xywevcqk.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xkrpqllf.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3gbrowryo.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3uhteqahh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3zzaoqdwq.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ofozvdyl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3vblivvyn.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3oxifttma.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3flxpdwbv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3yictadum.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3shndiqzq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3rsojkskp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3yvrtkkiw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3kicwyamd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3gjkxwpug.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3wrxdndao.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3yrhtxpmi.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3tojpezqm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3qdfcdiof.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ckqygjsj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3tvzrotyb.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3edsispcp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qjwbxtdp.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3dbftotgx.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3aoxmucyy.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3fpzmjyde.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3qilkozrk.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3ezvepiir.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3dgzxqqad.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3ysftbovl.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3axplngvz.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3xuctgcup.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3yxgihwmd.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3adrkbmmw.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3zqbwvlvx.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3glctazow.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3zprlvffh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3oczkhsbj.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3cuvqwdqg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3xlauencc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3yobrnbux.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3cwkqkpwz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3qpjoxauh.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3smhmxidi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3zbmmcddr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3rhshgewz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3gquxxhfy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3swlutpxm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3jbfgfrnn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3tfbqjxhh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3thobsqia.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3uhdudqqm.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3micjafzt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3bzhgmuwn.html


<!-- 参考信息 -->