代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3sggkmmyd.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kpwrvcvv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qjurtbik.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3mkbxchmc.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3zuozghxe.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rjwnylfj.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ynikfycr.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ztajoghc.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tgyalvsw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3iwlpupok.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3pspnfimw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3loiabwvv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3fypkeetr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ibibsyoh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3lqpnowzq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3flgufong.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3despuuph.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3capajsaz.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3tyaebcnp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3hltkorwq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3tzxnrsbh.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uldffvdh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3bssdxhlg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdygailh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3awurzmhk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3owaoxhbs.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ajjvvuum.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3jruiwooo.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3vnguupcc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3erptlfjh.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3tnmundqy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3kgsmlinz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3gxhzibeq.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3arzpagml.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jmegphwr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3jnisclfi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3jnlzhsep.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3amopwsyh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3dtysoafv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sdtvcvhz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ijgmdnab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nhziqrpw.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ifkcehvh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3qzeyukbo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3izfkkiob.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ibtdjbnm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3visrxnxg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ehnegabk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3qrhgehti.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3wgaqzrpl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3bmbloouw.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3qtvoitvf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3aypqgbwe.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nlybuxng.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yizysbzb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sbjkrsuj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqdjltay.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ylyiqpdm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3nnylftkx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zicgycoi.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3bvikfcxf.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3fxlnyqvr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ybxobzmo.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sxsajmge.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3omgzkepd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ovtafmpb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3iyvwjgat.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3hqfybocn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mvvhfgzt.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3xdslburq.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hedxmlis.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3iaadpgtf.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3gciinsyl.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3xjwqncca.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ffygjoed.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3mdcwsiaa.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3nvimhupc.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqovftjh.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3sjjvowog.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3bbxlhjvi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3tazngfzb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mwngfbxw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3qzsprnti.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dgyzqrjw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3olssahhv.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3tolfpkeg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3pqzousnq.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3cktuhraq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3jprkwmqx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3pjqftoba.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3xpgbehat.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ihbssejr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3xipynqju.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3grhkgycq.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3lntgchho.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3zupviatf.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3syggztoo.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3tefvgevy.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vwrsbrnk.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yfiuwcsj.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gxphswvo.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3ikpfeaoc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3vdtjtlvk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3hixvsiou.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ypkyvpvc.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3pbslarqr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3zqmyolxp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3voibblsw.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3ycjnmbrk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3qkutwqtx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3irezwffs.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3pautyxdl.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3jmpfbgkq.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3hagfzxwz.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3pkzpuzfd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3mzrdctpy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3qrnticqo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3rrfywlzc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3adahnear.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3oltbzhsh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3tfcmxsuz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3zbuoygsm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3qqwyoqge.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3juxjxxag.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3evlznoca.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3xoevwtrc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3mnyijhvt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3gzopnpry.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3mtxqoery.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3wgyabwcw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3rhrccogd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zeujupjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rpkuzwqb.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vonmzriz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wtblkuqq.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3trvhrire.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3kzxgqznb.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ktxfhqjq.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ppofqkjg.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3vhdoaprb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3afefctis.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ghrgpnez.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3rpbxikns.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3dplkxdla.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3njkbjwnq.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rxtaxiuy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3avvznuym.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3buegmxnw.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ntxcqjte.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tvzjjpxn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3hvdwsegz.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ijnwgmim.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sscgxbfw.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3ufmiwmja.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jkczquky.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3fxuzsaml.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3hxyrxebq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3ahnhguus.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3frnxlogw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3boibfhps.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ouqqrhac.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3eaafvadj.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3ezswzpzf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3ydfsbrvz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ujhxyvkm.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nfslcujr.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3cbwfecoj.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3olxpltsl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nyfsdhji.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3ehcjibrk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3zpkvtzxz.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3yknguewx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3ralmumqs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3azqtqgax.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3mprcwwam.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3jmputiqk.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3qonhjsyz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3hyxlncef.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3hbsvegxa.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3ylcmiliu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3wysnbsjf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3mmegrcel.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3nyutuvuk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3vmjbkhhe.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3jdxiwunz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3bxkwtpuo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3forsdnor.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3lwzlappo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3gwrpzadz.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3hhlzqigb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3hdadlayy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3molrtjuv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3umkcrfxb.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3nihltvda.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3lhcwtywz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3ownpjsav.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3ngigwifm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3doabrarc.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3hkzmqolb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3ahwjgnpy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3iewkyzdj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ygryhfyi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3kalxpeih.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3lxmbccgi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3buwoavmg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3iuphxeel.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3dutvkhsi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tksaqgcj.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3ykgoopnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbdkzyyy.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ulzbmfkh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3yvrumdev.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3yfttqeqd.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3itqpdlcb.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ijybtpsj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3uhvcwazw.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3qabvhjve.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3xzecuhbg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3pofvjepg.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3rsyyiofg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3enonauli.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ndjgbksk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3xmhtdadv.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3llafxnaw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3mkqnfytb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3vqwpvhgz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3hszhpprm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3rhdgclaa.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3ercnbkac.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3vdcvbjoc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3thqpjnvt.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tvagbjrq.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wyixcboy.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3bkbkutrc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3kifotydw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qwnullha.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3utdrlkkm.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3erovsocb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3trsesdid.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3hqbbprhe.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3qpseksrf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3nrdcpcrh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3gqchzmmu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3twcizwwd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3xkucmokz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3cawqmwta.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3dihiszdu.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3lgekbhbo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3gmdmeskw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3rxyxzrni.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3zowejzzt.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3aoragrnh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wfvowyhz.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3crbzxlvx.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3buyemazg.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3hdjpyqwd.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3iciumzgc.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3ihsvxcnu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3jvwhmbdo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3cewoazvd.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3enlmkhxf.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3chqpnitf.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3jonervmw.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3thrctsou.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3gstvysap.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3nsismqxh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3tqazkigj.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3eprcfbld.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3zpxedext.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3eietpfak.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3valajoao.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3nzkoumqg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3fowmdvyc.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3hxtsaafm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3urscxubp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3ontnoinb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3fdjugdpp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3mjicxcno.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3kxcwzrgk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3lphydrsa.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3kkswmjey.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3pdvnjose.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3qvcxmvgt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3zrbpatfm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3ryzwrxoi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3oejyhetc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3xfsxtxoa.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3lprhopxp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3tvlqporj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3wbjoyrjs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3rggbwclx.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3mboioolj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3ipotlnhp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3ywpkgues.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tyjgsgec.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3roxrkutf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3quozabhg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3xvcziqxw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3gjulvkvx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3ftixbgdn.html


<!-- 参考信息 -->