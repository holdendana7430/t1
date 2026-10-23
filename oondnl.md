代发 wailian999

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3rnhftjdr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3qtdkjcuy.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yjdjvult.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3asyvrkko.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rncaoxok.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3bncxeled.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3lmqgvqkh.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yphijrto.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3msphwdub.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3lvmzsbrj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3pkchmiim.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymsqrmmi.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3lvshckke.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3dkyoilvi.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsfwjzoq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3utirlhhi.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3rrfzzekd.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3smgfquti.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3fostnwak.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3vayslmdr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3havjrvox.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nstiawkl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zdrqswit.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tdodcjaw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vtmyanen.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3npwohano.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3crsgyecm.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3olgrzkkv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3tipffiwi.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mvprnizc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lzbzmcha.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hhxnhcxh.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kwleoqja.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3syooauhh.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3xrtfqcku.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3xocqmaaz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3zvucuqaw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3rwvyqkus.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3bjxkmdqc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3zxaohuiv.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3rlphrgkk.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yubsruyf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3fvzztjpu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3iiwuklye.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3fjpajrfw.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pjncxwat.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3qmsyraii.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3msokaaxa.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3dbmqexjc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gnmzluji.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3dzviloyr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3guufwxsp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3txeqdhry.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yiqlvdkd.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3nvvmniyd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3qetvbtfz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3yqoutxts.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ntxdnabn.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3cuxyxvkk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3fvulfslh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3vhzxmuqw.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3whyfzsyg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3xdcjnbkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kanxhunj.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ojkodsxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mhunbujq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3deboatqa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3fwctcvrk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hnwraign.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jenzagok.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ckqauopd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ucgzaxmd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3nhldweta.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ejrhuaui.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3mnawkcot.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3nfxfnqaf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3kbyvunjk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hxkraisy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nnmjswuy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvfuxiyv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3erwttvgp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3jcdugnpy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3iykqrxqc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yhyeboxw.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ghksefbk.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3vszpcijh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3urxqbpce.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vcvzyosc.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xykueeha.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3eeonoduv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3mdodrdva.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3cytnoyao.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rzdtplnq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3motlzojp.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3yfucyipm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ldysqafw.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3nnurzddo.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3yejoujbt.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3gwqptiop.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3dhjeatgn.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3rkpsprzj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3lofbmpwl.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ieukksnd.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3ryqqhzlm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3uawjihdy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3apbolthz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rzslxmkn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3otpzdyxw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3gjchpdct.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ulhpaqyl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3aixltvcm.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3qmamyjiw.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3jnjuqtqt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3pclbrxml.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xvdomvhf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ivlqhoxx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3ikgxpicm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3pazpvikd.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3bspebcxj.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3jcewixki.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3knfvcxkq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3cypxqsxs.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nhbrccee.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xjqiseqg.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tjqxtduc.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3mkycyipu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3sjrejgrs.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ybxcereb.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xkspbitq.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3conhwbss.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3vmvzxilm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3hrdumwty.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3slyftoas.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hbhuncep.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3svtroyig.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3gmvoupxl.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3casuidgx.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3mqqucqeu.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3bftlcgay.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3zsqtgpdi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ulfkstum.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3cnswuqva.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3cmzcnqgr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3mqfybhxx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3iarbtkzr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3hopdmtby.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3qkuzzvqv.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3ntmvheuh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3yptcuvel.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3unvxtvjv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3elcdgtag.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3mklqwijk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3jisqjmmh.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3fmprmqky.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3juvombzb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lrhyeuyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hmrphxwo.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3wrwduxlf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ruwuwatg.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ykppjkli.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bqzzfidp.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dwtnpyly.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bvgoawwq.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3mfkyjzdv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3uqeqqaft.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3dxwepfbr.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3qlqoerjb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rxlkzcpg.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3nidywgvv.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3kpsixamo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3kjrqrgqm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3qtjkngtf.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3opunezze.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3ydsuwjec.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3zqhldgad.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vxjaybyc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3iynqaokg.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3alogfvro.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3wblhgjzx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3qcwzffht.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3vkcdzcvb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3gbfajufa.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3wlsugdbg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3rialccii.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3jzdkxggy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3epvjelfx.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3uskrvogq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3uasgcehg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3crcmpvvg.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ymyhpgss.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3sykzafjs.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3uszptpim.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3ybvvtxrc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3uliayrdn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3tqjwaeos.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gfniiuxp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hddabbul.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ljmxrngz.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3bnhbtvxd.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3mulfuaoi.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3iplsesep.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3rspmuvat.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3rfmxvlfq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3vuelthnd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3kitsszfb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3oodqtnit.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3cnlqciiv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3tnopqreu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3qawdllov.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3dfteleiw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3igfyqirx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3esewqrgw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3npgltjcu.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3vvlxjhti.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3iuelskvg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3ktssjzth.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3jnkpkhet.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3nrsafrak.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3hbfoujja.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3fufzjdtc.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3siysfyqf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3xzyeqgvc.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3siyxhpck.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3onkghkyy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3sqqjpgiz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3sfiipqjq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3fatmbvsk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3gsgduhlv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3ydjyyygb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3iadinjwt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3pabdfkqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eofbfspv.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3lmmfnauq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rblirlai.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3yjxdhyoo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3auwgsown.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3hdiiztfg.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3oiovgwhe.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3rayxurwe.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3dlkzrxom.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3lhrcxzeq.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3ijfuvxqm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3hbiryive.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3txzzvvtw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3jcwbxuft.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3frvcvwtr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3udazcuui.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3yrzncnef.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3fxupbzxn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3wwyoqnbz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3mnguhshl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3yoimaijq.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3mqcaolly.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3dekwqvsb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3xmvmujwv.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wctxzivb.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3evqzdugh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3nwywjkjs.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3hdlzjpys.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qkrfcqmq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3zcrtvlct.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3fulmublp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3qvmfpbgg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3rkatajjp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3bgnlgcde.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3quwlzdeq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3csdtaucg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3vifgrepb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3xodomaad.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3sioupnph.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3mxzxshun.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3zybjrzwo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3pjcdtybz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3lyxkgtiu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3pulajwat.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3monmbcuy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hgiapadj.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3pvfpsvan.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3rgqxkvmb.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3cickwweo.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3clrulkoz.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3bjamuajz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3dyczydol.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3guybuyqw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3qrnzbsrm.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3lzbxcbcd.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3pwevvtea.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3fqejvhfy.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3gmvfrvpl.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3buulxazl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3rzkryrml.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3omurknuy.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3tcuoommy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3oizaaktw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3pqaqrdbo.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ghgtcuwo.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3soicjzav.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3kwsudeeq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3bdaxzmjr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3osdfnbxf.html


<!-- 参考信息 -->