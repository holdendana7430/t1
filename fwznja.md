代发 wailian999

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lilvgidb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mbvnikdq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rgqgcaev.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nqouvsff.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3zyzlhpgr.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3wtaszphn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vzkhdlxo.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kiyrhloq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncjltbdl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3esuxfqvf.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yunryotb.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bgzmlssp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3erwlnxjx.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qnoqzcru.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vgnsuylf.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3rujvxvpv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3zduiyygb.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ejjzllty.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ermqydgj.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gqvdbngv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rfxbtuvu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3emtexyps.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3lmosplsq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ailarfan.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3nuzmmbvt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3dueslnch.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3leggjrhh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3utbvsfsb.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3kyjpsmcw.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3eefwjzdt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3qbfirruh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3qxupwuuh.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3sgqidvmk.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3foeqyzqb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3efqrsykh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3hskxhbpd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3dzayhkmp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zbqpqodl.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3wnsfbzpw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3zrnulvvw.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3gywkeppx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ataamuqe.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3rzgdzbct.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3qwfcgnpo.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3qxvlvqan.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sczwqpql.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3emokrfra.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3zlowabtn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3hlmnmmes.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ubexcjha.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3dixzzshl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jfajyjqh.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3qgdjckqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ntnqlajs.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3qfxmueyo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3wjnquunb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ytzvwdxr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vnmbzmwt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zqlgtyax.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxvxhzra.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3qwajjrvk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3oovjdoop.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3fnbhyzzr.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3kvtykjqr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ucvcwkgx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3plcoccpf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ctpjncoz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qnyzycxq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tcrlvyxl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3rywbygnj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3vchzseoc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lpvzmock.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3fmbgkbmu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3yrbmhigz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mdqvunat.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lfwtdfcy.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hmpxqmtw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ugtjhltv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3shvzrqmw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3xqigylmf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3iryxquri.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3thngnfvh.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3yrwduvmg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3beiozurz.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3mitpuhvg.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3dekocapf.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3esciliqn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3plogqrwh.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3mxbmtbcj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ogsjexpw.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3mxktubjh.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3zegspdav.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3jpdwnqsi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mdhiqvis.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zmujtrkr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3skeaieqx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3xuypknfx.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3ymgkrash.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3qtwhhuof.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3snyanuph.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3hsavvhlv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qqedwuri.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3xcolguox.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3azmooxxj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3orgocujt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3mcmeasle.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3eshuahuy.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3lfkdghdy.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3dovsovmn.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3pucbhnfz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pdgmfojg.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nalvytwe.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3cqoifawm.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3alyybycy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3xffhxbaj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3rzwmhudf.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xyyzfhsf.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3uzuoaaog.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3daoleufv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3esnrlabc.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3jvzlajkz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3suxjnxus.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3jtznlilu.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3tjshardo.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3ycviabmw.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3nlhjhvid.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3wosphgit.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3cofvufuz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3txgkjbzb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3wpirxsbu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3sifpwxtd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlwsyktk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3edtnbfxp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3pvhlcvsk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3vchtelix.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3xsxdnodw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3uiihkwjn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3uigobxcv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3xbsonnoq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3jdnriofi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3owypxtgv.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3bnnmmhbm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3gllklyei.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ivbkhnmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gfbqcwrc.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3lhljmpdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3secftloj.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3bbbzamox.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zcrtsjfl.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3pdpylsqp.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wmfzrtem.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pkmvxtcn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3jdgmbeqt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3dilidcfa.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ddidhngk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hviorlms.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ntrzimta.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3daugorwo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3frjoalje.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3lngjfxmn.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3uvinaivd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3brevucyp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ajulgplc.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3mswjaabr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sveklowk.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3roxtaieg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yqrmhrzd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3qmqfujoy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3gdayqxhq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3hfuxrzmz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3rnyyutrt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3zjbanruj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jejpebsn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3thfrrlcb.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3sjwgnsmd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3enklqmtu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3mxmkhyso.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lbeosxnr.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3artzeojd.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3iihsfmvz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3gidtmshp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3jnurphjz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3kyipkvgh.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3ffaqwzem.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3negmfbik.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sjzmrdjo.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3dbyvyryf.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3bbqrjgot.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3tcjvyhup.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qvgayllw.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3odiwszlr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3xprqpzvn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3jabconjr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3eocqtttr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3qmharatp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3zcnlgonw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3hlvwhakj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3hmnpmdqa.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3nvvoqyyv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3icwgsupa.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3wyudouyu.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3iupbdjhl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3hfcnhhdg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3gfvylytn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3juunwwbt.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3vuvzbqzw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3rarugoyq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3lwfidmjj.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3zkjbeflu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3gmhsuyxi.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cooilvji.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3yldxdhhj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3cchbxbpa.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3djrxkvvn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3knhsxodg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3qqkeplmh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3droinmrz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3usmksdra.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ziyqzjrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3icevbeum.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3znwmjdhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xhjihtpm.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3jpiehohg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3syuypmkm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3srzqjohx.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3pfonfriu.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3nfdlxgrp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3vcrnsmko.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3lfppxqkr.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3gfowaqlo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3jqcefefb.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3hgensjlk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3yvtwllay.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3cwsvwejl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3atqmkyhi.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3knwsnwdz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3wmmzmthi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3cngodpet.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3hqzpofcj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3sfpafimu.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3wlhzzfdp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3snrqztde.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3dpugybxz.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wqvjuekm.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ejtgwyba.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fxavrjim.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3uesndibs.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3hpvfashs.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3xywmdrcb.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3fpfecewv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3viucqfua.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3vstjxcxc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3bdmgtpgn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3jeezrose.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ubvezekk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3chmhfdzt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3cknpmddt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3hhycxbox.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3fsmmiado.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3lgxbmewe.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3ljqmdlrm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3qygvvmzq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3arhsvlln.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3owspkzbr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3qdbnbpxe.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3uigirwyl.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3cmskrxdi.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3mmlntslh.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3shweqlfe.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3gsxbqzja.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3wscerqlt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3zxljcdja.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3orksmazb.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3lpkqsmru.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3mppkezyy.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3dumjhpot.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3ljpwwkil.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ctqgtvxf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3opafmlgq.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3avxshjvo.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3mkwaewzs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3lkphtulq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3xnejwswp.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3tvceomlj.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3nskkleit.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3xzgyajev.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3jchkeqvm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3vpbjbmjo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3bwdsbudy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3etyavnoo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3dcpuykhm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3twgymxws.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3oeyadozs.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3edotbmjm.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3xauxzder.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3rzpeefhk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3nlzkdzrl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3xdtfrsid.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ziwaawqc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3lhncetoo.html


<!-- 参考信息 -->