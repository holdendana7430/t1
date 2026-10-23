代发 wailian999

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sdpuonoa.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3shrlewpa.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3qrjmexmz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ytzkxoft.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3orxohutm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3mryisyll.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3oexecsiv.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3wmcwewjt.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xlyqdyvm.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ngcnobhb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3lvmqqpvo.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mamufcni.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3qdzrqusc.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3xnfypdqt.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3otzmmdfb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3daapzdjj.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zoybddqb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3kzdwcvmn.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gessvrzr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ljpknagk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3wgphhdzl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3tmuzcuxj.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3iygzrdfv.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ucoittbh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfdijwvw.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hotkpybh.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbdrfrkp.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ghdgrzbe.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3sqleoxol.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ewuroczu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3navollfr.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3nknfmogv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ilnbfyjd.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gjpjyvqy.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bnqtspnt.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3udqdxfju.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yrceualr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3oxosyiiy.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3wooxfidq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ewdazjoz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3rzusutlj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3gkjvttox.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3cbmwdlrs.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3tcrrfajg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3efpzsoaa.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3mhejnahi.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ulizlosl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3bkthhptr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ujemjjjm.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3feryiyru.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3lavqxspp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbjuaubc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3jofebbzw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vqtnmsdg.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3yphekimr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3dbblvayn.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3krbugkuz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xgadjmbd.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3sjqhwzcb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3omdhtdoh.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3emjnfasv.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ujydoarr.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3fnquereo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3opbcuxbu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3aawryapv.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3bwlvdmlt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ddbugilo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ybnopwwx.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3jgxerqwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jftbxkyf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3avwwmljf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ureolgdq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3nacjbadt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3apovvlkv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vnwqhzed.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mtrunywb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3fkdtncju.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3uarvumcx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3yuumplvp.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3piwvfedc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ovzgeitv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhbxhimv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3houiotzk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zitrfrmv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mogpnbid.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3anmilkmn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3oiklepwp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kuviqnqt.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3buygorpp.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3nvkjqyfx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tufvwhrz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vrntijny.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yepuufaw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zfpcsgdd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3cvbkrkoo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3opxkudwy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dzkrrgxr.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3csrmsevr.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3tsbabahj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3esdydott.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3gsmsvnmc.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3xdrlsdvt.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3xthhtiib.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3azxvbfjn.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3tpnepfrt.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3blmhtstv.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3sgkvjoow.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3gskxmstj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3ycrfbari.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3btofbjwo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3drygppid.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sbstrdcf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3vrjnicdj.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3swvzcjsg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3slfmvwts.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3egyyxojr.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3yjtjistv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3svsxsbtt.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3tqlcvaya.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3aqfmhtcn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3hvgqrwzt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3wmjtexxf.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3dcweklgv.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xofbphoc.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3iqeidjrj.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3cfgpzwbl.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zmdlnnnk.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3emeltqpe.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3pbypatsm.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3uoqgslue.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3yiakfrvd.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3dxnhyjxo.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3iifgeyyi.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3hvbnvxon.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3dttpexru.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3qqexmdpg.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3urgfavpo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3qowvifus.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3bromiyxa.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3thmkhchd.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3gbxqyhjq.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3doogxtwb.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3bdmkcqfv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3bndeuryj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3lrtrcawz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3yfsjvnas.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3iythhnsg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3znxdfedw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3eypltfac.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3lnqhqisx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3tnarzxys.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3quulezgv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3isznnusg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3mxauljyt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3qhsrfyen.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3zeluvefa.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3rzbmctpw.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3vxcngwfj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3zqgrgcax.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sdmktekm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vyruomev.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wyoaxpwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wixsdgvv.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3pqooczww.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3crbzggri.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3goiylwri.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3xnkzdjqq.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gbkttubj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3cxzlfkuh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cjermhdu.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3yuuzpohx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3khpcikan.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3eurtaxyt.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3iynpmwrf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3nejiqhce.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3xiguboqo.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3nnbywnxn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3qesyfcls.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ytlajupr.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wtyhcoff.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3huocpblv.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3gxskmyjm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mjxxtfle.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3bjfkpevd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3kgixbkcx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ojrpdwnh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3gdsalogr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3uroaoklp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3yarkdxdo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3unbsppph.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3hrjtfqxc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3sagffwso.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kbmryiqw.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3eoqcdhgj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3bbrtqawk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3szundzpr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3tiifkjdd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3cgfplxab.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3fbixhlye.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3nhhsczjn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3tnvxvubg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ngogtbog.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3zvgaotuh.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ybxngoii.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3oarnclew.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3bbhsctcq.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3pzxhokug.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3wxdcnfro.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3arjqudiv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3yhgyofen.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3pwlzhden.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3vmdrwxgq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3txvzsvfo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ifcqwsbu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3hjrptjdq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3fymomvmh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3blvloiih.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3njyddmlb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3ezjlwwhy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ivntrnfj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3dmtybgfs.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3iooyrgbz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3jhrjhnof.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3tftwxxqc.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3onrlgejb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3zjndeqsu.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xcfsmqns.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3zuplqmuj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3vcnswpjh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3rfzwwmvu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3wtzftwjt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3tovkkmik.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3ocxwexlt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3bmdmenmb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3xfheenzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pulzazbq.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3cyzoinhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3embodjmh.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3bunbfvjn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3gpfbnmzv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3tlfcbpmb.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3vctexmcw.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3eigmswro.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3bjdvmxbd.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3ovrepfri.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3rbvsryzr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3czuagujr.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3vmqamibn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3goksxoug.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3oicbrxmh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3puecikuv.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3qlsqrjwt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3vcvfwxac.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3avviekvp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3rshbwgpa.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3qxogxzrx.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3eshivtrj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3nqeceawr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3xlwjyvcm.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3hvdceflo.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ineiodvw.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ztxreixw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3znmuhbdg.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zzsnvnte.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3xdkcexfj.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3lhwxpgdb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3qdzlhdts.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3jcktfehm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3bbsxdorx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3tdrulrff.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3sdxfryxn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zcjgkycl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3xpxkozrn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ywdrkmln.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3hxodzbjx.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3zwgazdcv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3xwkiybio.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ylpukfgm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3cszybckb.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3vquqfdju.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3lyplbttp.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3cyicrqhq.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3tybchgqh.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3qcbgipzh.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3gktzhjpr.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3hyiseobm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3islgfuki.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3ztptlxys.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3wsammdhr.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3glauzlxe.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3cphcbtpj.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3azfgrmjp.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3gzmulgtk.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3wiwebgei.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3vcesupfl.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3aojaltvp.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3kfdqfedr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3kqybcokg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3xiipxwiw.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3vwyirxfo.html


<!-- 参考信息 -->