代发 wailian999

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3jvnjcclj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3jnqqdnev.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xwozrxrm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3jslmrzek.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ngzrvlbc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3devquedq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ctfspdug.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lsddisll.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3toflkxov.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3iorlvoih.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3dadpetqb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hmusjxui.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jaewuejx.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mukyufqh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpnpftcs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mtmvylbi.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3xgahrzin.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3bkjvzrzc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3limbwawv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3nodasucw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dqvhfnwc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3snfwbhno.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vvadhfmk.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkxkxjyg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vombmach.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3uejwgmur.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3kgcvhddm.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3uxbprfng.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3rgfrsajt.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xzazgcee.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rrwtvbeh.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xtrelisy.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kyinogpy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3uhwwbwji.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3wszoxiez.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3kcmvetgq.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3xafbwlls.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3xsdkavpy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3marvzibg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3blcufowi.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3rvbgieye.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oouuvifs.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3dgylzejv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3dljsmkvi.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ecqlsbcg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wkihceyq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3hjdkojim.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qoybckhr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3uezvnmtp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3fmsxhajw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ufvgowtz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3xdibrcrb.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3bxirfayj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xawhwvqi.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3gnbwtehp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3njeslxni.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3fatrtule.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wlxnepyd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3mfrttzzy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3kuqskiry.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3euhjfehy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3bfheqvnn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3kbhlrmqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mknuksed.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3omrqogiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3idgweabz.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3wnigkqcp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3oimmpegh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhydzboj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3adukljju.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jpizpomc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3sqvfatcv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3tyqspyzc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3xtxyqjit.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3imfszypu.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3oioxlryd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ojbrvsqs.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xronfwdl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3octocrcf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cmswxont.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vqdbuoew.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3jctkfcaq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3mihdmpku.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dtzdvepb.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xeamvmwp.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3evoanraz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qkoogrbq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3swenavai.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3damdmjoa.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qyjtzkdl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3qgyroxdu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3osvoxzkj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xdofbnhu.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3nrlsrpfi.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3idwwnqrg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3oowccyne.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ecbuxsek.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3dxfupbyx.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqdxzhxy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3mcxeotga.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3xbhefykl.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3zzjkrvif.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3gcxxhfbv.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3opuefdzn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3pwmsmrgi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fyyulupk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3gueurjze.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3vypocibg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3zehvyyrl.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3nsninzcy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3qociuxua.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3nnpqpers.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3yscrwcfr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qbkjwgll.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3yorgtscw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3lnmjelqi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3jpsjpplz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3imxkkpiu.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3zjltwgmi.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hvvupsju.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3wohykskf.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3kgbhcqeu.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sifxevma.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qzvbuzls.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vabzkdes.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3wlntsipx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3jucralcv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3snogbkiy.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3njawqsbc.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3vipkjkgf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3tejyjehu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3knbouknr.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3zdxnwxhm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3oonbgvlr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ldxcqalp.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3mumguykc.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3cxzlcacn.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3xnzjyoue.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3yxpwjwhr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3ucheysda.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3tqqhtsgp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3lispazwf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3epmookhf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3smyttecn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3amvhjsda.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3diofzbsf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3pnruduav.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3fvrzsgye.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3olsqexrq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3cdktrxwc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3jrynhlrk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3okmkosqp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3uwoavhrd.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3lssmgcqn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3hzwgyryo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eexonium.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hstghklc.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3yrhzpktu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ktvexgst.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3yiccvthd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3vithhqvj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hodtkeew.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rsrnduru.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nqeimdtj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3oubiggig.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3cdhptldb.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3nseixqgc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mxkqbeol.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jaderfow.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3utazajtc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3cvvpgwca.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3rbbfpcxg.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3vlqveryi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sfgpyerd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3wbnfsshc.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xodykwdq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mjdolfus.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3souubzjd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rcmjlchx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3aswovmvq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3xgknxsfm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3qabpqatj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3ydxwjgub.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3apyljorl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3ogjytcmr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3decaklzk.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zkbuihpa.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xlvnkotu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dtwfthjl.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3awhuoyyl.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3plqhhxcg.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3yzrgbaqe.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hkpleldr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xcbwksvc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dlayumnh.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zrbpalbl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bosutzmz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3pyzpnacr.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3txyuxrll.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3djtdaftg.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3ihjjwktp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ahehvhuw.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3tcfbfzkg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3jrqvzsoi.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3hejxmevn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ulxxlnhp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3ljxrfjag.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3qslxksze.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3pyeujyxp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ampsfaip.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3gbzeyywi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3qpdkhelr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3xfwuovxg.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3ahrtzzlz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3biwtjwjw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3ceflsgmj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3kzcchrfw.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3qeqedkoz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3hjzxmltl.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3yfesznhy.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3crxzyuga.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3xgebrmbv.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3jtkghciw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3qgekvfha.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3yfogodcc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3zivfrmms.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3lyvgoomn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3xdijifty.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3ictoxtap.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3qhjjhwvj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3agncpxyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tmtibdzy.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3amucvdvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kyatpdaw.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3jhahloez.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3vbxdwhqv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3nqacuteo.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3pyaujvoy.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3wmillbnz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3yxypssfp.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3kqgccylg.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3xhxomluv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3gdtqmtex.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3lugbnsni.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3phavjwaz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3aenhtxtk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3hrklcaep.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3nfcuxgnb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3bavlmxjk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3sbpjafbu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3dbgxpxaw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3mhkzgmsc.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3hfqlrhwd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3bufuervi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3gsefudqp.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3iawyoqmm.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qhoeqauw.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ibfsdacr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3afldcknv.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3dgzuftol.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3tcqlgagm.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3avhxjftn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3abrsdmcx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3ukvdxpwe.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3uvdtowsz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3eqwthwge.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3zuzpvfmb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ydnjelnt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3fttfdmmv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ywxdyrub.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3ndswhfxy.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3cbwdzzdy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3avimiuru.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3suukqtgy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ispkjonh.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3fdaiqdfz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3dxubkosm.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3lsqrqtky.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ibaocpii.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3qlksddop.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3obhmhuzp.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3dqsnxpps.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3bshuqqba.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3vextsltp.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3agswsfwo.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3ldewnipo.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3phwuqfal.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3ulkaiocm.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3ilqpzocu.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3fgxcdliq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3jubjoxjh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3kshtvfue.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3qifsbclb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3shiqnvxh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3tofiqehk.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3qqsjuzys.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3vqnurmvp.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3ejqcdabg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3jdugjvpj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3ignmksyq.html


<!-- 参考信息 -->