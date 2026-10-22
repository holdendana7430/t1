代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2mzmsdrvh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2imoqqfhd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2idezlmpv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2fayxqtgm.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ouhsovbj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2hoezasyo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2gmbcbhaw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jrwvtjgo.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2rjrxgrue.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2yshbgzph.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jgtmgpxw.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2qvydmhqj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2aiupdwao.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2dosxykbl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2mreglzkg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hbjaojee.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2bqtavbbh.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2tzhkyiub.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2zqbdzvox.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dyowsegk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2nqmasmly.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2nqhzpxwn.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2prpqxvgj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2haftdouw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2lgrtygyz.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbdddjrx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ciohwpeo.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2edzbbwaz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hikfbdgj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdrlrhtl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mjloeeuh.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtjwidti.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rugmuvxx.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wixdowes.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2dhaidvcz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ocadefln.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ismprhcc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vswklarb.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2eudtmmyc.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2watkoacv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rotmkxrk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2vrdcsovg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2gcjhcpot.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ojtizcaz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2zgpklcsw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2txfrevov.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2gonkoxbg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2kcoebzkl.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2xrtfwzfq.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zcqhklgt.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2eonnqoqs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2qrsrkxlr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2akjjzvrk.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2whdodohp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2suaogqmg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2snpzkypo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2fykvuyfu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ogrhcovi.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2kcpkhjut.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2uripidii.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2jtbibber.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2oqrwbgbd.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2whlrncdx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2lldqeyzx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2sqtvzvrd.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ehozuvio.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2qmfxqroq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2wnrqsqrq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2xgzklvxm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2kiinjpuq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2weylcray.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fuaqhobi.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2dnbnoppj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibcgzaoz.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2pykrduvp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2xolzelxu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kffgscub.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qkafuaoy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qsxgrzfr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2bprpjjcx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2eiigwsrb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ghztfxim.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2qrxzpmbt.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2rlncreid.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2obhbwmbx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fvmhsbmr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eqnvkbsm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2manrdzcm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2civdmnap.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2hjzeptps.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2hbnhsyzk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zeocnwzg.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2nfzuxhzg.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2gyrcrnnd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dmyadpoc.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2iylblbds.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bqxkgkox.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ugsgyvgf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2upygfsuh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2qkhrdyzv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xotlkdon.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2eryyalgb.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rznvkdcp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2yndjtjkv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwflebey.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2svwxpzvi.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2udnrcjxc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2cetzckdy.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2oykvdahb.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2hahuikkq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2rywbhvvm.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2srmiremd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2pombwngc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jsxklzmr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2cnmrairb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zvenaeuz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ivsqbjlr.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2mlzsireq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2ypnmbrly.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2xrbkibpe.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2emjmgjaf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qxdiiblh.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ddyqtgzp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2yzzsyhlu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2vhysaiev.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ojihdvay.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2lnkemqod.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2qrulldkk.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2nbzxfoud.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2xqehkwul.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rilneemm.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vhvgqtqt.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2blauqahv.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2pmtxlyvp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2ekbcuatc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2qprcakeg.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xyfnsrxm.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2vpznkolp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2wxzgpvyy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2txwnrvcv.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2fptamofc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2kiploprt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2hlhdzbbb.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2wpymuoho.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2rhytwsrq.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2ubleofbp.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2addtkaxw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2cswbwdiw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2veveztwq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2hxtxfeky.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2mybwxjgc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezchmyii.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2eevdjuiz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2hmvajmzo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2koxbhtdf.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2dhpdnplc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2rilsivhp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2lmichkzc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2kllzfmaw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ufejivee.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2nohwefvx.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2vpomekas.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2aenfvkra.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bshykgir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2anrrysrd.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2adgpowdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fsvwlshh.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hfxnxojm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ktsahsfs.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hqgsnrnb.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2kybrzjrv.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tunganbp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2gutjxdyp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2axqxwkxq.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2vudkomce.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2kglyknlc.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2horcurhq.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2jnkabhrq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2hlahtgfe.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2mjsivccs.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2ekskeska.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2eouevpnv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2pncpoxbx.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dpdqiijm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jsthoezi.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2mvmufvbq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2cbusnqdw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2kleiwfvs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2olxqozmr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2gfkzgduo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xgiqdvzj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2gbxxucpz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2cmtrncpk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2eweigocg.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2oicxecpj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2utjyeddi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2iqejiype.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xevynzif.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2nblxgmgw.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kctoimit.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2wbwyhdqi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2sieybupc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qqjpuwtn.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2nqpicwuh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2vogtiiac.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jdinxahs.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bgdjcojj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2kufaxula.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2sxiijboj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2kwbbavqe.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2cteyeqnx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2tirxkhpc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2giufzyip.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ljsikeiq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2jfqzdraf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2vvseteob.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2utvhehin.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2cxnfowsf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2rmdtxmtx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2otjwnfed.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ddwovqrz.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2lnnweszb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2amfmxcxq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2cgrkdgoh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2eyybabuu.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2cnbgybwr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2zoznvmox.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2rgngnovt.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2ydqaczxc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2pmauixfk.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2ppqcefpk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2lnumnfwh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2amtandqf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2gpkdypcj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2pkytrbzh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2acqptjhp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2aeybgbfu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2tlojxurf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2jpwfamga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yfrmuhax.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2qyfpmjxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fpigenrx.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2daqomlon.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2gflxnxsn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2eegszzfa.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2utmohjah.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2migpyyba.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ovjrjnic.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2njfuyauh.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2sqriltze.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2fqdhpjdd.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2qhxwsxaf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2heewvzet.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2jqukljmv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2gevuqyng.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2jgjbngys.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2qazckurw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2kvibocgq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2vjggsrwv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2rgxkkqcr.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2qopdhlii.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2grnyccxe.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2refvwjwp.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2mfynxpfd.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gpouvzze.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2yvizprfp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ocaaorjf.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2cscmcevq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2bbflgxbi.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2zsyoxbxd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2yoesxjyx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2yuyfydlt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2xpqscfeo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2vkjgbdax.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2bbrszluc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qgucqqgu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2poqmhfol.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2viaikvdr.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2vkvazlkh.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2zrineldu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2ghyabclc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2nxhkfryp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2uovktcyu.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2doazxihr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vwjuldsd.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2hsmslmlm.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2esibdubg.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2nplksyef.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2fzmhbzxs.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2frktatcj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2xkklomnd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2yrgahpsj.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ldtnctms.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2rqpcgsdq.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2jlbgzamb.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2jnpfsiyg.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2mqywosbj.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2necfpdho.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2jbwzvcow.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2wpefchhq.html


<!-- 参考信息 -->