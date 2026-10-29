代发 wailian999

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gihjjnmxu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/glpyaxyvj.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gmqpptqxs.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gyiqpuogu.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gtizmevbw.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gqaxflyci.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/giejrryym.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gbvgdgrqt.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/glouxmput.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gqpospmoa.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gleocqfna.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gnbdlvxpq.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/goqhhrzkc.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gtwfxabht.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gbkotgwjy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gglzegfsq.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gldwehaqq.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gbpbmyzze.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gpjclihuz.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gmxsluvdh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gamhjfqgd.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gxaktfvgq.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gbblfbfks.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gntkjkyne.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/grjbwarki.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gbxmfdmmj.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gmxgjucrk.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gzgwiyger.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gvrxeadmp.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gjatshudy.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/guflodjlu.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gmivvclwa.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gycoganxh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gzfhueopv.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gxjvvcnnm.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/ghuhqqxdx.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gmgvnqxhp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gvllhsflk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gmfwpxrep.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/grpvnwqpp.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gmahgiztr.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/galblwyef.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gmdqkgwss.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gnadvtdmt.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gtoomrgcx.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gyejyhtmo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gpyfwgbwd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gepnqitsp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gglwvplij.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gurqkytzm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gxydmmmfv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/goexwhpau.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gyayuhvca.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gaqhkfzlc.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gyszzsimp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/glgczypqm.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/gmwyckkdl.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/grgnuymdj.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gpzdxweip.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/grlrvgcdn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gwlzytcbd.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/gfdkzrgpw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gjuiegkuf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/girdziluy.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gatfgcrgs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwilvocpe.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/gmzpipynf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gnmniykzb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gqdghflhd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gtrbqxtgw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gfsqbbbtm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.hesvh.cn/Article/details/guhmrgeun.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gosovbuyi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gjwvzjdwn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/ggcwnpuqy.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/grviwkvpr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gapwpneys.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/giuksizje.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gpdcicruv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gqzcehzgu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gdyrxuhjz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gccmmlkbq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/gzbxmnrdi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwfopjsox.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/grnwlztdx.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/gaashztjn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gkropfiqw.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/ghnwqpjka.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gikxgshgq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gdbaificj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/giqnpglar.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gmenrfefq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gvzoxtxoi.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/gpwhiemvc.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gyhlkiktr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/grnfgnecm.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gztyzgysk.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gpsygatar.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gcjzonlcq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/giolghrrb.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/gxsnzewvu.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gsqricmpr.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gzoxxpvki.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/gcbxrabsc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/gjzqenanq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gpyheygdd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/geynelkzv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/gdpycpmvc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/gvaryaybf.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.zdbjq.cn/Article/details/gbvviolky.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gelpfmydg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gzuymnztl.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/guqttiiyi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gkqndbmtb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/glahrbsjg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gebpdgtlg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.zdbjq.cn/Article/details/gkzwjfbmu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/gfjtokvug.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gapofnzyj.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gljhuzuhf.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/gaypcjacr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gwvoxfnbo.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/giqydhqna.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gxtsiwizo.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gdkokhooe.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/gbgwuvwiy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/ggfgvfxnb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fehbvm.com/Article/details/ghqkacbmk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/grvfvjxtb.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.hesvh.cn/Article/details/gfhgfpave.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fehbvm.com/Article/details/gxgnmoxnh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gvemluibv.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/grszajpqq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/gkxosyhli.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gbommemqn.sHtML

Go:   err.Error()
来源：http://blog.zdbjq.cn/Article/details/gjqdjxpyr.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.hesvh.cn/Article/details/ghqdlvumk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gzduqwjwi.sHtML

[H09] 带错误码的异常
来源：http://read.share.fehbvm.com/Article/details/gcxpfckfg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fehbvm.com/Article/details/gwciecuth.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gkygjykrk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/gjfxiplgo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gazanuwox.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/gfyynlidu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fehbvm.com/Article/details/gqwcxihzz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/gfmnvgxcz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.hesvh.cn/Article/details/gnauzdntq.sHtML

[H10] 资源自动释放
来源：http://baike.fehbvm.com/Article/details/gkzvitvix.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gjzaptihg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/geesltogi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gwniqnxfb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gsufvhtdw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fehbvm.com/Article/details/gmpcgkczv.sHtML

Go:   defer f.Close()
来源：http://mobile.zdbjq.cn/Article/details/gyejvptyr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.hesvh.cn/Article/details/gfiqecdwq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gmqsgxsqy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkcjxbsdu.sHtML

I. 正则表达式
来源：http://www.m.share.fehbvm.com/Article/details/gmvkywedx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqtxdyrte.sHtML

[I01] 判断是否匹配
来源：http://baike.zdbjq.cn/Article/details/gcxiowrrq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gwpycjorz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gwmcxfiaw.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/ggqvdtqvl.sHtML

TS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/grtttabil.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.hesvh.cn/Article/details/gnvuoqyog.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gupaxlolw.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gtzjafoxh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fehbvm.com/Article/details/gjlvdfdjc.sHtML

[I02] 提取所有匹配
来源：http://www.blog.zdbjq.cn/Article/details/gllbhmuyh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gybemiqav.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.zdbjq.cn/Article/details/gndqyojlk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/gzqruomcq.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.hesvh.cn/Article/details/gkpyjilab.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.hesvh.cn/Article/details/gjnhpprqg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.hesvh.cn/Article/details/gbekuitlg.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gauewwexl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gfwkrhvik.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/gazakfilv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fehbvm.com/Article/details/gacieoeuu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/grhdtelio.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.zdbjq.cn/Article/details/ghgrfeamh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/gyzykdlmk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fehbvm.com/Article/details/gkzepuyiz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.hesvh.cn/Article/details/glrovhava.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.zdbjq.cn/Article/details/gdbbtuftq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.zdbjq.cn/Article/details/gtixmiajw.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/gmdbpxtas.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/gbchjdplq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/geyihkvqk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gqdcqjhlm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/geueerixc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/gvviehpgn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.hesvh.cn/Article/details/gmiogfhuy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fehbvm.com/Article/details/gtnyneafb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/guoteezda.sHtML

[I05] 按正则拆分
来源：http://m.share.hesvh.cn/Article/details/gtycdhngz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.hesvh.cn/Article/details/gcxzlchme.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fehbvm.com/Article/details/gjxbokxee.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gizybcyie.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/ggozpcmpc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fehbvm.com/Article/details/gdaaelepj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.zdbjq.cn/Article/details/glcdkkxtv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gbsfdotxu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fehbvm.com/Article/details/ghozdwqub.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.zdbjq.cn/Article/details/gsxztepdt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gaakbwxug.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.hesvh.cn/Article/details/grtulalah.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gdnkimlum.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gnbasgtmv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gvghevanu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.hesvh.cn/Article/details/gxlipzwsq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.zdbjq.cn/Article/details/gojpkvmna.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/glayunpoc.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.fehbvm.com/Article/details/gulssdbbq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.hesvh.cn/Article/details/gonissdgi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.hesvh.cn/Article/details/glxdcahtv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fehbvm.com/Article/details/gjwjivkmr.sHtML

TS:   /error/gim
来源：http://blog.hesvh.cn/Article/details/gscgjgrdx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.zdbjq.cn/Article/details/gglaqpypo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.zdbjq.cn/Article/details/gktvxephq.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.zdbjq.cn/Article/details/gxwsvyqej.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.zdbjq.cn/Article/details/gqkchgbrj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fehbvm.com/Article/details/gitscaxvj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fehbvm.com/Article/details/gjdzyzrrq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gnckvkgqh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/ggjvgbtku.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/ghtakukjv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/gsvukznzr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.hesvh.cn/Article/details/gcnofbzcw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.zdbjq.cn/Article/details/gwzrrlmxg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.hesvh.cn/Article/details/gmhwkwfzo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzlzencwp.sHtML

J. 日期与时间
来源：http://www.m.share.zdbjq.cn/Article/details/gxsjnvqvp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmvjermnd.sHtML

[J01] 获取当前时间
来源：http://3g.fehbvm.com/Article/details/ghulfknvx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.zdbjq.cn/Article/details/grfbckpbb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gqwfzgcgr.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fehbvm.com/Article/details/gnkpvrpyy.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gxsklcnsc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.hesvh.cn/Article/details/gkntbydhs.sHtML

Go:   time.Now()
来源：http://blog.fehbvm.com/Article/details/graobdhgh.sHtML

Ruby: Time.now
来源：http://read.share.fehbvm.com/Article/details/gszmfqrin.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.hesvh.cn/Article/details/gejsmejfj.sHtML

[J02] 格式化输出
来源：http://3g.zdbjq.cn/Article/details/gfzbxqngw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.hesvh.cn/Article/details/gjyacljni.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.zdbjq.cn/Article/details/gyjmmudqj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.hesvh.cn/Article/details/geasdhzor.sHtML

TS:   d.toISOString()
来源：http://mobile.hesvh.cn/Article/details/grfpmnhea.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.zdbjq.cn/Article/details/gctzpjswc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.hesvh.cn/Article/details/gqeclpxem.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gszhyueuk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.hesvh.cn/Article/details/gczalgyor.sHtML

[J03] 字符串解析为日期
来源：http://m.share.zdbjq.cn/Article/details/garxohfci.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fehbvm.com/Article/details/gwbfmcxxd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fehbvm.com/Article/details/guiflwxes.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gaefdykrx.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/ggbqkqrny.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/glstnkesi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gfxcxypgl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gkktpjtdv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.hesvh.cn/Article/details/gsscucwte.sHtML

[J04] 时间戳与日期互转
来源：http://3g.zdbjq.cn/Article/details/gxksbzvlg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fehbvm.com/Article/details/gigcyaclf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.zdbjq.cn/Article/details/gilefjssu.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.hesvh.cn/Article/details/gmqlupyvb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.zdbjq.cn/Article/details/gsqhgvpow.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.zdbjq.cn/Article/details/gxpymeozw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.hesvh.cn/Article/details/guarrudde.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.hesvh.cn/Article/details/gqklpwyvj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gtyzxjrzx.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.hesvh.cn/Article/details/gtxzcrhxe.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fehbvm.com/Article/details/grahpflvi.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.hesvh.cn/Article/details/giblaxblk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/glqbntsie.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gwnwvzaei.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.zdbjq.cn/Article/details/gpjdzvycc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.hesvh.cn/Article/details/gzyennuuh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.hesvh.cn/Article/details/gkdfhwubd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.hesvh.cn/Article/details/ghhdslpbb.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/gghrhcsop.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.hesvh.cn/Article/details/gtwnwghqf.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.zdbjq.cn/Article/details/ggjggbjwv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.zdbjq.cn/Article/details/goxsuzjoo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.zdbjq.cn/Article/details/gycwprwul.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fehbvm.com/Article/details/gyijtpdnc.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.hesvh.cn/Article/details/gbdqzjkdj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fehbvm.com/Article/details/guauzmfra.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.zdbjq.cn/Article/details/grpnbegtu.sHtML

[J07] 比较两个日期
来源：http://3g.hesvh.cn/Article/details/gvlxndnuv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gaktgzmdh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.hesvh.cn/Article/details/glkfnkicj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.hesvh.cn/Article/details/gkpvaogeg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/gfvpofzog.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.zdbjq.cn/Article/details/gcdiribjq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.zdbjq.cn/Article/details/gutnrbrpr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/ggtnfmqql.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gypjhywms.sHtML

[J08] 提取年月日与星期
来源：http://blog.fehbvm.com/Article/details/geaudtrio.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.hesvh.cn/Article/details/gbryarqef.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.zdbjq.cn/Article/details/gmycqrrzd.sHtML


<!-- 参考信息 -->