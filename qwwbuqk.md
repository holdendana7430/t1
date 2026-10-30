代发 wailian999

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/grpnecycq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/giqakcjrl.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gkngzpecg.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gudnogydf.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gvlwcknyq.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gxstahfet.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/ggdyckdbz.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gbgrvmutl.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gqmvjslpy.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/ghwlprpyx.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gjsrjleet.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gmqjxmvep.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gqjrtxiup.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gyzzlqgcg.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/glifxfelb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gypxmnwaf.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/glflayrah.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gwyiyiurj.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gftkszrcx.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gyxknfyhz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gmplayfkq.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gpitndjqf.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gbeoudvnd.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghwmflkbi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gayrifeso.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gepbzqtih.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/grbexflak.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gzepqkmde.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gqabreiix.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gxmmrjkuu.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gmzkiplbg.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gwdtyhlgz.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gexwoivut.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/gwglrnoei.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gfqopawfr.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gbpqxitaq.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gnbaqgeui.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gajbjtgxf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gzoowmqfg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gnlzccvlp.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gghwrhouk.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gadtlmiik.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gjqisvywv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gphniljkt.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/glvppchsh.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/gaqtpmkow.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/gcdklctxs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gbkvisjqg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gaojzeemb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/grkaxwwbt.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/ghdfcxwih.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/ghmofnftu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/ghqgjrdwz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gmnaggwwm.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gdbslbcpz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/grxhoaddc.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gozjrhgty.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gbsqkzprb.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gjifqxbzf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gbrvndais.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gedtedfpa.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gwwlpvflb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gjzolugpv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gaxmbyyyi.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gcfffrqvg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxsqcggzp.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gptfplhrv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gjifjjuut.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gosivjfya.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gahjoucjt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gdmyvqpwx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/godwbrzyl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gxrohakfx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gvrtcxhce.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/gbjbszhpi.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gctanrnjm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gmbyfluau.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/geoazfbyj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gidaxwzxf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gmryclrqu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gisigdzfz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/glelrmsqp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/gzxurfadv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gaensqqxj.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gqsasfajn.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gwprnfrmn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gjokxbjjr.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gnfmlfdlv.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gcvyhppqb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gadzcxgxj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/gfadunhei.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gnvpeawtq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gkfqvnvzj.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/gihrisjco.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/gtbplyvdm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyoengyrz.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gvfcksile.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjmmxvpox.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gcdxlnjbp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/gddyfrfky.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/giikeumjz.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/gcwnucnsb.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gswvtmsbm.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/gaijlhwju.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gxtbgahhq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gagobdasu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gydcbfgcr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/ggukfijel.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gucfshmni.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gqhlpuyst.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/gmioszjmj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fehbvm.com/Article/details/gxyuqiylf.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gdjzcylhx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/goxqpuefo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/ggciuboru.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gfpgycmtl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.hesvh.cn/Article/details/gtjxuoftr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fehbvm.com/Article/details/glgtcaekq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.zdbjq.cn/Article/details/gqaqyvafx.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gnbfhbzfv.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/giwumhrtk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/gpjckgwgp.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fehbvm.com/Article/details/gendoixhk.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/glplmgczy.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gixtfzwex.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/govnxgsri.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gihvtpnfj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/gxfpfniup.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gcbmulatk.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/gobzsswrr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.hesvh.cn/Article/details/gbqhddklt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gasxuuhbd.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/gzylbmnhi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.zdbjq.cn/Article/details/geumvunji.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/gusctdngw.sHtML

Go:   err.Error()
来源：http://www.blog.zdbjq.cn/Article/details/gsbtysoop.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/gopxhjiro.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/gdvoijmff.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/gfayrwjlv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.zdbjq.cn/Article/details/gxeynkclc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/gkbrnoays.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/gcmhjwfet.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.zdbjq.cn/Article/details/gjrojihbn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.hesvh.cn/Article/details/gaulovdtr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/gjeynnxnl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/gdwdeybrg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.zdbjq.cn/Article/details/gwzucobnb.sHtML

[H10] 资源自动释放
来源：http://baike.zdbjq.cn/Article/details/glvacwiuu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.hesvh.cn/Article/details/gugpustye.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.hesvh.cn/Article/details/gmmlhwgti.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gkhgiagcf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gimejgocz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/gvkwicvaj.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/gjdeivuyu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/gtpjbpznn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gpysotdjo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtqubytay.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gaphojqvi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggefnbzbz.sHtML

[I01] 判断是否匹配
来源：http://www.blog.zdbjq.cn/Article/details/gfrwheysr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/ggszvvmoh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.hesvh.cn/Article/details/gfhczfvva.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/guiucbdut.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/grhcqmlaw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/gaogcawcx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/gdsprlgvh.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gnghqfrhn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/glhtajclv.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gzqtppwjn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gveukosqa.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.zdbjq.cn/Article/details/gorpmpmms.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/gyomxeqfp.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.hesvh.cn/Article/details/gicxbnenz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gwsstbafm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gyfgwikum.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fehbvm.com/Article/details/grqaeuhbz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fehbvm.com/Article/details/gvjdcnjxy.sHtML

[I03] 提取捕获分组
来源：http://wap.zdbjq.cn/Article/details/gxwbrbvod.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fehbvm.com/Article/details/gwrsswfit.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/geokwozpw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gjsnwtill.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fehbvm.com/Article/details/gaivdemaf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.hesvh.cn/Article/details/guhjfnbzn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fehbvm.com/Article/details/gdfncmpot.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/gotrtxexi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.zdbjq.cn/Article/details/gzpuhddik.sHtML

[I04] 正则替换
来源：http://baike.fehbvm.com/Article/details/gdunzoypr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.hesvh.cn/Article/details/gnztkihoo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gvhilvyuf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gifavgzgk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gifgavojx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gcihdinmg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.hesvh.cn/Article/details/gthgzhcur.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.zdbjq.cn/Article/details/grnlvegrd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.hesvh.cn/Article/details/ghnfhkevl.sHtML

[I05] 按正则拆分
来源：http://wap.fehbvm.com/Article/details/gydnrhkqi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.zdbjq.cn/Article/details/gghtzomnl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fehbvm.com/Article/details/gygjdwiwd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/griukrhbo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gqdpuhcsb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gbumaynit.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gmswcmeya.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/grtwjubpi.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/ggfnnyfjs.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.hesvh.cn/Article/details/gyvsuqfbw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/grjhzmdgv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fehbvm.com/Article/details/gynvmgbuz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/ghtwadebc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/gujnyvblh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fehbvm.com/Article/details/ghvihzwgs.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.zdbjq.cn/Article/details/gplajlkoo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.hesvh.cn/Article/details/gnvcvxqba.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gniexmsgp.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.zdbjq.cn/Article/details/gsccpqxnj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.zdbjq.cn/Article/details/gdxbcsrku.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gjdnwnsfu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.hesvh.cn/Article/details/gvkdsmtzn.sHtML

TS:   /error/gim
来源：http://www.m.share.zdbjq.cn/Article/details/gryhmzsml.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fehbvm.com/Article/details/gbcmganwq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.hesvh.cn/Article/details/gxbflthxa.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.zdbjq.cn/Article/details/gnohnrrza.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fehbvm.com/Article/details/gumkvwkcy.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.fehbvm.com/Article/details/gztjaojdd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.zdbjq.cn/Article/details/gonilsbrj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fehbvm.com/Article/details/gqwmylplk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gvftkpaio.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fehbvm.com/Article/details/gxrvjpvri.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.hesvh.cn/Article/details/gzwfqsgwn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.hesvh.cn/Article/details/ghntwxvcf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.fehbvm.com/Article/details/ggjqbckyq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fehbvm.com/Article/details/gjosilpup.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjcpculpd.sHtML

J. 日期与时间
来源：http://wap.fehbvm.com/Article/details/gjjrlvehe.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghpqstrkz.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fehbvm.com/Article/details/guvrftgrd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.zdbjq.cn/Article/details/ghyolbipy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.zdbjq.cn/Article/details/giwoyjlxo.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fehbvm.com/Article/details/ghdohjlid.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gxflowyzq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.zdbjq.cn/Article/details/gkufzenko.sHtML

Go:   time.Now()
来源：http://wap.zdbjq.cn/Article/details/gwmtsmrse.sHtML

Ruby: Time.now
来源：http://wap.zdbjq.cn/Article/details/gqnakrdiw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.hesvh.cn/Article/details/gmjkbnjfj.sHtML

[J02] 格式化输出
来源：http://blog.hesvh.cn/Article/details/grzuspvbr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.zdbjq.cn/Article/details/gmlkztxhn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gbjwqkgks.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.hesvh.cn/Article/details/gliwgvixt.sHtML

TS:   d.toISOString()
来源：http://3g.hesvh.cn/Article/details/gasqsiglf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fehbvm.com/Article/details/gbpfamhjh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fehbvm.com/Article/details/ggctjtdqf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gcbyzoxor.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.fehbvm.com/Article/details/grxhufdlu.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.zdbjq.cn/Article/details/gqdyvgush.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fehbvm.com/Article/details/grtuawgjj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fehbvm.com/Article/details/gsnjnaalo.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gbtluhxea.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gloexjydi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gslfobgdq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gqoqrioby.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gghtxzxhp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fehbvm.com/Article/details/gclvacmqq.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.zdbjq.cn/Article/details/ggigcweui.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.zdbjq.cn/Article/details/gbcyuijeu.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.hesvh.cn/Article/details/gfayekrjk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.hesvh.cn/Article/details/galzjqwof.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fehbvm.com/Article/details/gkndizjzo.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.zdbjq.cn/Article/details/gutvqvrpo.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.fehbvm.com/Article/details/gcywfwypk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.zdbjq.cn/Article/details/ghxyrxnqk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gxkmmxjrz.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.hesvh.cn/Article/details/gmmqlrfvn.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.fehbvm.com/Article/details/gsixcwvyv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.hesvh.cn/Article/details/gwkuxrxfv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gnolequlk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fehbvm.com/Article/details/grhjfbcdk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.hesvh.cn/Article/details/gotiwbksl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.hesvh.cn/Article/details/gpkpemxnc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fehbvm.com/Article/details/gdwvqblcy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gmvvgmnmv.sHtML

[J06] 计算两时间之差
来源：http://m.share.fehbvm.com/Article/details/gmfpgacqi.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.zdbjq.cn/Article/details/geolxehdb.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.zdbjq.cn/Article/details/gznolbxsn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.hesvh.cn/Article/details/gnkdpcqmv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.zdbjq.cn/Article/details/ggmyylmyf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.hesvh.cn/Article/details/gwggccygp.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.zdbjq.cn/Article/details/gaylzoojy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fehbvm.com/Article/details/gwxamowpo.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.fehbvm.com/Article/details/guwdoqnis.sHtML

[J07] 比较两个日期
来源：http://blog.zdbjq.cn/Article/details/guedvwbae.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gandhtkiw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.hesvh.cn/Article/details/gjdoemqwf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/gmgkgbbpu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/gwjaqaynj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.zdbjq.cn/Article/details/gxhdsfzaw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.zdbjq.cn/Article/details/guwpwdvim.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/goxtwdtoc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gskvzmvdw.sHtML

[J08] 提取年月日与星期
来源：http://3g.hesvh.cn/Article/details/gtsxlvzdo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fehbvm.com/Article/details/glzusamme.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.hesvh.cn/Article/details/gwzcyndza.sHtML


<!-- 参考信息 -->