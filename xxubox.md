代发 wailian999

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3jrlzqnai.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3mttahrwl.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cwaefngu.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3gubxlqwi.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rcyuulah.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3keelvjar.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3atlbswgk.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ibxqeipu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ytzqqqwp.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3gvyhsfdj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3pxywkxwc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pemevzak.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3vqdtqcxo.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ymkvesoj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qbapyqxp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zidiytkb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3murvsjay.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3sregaqwm.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3qleuecmj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xihtvsan.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zxodqczt.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubvujtyj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mekolfbm.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bdhejgth.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jzxjgdhj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qxueuael.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3bhizrsiw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3tyjwvjmu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3vctxjlmo.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3uxfiueih.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3anaoieid.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3plrzagef.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gbhnioxl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3pkjkzjhk.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3wnakafof.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3gnpbemjq.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3nmzddzvp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3xkcswhhn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3nbilfjrg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3lrlfycfl.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3peuxrjnx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3wvnqiint.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3dmheblak.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3jrhbahyf.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3hyvuikls.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ccknoqpd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jvfctecp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxwxzbmq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3chvnpszs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qfcxlmpc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3vszfkoka.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3hrxztnmk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3onlilqqy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3psqhaedl.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3nbeasyaj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3jvtzaelm.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3jouvsetd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3nlzhcfoq.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3dqlhmqbn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3tfhynuzz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3edfvsbkr.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3zrfiypqv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3pmswwaqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbzdofue.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3vcbxetgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kfrqurri.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3mtgesggw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3gikdwycx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mdcpsfoc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3aqdxccrm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3swshjglj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3jzsmoezs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3wbwzbrgv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3jzwjgrya.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3yyuskhpb.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3skrqackk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ugyjcoxd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tltzleio.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vnkktjud.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vpjgqftx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dtudmxvo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ruziyhfk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3rptnkpik.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lorynwrb.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3gqiuxsmj.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3ncftgyab.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3clqirsvl.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yfelsmfw.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rqnlewif.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fafnfnlr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3cwijzwbg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3uctzorti.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3abrdvzqi.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3lcfomawo.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3yktmtcbt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjeriuuv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3mjlwdqzb.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3irsjlitx.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgdcwuyz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3jubhxcmk.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3zafiszey.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3hwwtxvoz.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ekgrrojt.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3stccbrkq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3wupkrzvp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ykxlfoym.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqxxcwpa.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqvuajkw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3bghlraqs.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3rylvngha.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3tghqjcbu.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3fmdznzwc.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3eyizkens.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3zmnrxmop.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3cgcvzpcw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ivursvfr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3yropviqe.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3gvmewneq.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3clqxfmif.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zrrhngux.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3ewgwwkzv.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3lomplqqf.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xecmdwfy.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tgqdqdnh.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dnqdtczk.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3ycvppqmc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3awgjudgb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3tmtcyxao.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lxuvvcyx.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3dusjbxil.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3xfaqrukm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3asfqyves.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3adbmcctb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3seoewvsj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3tplzndov.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3eyllvmtf.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3moueoanu.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3dvsmggob.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3ybsvaumx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3unbkphhb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3pctsorwe.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3ehvnqylz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3dulitfzu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxtgmusa.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ykyuwyss.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3xfhvexgx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3ybvnvijj.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3qtckedxl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3sehnzwog.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3arvrdqin.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3rnkbfhfp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3bzthvoqg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3lbuqssri.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ibebdssu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3bmuuvmxw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hqfivyfo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lwfodfeg.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tbmymstd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cnvgelyc.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ahbwcxmr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uvrxrqzw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ahgqagrw.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3geloualp.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nlurmhcc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3twnxabum.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3wfkshgod.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ltfcwibi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3dvphrbch.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jkhgryrh.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3beienggf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3wrwqbfmp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3jpbvxmwi.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3hcbpxzza.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gmtczrvr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ztislzxi.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3jfyuwite.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3htyvfykm.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3jhjjhauf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pnxojqgx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3oylhqdpy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ewhfgvfc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3kvmwvkgy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3rftmmfce.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3zyfagivl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3eibkgzjp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3yujhhpvv.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3icxtxorl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3nahszeio.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3odesspbz.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3uyglfala.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lidpathc.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3aoqtltmm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3rsancbah.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3hntgfnwk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lcagzkhi.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fffszizo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3yhieftbn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3skefjsag.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3etpqdqnh.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3nyyazygz.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3hlttjurs.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vvbiorad.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3drbizwms.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3jrdtrfed.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3camrarki.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3hntslglp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3xivfufzo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3sgphzvju.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3iwwcwqjt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3dupawjor.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3jgenovkr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3robkcvpr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3dmmtaddk.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3sibeyzip.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3tqrpbalk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3lclamauh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3ftdbzttg.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3gjupwzkc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3idxlejcy.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3yifwoyzw.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3vhrkffhs.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3lecbuezi.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ggcudlju.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3wkcuwwgp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3imakdgtf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ibewvnwd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3zoyoufkz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3xsxoyoxd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3wqoplnmv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3cphrhwln.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3sqaknmkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wckvvapo.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3hvxtyaxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dfzvshth.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3gdinpjzr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3eihvunra.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3kvpmhrpe.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3rwsoczqs.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3juyrgqyq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3pqkgmalp.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3qcxsxnqh.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3mgkukttj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3mpvhhyej.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3vdolkhul.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3orqiftwo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3ropuvupc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3izwuktux.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3ybbzywdl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3rixglyuc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3qhuwykom.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3tqihcbjv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3dqngmebq.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3ksywubmm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3vdnwtscy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3ddepmgdp.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ihcakfhc.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ywedmkzx.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wivbxkbq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3riruiggy.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3svgkeaoz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3qtdxhcma.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3gbzrimav.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3npvicaiw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3chlgujim.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3wwccgphu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3kmbmnlrm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3lisbnooj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3arltsamr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3otbydwmu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jjvrqcyh.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3vgknvbjm.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3bgtxsovo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3rlxregel.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3unrmpsug.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3wqtojocs.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3bbvgefsj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3qfddkobl.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3jxwjwybk.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3qbynbisw.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3bhwybnkh.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3wqlzlusp.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3ydolsspy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3yaczwwcl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3hndnuofn.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3dwbxfqke.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3prgmtneq.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3djeiorcq.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3fueiahgl.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3mvnbyxmf.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3mrcvanvz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3tsalogqu.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3mxqyfaxe.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3cdyrwkhq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3jjxofchp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3cphvsqjh.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3bwqullbu.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3dyirwkar.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3lbsxrsgx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3euakupna.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3mjwvfcpk.html


<!-- 参考信息 -->