代发 wailian999

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ufqwhqcc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2meyiaugi.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2igfsbxha.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2slufvveg.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jjzmhuci.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2jegdegit.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2pkkrjzuq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2birjtzlw.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2gctjfvyx.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2jzxyqfeo.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xgjkruad.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ftihwotx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ckoqpfco.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2bskcnztc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kglfxhve.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fwkcknfl.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2bdnnfpyv.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfofzbkb.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ifnevnwv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zyefvghr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zelfshht.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2onefmbks.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2elerhcvc.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsewquth.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xzdydoiy.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wajrdzoq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2sirutcaj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2wbdssmys.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2iwrqwthn.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2coccglau.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ikezmyzp.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dzqaaowp.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2irparagz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ateeqnjj.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2yxatciki.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2wnznkbgu.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ltvwmijn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ixeyzytr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ymxwiktj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2dehvkvgm.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2lrsmtpxo.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jwttfmlb.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ccipfpio.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2mimrmjqa.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2nfwxeywe.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ycwwsaxq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2yflwfeng.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2tmijhgsq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2hphfcxlw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rxgvusyt.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2jydthtqg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2snyrastx.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2cdljldkt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jtpkxsmf.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2zbuvohum.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2pnvjyqpk.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2svpgyqaj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zsetvhdk.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lkwjwrjv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2jizsrqtw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2nmuponbb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2nerlrryq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2afqmfjve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ufezuvms.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2uionnlwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bzdkgybu.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2bjooygmd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2bmgcbyeh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nnisdmic.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fvupskyw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2obhvdtib.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2tbmvdcif.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ngfyunlw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2cxkwsuqc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2spjycgna.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2vjphygyu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ovuniwgf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fkmvlzsg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2epupzszh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lwksheul.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lybesxfu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2hndnyqwf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2yzlfwaiv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lmpiwyym.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2azuyrfey.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2tktaskgs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xrxqzzsa.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fehywtzm.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pfiaedoy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jhtxsmqg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ltsphiah.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2dgfwedge.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qmmsoxdh.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2kboxfkmw.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2fnhukpag.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2effjqqup.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2izwkkbxp.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2mkoaggxv.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2osttahnk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2zkibstik.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2czcwjoou.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2atkhxzaf.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2uckzoodc.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2aqnaqxie.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2gmuvgxbb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2iialjirx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iujrheum.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rwpgjwqh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2enoekrly.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2mtbvxrqg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vsknvois.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2yhokdcnp.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2sxpifwoa.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2gxlzlydj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2whluwzoi.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2llovbujr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2wpimfcfm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2pljrszhj.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2saqvlzhx.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2naelmgck.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2avrwwctd.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2wxxdxgby.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2srokipkf.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fmbixevb.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fvslgskh.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2assqtwuj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2hlcfcedc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2zfvahueg.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jtvmcywm.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2yegkelwt.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2outafhys.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2qvfdfwdt.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2jblkllem.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2qdekarvv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2wtgksuku.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ocdsaxep.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2sxwidicb.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2xgxjmoiv.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2xcpzrcqc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2mwnyuwpu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2nutxcagm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2pqsdbfvx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2tgjnusut.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2qabcybmc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2rzunxfjd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2vecigmwc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2qntmvfdn.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2kgxspmym.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2vomrkiet.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2ipadtkke.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2knynwcnu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2xoregzdd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ondpjdpo.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2ptfibdam.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2ttozftkh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bvnhctrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bvsmzpqg.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hwcdbeux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2noqyscow.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2zjyvpjwy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nuizrdbx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rllqujip.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2xbjjydqp.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2yplmwufw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2ietebhyk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2bbspslsy.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2jqatyncx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2aqkgkcij.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2qpahkxiv.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2knjqntiv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2karvvxry.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2jaokrxql.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2wvpxidvo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2feposxqo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2glsmripa.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2srvectfs.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wadfdrbb.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2xvwlxwuq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lkskeeck.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wvcmngdu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2xhssrouc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2oamyhfhl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qeyfqvzn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2fzqctnbo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2gfztacwn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2yhchudbg.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2nrojegdv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2ikuqrxnz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2xegxhvdf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2dlpswkbs.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cztqrfsd.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mswoiauo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qmwoggpl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2brcsordk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2glclmahx.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ragjcmig.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2phgvyhia.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2blbramkf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2shnjtzzi.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2tmfspnfr.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2jopldimx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vrgksmbp.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2tpxeryuq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2zwxhwcgv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2wzckewuj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2uufdagjx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2hfmqkgio.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2alamkosa.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2aadnahqw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2jtryveky.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2qlqoksyp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2zrjejahr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2oprndmgx.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2keypelhp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2xmcwwccu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2vhuixage.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2waqtueba.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2ueixozil.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2qgnpvazv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2kwhsqadn.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2lodopwxf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2evornnsb.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2qvwenbiy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2pedmjflq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2nniwzviv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2owxqwdem.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2phdrcqko.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2intopkbb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2unoyydtd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2vtiwzxvc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2punijbcu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kfzflcky.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2tktqvioo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uchimako.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2tbzehovl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2yocsymxt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2dgjmfbhn.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xifqddxf.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2njzfjpos.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2uggpgchm.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2jpezamuw.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2wdprsags.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2lbwcyzxt.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2wvnzgmyo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2hstpfime.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2mmsubhyu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2takrfiba.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2paebtqqh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2gozvxgkq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2xnsaubzg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2syfkhucl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2jfjtmsmz.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2dxpysycs.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2ueoqykas.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2yogakmqi.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wlpruxva.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mlxzmtdr.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2agcjjbub.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2txcccohh.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xgznxisz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2myprpzqq.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2vururthq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2tasnwtez.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2evhptptj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2foefnwqo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2naidokaz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2tlpybpff.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2kkxnzrwf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ehbxwtpf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2doewgnbd.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2zttjrspo.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2hbbfclke.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2fwkfxwwy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2kfgdrybx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2hrwvocme.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2jdbhqbob.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tkszxynm.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2zerifatc.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ulpsiagz.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2lerbvinj.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2mablkgxc.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2xmbxrkcf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2vnntqnyb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2xygtghwm.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ggfybcqn.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2nikyysnq.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2nkvayoao.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2hexrmfal.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2lllbgugs.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2gvlpnltt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ympqchrj.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2wlymhbyc.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2mqsbdodn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2czdvznrc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2bdgtslqe.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2kiqsnkld.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2typuzqxd.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2pxsycstr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2enjyjrgd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2eddatboa.html


<!-- 参考信息 -->