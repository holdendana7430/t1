代发 wailian999

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcwzyjer.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttfyxpvh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hjhzsxmk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mecjrwov.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3unjzdark.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3bipqrspt.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oqyiubzt.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3odkyyjfs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3npzgekgp.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3luhkulpl.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3octxjtxo.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rqsheeim.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xtvygxeo.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pzgsbpwp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3cqsnlrfu.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3deksjtcm.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3kbgncjla.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pvcicjqm.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rzbctuij.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ccnrdlld.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ddtzrxrq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3vcocfmcf.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3xubtrdtf.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3qufdauun.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3gepotdwj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3nbfmsbvr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3twobnblx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3kgtiuqab.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3mtzuqyvv.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3puflyemk.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3kudjeqrw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3escviavj.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3qnltofhp.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3tvwkjhao.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3cuawrzeg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtwptjei.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3qdagdlbq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qgxwatjx.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3aqsaldds.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3cxtaffkq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3uxjtsyyf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ciajpupl.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3xgejiudj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3odszbupu.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3zrdtkaua.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ualfbpbq.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3lplugxop.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3toeyqwoz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3qokprsni.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3qziyzirb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3gvrlmsnv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lpnpxltz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3uvqhgtfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dfrxltyq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3itdpjijh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3yixlnwbb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3orlhtfzx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3drjtmyrt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3rcmhvzrp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3nenmyhwt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3frfvjsha.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3vxlmpqmp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3qndeteev.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3wnvucaju.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3xhmfbyym.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hltpndmh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qoudekrq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rleayauc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vnpgvxeh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ujjvqgmu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3mjskzveb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nrhjexmi.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3cgftldsb.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3bncfothm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fpqwmsay.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yvzcighj.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mqfrwbhm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3axrkjjma.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3wdujhjjb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3gazztpta.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pxjqivpa.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3rubcrmul.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mlhqqfup.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3zfpedqra.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3kfwptkwp.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3nmxxlrhh.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hfxoutzr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3lqzwudir.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3xljgyvhv.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3hapdnpba.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3uqbqoewn.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3lorounqa.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3quaeuaxi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3whtwpkrg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3kjtedplf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3axkvidno.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3cyvnoiid.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3eieqdhrh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3fkannvcd.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3pfsbkouy.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3frxwuyea.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3cktxajvp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3lnwknroc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3smdmctxs.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3uujbuiia.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3smimhyof.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3avmubgdl.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3zfoegncl.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3ygmsouxc.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3uniopcec.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kyayyibw.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ewiabagf.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yfdermkx.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3yscwgsxp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3bfrjjsyk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ubenwlcl.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3benzdhzd.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3kxzajuln.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3emjfcqsv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3toddvkzx.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3rqysjuxq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3qjsgkffq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3wdorssfr.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3zrahubrc.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3odcjcwcg.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3diyjvufh.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3oerkotgi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3raqryznu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3jongoxnw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3iytnmbul.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3qahcyylx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3hdviivdv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ucbsbqpn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3hnqsjdnm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3cwztmssq.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3ggblbsrk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3nedfpiqg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3zjbuwepi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3tbubwadi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3hbcfhprc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3dkseibfk.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3oqpwvqxw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3bxkktekz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3azhzcmll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lduoteam.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3dkdtaalz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qqedyexv.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hotvzrdp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3aakgjgrr.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xcffipwn.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vxrzdvgw.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3tirgwfuh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3cruwglmv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3yueuiscv.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3crlrxlfq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3qgnfwnry.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3moqpbutj.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3yytevlva.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3dyrbsqkc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3xgjgzzkw.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3nbphsuql.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3ueyskgxr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3qpcwxupr.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ugdlhipn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lwhqhlde.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3trkxfyit.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3slzwsoox.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3khzfdhid.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3nqhlchcs.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jncdgpse.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3itsapccz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3ggrecweu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3pbbzippe.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3ulfhefba.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3vvbgtcos.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3axwekccl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3bhgyywfk.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3cotziqsg.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3qwfulujp.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3cxfnnygt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3knbqffon.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3issqewqo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3azkrklzc.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3sebxbbtz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3kemzunnq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3egctueef.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3obkklryn.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3mmsebket.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3nfgpxyyh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3kghgngfr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3qlkirejm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3hdshcwyt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3uiztytvg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3jevuewsw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3bssdcaas.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3asimpqcr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3aawpnuxt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3bwdfafgl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3zuupwcim.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3whuntats.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3uszlghxg.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3ygskkgni.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3qbtvmlio.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3olomijbp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3xzrudrpo.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3macscdeb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3oczyagiv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3gnicomzi.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3fqtzakwx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3mitrueus.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tbpzipwt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3qlupkxqa.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3mdaqznfq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3dabaupeu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3xiykyjtx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ztvmhbkx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3hajnayfo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3ptgqtdsl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3smjlbddg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rrkowbhc.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3uwpvbefe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxsujnyp.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3zdxiyebp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3kacsmwft.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3mpkqwxsy.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3njqligcf.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3epvvnhij.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3adrbsgvg.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3qnqbjqti.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3ndnrqvcv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3ocwryoic.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3neiqazic.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3fheyenyf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3tnepcbfy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3xxraegfg.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3cgojuyhx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3znchyind.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3ldsmcfmu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3uyejsmzo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3xwdpcmse.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3jrrzhptx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3knzllryp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3neyuefce.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zfdzqkbr.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ufrkxqws.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ftdiukki.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3nkzsmxsd.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3jgnouozx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3sdgmbuje.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3xvothrrp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3ruzvrcdq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3ymleqqqt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3ostgcdxf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3btyolclb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3mdgowvoq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3rneogcvx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ionrognh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3xrldkkob.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3ifsbusln.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3ueenvpch.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3nixhrzjh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3vapvdweb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3hbwctast.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3izeygmyy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3tvjeogje.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3iaxxpavg.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3tixazqcs.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3umbrtsdz.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3anmxbqrb.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3kartuovd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3sjiczqsh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3xmjobobo.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3achimexk.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3wikthuma.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3huikugbd.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3iqgchoal.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3atwdrirj.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ghbnupwg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3wvgqqfho.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3xrcvmwcc.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3japfmmyg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3mssgdiho.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3osjkdend.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ufqdytdj.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3vfmpwjai.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3xurribte.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3rpqdyemy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3rkufxqzv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3mxoxylcx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3yafxjguy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3uarchvzi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3ujchxakz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3jjjuyoxe.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3albwxaxy.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3pjnpadxw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3taprwstj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3rutsrhkq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3tkvmtgku.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3xgoucabk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3aegkmuir.html


<!-- 参考信息 -->