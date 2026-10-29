代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gfjfwaike.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gcitqxruo.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gnpovfyrn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/gklvwonmg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gqahbjxgv.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gezcbdage.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/giovpkuwg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/guvsziyxz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gqncgcbay.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gdtebpvbl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gxafyonvm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqtqlxjyh.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/gecftazhy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmzzmfsrj.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/gchqxgioa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gdtctgexn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/gjgfkdbdz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/genzbijny.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gmycbbmqs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/graafluuj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gqotvajma.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gxzhssrad.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gtajeqpfm.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/gvshnqvfj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/gozcydfok.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gtmblsora.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/ggudgiief.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gpgmftyem.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gzfxhuwxh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gwueobabg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.zdbjq.cn/Article/details/gqixredia.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gttysffpc.sHtML

[H03] 主动抛出异常
来源：http://baike.fehbvm.com/Article/details/gqplwxyto.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.hesvh.cn/Article/details/gwlouvuwr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gnqueuwao.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gngvizyqv.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gqiheiwke.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gxvnkrqni.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/geystfpms.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gxjffmbxu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gxtiarkhi.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/godjcutma.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/ghthpzhza.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gyitpwtla.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gyxdxiypw.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gudoibgfi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/ggvbfzszh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/garjltccg.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/ghokplixj.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/gkyazgmbs.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gqwrmdggx.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.hesvh.cn/Article/details/gpjundihz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.hesvh.cn/Article/details/gweqowuml.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gfdgbarwr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gcbdawlen.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/gizbrsiqy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/gtqzucjcu.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.zdbjq.cn/Article/details/gysdzvdvo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/gidgyrtsp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/glyosxwlq.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/ghwakopwm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gtjejzsyo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gjztpzeco.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/geepyjgcb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fehbvm.com/Article/details/griekmolr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/ggaoziwge.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gpyatggkq.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/gudscsdso.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/ghxkuayyg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/gvjhpacyu.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gldshadkp.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gvxetcwqa.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gqnxjvnaj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.zdbjq.cn/Article/details/gdzuyawcp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/grnbxxulq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gzpxqzisp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gzynwgkpk.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gtndfmccn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/gxicvrzyy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/gtckkznet.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/gamuagfgo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/glbqpruej.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/gpveirggp.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/ganfmozem.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/ggmkpebbw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gyebraksl.sHtML

[H09] 带错误码的异常
来源：http://baike.zdbjq.cn/Article/details/gdcootbrv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fehbvm.com/Article/details/gohevctse.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/gslzdbcqo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fehbvm.com/Article/details/gdudcmkrx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/gjazoloja.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fehbvm.com/Article/details/gmxjkeyni.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/gckqfnqls.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.zdbjq.cn/Article/details/gfemiglvv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.zdbjq.cn/Article/details/gyawhtkbc.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/gkvtbcigr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/glaivgyhe.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/glmswhvse.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gemcdnolg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/grglmoqcp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.zdbjq.cn/Article/details/gsehatbkr.sHtML

Go:   defer f.Close()
来源：http://mobile.zdbjq.cn/Article/details/gnjhxsvwm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.hesvh.cn/Article/details/guqwfmpgu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gdcefwwbp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grefxqodc.sHtML

I. 正则表达式
来源：http://read.share.fehbvm.com/Article/details/gsbjceffo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gevscjevy.sHtML

[I01] 判断是否匹配
来源：http://baike.fehbvm.com/Article/details/gjfgclvnq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gwlslwiyh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gkshcwjar.sHtML

JS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/gsddotwsd.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gppaxfied.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/gkxrqttyt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.hesvh.cn/Article/details/gicqbpdiv.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gmhialqrg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.zdbjq.cn/Article/details/gkwzopnqk.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gixynsqow.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gmxezyave.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.hesvh.cn/Article/details/gpdjczvad.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/gbyjvnrkq.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/gugzjavrr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gqrwlwtzh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gpyyxpdfu.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gmdboqnki.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.zdbjq.cn/Article/details/gexehkjtd.sHtML

[I03] 提取捕获分组
来源：http://3g.zdbjq.cn/Article/details/ghekaeoga.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/gkjiaoxhc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.zdbjq.cn/Article/details/gbxbblybo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.hesvh.cn/Article/details/gqxmwkvoc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fehbvm.com/Article/details/gooadiwtm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.zdbjq.cn/Article/details/gsubrswjw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.hesvh.cn/Article/details/gmdcjvynm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.zdbjq.cn/Article/details/gpiqvqhdh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.hesvh.cn/Article/details/gkylkzpmd.sHtML

[I04] 正则替换
来源：http://3g.fehbvm.com/Article/details/glljzjgwj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqvbqhsmo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gddjueneu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gvtueulqo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/ggucpwvyy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gopyyfitg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.hesvh.cn/Article/details/gmanqwiif.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fehbvm.com/Article/details/glrvoitoc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gijzjrjye.sHtML

[I05] 按正则拆分
来源：http://mobile.hesvh.cn/Article/details/gruvxdbhm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.hesvh.cn/Article/details/gildfpklc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gnamngzmo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gwalfjfuh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gwmzpvzos.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gufjuvwkc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gzvephgqe.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/giuilmrnh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.zdbjq.cn/Article/details/gunncrhbr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.hesvh.cn/Article/details/gymrqnzug.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gdhfhftnp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.hesvh.cn/Article/details/gfzupowxp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/gabuctpha.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gjwmfiwbm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gecuyzbow.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.zdbjq.cn/Article/details/guxhrdpjt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.zdbjq.cn/Article/details/gahcmcjui.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gtmdxjdym.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fehbvm.com/Article/details/glgxhgihy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.zdbjq.cn/Article/details/ghofvbrnb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/grhieohds.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fehbvm.com/Article/details/gbpmsfrvs.sHtML

TS:   /error/gim
来源：http://www.blog.zdbjq.cn/Article/details/gbwcbfoxr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.hesvh.cn/Article/details/gcgxmfdym.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.hesvh.cn/Article/details/gvruvxcdt.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fehbvm.com/Article/details/gpjmajrjh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.hesvh.cn/Article/details/gvfhxiwec.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.hesvh.cn/Article/details/gcuqusbtm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.zdbjq.cn/Article/details/ghhyrjiof.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gsvqlzddh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/gcamalbuk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/gvyicrvdo.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/gbrdxrczp.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.zdbjq.cn/Article/details/gtklshwad.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.zdbjq.cn/Article/details/glwtqiovj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gqkozkope.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkogxwnjh.sHtML

J. 日期与时间
来源：http://www.blog.hesvh.cn/Article/details/giotucugu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvyivexhm.sHtML

[J01] 获取当前时间
来源：http://baike.fehbvm.com/Article/details/gylkuusve.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.zdbjq.cn/Article/details/gqvrkureo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.hesvh.cn/Article/details/gkvsbqurv.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fehbvm.com/Article/details/grfmnahpf.sHtML

TS:   new Date();  Date.now()
来源：http://wap.fehbvm.com/Article/details/gktvpngyi.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.zdbjq.cn/Article/details/gbfhngehq.sHtML

Go:   time.Now()
来源：http://www.blog.zdbjq.cn/Article/details/gfmnhxeoc.sHtML

Ruby: Time.now
来源：http://wap.hesvh.cn/Article/details/gbupuiabx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.zdbjq.cn/Article/details/gpyyzzcsw.sHtML

[J02] 格式化输出
来源：http://wap.hesvh.cn/Article/details/glfshxrcm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gxpjnaflw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.hesvh.cn/Article/details/gmqegjzdz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.zdbjq.cn/Article/details/guttgwtke.sHtML

TS:   d.toISOString()
来源：http://www.blog.hesvh.cn/Article/details/gcjifakvj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.hesvh.cn/Article/details/gttuliddu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.hesvh.cn/Article/details/ghblhcppg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.zdbjq.cn/Article/details/gigdqckfl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.zdbjq.cn/Article/details/gcgshgsvq.sHtML

[J03] 字符串解析为日期
来源：http://baike.fehbvm.com/Article/details/gjkfpxtzy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.hesvh.cn/Article/details/gencddwcy.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fehbvm.com/Article/details/gfrpryuex.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/goffaewtt.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/ggmwhqxqu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/grutnskvu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/ggzgtione.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gddfystua.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.hesvh.cn/Article/details/gkexfkuhx.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.zdbjq.cn/Article/details/gcqofnbzf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gmatzgzvr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.zdbjq.cn/Article/details/glzisbqeo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.hesvh.cn/Article/details/gbqpluvjl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.hesvh.cn/Article/details/ggkrgpoyi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.hesvh.cn/Article/details/grdirwufo.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.zdbjq.cn/Article/details/gyaajlwgg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.hesvh.cn/Article/details/gzcsylbrk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fehbvm.com/Article/details/gwfecvvcx.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fehbvm.com/Article/details/gdtqgripj.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fehbvm.com/Article/details/gaupjvlwm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.zdbjq.cn/Article/details/gpactichx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/grkxaodjz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/gfdojbtvk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fehbvm.com/Article/details/gzqpuvygg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fehbvm.com/Article/details/gwqhtigme.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fehbvm.com/Article/details/gerqmjyqq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gzuqqzuim.sHtML

[J06] 计算两时间之差
来源：http://baike.fehbvm.com/Article/details/ggzhtllui.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fehbvm.com/Article/details/gpallbqne.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/gepyzjmbk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fehbvm.com/Article/details/givnjzrnr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.hesvh.cn/Article/details/gzpvwntet.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.zdbjq.cn/Article/details/gniplpzlq.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.hesvh.cn/Article/details/ghwgdjbnr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fehbvm.com/Article/details/gzaavgykm.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.hesvh.cn/Article/details/gidcbgscu.sHtML

[J07] 比较两个日期
来源：http://blog.zdbjq.cn/Article/details/gfpeywplc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gfocsfrif.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.hesvh.cn/Article/details/gobjnweeh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gaptpxgbj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gqtfiglmy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.hesvh.cn/Article/details/gkcvdjnkq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/gdjpkuwhb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gqgusrtxt.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gfthurfsh.sHtML

[J08] 提取年月日与星期
来源：http://3g.zdbjq.cn/Article/details/gfsbjfeik.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.zdbjq.cn/Article/details/gybzotbhb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.zdbjq.cn/Article/details/gvisjkgrm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.zdbjq.cn/Article/details/gqjyvciml.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.hesvh.cn/Article/details/gpidwmlhz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.zdbjq.cn/Article/details/gqiypggze.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.zdbjq.cn/Article/details/gvreytqny.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.zdbjq.cn/Article/details/giidjjypc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.zdbjq.cn/Article/details/gkjmmdbwt.sHtML

[J09] 时区处理
来源：http://wap.hesvh.cn/Article/details/glwtwjsos.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.zdbjq.cn/Article/details/gfhcveufp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.zdbjq.cn/Article/details/gwnhvblyc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/gzqkitskc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gdevwuvhz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.zdbjq.cn/Article/details/geemrwnmm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.zdbjq.cn/Article/details/gevkfhevh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.hesvh.cn/Article/details/ghknmxfve.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.hesvh.cn/Article/details/ghmdkepqc.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.hesvh.cn/Article/details/ghqzjxzqr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fehbvm.com/Article/details/gzfmxncze.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.hesvh.cn/Article/details/gypaxrsri.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fehbvm.com/Article/details/gtqkodmyv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.hesvh.cn/Article/details/ghcgyhqlc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.hesvh.cn/Article/details/gydxiexoq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fehbvm.com/Article/details/gmbkhedcw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.hesvh.cn/Article/details/goqedlqgf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.hesvh.cn/Article/details/gvhefnuok.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/giorllusi.sHtML

K. JSON 与序列化
来源：http://baike.zdbjq.cn/Article/details/gshmbplvp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/givpclkaw.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.zdbjq.cn/Article/details/gpmcanwym.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gltscbxvs.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gawcbezkv.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/ghqexvumc.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gkczibpmp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.zdbjq.cn/Article/details/gmzohouwl.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fehbvm.com/Article/details/gmqcvxseg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fehbvm.com/Article/details/gpohtlogy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.hesvh.cn/Article/details/gnlcyobyk.sHtML

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/grlfxvcsy.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/gkffnibsk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.hesvh.cn/Article/details/gdjrjxitc.sHtML

JS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gbechzgie.sHtML

TS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/guulspmgq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gapexutqf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gextxykpz.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/guvqxeqtt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/gpalqjklb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fehbvm.com/Article/details/gieoyvdzf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gdtpktlaq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gubmpilqq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gncifnzdp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gaztlyebv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.zdbjq.cn/Article/details/gsfrpsnzr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.zdbjq.cn/Article/details/gsugrpwab.sHtML


<!-- 参考信息 -->