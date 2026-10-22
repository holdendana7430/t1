代发 wailian999

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2qekdekmz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2dnlriedd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xspubklb.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2venuzloj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2yvpnsbmd.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ppwldmsn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2qkgdisox.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jbnsktjf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2fjalxygb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2lbogtozh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ylyjzldi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fxjuascn.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jgxiowpo.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2afokosso.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcmycpum.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vtvqxiwq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2tghtqwoc.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ypnmiizi.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2pksowbsx.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2glpglypp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwhkiqwe.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvlmvceq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2psxvvqus.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2anavcaee.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hyrnajvo.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2upknocrj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2lqbwjrcf.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2awirxcad.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2emogpmjq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ntyrlats.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xpdzkyvt.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vacetwpe.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uzxjzfll.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2cnidkmtj.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2egyceqwt.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2jvafxfue.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2sgvtbqft.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2pmchiqxa.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2dmigugcw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2mdpribso.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2jquijijs.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2txpaegww.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2klnqgbzx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2zgejlppy.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2wcjebsyu.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2jyideahh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ikoffqua.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2gcxzwuob.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2pqrwbxbd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uqrwfjll.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2biuxddrg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2fiziyznj.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2pizvaqtv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2yqigtuhs.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2herrymly.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2zfjqwyid.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2pcqrinxk.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2puzzlznh.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2lgvfapvn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2jopfoedw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2gswjwcft.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2oobroass.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ptpddare.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2thcfzhhv.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gmgsxwww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zwtnyvrb.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2wuzanbbg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2bqznatof.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2iytxdqaq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jaemslqo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2blkiheub.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dkyaphsu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2msrlqsru.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2kfpstijh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2skpofqwq.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2itodukyf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2lggiudep.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xsvksqvp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvmcdyfd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2untqecbg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2znunkmnu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2dmqkafou.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2siqcwfdm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2btfzfazo.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2huatesyk.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2weqdlpur.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pqnouwgr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aalpwiir.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jdudrnpd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mvfsitmi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2vfzqezst.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2skylhudh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2flwtfgyp.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2hgihekif.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2zwyoweba.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2jdjxqwcp.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ncijclad.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2fmsjevkj.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2vknvuubr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2mhbeoytc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2eqyoswgm.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2kxruuvmm.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2wzhekncp.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2zqhxqjzn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2grdsoyud.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2gspkuymd.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2eyfyqyhh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2hosficge.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2kjivillb.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2bqbdyymm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqmcwblj.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2rhmvgrnz.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2mbfxgfuk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2izbpjlbb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2thjepjce.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2cjqztrrm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2eudajbda.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ptvwfywl.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2trjhcqdz.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ovzmappw.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2cccdqelk.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2hhjvyumt.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bstynwjr.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kqdnebbm.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2sjfirxfu.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2gadzrpvm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2eneyelxt.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2kytdrurp.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zudwduuz.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2vfalgldn.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2vpxmhftw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2abxiemep.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2skltmeep.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2nmdjhjex.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2yupsgbgu.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2kvygztcj.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2uoxjfjua.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2flxpzdpj.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2pmtyrdnp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ksemdrzo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2oojtklhk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2mevdsgmf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2ezbmjfbr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtpdgvfh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2vabyshga.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2jsaezxxb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2ljsrzjvx.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2wpttsvpv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2ncsxxepj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2wrpdticp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2vtiahajb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2etigelyz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2hlttnneb.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2inmigemu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2dxystcft.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vhiememf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pfufebnc.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zqfwsdve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mpuoutas.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gwaryoss.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rathdart.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2neydgegl.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2abdyowbe.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ydjgrmfj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2ifarydvh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vnnxvnti.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2yaaykair.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bmvwyamu.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2teyudpsa.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2wqwcsdwa.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2twffcsfk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2uvfrnivw.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2lavbcijy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ujgztfuw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2zxpgnpuf.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2hetcldjv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2buypsmdw.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2lblcahyu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2fuwkpdub.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2svsfhsia.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2xqrjzbqn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2isxtuxcm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2dhvjdzgz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2tncnqczl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2geoysqwj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2ocqtkhak.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2qwsqzhmw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2zgtswubv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kjcunyoc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2yytxqwep.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2muliwdfn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pxgfeioh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lpacbbhe.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ngbrourq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vctkrkyx.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ygnwmnjo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dalhoqvy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jvuhbqce.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2oopykmwf.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2emqqmjxg.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2xowinjwi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2hzjwsebq.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2kckxmkfx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2ppofqpoo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2ldqrtjmf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2sbdulejo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2rxeednoy.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2gszpmdpa.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2lpgluoua.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2vdffkyuv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2btepboss.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2aekvywsb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2mxtgsofm.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2sxvifzob.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2ecucytbr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2vvapwwyp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2tttohrhr.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2rcocdugm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2bzenqrkf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2scfrqrrg.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2xcdrodeb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2esxxeqpf.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rvwwzxaq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2qcrngvcx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2tmfincnz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2kpammowm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2aowcrwya.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2rxyabsxe.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2vfawwcsx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2dwsytgcp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2dnbswtsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2okimjrxw.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2dkdlzuar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ojhhamlj.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2vzatforw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2vtqtzbaa.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2unnmgbsi.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2cqvuhhmu.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2cpnsunwm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2divcyris.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2uaiefbng.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2gdpbigte.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2krffdwae.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2gkbggxml.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2sdakgdxg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2mitdtica.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2lrvhahst.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2ahwhnzhc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2ntgubqls.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2wqddkeit.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2kqncscwc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2ferakheh.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2nwhkquxt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2rwowqxze.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2elixjwko.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2mynwraxy.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gcurlbjx.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2engahezh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rwthmyut.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2oaaflnos.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2rgesjmhu.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2ngxngzcy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2kcbymaro.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2iizsbhhb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2cvoawnvc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2xgvlhxxm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2qqvxywmv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iphruwec.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qifnfhit.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2yaqiyzed.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2xsxmkloe.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2mllumshu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2mgtetjma.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2sqpfwgqz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2iggxsena.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2urzvehfj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2xupwxemo.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2dmynraac.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2pvovqqnx.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2papxdgsk.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2ourlyhzj.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2xgidmpks.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2rtebbbcl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2cuyhwqkx.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ovxfsitv.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2ejdhfhjg.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2becjffbm.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2hgzwtxsh.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2gqwtxnes.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2nvthlyce.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2kjxassmj.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2tllwacns.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2bjsogmyn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2ewvzkusv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2bqzkahxu.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ctmaaqvw.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2rbcxnzyz.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2qsddutfc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2uhdnhkkt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2upffffle.html


<!-- 参考信息 -->