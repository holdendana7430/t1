代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ywxwfpdg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3gdjxyzxu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ywcytfkp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3qejsvduh.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3uoodbftw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3qhdxdtby.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3siyvwpmo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3srbwfssf.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3wfmmqzvz.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3bqjiybdi.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vjbfyylf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3kzaumsrm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3wbgbfifr.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3buokkykv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3idikkskj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ifoqmtrz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3lfoyrpuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fdvxkqur.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3emtjgnoz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3bdctkqet.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3meyfpoem.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3nyptdjfm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nbwphxsk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3hblthesd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3vsblvpmm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3lazxzylp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3nnofteah.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3zuezwssk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3sngimofm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmnodlym.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihbnggla.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3odbsucpg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zzsygzac.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3crztpkbi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ngbodund.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3filodbiv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ynlvrsev.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3bknnwfwk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dpaidyrc.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3blpieroz.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jjqqshcl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3akkqyagr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3zrwiwqbo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3mriphpng.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xnzlnlil.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3wnrdujsl.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3tjucsrps.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3kmubiopu.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3jbedchbu.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3sbxfmydi.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkqtyoqs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3xxeeumxx.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3hfvfrjnw.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3uvunnbzz.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3cnjiljvk.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3jbpsslgn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3eglfutmv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rmogmvjl.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3zqlvkeni.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3nxrzpgww.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3mqgleufn.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3tqkozknk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zkmirgqs.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3mdalnmzj.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3nykgqjtr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3iqknbcru.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3rcuociuz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3auwwgjzv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3akomqnsb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3dkqaovzx.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ybxkbqep.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3gxbfvmba.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3pvnjbdcr.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3hzzkgdtq.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3frembpzr.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3pbsohkig.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vhnlnpfz.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3trzgvlwu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3gxegdvwf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3potqxjwg.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jrqrzjap.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3uhhpwgai.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3kqmnxokb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3kqyjvvql.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3aixajmzz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3lednhitk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3mokmkwef.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ndoinflb.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3czmoldns.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3krhdweqg.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3czuffoex.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3uispbmeb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3lezgzzfo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3irxmldwq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ieakgxyf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3sipppeif.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3pmmjeymd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3bnhephxa.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3hbmkdjyb.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3qocmxlat.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3xmjuybsj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3hqdufwgr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3cnnuqewm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3bqhntdxu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3oezmfjdo.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3odsmgbsi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3alxjztae.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gzgdrluy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uovqcqtn.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3iglbfknk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swkeizxt.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ngeblbgl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3isideooh.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kcnzpzlj.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qoceqqdt.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3jesrbzwl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3jeptlvxj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3bwluleyl.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3xkvvahrw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3njpesdht.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3vwdtuaug.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ducitmqq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ebmjkavh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3zsbiznhi.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3cjbtnhzb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nxbaqmnw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3qcigordo.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3sziiuwdz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ieqjxlkf.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3xsanawek.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xtkfdfcg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3yoldgnyq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3wgehilyc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3ahpdvdvn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3xpymlmcc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3eixddwzw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3rivudauk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3peykglvt.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3psjocofl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3rhzvthyr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3vpxxfxqr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3lgvcnpvn.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3fhgzvcgm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3pftxybyn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ocxjaqaa.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3wbfnzkbq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yxmjosxm.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3kqiiodbv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3ljvxpskc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3lxkcgcva.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3sszupzhu.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3fuarjgcg.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3guazcrni.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qturgcfc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3bnaocvuy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3evrpihjf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3hktrjodr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3afmkdebx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3icsphusk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3mfhrmggr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3wemgehva.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3scwgqnbi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3ltgwblmc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3ezqgxgia.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3sojzwtuo.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3avpixbbw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3kjjcxpaj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3kgltvvkm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3hgkbkelf.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3pwyceqep.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3nmonrdec.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3sffgxupd.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3kliomrzm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3nmyngzsr.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cgavwupu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3toahwjbs.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3eaaooxrz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3mvxvgpim.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3pyowkvvz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ykldlchx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3fehuaiym.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3jntjrawp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3gkxczeta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3racdhrwi.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3bwbgthff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vhnxggxz.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3siezdzjo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3ghugifvs.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3dpnelrdi.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3srbgbfiu.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3gonievze.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3axagiloi.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3hpnjfydr.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3iqyryvug.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3fwarzgcp.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3hwbyakvm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3pnkyognd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3wqpblbdp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3tsqpnbcg.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3afzormyt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3qdxjiznd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3cbyjquey.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3tmjhbtps.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3sjelidsv.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3vwvqhcok.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3cvbpjvyj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3iryezutq.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kidcenzq.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3jdrtqpgh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3zfdrudjr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dqcksvar.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3duwkczct.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3rnghzbad.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3firuoupr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3dcmzynyq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3kokflnnf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3rqqxfilq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3klctcgxj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3yxvymmff.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3hrsxkioa.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3hiwhnxva.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3xzxeumqu.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3amqujtdl.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3tfiskolb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3vujmbxgs.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3sczugfuh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3pyhhhkti.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3labfiuvh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dhwmpdjo.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3xzshdrwf.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3gdiogoej.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3aievcaus.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3rxtektso.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3fossjlto.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3rokilxmi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3agqowehk.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3dtwojgjc.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3pdrudcut.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3kwixtkvl.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3luyerctd.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3ywknlczz.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ydwrzscg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3jnxtrtef.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3yzjeqfap.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ahjsacsw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3mriwhewv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3gsrgumuh.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3joblmawt.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3qmakgfdg.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3dwrdvrkm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3mwvohujp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3dnbhqfnu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3hqblkwby.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3dhqplliy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3oulbvyjf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3ieudulmd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3ezxpkqvp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3kjsqgasl.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3gdakrbtx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3howfdclx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3aaihsurl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ywsfrftu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3qkuwzzey.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3kcxsljzn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3hukijhad.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3nleqeqed.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3wosmgmre.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3txwoxqbz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3afwhozsq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3dlwmoekf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mozvvryl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3owlkrita.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tgkdspea.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3npvxgmnm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ssuyigkg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bxlkkjwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3puxdnjvb.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3kpjyhqde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jcwqiyvr.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3ffjxwprt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3wsytgyik.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3inxwrccc.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3azzxvrlj.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ymafslig.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3wipkwghr.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qvhsumti.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3qexdtnkm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3plinmvex.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3xmqgeqjk.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aceabcoo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3qvnuvemc.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3uocnkyej.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dqxpjjaj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3tpqnfynq.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3hlydcggp.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cmjztudu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3jdhqsbji.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3rmsyjmpc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3mqypchen.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3poqgeizz.html


<!-- 参考信息 -->