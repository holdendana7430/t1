代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2uqvfvgce.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2lypffoyd.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2hnpkfpmq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2gvpzrrlm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2qvabmgvp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzyajyug.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2muegtnfu.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2enjkaxiv.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2feoybjlt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2rwjwgwct.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2mxcntenn.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2xpdungbg.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2zehlbziq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2uwfguink.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2onrsoupl.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2kzzhbnjy.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fcvzwwyl.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2yvlxfjkh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2wkkktzdv.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2uhrcuojl.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2wuqpvbgs.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2nlqrcmnm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ujcuckoy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2repvxixq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jhgdkybi.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2myurhfys.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fcbwgazv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2dxvimjud.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2gowsymcv.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2gfpnaxot.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vywjazwz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hrftwtgh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ufopqskm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnoooqzq.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jujoiqnz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nhxleksh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2igwsnxvc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dexicbuf.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ybwphvai.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2eotqrjhx.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2yqgnefsx.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zhxzaryh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2waiuadnv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jsxtliqc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fqfjaqfi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2unyhskky.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2zwpzoscm.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2npfoszlw.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2yosjyutk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2rkeszunf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ssppkiaj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2irojkgaq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2xjuiowvb.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2yiideaqq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2wsxiyagz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2okorhqvy.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2dkoyocxg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2rzkntssi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2xahhtpvw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2sidscpnk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2sjnkpfds.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ukxxyome.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2zqutcojd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2xiaxzbml.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2mptmfhep.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jifhonol.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2vuvjvgks.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ttsnbdxm.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2hqvsyhht.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2hsuyxyla.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2rmeoiaeo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2caazxbjq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2noligpzj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2pabbcrro.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ggwqlthb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzhgjqix.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ejetdmls.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wlshohfe.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2nxhqszll.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2vsibkwfp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2bfnavchq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tpwyfill.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ulprskhy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2zvsypeks.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ywvdzpam.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2oqrkdsjz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2owecagyr.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2zphecgnq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2gsbmjdlo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zxdrcktp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hzqmkeen.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oouhqyvw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ytwvbwtq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2pkyiwnqx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2cqksubtd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kuxxvzyq.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ipbgaose.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2fscjofwq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fdddupmt.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xepdewxb.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bwbzwmpv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2trkqjlbr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2qyqfiayk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2qjwecxve.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wqlteqad.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2kjzwponn.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mlbtlyhf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vzfwbess.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2brhukiqh.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ytslyxbn.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2jddhqxrj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2rgzxgiqk.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2xseewfle.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2hxamdruy.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2iqsnlxei.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2fsuyyzjz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2zodbqrim.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cedpahph.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ryxjkvpq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2awcwrjsh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2lfjtekur.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2pmmfaujb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ugvdygcs.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2vnruhgna.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2mcshrkel.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2llomnzuo.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2fsvezier.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2icbvsxcs.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2tfwptxpt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2szyirihg.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2qqyfhryi.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2rpxwmrwv.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2cqbgfwsx.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2fjedmblt.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2anvkslpl.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dgcktgsi.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2omvgwntx.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2fdpqbpwg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2qahfhnbs.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2gtpdpktd.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ytevkjkj.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2qjmfykgl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2iqaqtvtv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2duarbmqb.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2khocokzm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2qgndvapa.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2gxalsfca.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2tgqpnnjz.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2pmhhwhqk.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2fmgsucip.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2qrxkudhi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2jbkzrqro.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2lnslrykk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2xxgulmsk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2juspykrp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2moyymhkm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2vpnqwjxb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2lwfbsxdu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2mqotbkxp.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2rfswzonz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2elkxedwi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2drndbnda.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ziabqqil.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2qewdyyhu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2tlytmryt.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2ucedmmpl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2lwlhcqxx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2obzdrojz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gkluwumu.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qrqoxjqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gkjplchk.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2kfhkneit.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hmcqnxqa.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2denjivtm.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2dnmrtcwu.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ozirfokm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2xzrpxyvd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2znndmtbq.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2wjngdhyd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2flqnhqbk.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vikqgnsw.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nqjdsryj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ddmnqatl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2fbmgrefx.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2csshrirh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ufuxyyzk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2accyfwda.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qwoimyul.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2illitjej.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2iefzrohd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jprbzptd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fcuhhrxc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dkzklpet.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2hcnxhyxt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xdojtjjr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2yymrekhn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2qkafmgyg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2wlhijxbz.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2mxqskbkb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2bahmbdpq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2yitqedyd.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2sqvdembm.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2zlnawmvz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2lhzckanz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bzjqoghv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ggdutozi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2rdjjxlqu.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gmmqpgph.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2mfxwkaey.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jbccymcz.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2oylfwkxp.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2cziahcqk.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2kxmlyosp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2xhhdivwh.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2xywjzuxv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2mxysmlix.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2wcdyhgfe.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2moretstz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2tffrlimf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2dxsakhfd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ozveuzdk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2xccyayjq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ncplkurd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2oonvvpbd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2jwaqocqc.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2uyqymkpv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2oylijhsc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2fayyotwl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2rzxgrwtu.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2rlikxupg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2hevzigol.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2zwwngiql.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2ljcesapv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2weisbhtc.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tqkpusue.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2ghkrkcst.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2lecemuwo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2fgsioyvk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2kdkrrufv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2dcsawmci.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2qolldkxm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2vamdiisg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2svtxncmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iotlhesg.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2ujsboopa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ghdyztst.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2fzxafeam.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2fxcpkidb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2fvwuvbvi.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2wcpmvwmk.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2wjayhtcz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2lgmokuui.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2dgeoarxx.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2torjebia.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2hzfihnyw.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2yisjnhef.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ouqyfxeq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2cqrlggoo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2uzikovcc.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2lmcyurux.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2vxazyvol.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2shrkktzs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2bsqxsked.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2vsbidoxw.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2ssnoyiiv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2iikcdecu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2fqzqukvs.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gknxyoea.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2flmdslwf.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zkjtzgss.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mltjqjcf.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jfqruozi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2juppsvyc.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2aefxibnp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2uflnzjwx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2jlguozfe.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2atwlefcz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2jsfmexcs.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2rukxdlde.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lhjaqrxu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2vwzqhauw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2fbyvfmub.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2rzqccfgp.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2uehjwaxj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2actjzpqh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ufjmcuew.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2oavivvhb.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2twxovhaa.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2bpgeeodu.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2bypxrcgx.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2tmexugrc.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2tulxblgp.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2luxetemq.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2bukifrdp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2vexvouup.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2mtvhjyaf.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2lsalasfe.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2opmlekuf.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2rxuxfqip.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2rggxwcby.html


<!-- 参考信息 -->