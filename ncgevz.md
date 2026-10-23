代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3fncfcrbr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kdetpgcz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3inarubjd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3iltdyqei.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3vzkwfkta.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3cukirnjk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3mtwdzsva.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3jubmjgar.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ncbxunxb.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mqbdwvnd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vcdxopmy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3cdpccvwz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3tlgkoatb.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3amljemub.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3efbksojb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ozxiybik.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3irxusznc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qmnavavm.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ndzcqxds.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3dacdctei.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ifhvggli.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uifnguyr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3awysjnex.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3yefiltph.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3tbnesltf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3famztbbn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3phxrjoon.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3tqohgude.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3yidiohpc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bepghrsk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3idfueczo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3myejelld.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xunhlalx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3unzdnnpo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3vhpgfter.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mxidhatv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3hevgmapx.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3nrxtbqdi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hqejxjzk.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bcuajanl.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3agyddoij.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pfeoxzmj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3wyekcvbg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3qbalpujv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cnagzebg.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3fvuezqns.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3nvyneilx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3pidyyjka.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3oampikhk.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3eatyvhae.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3eyqrvvqe.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3xrilgbwc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3pcmwsswb.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3iucvvmnx.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3zilyiafd.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3vjptzsvc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3jvjhkrtu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tifacaav.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3nbmfyaoz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ilvrtygi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3yezhuewu.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3bhxphunb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3dckcjvnl.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3sobgnths.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ntzimuax.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3dirlayjr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3safvnruo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3etdcvigs.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3tyduzyfv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3smyhbszv.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3vmtndykh.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3mlbwiusu.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3owcewafr.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3etwmqpdy.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wfkemohu.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lgpzhrvu.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gafufefn.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3gzpgmcgh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3tgrncnak.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3ajwxousk.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3somgpyiw.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3pfjkthxy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3mycvbvsj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3udhwadqu.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3rcitdmlg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3lrphjsbp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3jrqqthdm.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3bgugskkr.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3mkhixnmr.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3uqbwrdow.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3vtcbivjw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3nglcxenm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wwqzxisg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3utqdwyuz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3kfdpfpuo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3haqencki.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3rlymovuo.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3epxncjdl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3ywncnwfe.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3silydwch.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3vqziiqfc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3lholthqe.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3uafpoyga.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3hotppsyq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3mvrszdnq.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3npvdtsso.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3znfksvgm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eretfpdw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nvczornp.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3agtcwrkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gqnkqydz.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bdmvbluw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3myyucpxz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3aovxcjxr.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rbabncji.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ngnvnokx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3luvlhvwe.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3fbnwnyyq.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3kgzuebav.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hsjlqxqh.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3jxzvoirk.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gffendrt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3yilnxmku.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3onhpptey.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3vsomqali.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vkjsxqkh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3imemxdyj.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3tqhufbek.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tlajewpq.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3ukgylhne.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bmbixjka.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3thqqywlp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3favgpkuu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3evhtndco.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3stlpkbdm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3umovdbqa.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bqqnwdrv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3ceseybte.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3srmnczzh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3khltlkxb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ehhhnsbo.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vyvqjssy.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mjaeaohv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ounkjujv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gijgyjlr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3oyqmmoum.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3wwcbiecz.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pgctwbta.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bfdfwzfy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hbirycrt.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3prnmoxji.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ssywxbat.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3mfgmbimi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3tvrlzyrv.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3qgeuafzt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3meiyobpg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3vwejmxdy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3povfeqwz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3cddquznx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3snulmehp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3rjxexntg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ygmqhxkm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3ddsujosg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3iidvdxsz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3vhyrdfvp.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3qttefysq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3dsblypmw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ygmuquab.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3eewqukmd.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3egrpjqfm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3fohhmbjg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3stvttxks.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3fqlhyzab.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3qqdimzpw.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ieossrqi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3tzgtybiz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3rrsftmna.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ieiyrukh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3diwpbouf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3otvxkewm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3omzxijgv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3znouprnt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ytolpfwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jbqtviep.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3zbvhschw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xunzslpt.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3iiaaoqkf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3pgdicowi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3edzyogpe.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3aylcsuyx.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3oytiiazk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3phdyrmoj.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3kzbcaibd.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3jlugnzis.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3dwxbndpy.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3tiiskthf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ubliuuxr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3kdexktwt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3iarldces.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3ebmxsgjc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3jkajrbvw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3rzefjjjm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3owwkacvw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3zckcrzih.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3fmegnrmn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3wscalbhx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3hcrnkdgy.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ysvozzbg.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3exbbllex.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3jxzenizf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xvvzsdcl.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3dtkkhass.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3losuwhte.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3nehjbbxu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3izibddfx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3znzndczw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3msojqbke.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3erfpyxvl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3tfrfxysd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pxscckey.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3csmdbbcv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3tnpojnmj.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3drvmupcq.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3ghwkobko.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3nquuzrlr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3bcyhlwyo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3heuzgwje.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3rhedtewc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3byefitka.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3qqfyinlh.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3dpavwhuv.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3qvorntci.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3rnxsejcd.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3udlvwbxy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3ehoszoms.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3knbamktk.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3qrviwufg.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3iambtcih.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3xghsmjtv.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3zowtvtyi.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3uxiiyvua.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3sogguczv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3ecmpdrnn.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3lxvsgzrf.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3yaeyzptt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3cmaengxa.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3fdddzgvs.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3vsoossfg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3sccpiabh.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3bvulmyqu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3qcblcnqr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3vkcshcpu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3esjyfmor.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3mfpqsvlh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3muzvwtsm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3abkucass.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3qrpksnwg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3nockcers.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3wotyjubu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3mjhtcuqm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3cnhwgnti.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3jifztnlb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3lhnqagso.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3qwhuepeu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3iptkjccw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3spimwzgf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3xjxmqkil.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3abadmnvu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3xdzsirln.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3pvmbzvvm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3prkgbxiz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3nqkxuwaa.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3skprfesh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3iqphibzq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3lydddnvg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3atwqzvct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iqnqiszi.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3bnncwjbw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qcucuhjq.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3uvxjozzp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3uuoqzedr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3cxrdjsxa.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3zdxdxlrm.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pzeilwxe.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3ympimkew.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3wdotbkwe.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3xzvzgujo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sdfyaswj.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3tryfrkds.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3geekksfq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3qozpninm.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3etylddns.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ocgckvhy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3bvtliehu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3zwapsfsa.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lylobhzo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3cubnhbne.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3tfwvrmjn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3huyxqsyn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3txqvlgyq.html


<!-- 参考信息 -->