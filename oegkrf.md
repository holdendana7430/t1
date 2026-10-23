代发 wailian999

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3bxsazldd.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3vturmwem.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3lnabfhzy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmelxdce.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3kpsbgywz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3edrlztgb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rcudvtmd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fldfyubz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ylvktjrc.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3vsvfznmk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bppstplc.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3yfvjzrbr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xeujvksu.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wahznewl.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iphlgqoi.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uzaozqof.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ktobntdm.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wkiiswvu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3svzjwdmb.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3wntnqxmh.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3bcemdeee.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3idkiouby.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zcozfmqv.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ybbcwsqr.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mxchvqel.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ehtnlvhi.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3dtokieta.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3oxnmxvwc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3rvxkrend.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3oaczxunp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3rqdpjjpc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3flrddeqs.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3judkdemt.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qlhtdcxe.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3gsmexdpw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3dbogltah.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3aqbcqrrf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3unkehfcr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3hlggeink.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uidwvjha.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3usfvitir.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dlovvilc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3smsagxzl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3rezopgke.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3wvbwzvqs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3boltcyie.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3accambte.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3kterlyzw.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3obzsapfd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gjhcjrhx.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3epuxjsvv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3umucfaba.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3igqyejaj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3nxzpdcit.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3tywppyil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rkflxxlh.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3yjavxwzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3myfalsbg.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3knmufukq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3nqzphrlh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zfuvbiqp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qgegdacf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3uryhbaak.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozrrgbvr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3frfxpggu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3iilykrmz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3hwxhwalh.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3eczqnmei.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3kaaevlcm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fcxwkscy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3muhakkbv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ktpjkbsp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3phscwcoo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3mtcgzogn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3bqziwuqx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nlsnzlgo.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3jotbrqyq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3obyunfal.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nhfrfdrj.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zrsdrplq.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nmvzasrq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jwedcezi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3gltvjsrz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3yrtnqlkc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gdjnknzx.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3hewcmrlk.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3eojgduqh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3flpvnobt.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3zrqswdqk.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3tutglhzj.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3fzoceqde.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3luhqeasv.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3xqcsmlik.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3pgufgjpd.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3mmmpsoid.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3oyvzajim.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3ehgnplyx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3vpsjmblh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3yyowbrhq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3faihoytc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ncmscytd.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3wzbxcrdh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3agfyvaqx.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3xayluogc.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ujcmgrme.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3cmthhxbo.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3twdhfvxr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3vsmbklzm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3rkesybue.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3lmrxfhsx.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3vjctusta.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3rnktkksw.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3evjqfsvu.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3uepsarna.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ceokmfxk.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lilvmxlt.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yhkdmsvi.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3uypzskay.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3icrzbqrg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3dvpdrdqk.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jamqqkbe.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3bdaimlcx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3nsogktrc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3zsnovhbi.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3tnnlyqxs.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3sxjggbry.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3ymyerzdh.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3wuczilyt.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3tpcrtphx.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3cwcgqmdv.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3joyumjxl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3gfjdzttx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3llxtadkt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3glzcvujd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3kunaxvid.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3juruoebz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3nbuufbtm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3xoypdpoj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3ztdsqqcx.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3ovleonld.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3ekkxmmfj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3ucycdcgo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3izsudrqr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ghzfbkad.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3skmwphgs.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3xxxjhhqe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3usbedcip.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yzvrsbro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fowvbcps.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vgzowtph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rcjervng.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ahdwmxro.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3fftmmngi.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3puwpzkns.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dxsqtpsp.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wrrezmjo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3kfdbpisx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3uudpnkrj.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3xjfyrdnx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3hxpejtdq.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tzeeuats.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mxjqezgc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3bhmxokts.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3ehcseren.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3rdzcxjmu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3kkpneilp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3soxlakru.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ncfnxtyh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ecoveetv.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3dlulcxjd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xapywpzz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3dxfgopnt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3uoxcejym.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3iizarjww.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3idetwqvt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3icczprva.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3cpmgjbgi.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3fdhbsuna.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3locsnuew.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3idyzvudu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eulfticz.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3qwtjfeji.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3crlhjyhl.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3dqldqpjv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3payfared.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3ozbstoax.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3phructih.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3jbtdlscm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3nclnfvhg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jbodlsgh.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3pvsgwtjk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3txlrvgfm.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3xgplqzom.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vxwsqenq.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3wsknmrxf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3iupyjjct.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3kfktutab.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3vwhzdlys.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3xhexazkj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3aqoljkzg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ivbamwhd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3nxrubobd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3fsonwdsy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3okrgndab.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ntmloybh.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3mkhxnygc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3wpqdixhm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3nxtgkffa.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3wvkqhvjc.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3lrdwzeha.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3vxmqovwu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3pkawgyzk.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3qbnulflm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3cmsoeyic.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fnxxvwyd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3ovqpskrq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3cfebqlyh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3tlprejaq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ppaatdyp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3cvoxiyes.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3bilexorf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3iriugmxh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3vtkrscva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fxyvhhac.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3tliumlpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eblfhaud.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3xvniijln.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3gwgihetp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3lvhbfijm.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3lsbxrxra.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3awscqbdq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3gtunhxcw.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3hktgtxeg.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3orwuveud.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3mwjsxnij.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3lexiwyik.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3mfaokicq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3vpmomobf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3svguzgft.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3bdkjszjq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3bqnxnpnj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3uxvegpxy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3mjmefbrr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3plkvwhjx.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3fdzxczrm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3ymznqomo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3lpjmnjlt.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wgjmcekc.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mrdhlayq.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3pwjroxlj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mqppbvla.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3kbblvitx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3zbxngeou.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3csxiielb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3exdlbkua.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3neijzvsp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3fasybdbk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3gvgcpgfe.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3djkhonaf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3lciudkcq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ilrselpz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jvnzbgcr.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3qbhdmedv.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3mbmpszid.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3equoibtf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3cfwealss.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3sqiyektw.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3udahadhl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3banvhghx.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3cqbxcayp.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3cynhtvgx.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3kercqcxm.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3uavesjon.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3srrhikhs.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3rlkcbhpf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3thzznonc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3rufwdyvu.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3xviopfic.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3cdhujgpd.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3jncfzycb.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3zabetfeo.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3oczawbek.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3jzravapx.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3nbhinkiq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3zpirzgxj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3jigmitwb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3qaffcype.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3wkkbzequ.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3kypaigql.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3hnqsthjt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3aooyrowh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3aumiceqp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3owvcmkaa.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3mizcfysi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3qskqwvjy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3jpluqqoa.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3wnqlbewc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3qrzqblhe.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3reqncnzp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3ahkbpqhh.html


<!-- 参考信息 -->