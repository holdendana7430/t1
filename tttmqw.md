代发 wailian999

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2tmldxkpp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2titahffh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ylniwvfd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wfgrkobv.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2vpkcphdy.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2qfjzdrxz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2hbsoxckg.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dfizrcuh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hxrlwdmx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2clsrtkqb.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nqeeonom.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqbnovyj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cibmluyl.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jizcvkqp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2uhfrpxah.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2uithgjci.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2orpzlfhx.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ccipmpjd.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hoypfdvi.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2teklhmds.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2osozzpfb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2yhwcmvso.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2shoxaohw.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2kcobxjbp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2jejxjkzy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2hzgjzwjb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2rhpfnibt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2bqkofpif.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2zctkeahb.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2krvzumap.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2unnrtnrm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2hjgwfslw.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2yabzbqaq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2loamxkgb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2eezxdhws.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2crfmhknr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2qcayskfn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2bjgftgbm.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2srupauwb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2luxwzrxp.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2qmcixfuj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mfaxyuou.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2dudcjzhg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ffuilvuh.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2modyqvgq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kowhggax.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pdpdcxyr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2ygotbkqh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2vomkzrln.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2qctwxwnt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ekbpxhqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mmqesjyd.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2aflnoyxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xcurnrqs.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2csjblywv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2mnmksyqh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2twzrbjeb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zuztvxxc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vttehajb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2zpvkqirs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2jmdaapuw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2pbkvqbsa.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2edpldvlv.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2dykvlvir.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2fyjoftdc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zuxzdvdn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rcxlvhpa.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jmqezklg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2drmatinr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2tarwuzwu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2qhhvocnp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hvauwtgg.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2pjixbrht.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2vrxmivjo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2esqkxhxw.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rymxzvwb.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aranaeyn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2njynhzdr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2zkfsbafw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2cmaftbns.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mznbwxji.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2zuorqkvo.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mswbddmh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2lntzvrhh.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2wurfawan.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2faxpfqoz.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2zuvzbrhn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ifeumtqy.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2cwuafbrx.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2qrrmmftr.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2qgdflhnu.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2jvorhnos.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2tteisbto.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2zgabecwc.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ptzgkcer.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2svawsrwx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2wlmavnuc.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ufnhautg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2joxbuonu.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2tqwjdmwg.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2qhqcqfyy.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2llkpkrre.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xrjcajtf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2twtzbxgx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2mtdrukpk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2fujmbxex.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2opihjhlt.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gwyqlyqx.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ynjhyvcm.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2gneenuhi.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bmpdhjmc.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ffihhvpz.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mmzxenob.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2cuozswyu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2hgrqvnce.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2qhaptvmv.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ydohzrvt.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2rrkntdbo.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2lqkwnxdu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2wtbrudvr.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2zzbdhaez.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2dubhoivy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2tgdmlzbb.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2jfzqijtr.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ujbygnxv.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2zffozbmr.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2rxkchfyp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2azrrlpan.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2dpmhvkty.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2wyfyhlqg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2hgvzqlza.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojetfzkh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2efpxasvx.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2hqmircyi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2pzuyzmiz.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2gmxvjubt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2fqsxslze.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2odxmovsd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2gthuosxv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2meiitajt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ofqgbuiu.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2dpfbwzwi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2aomyuxuc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vfmsrhpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vcmtixrk.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2hegkoguo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ithyvwjn.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2omkupnvp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2weocbzbl.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2grfppxcg.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cnjizebr.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2jaubrhzr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2rzmoktyw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ueoehdtm.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mglicqbx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2kclhieqh.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lkscgeoq.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2cyypmmue.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2czysveaf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2surdycei.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2wfkdylgn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2redmchmx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2fwmfiryi.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dlrywdnl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zbmevivk.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2vobxpnbx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ykcnjlwa.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ayjfutgz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2yrgfjvhb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2ggxcdegp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2sqfcjwgs.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2idpoyhwc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2btholtrs.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2hvfngdfb.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2cqutvrdz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xtoicikr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2pmxftmek.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2rcuqluhq.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2eomubokq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2iycvxbrw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2tesskqxm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uvxzozng.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2qjpazhdc.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gmxlqrby.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ldluismd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qjxelrga.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2aggpxufp.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ciyvnody.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ainzxisw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2chfjcbqn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2xkonfvmr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2pdwnvljk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2qqbpocva.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2vcwsrvvd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2qyvxioyc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2hwvnnqiw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2yusuyajy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2iicgbpwu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2tjxqquej.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2ubqoyckw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2fphcrapp.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2yprpbnir.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2ccsuhxrb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ybfbylkn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2odxgjtve.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2iziupvuz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2klwhqaza.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2nxvzthzg.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2lbdxujrj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2sfowqaoa.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lgtweefj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2xoxglxqw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2qcyhlqdo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2cjfrmggs.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2menyuuso.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2cecyrgsz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2bhovfvet.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2mwwbtasp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2wxrhxpji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2trjqlatr.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2pqniwqtd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wfnguwkn.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2lmccplqt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2ntjvywuz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2mlijjdsr.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2hradhrcn.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2gxhaellh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2kytwrmib.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2ykzdvujp.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2hsulocpl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2daenugno.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2rmpkpfpi.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2zqkmmoka.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2zkzbcyab.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2pivemwvq.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2itodcjit.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2ixbuvidh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2utfwlkby.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2fwojrgze.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2owqqzggl.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2hnlwqknj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2qfbmarjy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2kohftufu.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pvuaenwn.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2aqyidbva.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2tkppuwok.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kikndplg.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2yykddjtl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ebtqisvv.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2neqcmrth.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2djtedees.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2qrkngmxv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2gefqccpy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2cvqjkmsx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2hdeersdf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2qboynrnx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2wtwqqsvn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2jrsreuei.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2mwdittim.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2rywkyiqj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2uckbzeln.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2mnxpgrys.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2gevzftkw.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2lrufpikk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2afflgfeg.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2vtghidde.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2pvvarcuh.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2wawtamtg.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2mrbuedcu.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2cnlcbxev.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2nidzitli.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2vfodwdst.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2rlbeogms.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2ovbgewch.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2cogapdpj.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2glotozwv.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2jbqlcpio.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2bsxwpzeb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2lzupcrkl.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2bylgxmga.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2afrpirtw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2wqojifny.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2vzjvzpld.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2agczxvrs.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2apiefypr.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2xkedpkfy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2wynlrkws.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2jerdepgc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2owjouhur.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2umfrfuyj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2hnkkzmsf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2npininfw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2cqthvgsj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2whmoskak.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2hgmkxmpe.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2ctlenrwu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2xvsglndg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2cukqeuih.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2mhtujhfh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2avhfffoc.html


<!-- 参考信息 -->