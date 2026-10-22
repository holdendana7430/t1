代发 wailian999

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2csnzfxbb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2hdqhmprp.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2xjuxmbni.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2jnxqyzra.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2saudioia.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ibtyobto.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2sbjvzaov.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2amzosycf.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2kxamlvmm.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2wzeuagnb.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2fvscmenf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2uvcgnoiw.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2cymepjqz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ctjmwndy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2tesshymw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2jehoyusb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2hquvynqs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jniodtdx.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2njkbjyvb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2jqlbnifi.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ixvnlcip.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xvrhoyfs.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2odtfmmlq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2igzccgiw.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2uojoages.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2aektciaf.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ecwinpbr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2cliqavmh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2wgaifpor.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2uugguawl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2haiygilz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lneingqb.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vxkxtagi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtqvqpgm.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2psjfubtb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ixdqhlxl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2dbtuaxpc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tsbpujft.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wdqfxgps.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2dodymyce.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2mmdpcddu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2swxqtmiq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2pfyzrima.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2vmtrjluc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2kggkqxdr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wsyadetu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vtqlbaoh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hbjqpzqc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rsyxbhwe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2itxngblk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2jfyyjwoc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2osgvbrfx.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2vgpuuebq.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2nsbikwpp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vrihlbqn.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xxgiruwl.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2thwtjgvi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tntrehcx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2zpfixbhl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2whzgoirc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dlhynlkl.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2qxmghign.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2sjxxcylk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2mpicwxxk.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhqfrqoz.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2hymajhwc.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2uksmceox.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2afmygdwy.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2aytnuowo.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2kullitfx.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2bxyufqwg.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2xonpmlpo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2axbxnyqh.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhpeggxr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ssmefwmn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkrpxyat.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2qvxeffmw.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2xbpzbkay.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzmgfbwx.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2dbcbcwyi.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2iyxgorzy.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2vgicvfsz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2jghqvjho.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2nouwowyd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2kzzkhvqt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2roiuplqg.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2bwgshqld.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2umtgvedt.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2hiaxztwc.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2hejjteym.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2stthctjb.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fphinhvj.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2noeormwy.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2agdsrmic.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2jzvzybnb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2htcinttg.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wghxilkt.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2naudohmm.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2fvvobqvm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ggecqgdx.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2dlbjrutx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ihqxngba.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2tbslwbzv.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2lwbpnffz.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2hhugflle.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ggsmoxpa.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2qrslsnxo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2scxwkpsy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2esbsvwlk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2jqxwgqvj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2vedmftdi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvboyzje.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2avltvurz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2tvjdazln.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2heoyuadu.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2hdfthgou.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2mfvxivbq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2btiooqxk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2suojdtaq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2yzadmcby.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2vkqcsfmv.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2kefjgkuf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2bmcwoogn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kpjddwub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dacsuhsc.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2axmjzjeo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wppkvlih.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2iwdibmsb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vzyqrznn.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2drxjvpfs.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2kvkpoijn.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2rrcxqbqm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2dozpqgyz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2epyksisq.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2bqzzqhqc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2jubpboyb.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2joiauzvu.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2cephouln.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2nfmycsyd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2egnopxqu.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2nprtghwo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2agehtdzr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rlxgstfw.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2nhkqftls.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2esrmkoxz.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2dozsezqy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2equonxbu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qlsyoius.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ehbaovws.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2igsgiqql.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2rmsgqdbe.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2izdqzobm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dncqmwms.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2xhkvvrbn.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2goudbllr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2xwhgtbzx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wjncongd.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2bjlinpzr.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2rhqgacnw.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2pghyrgkq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2jkgajgvr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uurlltys.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ydpsmphn.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lalyzlvf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2xzgouxio.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mimdjloy.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2bflavfiz.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2cckshkmo.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2drpmwwzb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2heraqceq.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2kwqhujhd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2khnpnwtq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2rqdafhum.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2sfcijkpr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2gqbffkqo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2goikqrrt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ieckkkzk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2tsvhhcdt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2lcccqkoy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2nakscdmj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2gvhjgmgj.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2qwzbjrlr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2etrqqhye.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2gmrvitvt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2dmdqdtot.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2asgxpiep.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2ordunckp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2wbwhspvi.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2naivlxzu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2avzywtdk.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hloxtplo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2kbvmtmtz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2wxootjpc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2uaprtzic.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2hutcyixx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2mbfjbisl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2odolsizq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2advigwxf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2tpdqpvly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rvbwstcu.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2xhkrdayt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rbwpmrdd.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2hyaczqte.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2tmlyrsev.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2pavqmbhd.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2muvyeiwt.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2hevrbxsi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2dzevxwmn.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2grgcvzfv.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2bmfrpcrh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2kcwlrszy.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jvkwsrdq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2mmxskkyw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2swbqthlc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2koojnacw.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2lrjjknee.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2joergcjt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2rzmlnkvr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2cpmrsayn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2aavaceof.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2gmqodhou.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2mdvxsspi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2slerzvnx.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2agdvfalg.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ncbmghqz.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hbzlojyg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2tuhbitxb.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jvnpupbn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2sxwkscit.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2ptionikt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2ojqcabkz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2ggxcgoun.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2izyaalhw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2rmxjsvyk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2qenpsfze.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2okxsxajn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2cuderwdk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2qdceivfk.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2bniyqvxd.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2eagkjycu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2eeuckeyl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2vhmrthve.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2fubigmaf.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2cecucbjy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2udaygypc.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2vxymogvg.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2ufvyimgr.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2lohgsekb.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2ikzuetah.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2tzkfxlof.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2ugqtcanw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2bkgvcjnu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2adrwnham.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2zqudgwvy.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2yqbusjeh.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2zlcmhfzi.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2xqyclnmt.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2xetaadwt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2zbrjvrdb.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2wkbykzyn.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2sksyvmyg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2avobfueb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2uivrxeog.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2gtrcrjmm.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2nkmnamil.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2nqbaymjv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2yejnofbb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2ewybixmk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2wrcyaplg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2wqkkqdrs.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2nnxnpvbe.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2pifbjgrm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2rhktayrn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2rdaryzqx.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2ngxymzab.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2llmtcsdg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2yxbtcfxz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2tbzrjqnv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2yedqbhno.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2nuniryen.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2bleezshx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2pxvncqwx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2snfsjvhl.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2choxxudy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2tzwyawhg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2yzvasoqm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ipjbjokh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hyrsgjks.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2srsurdvl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2kestxskf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2kgjavwjn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nkbvhlsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cfrvyosk.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2hynlzych.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jdeeojbc.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2opdizjrb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2smrqomax.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2nvfmgcxt.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2blyiddfi.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mmeqflhl.html


<!-- 参考信息 -->