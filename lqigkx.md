代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2egwifhdv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fjsksuem.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2xdqpgfhg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2yxxgqyab.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2gmvpnmke.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2engnkvoe.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2cpkburqc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2qqzhsezr.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2vgistjpp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ojwgargi.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zhhyneoh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2nmxkxjqs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2blouaegv.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ikrlllro.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2whmebutk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xzwrmcvu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2snjjhrgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vjoodkan.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2zvoimnne.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ypkqliwx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2rqtieywe.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xcfemzqo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2sjgrzkxr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2hhumtraa.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2fpkhamrx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2sywaippf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2fjdkmdxj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2gcjvfkbo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2qrfghmoy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zgzurqzn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qgjvkpkk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rbessjli.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2aaltlnyv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2mckhflxn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2yzcnttkk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iyeruljy.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2udjnkmcw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ldmipksr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2maehfqme.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2iuqcjuau.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tmsxiqbg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2btclzqsb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2bqhoxzaf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2megccnqp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vyoyqgki.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2irewvvpk.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2gvsnwtls.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2fbawqfac.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2cfollvhl.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2vqvnresy.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2gmvqwtsx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2azwcjvno.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2higaqsdd.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2hfnetufe.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2udeoljjp.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2gpiqkijj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2pblplbhs.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2uhcsdbek.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpiccpru.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2beqxkgit.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2tylijthp.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2gfmjocno.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2slxlywva.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2hputdrjr.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2kcflhmbe.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vafxvhni.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zkhdsasi.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ckrnojfs.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2tkmwyncv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2zwznivga.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2seytsvhx.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2uvitvoua.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2sjvkuogc.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2nubcdmzx.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mwwnjwzt.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wtastfqj.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mksqbger.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2vdlxozcr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2zlnwwklh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2jxnsjimw.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2avtpjylu.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2jmaoaklb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2kecqbvim.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2rsutufya.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ektqhvxe.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2xvxipfpx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ycjsapof.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2uughumee.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2vryypvdn.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2amwhavoi.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2ebganlsy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2hdqhpgjx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2hginlzju.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2xoibjhoh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2wzbmxsud.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2bcwcwhia.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2rhijjejn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2ccyqfsar.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2yoxvfxvj.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2jbfqdood.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2hzqvcqjo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2roqhiegt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2bwbfvqjd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2oixnxqlg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2axwvjurc.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2whmfwchf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2ezeyeleh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ewtddpdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ggabitxz.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2mknonaqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqnqepan.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rqomcnsa.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2zngpfsth.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ynoekfdy.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yhjelegx.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gukqhonn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2fuiaelhg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2juecgvcu.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fjkejuay.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bscfpdfw.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2ppwsmhxf.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ijejdspy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2ubmszgfs.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2hgzbogae.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2waydkril.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2xrtneikj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ibexdvbp.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2jyjxrldx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fkylnlgm.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2mfzyqivb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2excjhcca.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2sufjjyfv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2wduxefax.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2cmppzdbs.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2zhczfhgb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2lksjvbcj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2tbtsclox.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2xdcwoddo.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2lfktnbpc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wsckursg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2msucuuzp.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2aredeqpl.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rdqjlpfw.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ldtzwfrz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tojdwwbo.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2etugklfq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2edcgvrws.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2txqvlmgz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2jhpzixiv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ydmckqif.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2lxtucmhp.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2xxkezkko.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2rwhhnbxm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2fifuirpl.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2awxpfhzm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2oprawckk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2kmweldze.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ncpzmvpu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2mysiwdyi.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2hpgfduca.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2otzbryvb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2fljdeldd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2sagbqjrg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2gaijufvn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2sfbvgrus.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2kootohfx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2mdrdqxbq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2sjslfnwc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2sjpczvpr.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2vhuvfuph.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2exnwzzjk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2gwxoczak.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2vkppvzfu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2viuseagy.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2ptcvxcwj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2lyfbhinp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2bbkutptt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2bqjmwdax.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2fdqtoiuk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2teeatidt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2oorfgyxp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2bgjifmlr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2jswdkziu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jjnfcams.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2hinuodno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nfqzwfql.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2gtduxjby.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2vxammpuw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2siqmejvs.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2kxweymbe.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2pxifigsw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2naykhkid.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2jsyorfxi.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2syyxhlsh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2lmeswisy.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2pirqsdit.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2pnlmkslo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ddjyzhij.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2iphbzuer.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2erdkmxrr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2nsctfnpb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2qzvqaohv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2owsihtcn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2tcrluhhc.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2hkjeenqw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2uwhrhwcv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2tlbowpri.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2nkxcuewd.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hfylmmav.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rtvsfoma.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2nlqopgtj.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2umhokvro.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2kpelzklo.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2secxarrf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2unjftncm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2khiixsml.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2kqjfnhrh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2wtxgsdax.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2lvgigeto.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2kxbddqsp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2korfrdgq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2mjzwhnbz.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2conkjazr.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2hotwqzsl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2woydxhyz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2wwcupgqz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ijeutyuu.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2jqbvxmhw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hdewrevg.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2rphekyag.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2awtiegtt.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2evuknxji.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2pslxoipl.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2wohkdtkd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2zaymwqgb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2hzsszgli.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2cxrpwvbm.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2nfidruwk.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2cuwdupwn.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2tdlybffy.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2sklwnjkk.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ifkhgzvr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2tykzhsmy.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2xbgqsdrn.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2buuwjlja.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2xththbpp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2vrjlvtsl.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2bxvsyodb.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2jybdhdls.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2unhfvifk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2kvbopzys.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2neofmdzs.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2sobxjrph.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2oblakzwt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2slcmoydf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2kuhohjbd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2ngeivcye.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2qodperzh.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2ngypuobc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2smcgjtlt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2jneokshf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2xwwxgkmd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2gqigpzfx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2ypnfsjth.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2ghkthviv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2ylgsbprm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2lmolvqeo.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2kxgmjtqf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2anrjvpjo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2slhlnbpi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pxtztfar.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gwjbuiuy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dbmsqchl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2gvumtkwh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2pwczpwaf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ijnddxqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oysmouak.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2eqidfsxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxajmgjw.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2ezosiqaj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2exrjgpyq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2bmszdrsv.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2rfqzewsh.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2retfqqvj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2qpkdwvsi.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mhcbboae.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2jmmsgxcs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2uijasfrh.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2skhgxbzy.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2uiyssojd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2emhljjml.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vvniunwn.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bqhxvert.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2tqnuudov.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2kgtubcch.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2emigdfev.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lebtctau.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2prbgiskn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ntybjcgd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2wvevmvay.html


<!-- 参考信息 -->