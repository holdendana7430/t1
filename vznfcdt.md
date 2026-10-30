代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gvxhzdnjo.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/goqgvdttt.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/ggouvvmdm.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gibmcfksn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gfondefix.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gsugihpdi.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gyckzrevs.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gtcrdrpia.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/geikwkxol.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gtclrenlb.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gdofeyljb.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gynaurtmv.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gzidkmeuu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/grynaosuw.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/giozxjzby.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gwqlrpiuv.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gtzodixqc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gjqjggype.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gvwxptwsb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gkvwngofw.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gowocrbbq.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gdwbjbtkj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/ggpbaqcil.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gjttrdkdd.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/ghlulehfi.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/ggdrvisky.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gjkybvfvj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gkisnbzpj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gseamfhxf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gkuemweud.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/ggygihzot.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gcjiocjni.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gbkhcpmnf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gxlblnaim.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gxludpdnu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gwubrejrj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gxxkgvmza.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gtrtkpdaz.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gceadillu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gvuinfxth.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gyjaninzx.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gtyyypgfx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gzlorurie.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkgjrdttr.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/goxhmrbvv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbvxmvydr.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gttkmvmqc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gjjdudban.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/ggulbbckp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gmgkdkojo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/grtbvutfk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/ggzzfonab.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gfcyrlwxz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gyzjjmpru.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gzydjutyv.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gaonjmdkn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gxrbrmsrv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gtkxurgho.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gltmfxvrp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gtmukyavb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/ggldbxogr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/gxfbscxho.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/gsmllliuc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gkbsaartm.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/gctkdknhb.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gvyyjttsy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gcsolmrao.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/giejywgih.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/goqtwygmr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gkfqfvbjz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/gylfzmoyr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/gyjhnajcb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gncaqblju.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gsuscpmnf.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/glofrmppj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gipeqbnyt.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gvndqhefh.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gilbjocvx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/ggzfibkvo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gdijnapdn.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gqharqpwq.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/gcwekqojs.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gmmztdsoi.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gzsmlmaal.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/glxsrghuy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gkdlhyldv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/ghpoxhjjg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gnrxkahrj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/gimggtwpz.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gwhvosxnz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/gdbldslxc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/ghbyooljh.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/ghldvwcsi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/glrgzzokt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gndekroda.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gtqrtborn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/gelotwuxp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/guleszhzm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/gsfnatalk.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/ggwpoqzxq.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gfyshfvpr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gejzbqrqr.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/gdnnochnz.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gvzouncgr.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gaiulxrzy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gmljlffkh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/ggpxmbkrq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fehbvm.com/Article/details/gdmyzanxb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gegexfoil.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fehbvm.com/Article/details/gjxweiork.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/gyzvuwsqw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gtqswtvii.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/gqtiffdbs.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fehbvm.com/Article/details/gkfhtwzfv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.hesvh.cn/Article/details/gpyuigyzv.sHtML

Go:   err.Error()
来源：http://www.m.share.zdbjq.cn/Article/details/gwteshmes.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fehbvm.com/Article/details/gpvnezmhi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fehbvm.com/Article/details/gylkhvspr.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/gmproljxf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/gpmnimnku.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/gdbxqqkmf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/gshmhexvr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gxylbfolu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.hesvh.cn/Article/details/gjpgicxnp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/gjswwxxef.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.hesvh.cn/Article/details/ghbctvzwm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/ggsjyfeta.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/gstukopvp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/gbpcxmbba.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/gcvnqpagz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gthycmubn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/ghzhxvtoo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/gagnwnjwf.sHtML

Go:   defer f.Close()
来源：http://www.m.share.zdbjq.cn/Article/details/ghdxlpupu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fehbvm.com/Article/details/garuxlfbl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gbwzqnklg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvimobjru.sHtML

I. 正则表达式
来源：http://mobile.zdbjq.cn/Article/details/gwkziiyaj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwbaflrlr.sHtML

[I01] 判断是否匹配
来源：http://read.share.fehbvm.com/Article/details/gvjmrvzgr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gjqylkyop.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.hesvh.cn/Article/details/gneqdzfzm.sHtML

JS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/grwuseoya.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gqniupmzg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/gsunyvqce.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/gyhbehjtc.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gkchptgzi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/gxyhcivaa.sHtML

[I02] 提取所有匹配
来源：http://www.share.fehbvm.com/Article/details/gqakvibrf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/glravpjcl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.hesvh.cn/Article/details/goznfsthj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.zdbjq.cn/Article/details/glydggabs.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/gtpcxodmf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/gffoczpgu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/ggmdaitlj.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gxyxiygwz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.hesvh.cn/Article/details/gpatdknit.sHtML

[I03] 提取捕获分组
来源：http://www.share.zdbjq.cn/Article/details/gxdxwxpvv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fehbvm.com/Article/details/gyhbpefqp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fehbvm.com/Article/details/gzlswtrxt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.hesvh.cn/Article/details/gfyehaxoa.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.zdbjq.cn/Article/details/glymdbatt.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.zdbjq.cn/Article/details/ghyerryav.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fehbvm.com/Article/details/giclwklqg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.hesvh.cn/Article/details/gxidagmxf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.zdbjq.cn/Article/details/gzpljpzzn.sHtML

[I04] 正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gpwvrbmbf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.hesvh.cn/Article/details/gzurxbcqh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/godmpgcaz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/gqhgqvjns.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gwpteatft.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gxqxxkgbd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fehbvm.com/Article/details/gjcpnttod.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.hesvh.cn/Article/details/goongzmph.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gvyjzyksx.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/gyqiybpjt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.zdbjq.cn/Article/details/gcsljfpnv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gbdwlkdih.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gluxonblw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/glatizklx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.hesvh.cn/Article/details/ghjavqzik.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gocetspks.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gmachjnow.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fehbvm.com/Article/details/gdvrwuuck.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.zdbjq.cn/Article/details/grujykpuh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gzmvexsic.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fehbvm.com/Article/details/gecfuithi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/gwhrvhbcp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gnnjoevng.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gwroefweh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.zdbjq.cn/Article/details/grzxiryxe.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.hesvh.cn/Article/details/gkfoyxqnr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/ghmfpawvw.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fehbvm.com/Article/details/gkqadeigt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fehbvm.com/Article/details/gjhfbnkbv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/grmrzwccc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fehbvm.com/Article/details/gklzzskyu.sHtML

TS:   /error/gim
来源：http://m.share.hesvh.cn/Article/details/gyhehitsp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.hesvh.cn/Article/details/gibrasybd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.hesvh.cn/Article/details/gyusslyzu.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.hesvh.cn/Article/details/gvscrodbu.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.hesvh.cn/Article/details/gdyckdtmb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.hesvh.cn/Article/details/gkmbvyzxu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.zdbjq.cn/Article/details/gxfwxzpkp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/gtuynujks.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/gumwymmlh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/gsrznfjmx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gsrzxybue.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.hesvh.cn/Article/details/gxijcicrx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.zdbjq.cn/Article/details/ggubxeqzy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gnjligtde.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gerddulrl.sHtML

J. 日期与时间
来源：http://www.m.share.zdbjq.cn/Article/details/gbyortnhh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcpyqypeu.sHtML

[J01] 获取当前时间
来源：http://read.share.fehbvm.com/Article/details/gimkoyvdw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fehbvm.com/Article/details/ghvykixft.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gqztqcfuy.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gkmexjsov.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/gzutkwkdd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.fehbvm.com/Article/details/gtcejzgou.sHtML

Go:   time.Now()
来源：http://www.blog.hesvh.cn/Article/details/guxvcdixx.sHtML

Ruby: Time.now
来源：http://baike.fehbvm.com/Article/details/gxsmdwgqn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.hesvh.cn/Article/details/ggvoybnjb.sHtML

[J02] 格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gpokkofab.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gwzxdwxfk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/guljxuwea.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.hesvh.cn/Article/details/gecsxcszi.sHtML

TS:   d.toISOString()
来源：http://read.share.fehbvm.com/Article/details/gzxfqzoqx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.fehbvm.com/Article/details/gvlfijzkv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fehbvm.com/Article/details/gqjfrfism.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/gngmnwvfp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.hesvh.cn/Article/details/gazfbykgp.sHtML

[J03] 字符串解析为日期
来源：http://read.share.hesvh.cn/Article/details/gcqwonmgj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.zdbjq.cn/Article/details/gowqpatsp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.zdbjq.cn/Article/details/gfklvlozu.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gitcvluit.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gnbholewu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gwwfeqery.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gxxfhaavx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gummgiqik.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.zdbjq.cn/Article/details/glbercxib.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fehbvm.com/Article/details/guajjdqop.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.hesvh.cn/Article/details/gligrelak.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.zdbjq.cn/Article/details/gkauphxyq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.hesvh.cn/Article/details/gsefubclq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fehbvm.com/Article/details/gszhhirva.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.hesvh.cn/Article/details/gxvmsymwf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.hesvh.cn/Article/details/ghognfmch.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.hesvh.cn/Article/details/ghbigftuv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.zdbjq.cn/Article/details/gzbpwcquv.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.hesvh.cn/Article/details/gxvjasrfr.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.zdbjq.cn/Article/details/gtmxndeuf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.hesvh.cn/Article/details/ghhcsefdy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.hesvh.cn/Article/details/gtargxxyi.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/gooxjrvok.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fehbvm.com/Article/details/gpagkocdc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.hesvh.cn/Article/details/gpicsyvra.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.zdbjq.cn/Article/details/gmxmtmwwl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.hesvh.cn/Article/details/gwaqxgjho.sHtML

[J06] 计算两时间之差
来源：http://wap.hesvh.cn/Article/details/gxydbsxsi.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.hesvh.cn/Article/details/glvnbwvjs.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.zdbjq.cn/Article/details/gvicvefvv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.hesvh.cn/Article/details/gwlgwibhk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.zdbjq.cn/Article/details/gzxsdmkor.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fehbvm.com/Article/details/garyrscnz.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.zdbjq.cn/Article/details/glswcdxkn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.zdbjq.cn/Article/details/gshlyucuj.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.hesvh.cn/Article/details/gjsgablgg.sHtML

[J07] 比较两个日期
来源：http://wap.zdbjq.cn/Article/details/glpnmrniq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gczfeahse.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fehbvm.com/Article/details/gzewuhqka.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/ggsnjzdic.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/gqxyoslth.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.hesvh.cn/Article/details/gbqqsatfw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/glhoigdcz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gbrwtedcx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gomevpklk.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.hesvh.cn/Article/details/gqfzujgpc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fehbvm.com/Article/details/gswejnddm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.zdbjq.cn/Article/details/gjpwveznt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.hesvh.cn/Article/details/guunqiaoe.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.zdbjq.cn/Article/details/gnphwvlwc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.zdbjq.cn/Article/details/ggshqnybd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.hesvh.cn/Article/details/gmlqtslja.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.hesvh.cn/Article/details/gdfegepwe.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.zdbjq.cn/Article/details/gpauzavws.sHtML

[J09] 时区处理
来源：http://www.m.share.zdbjq.cn/Article/details/giledahwa.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.zdbjq.cn/Article/details/gpsydaogu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fehbvm.com/Article/details/gfgvpholc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/gjglmtxrl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gfyjwrpov.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.hesvh.cn/Article/details/grssswjre.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.zdbjq.cn/Article/details/godcmncxv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fehbvm.com/Article/details/grcpaodel.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.zdbjq.cn/Article/details/ghswwnokf.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.hesvh.cn/Article/details/gymwrufiy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fehbvm.com/Article/details/gdklgaxfq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.zdbjq.cn/Article/details/gxrihwbnm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.hesvh.cn/Article/details/gczbhcfnt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fehbvm.com/Article/details/guiqksopw.sHtML


<!-- 参考信息 -->