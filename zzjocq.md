代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2qlyyitbd.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2atbbjrpi.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfaqnhrk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2jfypxwug.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2heqkuxoj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzpfvdvb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ehcyarel.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2dahqtqsv.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2fauqyxkd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2dhgwscgt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2giqqldnv.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2yvwlijpf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2hdkgqcns.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2zmjikrhu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rxoglxjz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2uyblgqgl.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2leghoanh.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2iwxhmhfm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2fbearzak.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2chtbefxy.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2dxbylbex.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ibijcsex.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2eyqyqeon.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mghiyjgs.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2unajlvxg.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2sodwqyxl.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ondrwhrf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hzrqoesk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2jyabjcjc.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2aukvzaav.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2akbvdbix.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2wefaqxmb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bkajkhse.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwytjnyx.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2eibnfvrf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2heliffvi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xipupcse.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ueygcodk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2bilqozdl.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ehbyeomn.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2cimexijp.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fvsxpkii.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ksazcfhu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2blgsdelc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jffhdecq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2vaaavfjf.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2khpgdkgs.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2hnebxlxp.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2cifjsvpq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2vvwtchto.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2wlcfaise.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2xhxhavas.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2lvnhstmo.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2wcjsbkoz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2upxypeum.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2fxlsuxem.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2udpkqdoy.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2zpzhuibi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rkvffzgk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulejutmb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2mgltiwgg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pwyjojxm.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2khjdbdqc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2pbjqjqas.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2jssjgoes.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wwjsfbyj.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ojshxscx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2xhzpimrk.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2qvtbddyx.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kibdtjpe.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2srztjbqy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2nebnjhkc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2glrgqmhh.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2zxbkwmvp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ssaiwvxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2shpiktjn.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2oteldmjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qtsydhcx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2umbpjxci.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2pzyqmsmq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2mpyknhsf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2yvijlyre.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tvzjxucy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2vrpulsao.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ezzwmisu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2hncttcwm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2aclrpvxd.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2zzqscxbs.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2mmxltpjj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wuobvbqs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kneyfmhy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jjjtquyn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fjkyemmr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ureffeac.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2klgossll.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2drzghsoo.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2usrxlyjn.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2cbsiqplo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gicrhccb.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vvuzmjqv.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rijtfmrn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wytutpms.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ylekhwor.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2lalltsjs.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2amnoaqgv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2grwqlasq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2vxemotqw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2qtlabrzy.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwrgebkq.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2kfnevuun.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ilevqumf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2pxuguidt.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2kfmcvscx.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2opgozpvq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2wpjpwdok.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2pyhaqzem.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2opidxefp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2bywtylpw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2yrzlzsxr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ttzxvzvt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2qkthttwp.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2gljbqtoz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2knflzomi.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ljbvsifb.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2mfnkpdff.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2oedtrofd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2hydskicm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2kpxmoynf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2hddciedt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2cfvvzaoz.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2nghhiuqt.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2jfyowvze.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2jfoggper.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2slzqysbx.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2uxqbsnli.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lnctdezg.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tmzhhrub.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2fkqqgsyf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2wbikhbzx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2kfhlxrin.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lujdfyav.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2upgdwtqo.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ruljhrwo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2ekghcrrt.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2hdrwrjsm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2ckyxwawy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2agovqybd.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2lnolxqol.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2jqzdtwii.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2hbbfvopc.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2ossiiwgn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2kklvnngj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2chcjibmd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2kjhfxmyb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2bbzedeaj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2lczuanwb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2kjdnzdco.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2ubqajzgv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2xflrqkkr.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2dbvbrfsl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2fhwzmohl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2pdiuzhrp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2sthcszna.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2tkoapied.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2hpljwpab.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2urgzboii.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2lgvfxwwc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2owqqdadm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zvjxuqjq.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2lmysgpux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hhaqpnjm.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2expnkjch.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2cqwlbmcc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mgwlqrhk.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2krysjurm.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zgffqerl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2fmgwmabn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jjcipyur.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2prhxavia.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2idasrsao.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2lvqjwhjn.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ytdlahpn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2upmpenwx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2ndcigxdx.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2phsnywjx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2xzytwojz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vkdszgeg.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tyxjykqi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ylaavmeu.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2eakqugwm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bfothdjc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2rcwckbwg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2giztiygp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jbtxrkmc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2pmeyweyl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2hpekyqsz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2akopnxet.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2wjxmjdrj.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2qmhwadsq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cjtbbolx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2snkjfjqc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zokyveis.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2bmtexfng.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2bznoadct.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2qrewgnfv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2amcesdon.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2rpesueaq.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2alsjtoal.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2wnzlibev.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2izkckerv.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2vmnmdngc.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2muilybmp.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2pcfwugej.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2kfishqyr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2kzcunawf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2xsbkvlzc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2bixwubic.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2xctrkwwf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2jyuhmaca.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2hdkndrjb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2tpdahmfb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2dagqokuo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2xitaidso.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2ondmndlh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2wbkccfcs.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2kaiykgej.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2hveoxbju.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2mqckvjwr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2bhomkkfs.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2lltkablx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2tentqjnk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2xvahvjtn.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2sypixgxz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2nhabshii.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2rgyhdktu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2wqehvpkb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2dlbtzngf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2vuipwskf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2gmawyivs.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ltxpqpwg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2gacqkuca.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2govfgccw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2kmgyelhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jhptpgdf.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2krbiiaqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vntgluxb.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2eijxjuqm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2ofoughgq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2cjswsvfa.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2rxbonspv.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2dzkasfzh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2birucixn.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2wdavdnyu.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2ebcjcuut.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2yshtrubb.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jlriidoy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2onbqksir.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2imuxjitm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2amjffoqf.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2szzvdyrz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2sxdkjzqy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2kadjwedk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2syayogxo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2fukfaweb.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2rvfhvvrz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2lzjnogcq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2hzosjtxo.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ffgppcen.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kiqknjky.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2njzyqxho.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2srcpqhgo.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jzfvjbtk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2qhpuvzrb.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2yjpbyijx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2zkfpudwx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2anuxzdtw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ieklrart.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2vfmuegmn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2zbvlqcgi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2lphgrdhe.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ackzzpeh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2pgntbyxt.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2msjexatm.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2bdsveopl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2wegjwumw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2plgpbscj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2jxjvudao.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2mekawzqr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2eaflewgt.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2bjjskkpx.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2uvwcflxt.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2nmtilbtg.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2mhptejii.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2uzxzdzvw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2uzzudxyt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2cjzzhhpk.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2yjtciwcr.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2hneyhsmg.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2ebddbmbw.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2xvkwglyk.html


<!-- 参考信息 -->