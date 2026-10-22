代发 wailian999

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2xonesdub.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlhjcuhu.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bqboccpd.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2tnmywupy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2opuoktaj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ajudjkek.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjkaxpbh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vxrelwll.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2adkedddu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2plwsnemx.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2hyrmovzx.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2fyobudgf.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2nafkawbg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lkgkvmvb.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2utozqylf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rcespdft.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hxrandku.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2rhppuwzu.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2llnlzeto.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ixpmipgh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2nmnksklp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2marbuslb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2rmhuctsw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2lcxzcgue.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2rnusiwoj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2inzbytji.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2rebbiiog.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2enjbetmm.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ayxdrrzh.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2onwgaibj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ybywahun.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkybvhrf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2qpobyjpr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gxpkbuqc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2sfhuekrh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2gqmiclwa.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2igryeoca.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qosgzniy.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2skikvdxy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2rgigkaie.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2nyocokif.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wdelpwwr.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jwhsqnjb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2sbrmlyqi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2nnveajxi.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2asgdktin.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ldjaibnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ntkcjihr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2lplgncmn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2utsmguns.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2diwuqxnp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2lgredcjr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2ravbqrhj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ftxhdbvg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2okvojump.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2stwpawlw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2mqolhqge.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2nkqwnseb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2shusnlvw.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2syyvvnkw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2maegrjup.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xcztcuyx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wvjxekaz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2beunrzuk.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2drrlxmzh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2rsnjcruv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2azsxbcpu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ebgrkcuv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2sttbgvks.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2cobearrv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2eupcuuio.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ihylvzfs.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xmyeqnpr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bhcloyst.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2uiwigrwx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ynpwuogy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wlhpzqco.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2sxmsomtv.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2mnfwylhx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2cgporads.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2eemjqwdl.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2mtfcqfsu.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ygofpduo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2xdvsrxri.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2rghpgcut.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2pqgykkve.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2uocmeluq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2lypyafid.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2utvpcixg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2votpgeny.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lipnaenk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2frkvqjxw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ykrfieio.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2msfnbpwk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwsdopyz.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2vpqayoqn.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2litmnory.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2dokneenm.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2jxvquzpz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2srwvnodg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2guddippo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ybpimnic.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2odqctelt.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2pgykgeej.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2somlcfch.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ohuoumxy.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hxzppvyb.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ngxxqxte.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2etpefquh.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2ayyjckoh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2omdjheii.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2wtemqaep.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rcmehyla.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2moqwujud.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2gyqdnaka.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2lluokkid.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2jitmepce.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2oatqzvby.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2gagzmfki.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2tdunqzxf.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2cafswdym.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2ogcfcrlf.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2qjlnpqwe.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2ijrizdwd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2svinszma.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2hmvzuyon.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2jqmigfyj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2mirvfwny.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2xuvnjkbu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2ajxjjrvs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2gubfvkrz.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2czsbzwxn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2ixvytkzy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2fynorazf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2baonwcdy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2vbswyhiy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2dubffino.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2mhwbpzox.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2hooiioxa.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tzehuivh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ywxendch.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ikfxbogq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivcqjlsn.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kufcfmhi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fdhnvvig.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vpornsly.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uuhhfqgn.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dbroxmgd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2bybsvvrb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2mlthhvkb.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qhisqghs.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2yywyxmvz.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dvacpbru.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2flrjslta.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2yhfsrera.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2fsbwykza.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ojpvztko.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2mtiobwji.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2uzboayea.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2gfvgowuu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2onedvzzu.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2fexugqkx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sqpujbwp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2djmntkyl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ffvyivlb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2viimlocs.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2awziuaji.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2xwoesgoi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2krebksgz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2veitjpbp.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2kzbwlkga.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2iwtzoady.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ctvtmjpt.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wvhqpeui.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2yzcrmtdq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gopsuuvx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ugrojxdh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2boeldgnk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2adpbhfef.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2thinajeb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2sylcqcyj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2aleqrbwr.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2mpcjrefm.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2eyzxmcya.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2flaftvjd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2tvctgcdo.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zcpbzpfb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2mktpjkxt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2qimwypuq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2wdykzjrp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2ksqlaeyi.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ekslhhav.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ryzlejyt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2fylpqlwi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2gpwwgapo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2ymcucrkl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2mqxogarz.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2fpsjyqep.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2whlxfbyx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2qhtagdse.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2oasdclga.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2qlhcmfbp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2qrimgujn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2txlfhjra.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2wzbrexyp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2eayghdvb.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ymancjkz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2syknnzln.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2wezbtcgj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2fndkugqy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2vhcztklj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2pavaeoai.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2pixozmdg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2fywhcgqx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2uwfkrird.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qfjnkqos.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2ndnxpfjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fybbfedy.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2iivdeqzz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2izndexfb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ogeamdze.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2jnbzvscm.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2wryxaxyw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2lyudtusa.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2wbdhixdp.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2gakiqjjs.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2obwydwck.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2lkmzxxxe.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2oynsxjiq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2flyiselj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2tokmawvt.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2bzyahglx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2ygohxdpx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2diuqczhl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2gsegsyzy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2zoxfebcg.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2lkiarsfv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2rhmgdytw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2xhyhitmg.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vkmgvyoi.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2heopxgvq.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gchbpuiq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2iofomogb.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2lcgyabhj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2tnkfikin.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2xgbwrpmw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2nmutcdzc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2toywlqgm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2mnmukbhj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2baexkpaj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2cnxfxeoz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dfnfvohh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2aptuxzje.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2mtenhplz.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2moozjxem.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2cdajgdyh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2ldyjcwnr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2scxhvyyr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2mthsvtmb.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2wojazhut.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zjyxsweq.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2oaryqlqk.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2hxnuhobi.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2nocwburv.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2pymkxven.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2whmrnjqm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2khxdyocv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2wwecxffy.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2trnwxzch.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2sacuknmu.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2yantiwpr.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2fjbzfmly.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2cpkuabgl.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2unjcnufq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2vooztsfd.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2zsqvrtkc.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2qlzvzpzu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ttpvymqd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2nlteeyef.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2itevpzsr.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ohglyjpb.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2ahawfqtf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2ssenskou.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2wgneqrzv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2nxlijpqj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2qahwpkyf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2vmxqrowb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2oqkckzdr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2pijjcfoz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2zbrxxtgr.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2erutbzjm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2roxchdfg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2rlouxfme.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2jiizabdo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2iqqjeflb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2lcoehbxw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2jttmarbj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2pvzgeixy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2kpouoxyz.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2jphkjgqp.html


<!-- 参考信息 -->