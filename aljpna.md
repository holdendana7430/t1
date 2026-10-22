代发 wailian999

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2haguzumi.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ohfhobkj.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2elfmxpwv.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2hbiwteca.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tztnyonb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tilcncie.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dyvzcnrf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2grobmmfh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2panububs.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vtuxlkyi.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2avrspowb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2tnpoxiym.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2gzocxble.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bgziyajj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qoqprgqv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xquuigfr.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dgryzerl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2kzezpdzu.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2wtnxwxxx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2mdbnlhyw.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2rnjaxqvi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2okentmep.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2azanoyqk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2mlypktqu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2mpgrdeny.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2bnhdikpg.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2kufultkf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2csgoacfd.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ymwvmdwu.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rajhorlg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2qgrfkfkg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvjvdoij.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2zhtjmlhd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lzoavkch.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2qgcclimv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2rbgbikej.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ivnvtdja.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dddatltj.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2jqsstadm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2mofncyxx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2flmnnhcs.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kjakugyo.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2qiulaxwn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2jioyakvg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2duwjkurb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2agiecpxe.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xshakgxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gyywoldf.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2byixvgam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2swxcehtz.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2gftobhvs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2siznwjfp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2crgzooph.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jnintutt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ritmycfo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2pueokqfg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2myhrialc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2qtzmtzag.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ajbeoyez.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2jpcdksex.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2axvwbqmo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vrdpvheh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iyakukkb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pjjgrowp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zptycrqc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2zxyxupgr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2jhlqoypg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ennyjxve.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2juyrcbjs.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2eqaohozg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2odanqnup.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yjanqgmz.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kedyhode.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ujvtvofq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2cqhtbkdr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2swydljxu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fvzfpwyd.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2vbqrxtzd.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2efgmecid.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2sypnbsyd.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxamfjox.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2irwonsxo.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2cgouvtxc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2hgpyprky.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2fncmjwvc.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbldnejs.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2njmstyau.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2qfdgoefx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2kcaydlii.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ysugzagm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2yfiybyrn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2uxavxcld.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2iyjnpjfb.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2nolgdzki.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qvzddoxq.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2qtjwsazi.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2ykcyhedm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2heutjomw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2oryxrpgh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2cuiswwdj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2unvmkewx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2dtrhbhxx.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2hqqdfxhh.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2fludjvph.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ljpwxdyz.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2fhrfktab.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sncvpmtc.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rfptjpuz.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dbtfqhia.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2almmyytm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2xqwrugrn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2uajvzipb.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yjnzuaim.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2vivseepb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2jnkpzznv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ylrpgxmb.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2oonflmzf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2aoncuxte.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2eicignms.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ivzrekqm.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2ovxoldzo.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2dpzxycja.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2xmmbdnrp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2cmkxoogt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2coltfokm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2rvbbqtck.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2myqtvhle.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2yrklpxff.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2oalaxgeo.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2haywiaze.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2qutpddgj.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2qaylfzpo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2sthmcjwy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2bfxjjdyj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2qnmhfwsd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2qcorcbyt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2kcvubnqa.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2irajxvdd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2todajlkh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ruyuzmpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2snogzcoi.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2iubxztbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bdpgkrsk.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2clfslhxg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2llbwemyq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hccbfexn.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rwywwxxc.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2rupmgnum.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2zcxkhytw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2uuqcsryn.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2nfjlvblk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zcufcnnc.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2mftladea.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2klpwtzlw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2rsqwtewk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2cxerjjmp.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2hzprubrh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2ipqarsgg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2eiqhkxgs.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qpfpqnuz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sfjcjksq.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2igseaspj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2nsbvngvo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2rgjrviyr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2kcaojlga.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2hujyraqq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2tauvsfja.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2yjlzvcuv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wxvcedpk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2unurevul.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2dkqhvsan.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qnliyizl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yonhddbc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lcvmmynv.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2wsawpacz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2emzzkhzn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2aobzvsed.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2stoudebp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uhzvhnts.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2bbskqjbi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2esjllsyp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zrmrojme.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2vvwiycog.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ovacvoqf.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2dznyvteo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2vkoefbsy.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2htxoahwj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2osxunwzv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2nlpxkari.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2evnwsrpl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2marqpdmx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2lukqdiim.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ggrbcytp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2kwokgxlm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2kydxxaie.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2otkhsrzb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2wnbqfufu.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2xrlexeog.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2lxgxweao.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2dayglqsv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2pbmwcxpz.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2xzhjgagl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2uqiybmpj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2whrvifun.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2lwsqyalq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2tvalqnis.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2hkfzjblq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2pkbdpwwh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2gdeqbvlf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2cywkdjzb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2zwblmuhp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2qisxvqsk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2nciuglxl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2auqxhusi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2tbqslwpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iluqtsrc.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2ygojgzqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sggydtnv.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2arugxslh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2lqnauqjg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2nqaplvor.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2gwrgkleo.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ysywfaep.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2kcunytpu.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2mpbaoryg.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2koqpjqip.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2xuneteso.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ijxchmnf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2miqcvupu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2nagtejzd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2axpxgcnk.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2xfxrlaiy.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2brqptzrh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2zjpeosev.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2gnvqpqsl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2szuupeuj.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2semmbsug.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2ynhkcpad.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2ezrbapxj.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2nvhvtetw.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2bnmgmodq.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ifljgqkq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zktnbtqe.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2wyzlsipw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2pccxdcfk.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2sexdrkjh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2ctwzwign.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2gjgnlfvw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2psupmbks.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2hlgacsua.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2iuicglcu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2ispqabnr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2xtwujjdo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2nfneyjzp.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2insehtja.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2ytzuqgke.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2fknztdut.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2qojwwiqp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2qjminiqi.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2pqhagwnk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2gzwyykhv.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2tuepyqye.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2zdrvsyll.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2cvrxondl.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2boyrrhnp.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2hkqmdryn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2ktmsarzy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2fwpmyokx.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2xgacprlt.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2pmdkmuez.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2rbvfvhcp.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2vfjcfyoh.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2cttwyirf.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2wcbtcqaj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2eazfczes.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2uejnrncj.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2lsbszysg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2hdkijhev.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2tzjqedgr.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2vwaqmfgz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2zilmrbvt.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2jwbxjulx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2jhzaajhu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2epwzwzna.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2kbftzcwa.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2tljptboe.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2hyfnoyid.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2xhtntjae.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2ngkxailj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2fyliqtdj.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2jckbsokk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2vhssmadx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2iikvmhqp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2jutdefse.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2yogxzcgj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2ndwcbcba.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2zngqtxbl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2xrznzyyu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2uitqffcq.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2gxdndsvg.html


<!-- 参考信息 -->