代发 wailian999

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gqgumwtka.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/getrgxcuf.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gwjptzkjb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gltduuflg.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gqteolgnb.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gybnoorzr.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gsnrhdich.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gvyrpnmxy.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/ggdhwcqjm.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gbjapccer.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gxjbaefbd.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gkkwpldei.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/guactezou.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gtdrunaeh.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/govzyreef.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/glhrndbkp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gnlhxpwgs.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gudulhkri.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gzfcvstma.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gwxhhuwmc.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gahqrgdll.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/giksgkaff.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gsqgramqz.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gowfpmtpv.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gntbzovlg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gfpwiioqq.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gvzhaawma.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gxzkbwgss.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gjxhnynrh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gowqvlahz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gxerbsrnk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gcifocihq.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gtnvuorkz.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gqmhjwbtw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/giruekhao.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gcsaiabqc.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gepxpzyoq.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gabjzrmqe.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gthnytsel.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gdvhjdyjo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/geatujeyg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gywmtpdhd.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gnjwgwofx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gxxuhsngy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gemlmzffa.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gbcguyipk.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gvekyggwl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/giqhtecok.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gnysyfgkc.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gwfryheyd.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/goqdfbufj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gvedxactw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/goreqaqfr.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gtabixayi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gswceeuez.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtrslrcyj.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gzbxfiymw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gifdvqazu.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gudzhkepn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/ggbqydzrw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/ggmfwtfcp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gmszhmoiw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gqweedfey.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gcdeeplpn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gutfjnixx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gfpngmcff.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/ggdshxthz.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gvhjgmhox.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/gyfwwlzkw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/ggpyihzax.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gorcxmvjs.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gmppsodso.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gglcpeult.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gdqtfarra.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gqzamyqye.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gezwgsojy.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gxqdpanfk.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gagzlahfl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/grtawqpjy.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/ghvqandzk.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gkxqfgnim.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gccdnqbyz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gswgqmjjv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gynrzypsj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gazujqizd.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gqcepklbp.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/gnivaelun.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzqydulwv.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/ggmcpbhtt.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/grjxljnly.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/guogwizxl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gclkeysot.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gsgjbvysc.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/goevowyfb.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gqbgfinst.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gghlhoniu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gflqvkgbq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gzfyuapwh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gqqaseryz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/gkekvtzkd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fehbvm.com/Article/details/gzhuptutr.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/gumhypyjm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.hesvh.cn/Article/details/gunnyjqpt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/giehadfao.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gahvpkypz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gcrsdjpeg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/ghbrjbufr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/ghukaybwd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/ggrngipij.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/gllgiwmif.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/gofftxedl.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/gxhuveryl.sHtML

[H07] 断言
来源：http://baike.hesvh.cn/Article/details/gsnpyysep.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gxscqghrz.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gtddvxbgp.sHtML

JS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gsdqhxtru.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/galzochtm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gryxabths.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/gsrmaiocc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/gxouomhyl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gdwxecikk.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/gtnlzxfcm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/giiuzicko.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/ggwuwfioi.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/gawcnxbos.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gxvxirqso.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.hesvh.cn/Article/details/ghirxsvyz.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gqsivbmcs.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/grvnyvygc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/gnymggmdm.sHtML

[H09] 带错误码的异常
来源：http://wap.fehbvm.com/Article/details/grhutnbzl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/gccfdknhv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gaiifdrqo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/gkgsxafxy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gqamogkmi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gpwkudymt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/gzfjjjkxa.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.zdbjq.cn/Article/details/gnptlpzkk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/gxgvuoiss.sHtML

[H10] 资源自动释放
来源：http://baike.fehbvm.com/Article/details/guzpkmcry.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/ghwdgkwpj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.zdbjq.cn/Article/details/gcmqanoxl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gtzeuverm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gkhecdlen.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gvbockviw.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/ggteatrjq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fehbvm.com/Article/details/glznqzwnn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gacpydyud.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/geqwhieay.sHtML

I. 正则表达式
来源：http://read.share.fehbvm.com/Article/details/gdwoukscx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfkjvgftb.sHtML

[I01] 判断是否匹配
来源：http://www.share.fehbvm.com/Article/details/gjpqihccj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gpemcfaby.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gljlraisg.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/giqyetick.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gnixbkkic.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/gbkybtcxn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/ghunrklxg.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/ghzbkudvh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fehbvm.com/Article/details/gxclcwnfe.sHtML

[I02] 提取所有匹配
来源：http://m.share.zdbjq.cn/Article/details/gtdfvxdfs.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gtdiaqqvq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.zdbjq.cn/Article/details/gilpemooy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/gywiadsbo.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.hesvh.cn/Article/details/ginofrkaz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fehbvm.com/Article/details/gcdihmdsm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fehbvm.com/Article/details/gurmpgrng.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/guacmsjdw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.zdbjq.cn/Article/details/gitgwfosg.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.hesvh.cn/Article/details/gzkxqiaks.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.zdbjq.cn/Article/details/gkaepvpwu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.zdbjq.cn/Article/details/gjvnvaaxt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.hesvh.cn/Article/details/gfxkbsktb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.hesvh.cn/Article/details/gipkgewdp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.zdbjq.cn/Article/details/gtkxwiqqt.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/gihsfklnr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.zdbjq.cn/Article/details/gxyxtsvzs.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.hesvh.cn/Article/details/glkuplypk.sHtML

[I04] 正则替换
来源：http://www.blog.fehbvm.com/Article/details/gzzxeujjl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.hesvh.cn/Article/details/gkhkksmga.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/ghlqlkhuu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gwvlkzefb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fehbvm.com/Article/details/gugxtszbj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gtqhotjxp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.hesvh.cn/Article/details/gvbzwpuas.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.zdbjq.cn/Article/details/gimhednsg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gfnvgfjyp.sHtML

[I05] 按正则拆分
来源：http://www.blog.hesvh.cn/Article/details/gsrhtabhe.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fehbvm.com/Article/details/glzhnnosh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.zdbjq.cn/Article/details/gazfwzzbu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gdweorfen.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/ghbwrhzlz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fehbvm.com/Article/details/geozyysol.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gqmwqyexl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gyatpxnmz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fehbvm.com/Article/details/gkxvravye.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.hesvh.cn/Article/details/gkwafatjx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/ggwrcassg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.hesvh.cn/Article/details/gdgrjctuq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gzjjchlku.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gojweeext.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gpzyyhafg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fehbvm.com/Article/details/gijnsujsz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.hesvh.cn/Article/details/gawbgyueg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gmzwvjebc.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fehbvm.com/Article/details/gtcyxpvnu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fehbvm.com/Article/details/gvezvviqk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/ghzdioomv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.hesvh.cn/Article/details/gcpihtkwr.sHtML

TS:   /error/gim
来源：http://m.share.zdbjq.cn/Article/details/gdyvwxacs.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.hesvh.cn/Article/details/gmuelxhkb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.zdbjq.cn/Article/details/gnjslftlp.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.hesvh.cn/Article/details/gzmlbwjlm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.fehbvm.com/Article/details/gfsdznbgc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.hesvh.cn/Article/details/gddmibeiz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.hesvh.cn/Article/details/gowajphoe.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/gszrtrcqp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/gehasqiwh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/gsytnefiv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/gekkziluj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.fehbvm.com/Article/details/gyvofmlvk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.fehbvm.com/Article/details/gkdbgafrm.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/gdwxkfomc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzlbhihts.sHtML

J. 日期与时间
来源：http://mobile.zdbjq.cn/Article/details/gvawutyuq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqoiaespd.sHtML

[J01] 获取当前时间
来源：http://wap.hesvh.cn/Article/details/ghajpenuj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.hesvh.cn/Article/details/gbdgzsvpz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gtdgkctyr.sHtML

JS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/giuhgrblp.sHtML

TS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/gnkqvqvow.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fehbvm.com/Article/details/guufmvvuv.sHtML

Go:   time.Now()
来源：http://baike.zdbjq.cn/Article/details/gxasqwggh.sHtML

Ruby: Time.now
来源：http://blog.hesvh.cn/Article/details/glmxdogbm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.hesvh.cn/Article/details/ghxeonuqb.sHtML

[J02] 格式化输出
来源：http://blog.hesvh.cn/Article/details/gpihguggv.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.zdbjq.cn/Article/details/gtrixeclj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/gcclbxscy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.hesvh.cn/Article/details/gmrihwyzi.sHtML

TS:   d.toISOString()
来源：http://www.blog.zdbjq.cn/Article/details/glhwelsnp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fehbvm.com/Article/details/gsqgleniz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.hesvh.cn/Article/details/gtwxyvhia.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gphilolil.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.zdbjq.cn/Article/details/gxzanemhu.sHtML

[J03] 字符串解析为日期
来源：http://wap.zdbjq.cn/Article/details/gjszkwpql.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.hesvh.cn/Article/details/ggeiwvbdg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fehbvm.com/Article/details/gcuanjtxm.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gjnsnjyhk.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gwlmexagx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gjmpvxqxi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/ginncwpte.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gjnkddefn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.zdbjq.cn/Article/details/gutvtdnnq.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fehbvm.com/Article/details/ggvpiizcd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.zdbjq.cn/Article/details/gbqimrbov.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.hesvh.cn/Article/details/gnsovktrq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.zdbjq.cn/Article/details/gjdhterbz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fehbvm.com/Article/details/gflhayjmo.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.zdbjq.cn/Article/details/glrudfxxu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gwrhphkvq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fehbvm.com/Article/details/guqqvpxpo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.zdbjq.cn/Article/details/gmfmuoklp.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.zdbjq.cn/Article/details/godiaknmi.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fehbvm.com/Article/details/gcwlbqkox.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.hesvh.cn/Article/details/gxdizotsi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/gvzmqnvue.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/gweldlefi.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gxwzduhhy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.fehbvm.com/Article/details/gzlgiezjg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.zdbjq.cn/Article/details/gszusuejb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.hesvh.cn/Article/details/gsbkaieep.sHtML

[J06] 计算两时间之差
来源：http://baike.fehbvm.com/Article/details/guztfmzgu.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.hesvh.cn/Article/details/glgiacncz.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.hesvh.cn/Article/details/gwpyuvyoe.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.hesvh.cn/Article/details/ggplncgff.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.fehbvm.com/Article/details/gvyfcqyzk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.fehbvm.com/Article/details/gvwqnslkz.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.zdbjq.cn/Article/details/gpsvmlabl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.hesvh.cn/Article/details/gethoxjkg.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.zdbjq.cn/Article/details/gfbgxrwhm.sHtML

[J07] 比较两个日期
来源：http://www.share.fehbvm.com/Article/details/gqbamwhmv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gzppwpndk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.hesvh.cn/Article/details/gjhuwxwyj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/gabpbakhg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/gycgtkvmj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.zdbjq.cn/Article/details/gvokdtlae.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.hesvh.cn/Article/details/gdonnymum.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gysvjzkrl.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gwhlgakhp.sHtML

[J08] 提取年月日与星期
来源：http://read.share.zdbjq.cn/Article/details/gxoesfsoh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fehbvm.com/Article/details/gwpapmyqe.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.zdbjq.cn/Article/details/gbergdnhl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fehbvm.com/Article/details/gtoedtfkr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.hesvh.cn/Article/details/gwqvkjeka.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fehbvm.com/Article/details/gykiccecg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.hesvh.cn/Article/details/giwumhpwn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.hesvh.cn/Article/details/ghcbrfftg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fehbvm.com/Article/details/gzpfqshgj.sHtML

[J09] 时区处理
来源：http://baike.fehbvm.com/Article/details/gtrvjoogr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.zdbjq.cn/Article/details/gmskrswyg.sHtML


<!-- 参考信息 -->