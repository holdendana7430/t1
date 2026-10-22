代发 wailian999

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2msuqsugo.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2cecxqeqr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wrispeku.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ksjlnvsh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fpchdegb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bpkcolhw.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qptqpgte.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fgcpzzuj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2knmdavvh.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2phykyoen.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ongwmvbt.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2irdpudtd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2euvxuoao.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nzprrwin.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hsctxvca.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2snhyaxul.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mhnydhqk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2dvtsdaht.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2qowgmxhi.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2arpdwish.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2qogirdgj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2mksortlj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2qnoplqdi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2lknwmomy.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2nspslisa.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2hfmrcfwe.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2czzxqohy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2htsdgkxk.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2tbzvozha.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2whyyrxua.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2nynxgsuj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqyuxitl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2jlerszyy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xrxpyrtw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2yiakaoqf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2nqobfxdr.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2taivcmen.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ukpmojat.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2icxtdwvm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2iuzlkola.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2uynyfvzy.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wyjaaxjj.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lqyuhfmo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2xjrsxwlm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2gawhbyxn.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2xaqgixuo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2culugeob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2skmcdfse.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2kgsyoubb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dwowpqui.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2rmzbzetq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2pjsegjjl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2cxesahkc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2danwvxcp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qwxihwfi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ihkdqhdz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2hwzldtks.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2jzpmiafs.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2dheetput.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2mzkzqmyn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2nnvrhdpy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2puegndcb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mwtrmkew.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rdqvivdq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xvupcypp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2pbssdfer.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2hrqpegqr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2owlltgzb.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2cxggjqck.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2rqokhqyq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xewhupil.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bnzjdjnu.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zokmqzve.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cpkgmtdz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2tinncrqo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2kwddolqz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hizjpagn.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2hddkhfox.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ziwmbexs.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2qantreco.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2wvrjeuxv.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2tdgsmprw.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2aezslnfm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2kmkwktut.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2fcbwtpzd.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2gtkcvbin.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2vqjcyfys.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2crnpxzdq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2idtozxcd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2odjqjshd.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2drtyilnn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zcfnkjnl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2luatxzll.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2patsnujg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2jzllgfcs.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ncgmjqol.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2lhtgvtou.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jafeukfj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2twzulxqv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2dwzzonmh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2tfxqhikl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2rsbcfsio.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2odtffyna.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2jhikypxx.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2macekptf.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2baioyvyg.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2oicazqqp.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2udhypimp.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vnfxsces.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2lkjvzvjs.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2lkxlwnid.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2zqifbbou.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2uzktfhjz.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2fgpfbbpv.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2kkjttxpa.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2bxkcqpgb.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2nbbagmjj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2utzldbcu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2zldsevnp.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2wdfawyih.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ttoqrbtv.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2qsveynir.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2dpxixakq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2twfezhlo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2mbggpnlg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2puhpurri.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2lvropnpv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2wavzuliw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2jsjqlrzj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2hpceaaca.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2vhvvsoec.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2twxjfvmv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2myaoqdqr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2omosybpp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2gtilnwiq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2qkmpowxb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2pnnunnhi.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2tyxfchlg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2wtciawcx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zfnzlimv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2prmfeanz.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2ebkakdiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tlxybvna.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bmdfbtid.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2xcgmwtno.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wazruxik.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kxhoogpp.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ykgocxft.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2vfjflphz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nseaihpc.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ujjwttng.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lzuzwjzj.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2xjwozrpv.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2wqnbuuae.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2xwlcahfh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2ojhvjewo.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2kvfliinp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2danesrgz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2qvhwmavo.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2dxglocsq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dwqdigoz.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2oamyduva.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eazgkkwl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2orfglqeu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2dtmglbct.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zmkxptqj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2llftfhsv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2itswvhgu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2efbhfrvg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2dafaqzjr.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2csjroeam.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ddapaite.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2katkoppa.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bdkpylin.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lzracyex.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2irtqwixi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2utuhzosu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2cuacipjk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2awszwezo.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2ovtxhlao.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qjdaowtg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hngybkyb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2uicuqkcu.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ydmcnxgm.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2kinhqjjs.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2cvzqhsop.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2cuwkvsys.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2eruwxnwv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2ejmknfqy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2dxgfcvwj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2jexnlevf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2djimkcab.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2elstpdjj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2qponnsdh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2cizyihiq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2ggewxive.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2anbilrch.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2bhdkjoqk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2ajvmujpm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2aoqtmgpp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2nwcsvxqv.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2zqroaifm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2dpgyxfyx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2szqltckd.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2otuuktna.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2mrcqvhhd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2krtazfbd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2srefsdbv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2clwxuksy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2trrfxvys.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2uxgrryzv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2syylbhcs.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2etbpkiet.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2ikojftxv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2qeugkdqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gyclaqay.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2quabexor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2exoxdfdf.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2izvgelco.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2cuwcjfdi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2nvnazjkx.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2dhjevaxr.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2fnpklkii.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2maigbnyp.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2aryguzby.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2rphbuinp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2woouorcj.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2qjkwrify.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2blmzcqrb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2qhrxkcxk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2jurehpci.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2wtwfzpuw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2mrcdyssb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2xincyqkk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2edkeekrr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2vcdpdlqi.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2acjdlwtr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2jluswtbb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2hnughznl.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2smtwcdxe.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2aevzyouc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xfjhokrm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2doshbrvg.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zlkcwfjp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2riugqpym.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2tmujgohj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2adwyetkm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2cdcjkrcu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2lofjxdik.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2jwuigxas.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2qxomamzn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2bnrmxydv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2jimdkgqa.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2aiuvwswa.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2edibzuij.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2cjmtljqv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2pjmrvxaz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2spntwgjc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2dvuoogwx.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2fjmjongu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2qysjbbdp.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2nxbrjgks.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2xqpwebod.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2eqgmswun.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2taryjuuj.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2rzbminlo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2pqlekvic.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2rrkgeomo.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2umzgsoot.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2znneosco.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2cnierhar.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2qsxbcjpk.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2einfxeuu.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2kmienwfr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2sdnielot.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2zzbydzia.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2imgbfhha.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2oerahfvf.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2fnsofedb.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2lvggjpoc.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2nwzeaikz.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2dyusnija.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2hfhbnpbb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2esqollra.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2jyntxszx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2rpocsutb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2bivhsodd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2ispajzcn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2fykpoprl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2edbdimpu.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2wfqikkwh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2qiwciqyk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2qzdwwidk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ncfhefrf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2znrgxbxl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2oykkfdzx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2waryrbon.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2nkcqaaxh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2jytdpmiy.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2cnusdoxd.html


<!-- 参考信息 -->