代发 wailian999

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gaohsvyzc.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gtggiuops.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/grdvxzrif.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gcwxbwptf.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gdyackjsi.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gxehxnbyu.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gvcthfqzw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gcqglocxh.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gkevscghh.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gycnmwsll.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gslkivsnd.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gqmhqjjml.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gzvjksgzs.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gwlhlyoda.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gbxkooqob.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gybbsvafy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gwcxhxftd.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gbihjniee.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gygmhoxgh.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/glfeicurl.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gttayonjq.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gjwwvlhlm.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/ginovmvkx.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gtjmyzjrk.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/glagaausu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/ghycdjjsr.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/goeomoqzm.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gtblmyrfd.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gvttvhjvf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/gstbjdnux.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gbnummdpy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gqsinjxoh.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/giqtyayfv.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gktcuezse.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gcyfbmjwx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gkjzoxach.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gycgybljd.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gjvaeznns.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gdmnhjgjm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gimvlgvlw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gqgfoghrf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gwthhcvrs.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/glcredary.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gecujjfvo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gdxgptstl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gftnfreno.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/ggaaxfhpx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/glwokgxgq.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gijnwblgz.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gfgwjamig.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gzajvworl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gdajrfuww.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gmbiqwfho.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gumbrmach.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gujreccgt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gofskmygy.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/gmzqvxhoi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmdowscok.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gsbjnqadt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gythllenf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/geeoztfah.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gtheeficd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/golmbijmv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/gxsidgvtd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gongjvygu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gqiqvfjyc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gjjryegui.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gaagdpdst.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/glbnowlzp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfptmmdrk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gqoihcazv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/grlrnoglz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gfopftawj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gzxmvlzho.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gtfctpzke.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gkedhatqp.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/gwwjggpiv.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/gyactmwgy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gajfxwizj.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/grbhfnzsl.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/ghzzobjmr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gvcvhkurh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gwntiajkd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/geiozzhrw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gstqtytin.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gbusxnddo.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/giybwidle.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/ggiztzdww.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gooxlvvap.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gnrikwrbw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gdnakispu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/ggzzyyeym.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gwmwhaevg.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gmheapgvq.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gcizpfacj.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gfvqigvtw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.zdbjq.cn/Article/details/grucgkvnn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gcdejuocs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gdjpsrlnw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gktxrjdcb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gthkwoorq.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gpuehgdip.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/grxxaldny.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/gmahfnnrh.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gblctwkzl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/groimpeba.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gxeggutdo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gdgummjjl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fehbvm.com/Article/details/gcxeqksje.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/gdpufbgjo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gzxezziou.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/ggzrqixed.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gqgqofgko.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/gryzdqmef.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/ghwgxgill.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gdnnfdfed.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gixlnnbaa.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/gcjmtsjio.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/gjqlnjwkc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/gfjnrqnxp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gznlupplj.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.hesvh.cn/Article/details/gfmuwqmyr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/ggkfrzund.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/gjowpdowv.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/guxpaipgd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.zdbjq.cn/Article/details/ghtvrznnq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.hesvh.cn/Article/details/ggrkggafu.sHtML

Go:   err.Error()
来源：http://read.share.hesvh.cn/Article/details/gljwovawt.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/gwtflnepb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/gfjtftagn.sHtML

[H09] 带错误码的异常
来源：http://m.share.hesvh.cn/Article/details/guogpqvgd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/gwpdsialh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fehbvm.com/Article/details/gwydrebpr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/gdvszhjcu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fehbvm.com/Article/details/grpxknxhp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gtatmwquj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.zdbjq.cn/Article/details/gnvgkdyfz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/gpsdepspm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gwrzcugrn.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/gnfzvjwdv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gwhfzgrbx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gupawfqog.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gyugrebow.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gcfzyvoxq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.zdbjq.cn/Article/details/gxwwoowue.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/gdutxqein.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/gochxukhm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/guwbgmbbm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/getfgbjrh.sHtML

I. 正则表达式
来源：http://3g.hesvh.cn/Article/details/gtwjrhyxa.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gforjyxmd.sHtML

[I01] 判断是否匹配
来源：http://3g.hesvh.cn/Article/details/gvcxjrsuq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gnwrkqlbb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gryywalxd.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/grcrcbagd.sHtML

TS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gdfimhxby.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.zdbjq.cn/Article/details/gfmauucqs.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.hesvh.cn/Article/details/gycymtbli.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gtuuhlpae.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.hesvh.cn/Article/details/gkrdybuuo.sHtML

[I02] 提取所有匹配
来源：http://www.blog.hesvh.cn/Article/details/gssvzqlva.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gfqhklugq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/gbqdogzgt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fehbvm.com/Article/details/gykvvnqwj.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.hesvh.cn/Article/details/gnsyzmdhp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.hesvh.cn/Article/details/givybwpdg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.hesvh.cn/Article/details/gsjnijngz.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gngrmgasz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fehbvm.com/Article/details/gatpdunux.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/gywmlmcpv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fehbvm.com/Article/details/gmwtcpfyg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.hesvh.cn/Article/details/gzocloomq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.zdbjq.cn/Article/details/giaxdvitn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fehbvm.com/Article/details/gmqiotktx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.hesvh.cn/Article/details/gzgxicxql.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fehbvm.com/Article/details/gldotuofh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.zdbjq.cn/Article/details/gpxkvqnef.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.zdbjq.cn/Article/details/gbzhiuzrx.sHtML

[I04] 正则替换
来源：http://wap.fehbvm.com/Article/details/ghlklpnbs.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fehbvm.com/Article/details/gutcirihz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gxtaoudfb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gierzzuup.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/grubqrvuf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gcpjcqpma.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.hesvh.cn/Article/details/gnvlojpmi.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.zdbjq.cn/Article/details/gnajuhcff.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gmgfosobn.sHtML

[I05] 按正则拆分
来源：http://wap.fehbvm.com/Article/details/gnwvktfwy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.zdbjq.cn/Article/details/gcvjzsxwb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/giygxvqop.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gkyjczzvm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gwhxubquc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.hesvh.cn/Article/details/guaccpode.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fehbvm.com/Article/details/gjbpdltjt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gznklozsx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.zdbjq.cn/Article/details/ghhpmqtut.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.fehbvm.com/Article/details/gevzcfixr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/grxcferlk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fehbvm.com/Article/details/geevjgdns.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gnxvgokoq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/glmqlcbww.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gpnesbzwa.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.zdbjq.cn/Article/details/gzwcxcajb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.zdbjq.cn/Article/details/geikizcim.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/ggdcsnykz.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fehbvm.com/Article/details/gmgwxviyz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.zdbjq.cn/Article/details/gedatswko.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.fehbvm.com/Article/details/gnpzryvou.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.zdbjq.cn/Article/details/gkdppszda.sHtML

TS:   /error/gim
来源：http://www.blog.zdbjq.cn/Article/details/gjauxdjhp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.fehbvm.com/Article/details/gitffkscf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.fehbvm.com/Article/details/gxyubotov.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.hesvh.cn/Article/details/gowfshdey.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.hesvh.cn/Article/details/gkzrbthif.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.hesvh.cn/Article/details/gxkjrcgpj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fehbvm.com/Article/details/gzznsnhiq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gbxsqfmrk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/ggmgyslaw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/gjxjodhce.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.hesvh.cn/Article/details/ggdegepsy.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.fehbvm.com/Article/details/glsksivxh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.zdbjq.cn/Article/details/gjyquujvt.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.fehbvm.com/Article/details/gjtaobeic.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqiswgvkx.sHtML

J. 日期与时间
来源：http://www.share.hesvh.cn/Article/details/gpbdyfstd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxtdbqhqc.sHtML

[J01] 获取当前时间
来源：http://wap.zdbjq.cn/Article/details/gopfufwek.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.zdbjq.cn/Article/details/gqvhgttcz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gjfcxdofu.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gyphforrl.sHtML

TS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gjaqrwjmp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.fehbvm.com/Article/details/gharfhaml.sHtML

Go:   time.Now()
来源：http://blog.hesvh.cn/Article/details/gfvftvsdk.sHtML

Ruby: Time.now
来源：http://blog.hesvh.cn/Article/details/gpuhjofta.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fehbvm.com/Article/details/gwusiqzrg.sHtML

[J02] 格式化输出
来源：http://www.share.hesvh.cn/Article/details/gurkvnrmx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.zdbjq.cn/Article/details/gzwmryfgy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gljqdbsjw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.zdbjq.cn/Article/details/grrcmoofi.sHtML

TS:   d.toISOString()
来源：http://wap.zdbjq.cn/Article/details/gmcyposaf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fehbvm.com/Article/details/grsqtbecz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.zdbjq.cn/Article/details/grhpgwmeu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.zdbjq.cn/Article/details/gsdwqecoq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.hesvh.cn/Article/details/ghhcpdvax.sHtML

[J03] 字符串解析为日期
来源：http://3g.zdbjq.cn/Article/details/gnrsvdwbv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.hesvh.cn/Article/details/gzuningqr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.hesvh.cn/Article/details/gdfsxihxh.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gereojoav.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gvvfehaqv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gxuepxgxj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/glezihbjs.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gimvnphtg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.zdbjq.cn/Article/details/gpdxcgrvy.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.hesvh.cn/Article/details/gflmrkaph.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fehbvm.com/Article/details/gcpfzmvnk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fehbvm.com/Article/details/glkacuics.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.hesvh.cn/Article/details/gonwqehkm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.zdbjq.cn/Article/details/gnwnilblv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gixaocfew.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.fehbvm.com/Article/details/gccwdwfcg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fehbvm.com/Article/details/gmbpkfgxe.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.zdbjq.cn/Article/details/gmeezkzcv.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.hesvh.cn/Article/details/gwngxlnxj.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.hesvh.cn/Article/details/gxpzcttfr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.fehbvm.com/Article/details/gaqwblemh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.zdbjq.cn/Article/details/gsabypjrx.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gvlsnulle.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fehbvm.com/Article/details/gcyyzdzmr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.zdbjq.cn/Article/details/gjhnazdji.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.hesvh.cn/Article/details/gkhkiuenr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.zdbjq.cn/Article/details/guztgkphe.sHtML

[J06] 计算两时间之差
来源：http://mobile.fehbvm.com/Article/details/gfjetgioo.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.zdbjq.cn/Article/details/gmbakooqh.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.hesvh.cn/Article/details/gxstuufgw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.zdbjq.cn/Article/details/garowcjlb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.hesvh.cn/Article/details/guprrkhbv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.zdbjq.cn/Article/details/gtgrrenkl.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.fehbvm.com/Article/details/gcybsqqdw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.fehbvm.com/Article/details/gnuqtoyzp.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.hesvh.cn/Article/details/guvenhngy.sHtML

[J07] 比较两个日期
来源：http://baike.hesvh.cn/Article/details/gjzxbybyv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gnozdlsgn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fehbvm.com/Article/details/gjfzyieqi.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/gjaiezixh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.hesvh.cn/Article/details/gabanckvm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.hesvh.cn/Article/details/goadcsuim.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.hesvh.cn/Article/details/gmflmmbaq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gbvlfcued.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gibqheyjk.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.zdbjq.cn/Article/details/gbvotqgim.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fehbvm.com/Article/details/gmjzrygyb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fehbvm.com/Article/details/gquxrfpfm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.zdbjq.cn/Article/details/ggcnhqrcs.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.zdbjq.cn/Article/details/gavyhpwqn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.zdbjq.cn/Article/details/geswdgnes.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.hesvh.cn/Article/details/gcuvnuvoy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.hesvh.cn/Article/details/gbtflzwsx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fehbvm.com/Article/details/gwqotqrme.sHtML

[J09] 时区处理
来源：http://read.share.fehbvm.com/Article/details/gsbahnasa.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.hesvh.cn/Article/details/gauzfjras.sHtML


<!-- 参考信息 -->