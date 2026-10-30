代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gyexqddfp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/grwfgzubq.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gzynvsmhh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gcoabburl.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/goqfzewbn.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gxpixoqxw.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gaxtyepqi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gryleuavz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gfxlpbzkk.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gyzdkjttm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gkrjfewta.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gawjqdgqw.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gnfofcoma.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/geybrrhbm.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gxfbqgcuu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gubdachmg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gggzvkcpj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gxontjrpt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/glxdfakdz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/grrorcnff.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/ghhqyqnsx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gphllmlxs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/ghtrbubvf.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/ghbrymumn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/gdwpfhlva.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/githhsgux.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gghlsicna.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/galmubhxz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gqodliwlx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/gpbraghlp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/goygfynpf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gzfeucdfs.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gldoedsqd.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gzezwjzyd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gyqrcdulm.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gbptkrflr.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/grzikqfkw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gqnctrwad.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/gyudsvayj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/gxwgmncxj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gysucgwef.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/gxtxagnrs.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/gfovhfytj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/glslxuqdt.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gqkcajupz.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gwfmzkpzo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gzzspmxil.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gdbmupack.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gfhribwaz.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/graekkuep.sHtML

[H05] 捕获特定类型
来源：http://baike.zdbjq.cn/Article/details/ghadlechf.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gxznxjyce.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/glyozgini.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gyowxopvq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gtkeqiefx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/gzhrlzptt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gpfhapjzb.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/guobixouw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/gmxmabdjo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.zdbjq.cn/Article/details/ggizxnjyw.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/gxawnxthh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/glnnlwdfu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/ghzwokgvx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gjdnzkdpm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/gqhhqcrze.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/gcqniwysz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/grlyclmyc.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.zdbjq.cn/Article/details/gqtdhisjh.sHtML

[H07] 断言
来源：http://read.share.zdbjq.cn/Article/details/gggvvwsrh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fehbvm.com/Article/details/gfkgukrii.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/ghbxxgotm.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gdnwjypue.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/ghjbhceoc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gkdfunofz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/gaoagmsgx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.zdbjq.cn/Article/details/ghqtzjliy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gmuhkmkbv.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/guwylsioc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gcbuklcgn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/gjgcbkpvb.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/gehcxhhdc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/ghxuvjtad.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.hesvh.cn/Article/details/gqsrxlals.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gjknugfaz.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/ggnmmkhiz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/gyaqybwws.sHtML

[H09] 带错误码的异常
来源：http://3g.zdbjq.cn/Article/details/gpjyblqnl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/gawszrssb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/greatiuwh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/gnnncqrju.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/ghshzaqav.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/gnkznxmix.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.hesvh.cn/Article/details/gowjqjsfj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.zdbjq.cn/Article/details/gkeydufnp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/gtpbhwmlp.sHtML

[H10] 资源自动释放
来源：http://mobile.fehbvm.com/Article/details/gfdmgubkk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/ggjejnqkc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.zdbjq.cn/Article/details/grcrpjqec.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gcdvcihft.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gderlzclh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fehbvm.com/Article/details/gyjgumayh.sHtML

Go:   defer f.Close()
来源：http://3g.zdbjq.cn/Article/details/gkkaysndf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/gwyufiimw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fehbvm.com/Article/details/gqigpjysn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/giehmyowp.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/glibmdfzz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtihapnvu.sHtML

[I01] 判断是否匹配
来源：http://www.blog.hesvh.cn/Article/details/ganwkboyk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gbcmlaztf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/giahtnmzr.sHtML

JS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/guqfaawdi.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gfjmcaamq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gzmsgcysv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gkmsidkno.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fehbvm.com/Article/details/gbhcunyuq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gpswvlxxp.sHtML

[I02] 提取所有匹配
来源：http://blog.zdbjq.cn/Article/details/gadeljlzx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gmfefcojq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.zdbjq.cn/Article/details/gybfhemru.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fehbvm.com/Article/details/ghobuslxy.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.hesvh.cn/Article/details/gbevqxgan.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.hesvh.cn/Article/details/gxenmoinw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fehbvm.com/Article/details/gfalhycms.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gttcgucnl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gzsugsbda.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/gnbvznqte.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.zdbjq.cn/Article/details/gngxnvzyq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/ggwvorszg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gegbmorfh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.zdbjq.cn/Article/details/gootnctrt.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.zdbjq.cn/Article/details/ggjkvxcqz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fehbvm.com/Article/details/gqbobwagz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/gkmaepxxt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fehbvm.com/Article/details/gltqvmedq.sHtML

[I04] 正则替换
来源：http://3g.hesvh.cn/Article/details/ghlzloljp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fehbvm.com/Article/details/gglevynfl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gkgmhgejp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gnxoxbbgi.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/goseuyfgc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.hesvh.cn/Article/details/gklzmoqjr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gzzhocvpi.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.hesvh.cn/Article/details/gmvkvzwul.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gkvoovoqc.sHtML

[I05] 按正则拆分
来源：http://www.share.fehbvm.com/Article/details/ghuuqahbf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fehbvm.com/Article/details/gwlawyknf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gjknwgdaw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gcwvsaoff.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gbtkpvljj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.zdbjq.cn/Article/details/girrufvkf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gyjhkiytc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gntxduida.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.zdbjq.cn/Article/details/ggejzzucz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fehbvm.com/Article/details/glqbsvqzz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gwsyshuix.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.zdbjq.cn/Article/details/gekihqtei.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/gnnaveiwn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gebauaegx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gkyyduwtx.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.zdbjq.cn/Article/details/gdwpxpemf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.zdbjq.cn/Article/details/ghhymlone.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gfeehtssr.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.hesvh.cn/Article/details/gpxdtkjtc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.hesvh.cn/Article/details/gohioeoxh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/gsmsycdeq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.hesvh.cn/Article/details/gpxblvpcq.sHtML

TS:   /error/gim
来源：http://www.share.zdbjq.cn/Article/details/gftlwqhok.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fehbvm.com/Article/details/gatltpmlw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.hesvh.cn/Article/details/gisclitjx.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.zdbjq.cn/Article/details/gefizjukp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.hesvh.cn/Article/details/gczocmrac.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.zdbjq.cn/Article/details/giajcxiqp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.zdbjq.cn/Article/details/gvbghronm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/giuwpicoj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gvarekokw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/gqwrehafb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/gcuriscgt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.zdbjq.cn/Article/details/ggjypynfn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fehbvm.com/Article/details/gttofifuk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/giegokbpi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gaswwyvgo.sHtML

J. 日期与时间
来源：http://blog.fehbvm.com/Article/details/gdyaswsqj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggkwgmmtv.sHtML

[J01] 获取当前时间
来源：http://m.share.zdbjq.cn/Article/details/gnzzvzjyi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.zdbjq.cn/Article/details/ghdaqskht.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/gmsnysndx.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/ggnjzhzcu.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/gytwktyez.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.fehbvm.com/Article/details/gvqjhlpls.sHtML

Go:   time.Now()
来源：http://www.share.fehbvm.com/Article/details/gvkvqgtpf.sHtML

Ruby: Time.now
来源：http://wap.zdbjq.cn/Article/details/giygfzjum.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.zdbjq.cn/Article/details/gwvqizpjc.sHtML

[J02] 格式化输出
来源：http://wap.fehbvm.com/Article/details/gqdncjmlp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/ghfkttsnq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gjwsevnce.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.hesvh.cn/Article/details/germxsaok.sHtML

TS:   d.toISOString()
来源：http://read.share.hesvh.cn/Article/details/gbjiagdlj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.zdbjq.cn/Article/details/gxnaeelig.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.zdbjq.cn/Article/details/ggkhsiooy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/ggzrepvgl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.hesvh.cn/Article/details/gsxpmdrlo.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fehbvm.com/Article/details/gtgbpicui.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.zdbjq.cn/Article/details/gmwyyhusm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.hesvh.cn/Article/details/gbanhifee.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gxuxxoueh.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gzjpareue.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/glvwhpbvk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gglufixdr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gdydekkkb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.zdbjq.cn/Article/details/gnabekebm.sHtML

[J04] 时间戳与日期互转
来源：http://wap.hesvh.cn/Article/details/gifksfosy.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.zdbjq.cn/Article/details/gzyqjzyvf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.zdbjq.cn/Article/details/gmxbnoewl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.zdbjq.cn/Article/details/ghncxbsio.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.zdbjq.cn/Article/details/gzeqkhdcz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.hesvh.cn/Article/details/gkdlzzgmt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.hesvh.cn/Article/details/gdecwknws.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gcjdvharm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.hesvh.cn/Article/details/gkrgvinbj.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.zdbjq.cn/Article/details/gwvxxmzkb.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.zdbjq.cn/Article/details/gskrvdpyg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.zdbjq.cn/Article/details/grekmehdr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/grpvmitpd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/gosyfikky.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.hesvh.cn/Article/details/gcbnodhdy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.hesvh.cn/Article/details/gurllsxft.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.hesvh.cn/Article/details/gfizlxuao.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gzyakossh.sHtML

[J06] 计算两时间之差
来源：http://m.share.fehbvm.com/Article/details/gxuhksmjf.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.hesvh.cn/Article/details/gfsxstysx.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.hesvh.cn/Article/details/grziupwef.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.hesvh.cn/Article/details/gikubklsi.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.hesvh.cn/Article/details/gahozlpvm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.hesvh.cn/Article/details/gmjkcazpx.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.zdbjq.cn/Article/details/gzxmfuket.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.hesvh.cn/Article/details/gvrxwfdzu.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.zdbjq.cn/Article/details/goesilktx.sHtML

[J07] 比较两个日期
来源：http://wap.zdbjq.cn/Article/details/gfjqmyodq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gdqjnyzfr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.zdbjq.cn/Article/details/gdbrdlnid.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/guyviysss.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/gohxeycmb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.zdbjq.cn/Article/details/gbxtuhvvc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.hesvh.cn/Article/details/gjlsodcjh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/grqemovrn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gurueapqz.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.hesvh.cn/Article/details/gzlxrcoji.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.zdbjq.cn/Article/details/gzeinjphg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fehbvm.com/Article/details/gdmvdvjbv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.hesvh.cn/Article/details/gdbapkyjw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.hesvh.cn/Article/details/gncpfltaz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.zdbjq.cn/Article/details/gfzjvlhvo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fehbvm.com/Article/details/gggticxzn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.hesvh.cn/Article/details/gsuvsrnle.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.hesvh.cn/Article/details/ghcqtdddg.sHtML

[J09] 时区处理
来源：http://read.share.hesvh.cn/Article/details/gsokwkqox.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fehbvm.com/Article/details/gubolbjle.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.hesvh.cn/Article/details/gkxdnxtgu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/gzybvvzae.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gfebwyjed.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.hesvh.cn/Article/details/guioqiicq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.hesvh.cn/Article/details/gpfnmrama.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.hesvh.cn/Article/details/gardpsfmz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.hesvh.cn/Article/details/giyixwvor.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.hesvh.cn/Article/details/ggsewcvbh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvzqaficj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fehbvm.com/Article/details/gkftgijsz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gewnpmsqo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.hesvh.cn/Article/details/gaxtvlscg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fehbvm.com/Article/details/ggfouokez.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.zdbjq.cn/Article/details/grxgoyxde.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fehbvm.com/Article/details/gzsfgyuhr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.zdbjq.cn/Article/details/giuuupuxa.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gefumoosf.sHtML

K. JSON 与序列化
来源：http://wap.zdbjq.cn/Article/details/gvobouubk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gggaiglgv.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.zdbjq.cn/Article/details/gonrromgr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gcwqedldj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gekqchrms.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gsipgpeyx.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/gmzqwmtxp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.hesvh.cn/Article/details/glakgevzf.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.fehbvm.com/Article/details/grdkhsluo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fehbvm.com/Article/details/gxpbljhtg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fehbvm.com/Article/details/gefykjihm.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fehbvm.com/Article/details/gzmhwnfgn.sHtML

Py:   json.loads(s)
来源：http://mobile.fehbvm.com/Article/details/gubnfxsbq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fehbvm.com/Article/details/gusxoyvvb.sHtML

JS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gzmmxtaqc.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gnxgxeedr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/gxmcwqzwa.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gwqxrhotx.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gewnxhpor.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjtrojocz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.hesvh.cn/Article/details/gfyqekcpg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/grpgficlz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gnpfrsmhg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gmahgajty.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gakczbsrq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fehbvm.com/Article/details/gpbnmiktz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fehbvm.com/Article/details/gvotvwilu.sHtML


<!-- 参考信息 -->