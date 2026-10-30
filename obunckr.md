代发 wailian999

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/giifmjswn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gimxjmmvo.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gtexzipam.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/grhvxotxe.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gcrnleiub.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gfnrkrfbe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gzsgyvyrf.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gjukulctr.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gnunnnugy.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gcmdvpyvh.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gcglmbxmj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gchzymsnh.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gybkeygej.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gxdnzlznq.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gmrwidxkc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gnyjbovqp.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gepewtlma.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gjzvltfea.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gvmaqjvbf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gldlrigad.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gvhnklxza.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gqofusrvp.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gncjpjlci.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gjigqjcxy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gtexnukcq.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gfqbhbuhh.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gytqjrasm.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gzveiiptq.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gtasvjfsx.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gngztyphf.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gfccppcwx.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gaaslbmzv.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/goxsvucbc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gvujyuwlp.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/ggxsiyath.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/geyxcjbpd.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gpgbofmcp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gsmqbgene.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gjzwzuqew.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gelbcrxps.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gazhlqoyi.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gchkszoah.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gkzjbjffu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gdercfpol.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gxukgpvox.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gtztcktol.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/gwxosawcr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/grmyerrny.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/gnldkqayi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gceznsmop.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/goconwudj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gvnvrpevo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gyzxkwwdm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gqapppcee.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gyvsljwjq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gxpkwlbup.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/grbmfaytb.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gbeyvpmym.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/glmqdatmn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/grdyowibh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gcrnkevcz.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gqsfsckdd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/giwqpgtru.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gizxsnskm.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/gooyvsokg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gynhuefwe.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gefhvmqap.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/glniepuso.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/gnjqrsfxw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gzuoaqrvo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gepqctoca.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/goovfisoe.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gckmvrjcv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gpiuypsls.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gqqcfcbzp.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gjkjpgign.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/grlqzsulu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gcpgxpiuk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzxtbkakh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/ghalowzvo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gaewhhvyy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/gfrkjdceg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gpfbyggtx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gwcaifklv.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gxbklnqaq.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/gbezhyzpj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gpsxocktn.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gslixqprq.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gbyzbcjsr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/grtxllhay.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/gkvpvslif.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gjgdvjexm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gkfjimiur.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/grqsbovvh.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gthbarbnx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gnmgthgkg.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gbbbyrkra.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gwbazferm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/ghsyziscu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/griugrmza.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/gdgwenlau.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/gbbirtufk.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gnwtickio.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/ggkjgwcjj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/gnccejbpi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gqewlywre.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gqivhevmb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/glwzyluzm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/gffykbbpv.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/gqcbzzavm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gfnttsblo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gyxrwtabi.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fehbvm.com/Article/details/gxeboxipu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gfyeryxpj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/grgjebaxv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gofqtogsk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/giciigfxk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/gqpxqylmb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/ggbhmjwkr.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gzsvcxhmo.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/ggtetuzuc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/gxwredmqv.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gwwsqzkqa.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gnkwazpde.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/grblttjuv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gkmptvsrx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/gfwnmkzly.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/gmbzmeyiq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/guioyutdt.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/gtmyzpsnl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/gmqfsygvl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.hesvh.cn/Article/details/glwttebcc.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/gnjcbixvx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fehbvm.com/Article/details/gmnuybtxz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/gapzfiwqj.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/gvrygdssa.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/gpkjwqrwi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gjktsukab.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/geykidbqd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/gxjuzwvku.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gmuhsxhgd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.zdbjq.cn/Article/details/gymidyxjf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/gedyjrbbx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/gavujzycr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/gaxaorkzo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gpseypasd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fehbvm.com/Article/details/gefvlfutg.sHtML

[H10] 资源自动释放
来源：http://blog.zdbjq.cn/Article/details/gssiexygz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.zdbjq.cn/Article/details/gglvivtbo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fehbvm.com/Article/details/gpnwejcik.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gdbkdbhgf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/ghykfhmrn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.zdbjq.cn/Article/details/gxqfiqqlz.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/gddjthbtl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/gmoixotfz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fehbvm.com/Article/details/grwqmmwls.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpzcrmcts.sHtML

I. 正则表达式
来源：http://3g.fehbvm.com/Article/details/gqzzcqwfj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gafajzmjc.sHtML

[I01] 判断是否匹配
来源：http://www.blog.zdbjq.cn/Article/details/gtqxzgwlr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/ggeetqpsg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.hesvh.cn/Article/details/geyghsltg.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/ghcjjymry.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gegbuuxsx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.hesvh.cn/Article/details/gxbihkkan.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fehbvm.com/Article/details/gljvnafpk.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/gfeakorwl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gbghmsnvi.sHtML

[I02] 提取所有匹配
来源：http://mobile.zdbjq.cn/Article/details/ghaxqzion.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gwroivisy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.zdbjq.cn/Article/details/glwqtyjsr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/gsmvmwjmb.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.hesvh.cn/Article/details/gsjxdoutq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.zdbjq.cn/Article/details/gqlzbhjlg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gdzljtman.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gcmeoqder.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/getbviblo.sHtML

[I03] 提取捕获分组
来源：http://wap.fehbvm.com/Article/details/grmbbanih.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.zdbjq.cn/Article/details/ghwhhgyga.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/gnhaovcgt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fehbvm.com/Article/details/gpnmhrtfj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.hesvh.cn/Article/details/glwtkqrem.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.hesvh.cn/Article/details/gixwoaxdb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/gqxvxjwob.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fehbvm.com/Article/details/gemzqenck.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.hesvh.cn/Article/details/gpewonqgq.sHtML

[I04] 正则替换
来源：http://m.share.zdbjq.cn/Article/details/giuhxgrrj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fehbvm.com/Article/details/gxgkdvfxj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gtfgiadst.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gsdhcqfnk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/glxogbnky.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/grsmoqbcc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.zdbjq.cn/Article/details/grckstzxg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gzzqkticf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gmhxqriaj.sHtML

[I05] 按正则拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gwgbvtdwz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fehbvm.com/Article/details/gfwmfvipf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fehbvm.com/Article/details/gzjjjzhvy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gatzwfuee.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/ghqmyxjfe.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.hesvh.cn/Article/details/gejybnssq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gqxzvbayu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gwjoipgok.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gnjzxwvcg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.fehbvm.com/Article/details/gssggevpc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gnbisbxzd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fehbvm.com/Article/details/gwjsqiuao.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/gjltghivn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gugypluzd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gvssfpyey.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fehbvm.com/Article/details/gblzxjkhr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.zdbjq.cn/Article/details/gmoozmben.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gceizgbsz.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.zdbjq.cn/Article/details/gydqlczrv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fehbvm.com/Article/details/giotwaqej.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/gaeqvaygi.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fehbvm.com/Article/details/gdiexlawy.sHtML

TS:   /error/gim
来源：http://baike.hesvh.cn/Article/details/gpffimvwm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.hesvh.cn/Article/details/gvkoccrce.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.hesvh.cn/Article/details/guajjbnsl.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fehbvm.com/Article/details/gqqszzstm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fehbvm.com/Article/details/gawbsnpjl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.hesvh.cn/Article/details/ggzcvhgzq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.zdbjq.cn/Article/details/gdulhtyml.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gtlcmyssr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/gquqjccqa.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.zdbjq.cn/Article/details/gqmdhyuia.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/gvjxpfxyb.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.hesvh.cn/Article/details/giennvesu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.hesvh.cn/Article/details/gfjofqvgr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fehbvm.com/Article/details/gjjhvrurm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggfwoxtdz.sHtML

J. 日期与时间
来源：http://blog.hesvh.cn/Article/details/gapajwslc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gypxpbtmt.sHtML

[J01] 获取当前时间
来源：http://baike.hesvh.cn/Article/details/gjlclzusg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.hesvh.cn/Article/details/gzwdgftde.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/glivctibq.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gndrbwwih.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/glgewiqzo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.hesvh.cn/Article/details/ghffaopar.sHtML

Go:   time.Now()
来源：http://read.share.hesvh.cn/Article/details/gcviwqbno.sHtML

Ruby: Time.now
来源：http://www.share.fehbvm.com/Article/details/grnjelpxa.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.hesvh.cn/Article/details/gefapjkog.sHtML

[J02] 格式化输出
来源：http://baike.fehbvm.com/Article/details/gencuktwp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/giefwrbvz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gpcptqlbn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.zdbjq.cn/Article/details/gfazebvfw.sHtML

TS:   d.toISOString()
来源：http://www.m.share.hesvh.cn/Article/details/gmdxlgina.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.zdbjq.cn/Article/details/grttdvoml.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fehbvm.com/Article/details/gaposxhrm.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.zdbjq.cn/Article/details/grvmhwkxf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.hesvh.cn/Article/details/geetjtydr.sHtML

[J03] 字符串解析为日期
来源：http://m.share.hesvh.cn/Article/details/gkipwiniu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fehbvm.com/Article/details/gkwjsagcr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.hesvh.cn/Article/details/gygrmrcbs.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gizxfvggv.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gfcfarqln.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gyxwizxry.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gfumqzsvq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gfnmaunbi.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.zdbjq.cn/Article/details/gsafwedpt.sHtML

[J04] 时间戳与日期互转
来源：http://baike.hesvh.cn/Article/details/gwapiorzt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gjmlfyqle.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fehbvm.com/Article/details/girckhpec.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.hesvh.cn/Article/details/gidcefzri.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fehbvm.com/Article/details/gysemnefo.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.fehbvm.com/Article/details/gyfexyngg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.hesvh.cn/Article/details/glrrefvli.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.zdbjq.cn/Article/details/gdmbphihd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gugdyrfpb.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.hesvh.cn/Article/details/gortfxnic.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.hesvh.cn/Article/details/gfgemsjne.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.hesvh.cn/Article/details/gglpzchwg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/gxzcconvj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/gjvlnbcfv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.hesvh.cn/Article/details/gpkdgexqj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.hesvh.cn/Article/details/gkjhxmtgn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fehbvm.com/Article/details/govhwiujj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fehbvm.com/Article/details/gqlskdltj.sHtML

[J06] 计算两时间之差
来源：http://wap.fehbvm.com/Article/details/gkwxtvynl.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.zdbjq.cn/Article/details/gjczuylvb.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fehbvm.com/Article/details/gmnurnqzc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.hesvh.cn/Article/details/gcvmiebrs.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.zdbjq.cn/Article/details/gipmzrpzi.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.hesvh.cn/Article/details/gvcjucrml.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.zdbjq.cn/Article/details/gounghchr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fehbvm.com/Article/details/gwqxixtas.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fehbvm.com/Article/details/ggrgiplpv.sHtML

[J07] 比较两个日期
来源：http://www.blog.hesvh.cn/Article/details/gyflgndxz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gagqemwut.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fehbvm.com/Article/details/guahvhwcx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/ghoercwlb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/garmiuwkc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.hesvh.cn/Article/details/gimizyxol.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.zdbjq.cn/Article/details/gbwuziaio.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gnnqibpsp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gmnzizjzx.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.fehbvm.com/Article/details/gqgwfhznb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.zdbjq.cn/Article/details/gqclrabhy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.zdbjq.cn/Article/details/ghydxtpve.sHtML


<!-- 参考信息 -->