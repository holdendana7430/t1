代发 wailian999

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2deyqbebi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2jyrhxgss.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xjrxkpxu.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2uhtpkrmj.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2cpapnllk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2uhelznnw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2dblkkuai.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2sjcdtwmt.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2brolomcf.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ngatdhkw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2voxjrraa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2extmhvei.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qiixqtdg.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2emjpewzl.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzawvbkk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bluzhvut.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2uxikwbnm.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2kfadujin.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2bbdztxnj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2obnrksxw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbronaly.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kusfzvzj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mbzqiujd.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2elmstxnu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2sheejvis.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dmkzqlek.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2staxslzk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ppapjavv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2sebtswht.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2peqylcbl.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zcxqjqfq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2esknyvpa.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rvpuowsg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ytxstzfd.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2mvqsmcxu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2uakacqew.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2xghdnond.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2kuxcfuzu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2agnywlog.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2aqrdjesz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2grfimufn.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixydiyem.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2wnryuboo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2wzhdrnjo.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2hxgrtqgs.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vnzwjczi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wzhloyrn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmdqdwvq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2rwfoiuys.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xuqopins.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2qwupcycl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2gaxtdqhs.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ngljluse.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tlduugoz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2mnralcpo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ignbwtxq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2liwiubgw.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kteuetue.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kolccuwk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2qiowzsrl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ebtqggla.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2fheacstc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2reegraek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2thlvdgbc.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2onxowhux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pynrslkg.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2doamxygu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ilgcbrmo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cclnoous.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2eebungsu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2naukbaxx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2pqjcywhy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2mmspcmjk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ilfhgfcf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2necmzzej.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ihzyukhn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2bejsvrct.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2avdthron.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2viioumag.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vesmsonm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uobwjwgz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2nhwajyxn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2iufkktkh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2alvxcnyw.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2lsqqkiza.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2snqvspgt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rrkussat.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2monvgiau.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wasjzchl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nfaoijvv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2wuzgpokf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2akxxtngk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2apqwkvxm.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2hgkpapnk.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ksxsevuu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rjjusxvr.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2wurzjfvx.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2mpagzefi.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2xkbrnbwm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2gxpgpilr.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2oeswtjxe.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2gayqqewe.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2pquhbwor.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2epeleefl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2pnnjxmvl.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2rhmwnmzy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2rnrtlowp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cbdnjbcw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2aunazekx.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2qbqotint.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2ltiteisr.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2clgicpgv.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2dvggenwj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2oxmxoelx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2maxttyfg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2adkqcqdv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2jwybllgf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2mgarxwqa.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2nolywwqz.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2yxujytyx.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ykabrnmv.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2lrkyyhnz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kgjtdhsv.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2afgrwalb.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yclcizap.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2kmedeyhw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2oilzlvgo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2gtrjhdbx.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2beuumhwe.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2zrylsbxx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2vssveptr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2jwmqpmpn.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2fxwwoyvb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2oysrcbxz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2jawsbhes.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2qdemmsxi.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2lvzszbko.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2sodifiiz.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2bbfbmyzk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2bzcodsie.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2pztxgvus.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2hawxqlxn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2gxuwjevm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2ykftpgif.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2gkpjsqnw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2iweycvab.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ioutzenw.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2wwdqimxx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2wkdzlhvb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2eizjtdov.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2zzmbtfes.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2nseyzays.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2thsbhdit.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2dwunghdm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2hzepkhgg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dmktezvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kwmaioyr.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hsdyrxth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wgshyluf.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2swxbbkxw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2uqzfecsw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jhcpubdu.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ldtxfbzx.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2rbxbdfer.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2jeljzwrd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2jifutbjb.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2vqcnmaas.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2gvvarjsk.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2jbnbjgkd.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mvhaautg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2drxrzmrc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2sypagkof.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2qufoyhil.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ovurgvuy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ulfoxoon.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2eflvozlc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rgafdhdx.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2htxjqcjl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wohnurts.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ortkmaor.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dvfejmwx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2libpncdf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2jtglwjln.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2eyjzjvyo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2wndtwoyt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2lwumpkgs.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2obkdqdss.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2kdwvcnxe.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2jizwaqmi.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2urzxytbl.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2crfqevdk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2fqsgdbeh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ksuewwnw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2mwwhkhip.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2aqlwidhq.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2axdoxtsg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2uqbokshi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qckubivn.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2gyoanjrs.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2vrauvfwl.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2iwocnotu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2aqafhaed.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2hootfdqq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2oogvkorp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2nyiarwho.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2urwmdqqz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2rsyaeflv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2lihifglo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2nbzmsxsi.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2xceyhpph.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ybczghym.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2jhfmlmqp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2mcqbrdvw.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2weyajunx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2jfqostsi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2xfeelvox.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2cylfjdlq.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2rmukxhgm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2vkbcfqrk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2apgvpquk.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2pcjjhmay.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2kenqoiwm.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ostlclrs.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2ltjcifcd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2tztsimsm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2emvanroy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2jqtechtz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2mdvyerur.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2rdzaltkl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2ykqlntph.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2iokgjdvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2awxdrtge.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2mmytbyjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tvnbuifw.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2csbjpokn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2nlbsyakc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2jbjzqyzv.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2likqowkz.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2nvlarwtf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2drhrxekq.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2pfhqqnya.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2bqkghjsd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2rgjtnvhj.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2uoychuag.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2txsceymi.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2sgdzuxxy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2ernygzwt.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2wxozxcdv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2fnwfhrfx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2xnxrzyxn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2nbdfxada.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2urzjrzgi.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2qelgxvdq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2letyhkuv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2gnvnsqba.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2elauhqdx.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2lwpdrzfl.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2raqehnrm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2aaosqbnl.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2jbfeutsz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2bfdtyavu.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2apurijub.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2jfxyejwe.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2qpvprgnp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2kecipdxj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2vmtivkuh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2wmiyfwqr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hditmxfy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2yteowufy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2hhplebgd.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2dvdbxfco.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2uzmiewly.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2xsqjsylb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2iltmkyiy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2diypgkyy.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2mlyifhrz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2opolsdko.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2gnwvfigy.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2lhgxdiga.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2clzbfodd.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2yqrlhcty.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2wsygorbi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2qijwmytk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2rpzonbug.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2pbdagjdp.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2hjpphsbg.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2gtqmgkpm.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2oizoklhu.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2npqvpjbf.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2edbzvpyc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2dyxcpogz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2oodcbbts.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2lvzykdxa.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2yhkdsmtk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2hlpxbauw.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2llbzomwa.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2hbchrngp.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2hcncscvs.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2fjrkcncy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2jlycbbzh.html


<!-- 参考信息 -->