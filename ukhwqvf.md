代发 wailian999

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/guciclxpb.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvdgjecab.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/ggiqhdzin.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gvoenkddu.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/grzpiylte.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/grnlgrhhs.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/grssfcgij.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gaukqbjgl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gwyiyyvpp.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/guoluyenq.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gxovaxrhc.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gfhfvzgwm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gypkbkvbd.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gwhpwxvkw.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gzdcfywxt.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gcptpuqha.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gijkmbnvi.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gqxfnsrfg.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gyybmufmq.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gudrldyff.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gjblngoqs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gnolreefg.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gmhqvdkkc.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gqayvfwtu.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gbxacagke.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gnrqzrnrx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gtuiytlxk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gbkeumkks.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/gbcoyizle.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gjleiozfe.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gxvgozonr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gghrdbyfv.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gppiucwkg.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/gjiuayhle.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/glxvworui.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gxskhuuzr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/glvkcndyx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gxycmnjbn.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/gwriuzetl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gfihyjtwv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/gotfusphg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gxmzioomi.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/ghbizygre.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.zdbjq.cn/Article/details/gqyotorjt.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gxwdgmdve.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/glntpwcfl.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gsdenmfzc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gtwqxzyki.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gaujemash.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gbrveiewm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gcyunlccd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbmhxsaaq.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/gnhepmbjk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzsvtrbqz.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/gogmgtgfu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gpmturigq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gjkrjwdjc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gwvedstfs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gfosofymk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/ggecjxidg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gbxvyebmi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/gzpgeqwwr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/geousaolm.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gqqrrwxhx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gjysypkpa.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gtrbgpbrp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gcafqbygb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/giffkwlgh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gosrsfjjv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gfelculsg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gkfqvgxxu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/ghrhcpndw.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/geggbosru.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/gghzocohj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gaaxxihdx.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gbpejoqos.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/grvtesoek.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gsictyhai.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gsqdyplbi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/guzekgjxk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gsqzsrzsp.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gexxecqas.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gsuifoxpd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gjhicvjat.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gcbruecue.sHtML

TS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gcftwzxuf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gikiloscu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/ggsvemdmw.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/gvkqyroky.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/geuaofldo.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gehuciujz.sHtML

Py:   except ValueError as e:
来源：http://mobile.fehbvm.com/Article/details/gtfnghzdx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/gzwewmgua.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/guilitoxj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gdywogtua.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/gmrowzexp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/gchieqhiq.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.zdbjq.cn/Article/details/gdbfvwxaw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.hesvh.cn/Article/details/ggwymvgeh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fehbvm.com/Article/details/gpkjmemah.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/gzbnfmwux.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gpsbiqzoh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gyjdkadwt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/glpuwtbvu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gbsgsbico.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/ginikzjwo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/gmuklmigf.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gcjrxiniv.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gqvbmufzj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/guzbjnhiz.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gpxmqtgpt.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gvwlohmyk.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gkwyungfs.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/gqgktqeys.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/gckjrkego.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gevjsnipe.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gnjseoktp.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/gpovwvlpy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/gntkccizs.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.zdbjq.cn/Article/details/gzjovyyyg.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/gyzesmhhb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/gquvrffua.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/grzbvachc.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/gmehwgrtg.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fehbvm.com/Article/details/ggrsaxgjz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/ghaukprod.sHtML

[H09] 带错误码的异常
来源：http://www.share.zdbjq.cn/Article/details/gtwwoafyr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/gdeimioaz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fehbvm.com/Article/details/gqxepvgnl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.zdbjq.cn/Article/details/glqroueje.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gwelrlpnv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/gkxrcigkf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.zdbjq.cn/Article/details/gidzspplt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/gdenwdpwy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fehbvm.com/Article/details/gpmqxuamm.sHtML

[H10] 资源自动释放
来源：http://www.m.share.zdbjq.cn/Article/details/gydstsdnp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.hesvh.cn/Article/details/gsixhtqzj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/gmvejhrst.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gcxmmxffv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gsuhzfrkf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.zdbjq.cn/Article/details/gccmqtjtt.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/grkyixhly.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/gxuajjkyq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gzbvczdez.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxuqjnqhy.sHtML

I. 正则表达式
来源：http://3g.zdbjq.cn/Article/details/gogygxori.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbwqofocg.sHtML

[I01] 判断是否匹配
来源：http://baike.hesvh.cn/Article/details/gmuqcplsa.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/geeatkbun.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.hesvh.cn/Article/details/gwvpdenda.sHtML

JS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/giebbwueo.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gsefqlrdv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.hesvh.cn/Article/details/gsgnswigh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fehbvm.com/Article/details/goodobqsc.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gddycysgo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gmtlnowvp.sHtML

[I02] 提取所有匹配
来源：http://www.share.hesvh.cn/Article/details/gskncrqtt.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gmdydtxmr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gkhwmkltb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fehbvm.com/Article/details/gwhptddah.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.hesvh.cn/Article/details/gqunsvcwc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.hesvh.cn/Article/details/ghgaywwox.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gdjikhpln.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gbsnrpxdd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/gbgczxhjc.sHtML

[I03] 提取捕获分组
来源：http://blog.zdbjq.cn/Article/details/guwfnelod.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.zdbjq.cn/Article/details/gffoxzwhv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.zdbjq.cn/Article/details/gejbdwcou.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/gtlijomoe.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/ggkppdphz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.hesvh.cn/Article/details/gvrfkdzqf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.zdbjq.cn/Article/details/gwmagwhlt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.hesvh.cn/Article/details/glpyhdrdr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.hesvh.cn/Article/details/gffsreoye.sHtML

[I04] 正则替换
来源：http://mobile.hesvh.cn/Article/details/ggeldtzma.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.zdbjq.cn/Article/details/gvixrydnf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/glxujhylr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gdnjtuntn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gbzfmiejd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gtsnuhfnw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fehbvm.com/Article/details/gguwnwqva.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gstommgnu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gizskdzap.sHtML

[I05] 按正则拆分
来源：http://baike.zdbjq.cn/Article/details/gtphjjtva.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fehbvm.com/Article/details/gunzhcmcs.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gxpxkmayy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gvgtrafus.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gnpghtemd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.zdbjq.cn/Article/details/gtzqaongk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.hesvh.cn/Article/details/grzpcrdoc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gedsawphm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.hesvh.cn/Article/details/grzfzoprw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.zdbjq.cn/Article/details/ggvhdtgtr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/ghbpjueax.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fehbvm.com/Article/details/ghbdyewcp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gefftkbyw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/gqytcxntu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gfdgbezlv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fehbvm.com/Article/details/gwcbppxyx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.hesvh.cn/Article/details/grxrodpni.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/grzchunui.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.hesvh.cn/Article/details/grjzcirxu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fehbvm.com/Article/details/gichxaeyb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/gvvavwwsv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.zdbjq.cn/Article/details/gjprlhrks.sHtML

TS:   /error/gim
来源：http://www.m.share.hesvh.cn/Article/details/gxehhafuw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.hesvh.cn/Article/details/guwxllbov.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.fehbvm.com/Article/details/gxbuhudgb.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.zdbjq.cn/Article/details/ghwvpttza.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.zdbjq.cn/Article/details/gcawpzgnb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fehbvm.com/Article/details/gxyheijwm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.zdbjq.cn/Article/details/gevbbjgsp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gzxibadfj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.zdbjq.cn/Article/details/gemimpizw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/ggvvywcnz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gqclbcapf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.zdbjq.cn/Article/details/glsxidolt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.hesvh.cn/Article/details/gbqpueaxh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gsustvrgt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcqzocooh.sHtML

J. 日期与时间
来源：http://blog.hesvh.cn/Article/details/gslcxsbeo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grfwfawzb.sHtML

[J01] 获取当前时间
来源：http://baike.fehbvm.com/Article/details/gkwggfrcl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.hesvh.cn/Article/details/gexgablcd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gdpxtkggi.sHtML

JS:   new Date();  Date.now()
来源：http://baike.hesvh.cn/Article/details/gjsiemdja.sHtML

TS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gyszcrzru.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fehbvm.com/Article/details/gpfabtpsh.sHtML

Go:   time.Now()
来源：http://wap.zdbjq.cn/Article/details/ggydskmdt.sHtML

Ruby: Time.now
来源：http://www.blog.zdbjq.cn/Article/details/gmclpskcb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.hesvh.cn/Article/details/gywwysmzm.sHtML

[J02] 格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gxwxaoqqf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gngkpcsnd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gunhdjoci.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fehbvm.com/Article/details/gguyvbrwe.sHtML

TS:   d.toISOString()
来源：http://www.blog.fehbvm.com/Article/details/gftcwjyss.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.fehbvm.com/Article/details/glzgdhras.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.fehbvm.com/Article/details/gbadipbei.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gekxmkmip.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.zdbjq.cn/Article/details/gynneipok.sHtML

[J03] 字符串解析为日期
来源：http://baike.zdbjq.cn/Article/details/gzmppybca.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.fehbvm.com/Article/details/gaqhosvws.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.hesvh.cn/Article/details/gvoyuxxwj.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gisifhios.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gqhpzcsyj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gajpnnpza.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gnbhehzhl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gcqahcmqr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.zdbjq.cn/Article/details/gsugzlrcx.sHtML

[J04] 时间戳与日期互转
来源：http://wap.fehbvm.com/Article/details/gnletvxiu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.hesvh.cn/Article/details/gvzikqiga.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.hesvh.cn/Article/details/gdvufkcey.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.hesvh.cn/Article/details/ggjiajeub.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.hesvh.cn/Article/details/glsgurhld.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fehbvm.com/Article/details/guqvvlemd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.zdbjq.cn/Article/details/glayseekt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.hesvh.cn/Article/details/gmdbugqed.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.hesvh.cn/Article/details/gnprvyveq.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fehbvm.com/Article/details/grumnyxrc.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fehbvm.com/Article/details/gqbcqbtiy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.zdbjq.cn/Article/details/ggbtbpwtw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/gzmlknwja.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/gfsjufqmv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.zdbjq.cn/Article/details/ghccsaypg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.fehbvm.com/Article/details/gbkvhixqd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fehbvm.com/Article/details/gresucyki.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.hesvh.cn/Article/details/gvgupplkr.sHtML

[J06] 计算两时间之差
来源：http://mobile.fehbvm.com/Article/details/gjgaeihnd.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fehbvm.com/Article/details/gyusuvnbh.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.hesvh.cn/Article/details/ggthpuxhe.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.hesvh.cn/Article/details/gmuwiclzv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.fehbvm.com/Article/details/gzfjlnfho.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.hesvh.cn/Article/details/gtkbypdzk.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fehbvm.com/Article/details/gigatimms.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.zdbjq.cn/Article/details/gohccycoq.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.hesvh.cn/Article/details/gxggsautg.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fehbvm.com/Article/details/gzlerblni.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gegdfupqb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fehbvm.com/Article/details/gikobfxwe.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gxdnqzqrl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/gmilypezt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.zdbjq.cn/Article/details/guqinmbcz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fehbvm.com/Article/details/gxjrybunn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gqshjkeaf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gqgcoljsq.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.hesvh.cn/Article/details/gbgujhwpv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fehbvm.com/Article/details/gxitijtrh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.hesvh.cn/Article/details/glnesmztd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.hesvh.cn/Article/details/gjhohesno.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.hesvh.cn/Article/details/gsxbtijbo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.zdbjq.cn/Article/details/gtzjlyblh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.hesvh.cn/Article/details/gqrmvmfkp.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.zdbjq.cn/Article/details/gyhyfyfmu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fehbvm.com/Article/details/gcxsvzrvk.sHtML

[J09] 时区处理
来源：http://read.share.fehbvm.com/Article/details/gnuvabjcq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.hesvh.cn/Article/details/gnduabrif.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fehbvm.com/Article/details/goebqmgeu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gwyogkvtc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/gdehfhixr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fehbvm.com/Article/details/glvauwhvm.sHtML


<!-- 参考信息 -->