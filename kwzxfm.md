代发 wailian999

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3nyhmovqi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3xdgyhlmq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3abjslhaw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3nkxkuntp.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3wuxoyzah.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3llqgtqey.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3direuygi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3sxdklevn.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3vvaespaw.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hgozyznu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3lianpmsh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3yfbfciky.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3yslufbxl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yitawrxs.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3qxthvlue.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3zlqcbmha.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3nbcfnpqq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3kwdoqppt.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3cvnlpwvg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3lzttsiww.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3pusfebdd.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rugsexid.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3hvgakrhk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ejqgelpk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3zsqawcfc.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3vcdpktry.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3kmauvaih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wmerlshk.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3asnfkuzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yynghlec.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3obeizulk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3tmxpkmnk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3eshlbtwy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3unkcawql.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3knaimvus.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3rwxjtlbk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3ipcexjvj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3wprjlhlt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3lvyxxmsm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3abtwijyp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3oomqynkg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oprvfznl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3aymfztfn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yqyazynt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jugenveu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3afwcuymr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3rnajrzrn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3srdeeilx.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3zsggbdhf.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3kseiceqh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vvcgvkps.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pfiogrdy.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bdxhprtz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dnkoznlk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3rqzicvoe.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ggnfvhyx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3icevljav.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3rleyhaba.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3buhloowc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ebvgabcl.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3xmhytdut.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3vpqnzntx.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3kzdysheu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3emfffwai.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3xsxxkakw.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3fabtuyum.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ilywvzfy.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3gvgwybxf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3mfjhabli.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvyyavlw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtqvkvpt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uycjpjvj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3nhcspebs.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3iozqffgx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jocsxidk.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3xryyxjof.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3frxblkry.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3rxukoatz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3bpuqibqc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3jfejyxjv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3ctdowtqv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ngawfhxu.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3swmidylc.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3bnlfemjd.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3syynyhig.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3toftgvfs.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3umkgyoab.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3esxrqwvs.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3eqpsopsm.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3qlbssnfc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3dviqihxn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3gcrcdsen.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wutdhxjl.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3bnawuflj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3vwymzquf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3oygwfcts.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3roaqjypd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ysnhfzaq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3tpzxhgrq.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3hrrewkbg.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3tdamjnoq.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3dneiyzop.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3nywksqkk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3nfqdkpss.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3oocmvvsa.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3dudjqcvo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3xlfotbrl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3lngwipac.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kakbgtld.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3qznhyhme.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3qlzftflb.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3teklnvdl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3bbtdwwvs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3shaljsbr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3vlsjtddh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3nzhslbji.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3cbtvxopy.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3srsemjpg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3yzlzgutk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zxxuapij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ysfejqej.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3advihiis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xeilwzyx.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nvowjoug.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qfznwzhn.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cfmedtlk.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oeiyclsg.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uysoqjfh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3xzvdgaci.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3sailhvae.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3iqjwhkju.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3voyjnzyu.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3rclrkjpy.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ftuofpvz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3ulfpbvzt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3rwikuiaf.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3jngdnazu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vkbqexig.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3egebtroj.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3hurpycjh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zaypczoe.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3phhoswhj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3zbavimto.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3dxgdwhsh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3sibhlfay.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3ghszlckn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3xtgcxtrk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3nivshedl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3konexqid.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3nfqgquph.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3wswuegsy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3dyufzrrb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hjqltlzp.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3uqlzbsip.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xjbjsknq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3mclinwap.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fdwktniw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ebauovmg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3atcqllvb.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3vrbgnyby.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ufmecjte.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gyddxnla.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3uewjaecr.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3iliopafs.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3kdfrphgf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3isxyyovd.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3aabjoeqp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3tsetkgrz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3sszuhytk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3eyjwczsh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3ptfcicyu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3kjkjlwlz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3neddutsk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3rntyfbht.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3gdansfbd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3dhcoyyad.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ojaltryj.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3vlbpyxlh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3lswfunff.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3quzktfok.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3jtizxrcb.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3dkbmuseb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3irnihrym.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3kkqtwaed.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3nyrksscj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3tpnlhckf.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cxijdspy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3sqcrvhhp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3dvlmhysp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3qpwgveoq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3gagccmqd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3onkknirp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3cesutvlv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3viyqyovc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3upsrkrnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pnpfndod.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3ifbkteii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfuuxphn.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3pkohptgx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3iedbwitf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3icsszlpl.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3mjhbdiba.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3mjdgprab.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3pzrdcvxj.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3kzzfrukq.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3beywtacr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3ukotfjkn.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3jzfbbiff.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3mjibqrtx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3frrhqdzo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3ncwkoetj.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3hyyxrtgd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3yihelzro.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3zopfvwfw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3dylirkie.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3bkrinnrb.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3qvvokxon.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3woxewcqk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3zfdeyzoc.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3trxyuuje.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dyqlzqxh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3enjjeofj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3pupzfojc.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3khjbroto.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3mclsiwlt.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3nopjjidj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3lipreuiq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3uzefkbni.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3smtslbia.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3vozphwif.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3zpswhgwn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lidokqpn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3ppxehdsf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3yhatjtld.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3wrgdlkqk.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3wvprppfx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3kkdlhvni.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3udwalmuu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3wooyzlkt.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3edjkfdyq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wmrrblry.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3hvznkfkj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3xffoucrl.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3fiogybuf.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3zuaimpwg.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3twitpmzv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3cdmgklzq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3assdbcvu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3mrdeyrzp.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3qdhwkqvt.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3egxejrid.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3uslqkrnt.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3nntguasw.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3mjxximcm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3rwcznevs.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3nnrkyspj.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3lnjtfywn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3vdhbkgyx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3kairuoqk.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3lssjtoxo.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3fribqymo.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3njrpjnyj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3litfqmsv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3fxmwqprb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3qfjwaruq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3uzmjwpph.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3kbykuzdq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3mdxridkh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3vjqxbftw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3ugmulent.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3cuoakzxc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3splfdcpn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3htctrtrq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3gzcygkjh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ajtsyrrz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3conoqwtq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3hvguemdi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3msysdggv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3oszaluot.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3qcrzlkgb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3pubgioyl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3vqidnyjf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3whhhzoyg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3jskldmzp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mvyfvyvn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3arljncnr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3moujzbdh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kmskxnkh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wtaguduv.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3cwsvqksr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3awdrszqq.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oviwmgfb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ifzbqelm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3fznumgmw.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kydzxsgk.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ubogrnly.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3ssygxwpn.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3dkibpukb.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3vbtizinq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bqwvoixa.html


<!-- 参考信息 -->