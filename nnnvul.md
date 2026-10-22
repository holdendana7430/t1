代发 wailian999

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2vcelfpwg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2acujsmcj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2pryjgwmc.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2zqxwoeip.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2huhovyms.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2huyfmise.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2iuvxwixf.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2wqqgepht.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2trdltzwr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2hnpxfxyv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2upylxvir.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tmnfccxs.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2qcxdbolo.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2pcnyuswr.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2dustzvmm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebjyreou.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2stafzlfc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2npbogpvx.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqziaigo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ulqylera.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2okkogcoz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ozkpzprj.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vvjwiino.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zuwfphzv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2prcgxntl.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgmftsaf.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vruqoyjm.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozkimhxp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2icrqffgb.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2puginnfm.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2xxaakkcu.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2pkorfots.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2kbifdkbi.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hshrrvhq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tdaadwwy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2stglodbg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tpujtqcr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ostxfnoi.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2dfqxfush.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2mzbtxeqk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2uzdxitnd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ioyrsgmp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2qyofpgom.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2boiqoeej.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2hefcmkyn.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2dwedgrka.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2glemhaah.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2oetsjhyl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2kheidlue.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lkftfacn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2hbkzdbas.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmjktkvi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2uqeegsho.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ywhqznrz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2ihqcxzpa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2chkmjybx.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2selxjgjq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dpdjwvxf.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2lopvxtyg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2yprtuonk.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2regibegn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2fhabeemg.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wsxquogi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2xbvzkxoe.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2tyqadcwj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ldpegjff.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2kxeggrsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lrqxhvko.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2tfiicjic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cpwzuvvi.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2vfwycqkh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ogspjnve.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rusqjyng.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vehzjpln.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2khcyqbps.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmdmcqmc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2kaxnspnu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2uemjmkjv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ukwimuuq.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2vlzpzyix.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2wlrinezw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fkestlvy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jtzoadfn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bkanlnhe.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fhlkjrxy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2fhcriurx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2yzasnmnj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2apkrujmr.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2vonevjar.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2aosehfes.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2arlzvlfh.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ncwinzcj.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ssdxvhgf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2urfsktns.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2nnyyorlg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2gxotghai.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cwxhmgcd.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2iivugdtw.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ncmlbizk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ioaihced.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2hbyjekvo.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyrusycy.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rkbcpfmh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2aqlonmjj.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2nnlacyxe.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2iniyzenx.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2eawysurk.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2jjubgvpd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2bcsgtroq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jlzhhkrh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2iaujroib.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2prviyaod.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2qcxfztef.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2fiyjznhr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2cfhqplnn.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2sityhvbd.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2xxauwnic.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2cjgkfrev.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2nwbjxbqg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ehoeeien.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2mncirzlu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2dkrphluv.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2kuwmkcwu.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2qnqweojw.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ebnadayq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2fslhcpoc.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xhrrolfu.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ftexsfxm.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2esxdoyhl.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2vcrxsiil.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2hlgocylc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2xmkrkllk.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ooprxiss.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2pgqutult.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2fpgapwsq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2qqglwbcw.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2nqntdovv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2mfpcblul.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2daxxvnst.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2gxrmhcgi.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2qwqxxfww.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2jvmjeadg.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ougsqivj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2croehafi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2xigozqcl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2xxjmqtje.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2ftisrovm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2ggllfftf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2xqlpmhim.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2llqwwwwh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2crntebyi.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2kjemkeho.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2rnlnaudf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2tocyxnge.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2eacgnxfv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2wavlchez.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2mjheqtto.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2jxiswfnc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2uflqhybu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gyjotssz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2inujitcq.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2etvzpzde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kffektjt.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2wmuhzttb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ubttuxpu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qgwtcjge.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zkbidysb.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wocugpan.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2uymvjftp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hyaqusbi.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2pydqiugh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ppgejxxq.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2qwadukey.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2inbwrdbw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2odhcbhrr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2zfcpjyob.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2hcyuovly.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2rcbapiom.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wvpzvtxi.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2zkumjbli.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qntgknzy.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2wrbuiews.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xhhevgjv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2uauoepdo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2rkkxodis.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2sxiizfcf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2jigzyrxm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2viqpvrdz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tgknbnbe.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2zhrplcat.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2vfxpzmsc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2jhhnhkqf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ghmsjafx.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2cxzhuzts.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cyvqdfft.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kvtgmsnm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2meoxypkt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jimwmllo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ebponvvg.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2ifjdjovr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2nanacgjb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fxxrvvgt.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2fywltyrj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2xdtsjtzz.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2gmnsfsje.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2bezpaabn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2nwaazsjs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ywhzecpm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2wilzphpb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2knixreqb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2jrlviheu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2jsfloloe.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2onygvadi.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2mbyvqlvh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2mvwooxaw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2mkgisfyu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2mipgasrk.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2rpmuayoe.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2kslsqwrp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2eomnxvoe.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2ixbsfqob.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2vzxqkmbr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2jkjwxodg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2sgvgicte.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2jgmygcib.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2dwbrqccf.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2cpkxbcui.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2omsrmmaf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2sgccjrim.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2lcpdacar.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2xlnjptiq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2lytgqmea.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2snvjbalb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2oruuhepf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2mtjrhgpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ffhpolqz.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2jlsjbysw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmjoxdkk.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2jnkiliys.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2mxejajtl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2gcmdolgh.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2hvfxglgp.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2tghawpqv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xwfqasxf.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2ujycofzs.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2gkjbkeki.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2ktcqbiuq.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2wvcktgek.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2sqbsdcba.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2cvapjkke.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2szouovua.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2ibkpjwex.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2oqnpwjoc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2azsiagje.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ybpdkfio.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2srfdmeet.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2sakhpnrx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2usizypfn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2xzsaxjlx.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2bccmkgnk.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vbogrsod.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2nxfqjtzg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2cyzmmmhl.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vhlpezek.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2dexzhcsp.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2dnvirzta.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2kdhdysid.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2curlkwfs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2rjyjaruh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2krbvjcwb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2vttdkeip.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2fpoybsnv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2pkvncpox.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2lwfthnaj.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2qtfkxvwq.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2ppvyixic.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2hdmictdm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2commyywn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2nuxjzzjd.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2dzvzyzdx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2gdfnlwui.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2ccnqtisn.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2ssljehng.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2oqimiepc.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2hjwansis.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2ipcwtvkl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2hfsjdteb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2voxfjbug.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2nvqsphnt.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2kjwnoask.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2fqccpeuh.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2dfrgbzqu.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2mszmufyb.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2dzajydzi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2xbjfiwvz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2byrwisjq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2venqiegq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2crreqyqr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2nlvcovrp.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2zqfuuwce.html


<!-- 参考信息 -->