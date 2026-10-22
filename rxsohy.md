代发 wailian999

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ovaiogcz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ziqtwbdf.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ltjwzmzt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kxatnwrn.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2otmxqxjp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgmurfhr.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nytrzvrs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2uvzqldbc.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2kcudlpsi.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2tvouohzn.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2bhlsrzdx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2lowlwbko.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2evjugxoh.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzkseijg.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vltkeonk.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zywimzet.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rsfvpjay.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2hurqbmtw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ymblbsbt.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2vrvommmw.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2bjwnotnz.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ngxmdodx.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mjuesmlr.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mjgmhpbc.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dygafvnu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2btnmqthb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2iqjddfaj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2zmbwujfe.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2qmtepwyc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2kjtktaya.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2xtpnndvw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2xqazbjyt.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2qwfmkacd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vsamhszq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2vvaoiyna.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2gudnsgcn.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2opwlmrqv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2jtrpntrm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2hceltgve.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgxlgquc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2nrmoyshq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nxnzymqm.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2uotnbgsm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2dshouxil.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2abcavpdb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2grftyjpo.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2jllfeiqe.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2rxuoqsxv.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2qnrcakit.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jesxrveb.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kmcuolll.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2udxineyo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2njrpeqps.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2hvcubqng.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ssbzdyvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxfieigq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2blxgfosc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2heivbfmn.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2inihyrxq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ynqxamii.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2advumxka.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zgvxtscl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2rnlpgzpp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2rtsyqqfv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2jxzghbnb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2qqywkwvj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2mbpifxia.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2yvaxhefp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2jitmflja.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ncboxlup.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2catvnuid.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2odtblzua.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kspenkzm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2curkdyhe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2kngypezq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdkupbdn.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2oxvefrir.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2xfmrcmia.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jadannyh.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ebitecun.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fwfgucha.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ijsorcix.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2qfsxmrit.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2xbldefnb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2osxbrdkl.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2hmnucjtw.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2gzijkajb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2vgvfwteg.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2vtvqmtul.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2olwrcahw.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2pxvgxwaq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2cxpaeapp.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2wqvzqgek.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2glkdrzvh.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ikfavmbm.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ayxmeukw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2jbjamhte.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2gnhgntgj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qzbqccbe.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2qeoqddvy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2lwpbldyx.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2cxkkjshx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sfkybinp.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2uhianwdp.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2xiwkswws.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2gblynqig.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2sjiohmbp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2tkvnlwmq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2qeltnwed.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ntpqbskz.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2drphilnn.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gdmckaqn.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2wdkckjwq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2uhjcdxzs.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jzhyfuru.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2feaxxhom.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wqxjghzx.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2czqqytqv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2dmaqbdcy.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2quspbnyb.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2adwwzqdi.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2srwojold.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2zibpibdg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2kbfizdqa.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ksxhbzbx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2oqkewfag.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2qyqtqipu.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2jkedkjlu.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2yufiqyjf.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2izqqlmcq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2qzsqjupu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2tkridolu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2pqanthtk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2zrpiadyg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2jrqhwacw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2mywaxboc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2atkufngw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2bgkwlqyx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2bgmgrarh.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2iakpkbzd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2apxmkqhv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2gbdzqvuu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2dfgsogdk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2fqroelur.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2oxumnufz.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2mhbgtymz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2xochhggn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fmwmrtjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvwdeyjh.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2jaaiousa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2laqabshw.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ipykkznh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tsamnfjm.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fkrvkblo.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xxvnsfsu.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ofuozqdl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2xsdtendt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jdhxaqih.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2inickaxv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2srmtguuz.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2prramdmq.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2xotkrzxw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2omxdbgzm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2djmwqfoa.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2yamhnphe.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dsbtwtgt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2nbnraoyy.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mameuptv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gkksenyu.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2hqolqxdz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nuayumli.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2thmqjboh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tvaqpslw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2nvquluge.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2pvmakitp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2nmvglvel.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2jznpuutm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2cxyyngzm.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2vodrpwcs.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2eilwhekl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2tzvmowvp.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2awdqhbfm.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cisfmygm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2tcvkrzpv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2tsqirvpd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2wubzqqkf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bcrdaibw.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cftjocle.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2xnbzbkxs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rdfourvq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2dbsiuodc.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2tsjgjcck.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2snbsbdeb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2vqzlfsxp.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2uubdqcya.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2qffxakuk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2oogversv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2degqvmot.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2utqlqaqb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2sbmtowcr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2bnkflhmg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2bbcbohym.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ssqomloe.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2hihkbbru.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2htiomvcr.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2ixdlmfdz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2hpymqlzo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2cqznggnw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2zvtqjory.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2gqlceupa.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2pzysawzg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2yzkummlu.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2uwidvpul.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2kpndkevw.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uiiszvno.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2jieannrh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2fziucfns.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2pymqjzce.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2jdveahnl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2bjhsgrwe.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2smawbuvt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2unabofuj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2amrppafk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pjnthrmf.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2przaztsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lpokqpbf.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2kjzyzvbh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2dksltpfv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ihjtfewl.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2dpvxldtk.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2yidkujvc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2bkrgeifh.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2wqtdmemb.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2bsjnkbiq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2shtzlhru.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2lwaphdcr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2rcnozwpl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2aqxrlnow.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2pcxilpqr.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2lzwqjzdr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2yqbkhrwm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2zwiqcvyr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2xhwrorxr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2porlkxyr.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2tekupipk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2ihbnerkf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ofzastob.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xzfwghkc.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gvtjauqf.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2idzydwbp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2nigkffxj.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2igjzpmaj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2nzoakror.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2fwwvntxj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2upwbbimx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2qvgggtop.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2vnhrbsks.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2tzowfbdq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2hyiitegy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2xzxdigrs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2dgkcbidx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rnilgjjv.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2pcsvpjlp.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2udvqrnrk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2autqokyl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2wsrhsvum.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2fwzrwpxo.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2kmzornvx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2epiyxtqz.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2jqtpjgzd.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2bdqfovnm.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2gnvrycyj.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2vlaakznp.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2wtyptkrk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2ihsnjwpp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2kolozpxb.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2wwaauyhf.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2fpjrukss.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2zccbeydr.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2kkhtqbfx.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2benhfoup.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ycmdgtal.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2xeritylm.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2cylaesrt.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2qsjimbsp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2dmtdjzvi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2uycwrkaf.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2oylaytpz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2safxdhrx.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2ievjoict.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2glxtfuzu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2zgajlllf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2sqnipmut.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2xuhdelbz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2fqnpocri.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2pvdszbvy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2nauvqyda.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2joktlslo.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2jpwcehsn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2idgjquhe.html


<!-- 参考信息 -->