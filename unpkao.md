代发 wailian999

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3hsaidpyo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3wgcpbtjb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3smgpyadi.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3husgjecg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hbwgvhki.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3sghuzslo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3zcykjnhw.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xvzwufuk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3fdffyyzp.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3qjjzuoey.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3vyodnbbw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcsgdutc.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3kienxnqh.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tariwjrq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wmjujyrc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vsrrmlwf.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3cjydintj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3btdzycoz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3xgoxdsbi.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3hdoizcvo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsptklrc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sgmiujhp.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubflezqo.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fgwktdes.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fivbalgi.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qcsrxtro.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3lihwlccx.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3cwtafqdp.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3jnldffeh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3anmwzljn.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qbkrpdlx.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3szmhwvuc.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kwrfyruk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3fnswceox.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3cihgaeib.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3hmtbjlts.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ckdepxpo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3vqrpmdop.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3wrlkomin.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3lhtihbkq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ypstmvlx.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oomrzixo.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3socvbboz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3eyythmhw.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3dlxvqtje.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zyfvhbfm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3senrxsrz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3leqbzgoe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3nxafujpw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3piybpzuu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3hscmquef.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3nnlsokru.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3kbcwbqfv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3klkojmmy.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3dugbwosf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3lcutllwz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3gvqnhcfs.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qlguwnwf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3epfnzvbu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3zttdcxdx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3yzrypgre.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3hkmagafe.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3dhltvqcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iufnuhns.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3zvjfevve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vqkaczgz.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3wrvittte.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3qpltiblc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ireurkph.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bmqtizrb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3yefuqmbj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3stnrqsge.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3zkeykstz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3bhrdnpol.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3krlvuobj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3azqjuqbf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3fyqagpgv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tgfvsrzb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yhdfcfyp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tesfhlfg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mxppdura.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3tvruajet.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3prdifalg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3imwckdky.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3hrfixjmq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3qgvldvnp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3guewsdpn.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3acqhysxz.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vyfenayq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nzaatdva.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3mixplrki.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3bcweovnb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qufugbmq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3udegaibw.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3iqvkgmta.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3zggwkjxq.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ngtzmgnj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztroscvd.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3sursmdys.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3zlveorta.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3meruyeqx.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3rzxytdhp.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3hfncmwvq.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3eiolcfps.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3wtbenuxy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3fifzqzbx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3lzryrksc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3nxajifka.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3wqmosoih.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3evwclggz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3bgcgjaza.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3evlriwyb.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3exppxuty.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3byckopan.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3lwitokyc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3gwxgolyj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3rvafsfzg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3cyzzsmph.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3wxdyvxmc.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wkdswuwy.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3glajplyk.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3fnstnlzh.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qyvyhsnx.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ppsjljpy.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3brfwumih.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3jcptcmxo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3wvbxegdg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3ujqxxxpz.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dsqpmham.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3wzxjwyhk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3oqbhbzez.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3kgqkckjx.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3mqecvigv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3fullmiqz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3jxaedmbs.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3dmwbhfyp.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3ergjflqy.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3qbgzhxij.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3fbpeexar.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3zzafzgqc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3waehekdi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3izgkorqe.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3wrqsjlcz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3gsnmnlif.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3lkppshhp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3hydugoib.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3erfwfdlx.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3qzcdmncf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3icdrfxsn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3aubenvkm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ngggbazx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3brmbgmwd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3sczrpwad.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3fbqyybnu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3qdhhzqum.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3koywmitf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cfzzpyiq.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3ayfcfbvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ojavwuxd.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3hndgflkz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3icarsyxf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3apfudnee.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3smqebbxb.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3wztlwidr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3pazctxzs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3smfhnjjc.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3kwvevuoc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3cwrxxlol.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bjrgrddg.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bwlkwqrl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3uqckncmh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3ejjtvoev.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ilfpmbwf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3bpsaetar.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3xvfuvxkk.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ewxgdxfp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hiqyhdbv.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3lndjhhzk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3xwukdqcb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3kvfczokk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ovqrtkvf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3euaceegl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3vhfhtavw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3iresrmyx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3lerlhypq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3lrsxryvq.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3ckfipnxs.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3ajmmlahn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ipfivwst.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yhftykpw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ieqvpqpr.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ttfloday.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3kbdbvjmi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3vqpqmjif.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3abjmydoa.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vonvgggk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rezqsbhf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vzxqenkv.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3hslklrax.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3fgfqbusy.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3oubzfzxc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3bkmgsirs.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3gfitshir.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3yqfppgug.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3limbtpbo.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3leaqncds.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3uqxotxov.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3bxbvrfvq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3tzpmjzxt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3piszlwyx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3cqozxrme.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3owycdauy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3zyhzbwlo.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3whjktuor.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3tjyuilkp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3tudntpas.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3qqsepmav.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3cdzsedoo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3mugktjmb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3lfagznjq.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3cwgccias.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3ktisuwxw.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3egwzjjst.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3syggozrh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3enlrguiz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3vuguanqi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3uysgbugh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3updafuwn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3areneoar.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3silwjmrs.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ipdylieg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dgnnjrbk.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3kcrggdgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qvxhqdwn.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3ayfjcdot.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3aynytvvq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3pahgbrdz.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3lencwobq.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3bqzksxau.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3uopfhoyr.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3wucuhdbj.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3cckwtpri.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3ivnyyuxq.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3mfghafjw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3lgttqkls.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3gkdcsddg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3nxtzmfii.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3vfsqienf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3ivugemzp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3junoqiej.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3nkhrysdv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3skfgfjap.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3gwctnafo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3vicanpnk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3hmaskzaq.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3nawywxgp.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3bmxmdoqo.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zgwitlqj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3hseyocbi.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3rcrqxicd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3ccfhpnsj.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3nruoillo.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3mymjgito.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3evgnbtyj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3zoxnlbul.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3ghaefrpd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3rkbdvzas.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3dqelnlvc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3ouangjor.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ramphbww.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3fizjzpcy.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3ukwbquin.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3lbvukttk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3grnlliic.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3igpvhjfs.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3gveaieag.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gglbydnp.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3qismgrme.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3ynqqqvey.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3ieqdzvaz.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3goummlov.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3ewjrtizt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3gymfbgnt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3vzqkjinz.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3wjtrzqiy.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3qvwqynig.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3ufgxlmkr.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3dyheoeuv.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3vzaatlgy.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ujewsbqc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3cgeclqhm.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3uacbxjnh.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3akyyjqlr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3gzieqbtj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3eexzxxpt.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3xdyzquvx.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3izahjbjh.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3sdzltktj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3pmkgmwzb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3qytfavqc.html


<!-- 参考信息 -->