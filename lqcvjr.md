代发 wailian999

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2vruyaacb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2nniqioqi.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2quxdfxwj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2keyoqmrr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zsstoofv.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2jbylemzx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2qslbjnus.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rfqvztbc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2mxauigsc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2obboyxpq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2qggrewds.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pccnakvu.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjvxyjwj.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qtvdqoiv.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulasbono.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jpnmhmpe.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2zrtbdsuf.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2yviaylsg.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nuptahwz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2nsypxsdy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2selamsay.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2idgwivmx.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sprjlffn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xsdpttoa.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gatkstru.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zwtjipzz.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2pyjiouhg.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2kcryvniz.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2wrqmrevk.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mnlvzulk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wotmdmig.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uywnipxd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wpdehxpj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2fqllmwqd.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2kugkvoxr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2mbcogvsf.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2jalqfrdg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2dupxjrrp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2niuerxko.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2syjxvfnz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ynwwzgxd.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2yxopjwqx.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2wbbbopfi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2mqlvtgbd.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2zlwhsfbu.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mtxibove.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2vbimdafn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2mlprjzqy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2fdjcqoyc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2pcbekldn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2vbugnfja.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ujdumkzl.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2metqlnno.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sftclsxb.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2nxpiveio.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2hxxxjbtu.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2bdhylfva.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fxnzgpot.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2fmxqzqui.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2noijgzfj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2tobvcyyw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2gcjgwunf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2pzeuancr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qiorupbv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2vlxmlnbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bueyrttr.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2uzxtjjnn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2anaycdxw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ezumzvmq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jauytcqa.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2pwucloux.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdbisayk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ofcxmbqk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2pzxpdteb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ctqxpkpr.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2nlrrpomg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ieqwjmed.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2faaxtblo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hkozzpun.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xmvodpqs.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ngrjoejr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2yqkvwifa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2gehonetb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2oitmxbjb.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2fxatucuo.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2qmcrqwtm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zgwqgkci.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bgvuooib.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yhwiqgnf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qkqorbos.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ahzwzuzo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2qgnwaouv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yczwfaut.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2hvsaxanq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2hoczziod.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2vbjqdglk.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwbrafoh.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2iwpvuusc.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2dlgvfmrl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2fkctsecw.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2krxjxgmm.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2hysqxaek.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2rojilosb.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2boqwywyz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2smrhlmwz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmdgcekg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dvfnlwsj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tohtceup.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ovstovft.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2ogpnajvz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2mlrfldrg.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2lofvrdoh.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2dtyncxwj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cvgvptgr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ufqjerfn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2jkphqtoi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2vxxnnyfx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2rdkmpmvm.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2hcahmhzd.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2flstuosq.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2chxaklgr.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2cwyuhsye.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cymtfcbo.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2znnzoahc.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2onpgobbl.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2iykmracu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2chxlmvse.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2wbjqupof.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wyvbzzbj.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2brvjnzxu.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2sbaojnhs.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2lcrnqryj.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2wjgykosr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2olnnndtk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2rghnofjw.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2srjtysjv.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2kybacgwt.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2jhfzepaa.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2reliihvj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2qbxgunhl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2lbzgxqxo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2jbhskpqn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2afwnabxd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycqqvdkb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2dyuusyqr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2iingqfpy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2zuabtdgu.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2nvvmkfup.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2fbqcisji.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2qdejvsbp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2weulrajf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2hcjrdbys.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2oafflfnc.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2aheascah.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ekmqbkcz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tnjteioi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vihxmvgo.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2oduhmwzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nireuzxu.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bclkumpm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gidkwqaf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jrmigiin.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2uvrroeya.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2canupjoz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2ucxaptkg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ojuilkni.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2moeykqvf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ojnjoaif.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ejuirzkp.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2gsuoadbg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2vqibdkte.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2ngbhazwn.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2qymgdgqz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bkebdzvc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2vdggrkzv.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2yhlqaqxx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yajxvylf.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2eederqfn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aeqiroje.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2lhqfblbs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2vaqsujia.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2jeubghnt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2ndflovns.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2rmnnnicv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2rotgwwgd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2bjfljfaq.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2atyugkzo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gaqdidju.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zcsndsvo.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2nsqljgzl.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2iemucvcr.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ynizpmtx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2mppuomwy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2ojeghnlk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pzyssuot.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2adffsqqv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lhfzojgk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ctpfkpio.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bmdflxol.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2vbbsswdz.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2uifjkocv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2egxuexvc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2raeotrcv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2eqdnvotj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2cyinhbwu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2jbnwzscy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2nozcnwlt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ogphnxgo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2wmpqeedu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2hqlapvew.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2orllkksk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2tmvwqpuo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ucoitdnt.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2jukdvfsg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2nonhldba.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2vwoxgfzw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2paggajkb.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2sjffftxt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2enrmlyvg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2ioahsldh.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2knjvykjs.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2ckbcvmuu.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2lcrrbvpp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2kwwyrcvd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2mmqugugy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2qbrvqcet.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2gyfmeggn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2xpmvtqzh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2rlpgejws.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2nsdgkojr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2btbyfkqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pcatbcnp.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2jameyqgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dqwhtqwy.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2oopeopge.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2xmndwbdj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2yqyucrbo.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2nsrkoyxl.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2zlfdhfmj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2csvprzxp.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2tzcoimoy.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2nqtbkadk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2njbexufw.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2suaeyiub.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2lrzchsfs.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2fbrlcozh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2fpsvagig.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2lwpherjn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2rkxehidg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2qytledcc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2mrldbanv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2wbhzdiur.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2nmjzefzw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2lhdfnofp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2bznhnena.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2upnowabu.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2bucjhrnr.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2cuisumlp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bxyqygvx.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2mgxnkcgh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2unoxmjug.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2hojscjoj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2lxcdewau.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2reycyosa.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2dszzjwcs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2eyzgrpru.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2benwrpgx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rwogmltg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2wjexefya.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2juwdtlko.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2mcahlefq.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2ljdefqjv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2ugdywjiq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2wmxcofuq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2dfeawgto.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2xakvsxwr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tbefvrni.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2zaugmjba.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2tfonygav.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2hhnvcufn.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2pjetdutn.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2yeeduvrs.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2xrjpgewt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2qqqvjrpn.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2aypvpcbe.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2jjnppnjm.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2pvutgohz.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2smyorxuk.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2wijedtrj.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ogadaswf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2inrqyqut.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2mhnwkhvz.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ucgsjove.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2gthehsbj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2wicqotox.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2lbvxubhs.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2gslbngbk.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2qundfwuu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2ihclyomz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2bqiagbxd.html


<!-- 参考信息 -->