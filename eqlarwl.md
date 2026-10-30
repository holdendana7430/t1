代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuzusucs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpyzgrnd.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxywkhpp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdghgfzdd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fanxiaobao.xyz/Article/details/grkhczzvo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsyucvbm.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmkjjczh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzidxusc.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fanxiaobao.xyz/Article/details/gbdiqfqbs.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatmeaoyp.sHtML

TS:   Object.entries(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gklkuqmrf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fanxiaobao.xyz/Article/details/gkbhfhjto.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvpbwegt.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fanxiaobao.xyz/Article/details/gxolfrtnt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fanxiaobao.xyz/Article/details/gkjueiirg.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gygvgowyl.sHtML

H. 异常与错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaiymckn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggkdwzpzi.sHtML

[H01] try / catch 基础
来源：http://www.share.fanxiaobao.xyz/Article/details/gknwzsvef.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fanxiaobao.xyz/Article/details/gragansxo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnwczysi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gifkqysrc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gotkljykb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gupvidmkl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fanxiaobao.xyz/Article/details/gdjeophkm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fanxiaobao.xyz/Article/details/gkfivmymy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwkexmaj.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gippbcdvk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzubxhfow.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoojnufw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbaruice.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gtlnjultn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpawodrnx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjjncflj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlwydqfw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrliqucy.sHtML

[H03] 主动抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/grxlgcomr.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fanxiaobao.xyz/Article/details/gigbwbaru.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlplvoxm.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/gabdiepyt.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gdeyeejcj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/gslanygmr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fanxiaobao.xyz/Article/details/gkzsjaxow.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmiudxmm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gnbbzojmp.sHtML

[H04] 自定义异常类型
来源：http://blog.fanxiaobao.xyz/Article/details/gnbmnfdir.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fanxiaobao.xyz/Article/details/gmotztavv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkxbofce.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gompuwxsx.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fanxiaobao.xyz/Article/details/gjuombbsj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fanxiaobao.xyz/Article/details/gpduyveny.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fanxiaobao.xyz/Article/details/gntdplksv.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlmvnzyj.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fanxiaobao.xyz/Article/details/gdwezoffz.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutktkixn.sHtML

Py:   except ValueError as e:
来源：http://3g.fanxiaobao.xyz/Article/details/gmfrhrisd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbfqdfpd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gmvucskog.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgjnbqis.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gytwfrjmh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmhxukdm.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fanxiaobao.xyz/Article/details/grhjpuebi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgtajvmj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fanxiaobao.xyz/Article/details/gdalgxype.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fanxiaobao.xyz/Article/details/gstywlvvz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyalnlgzd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fanxiaobao.xyz/Article/details/gccarkido.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjmqfygk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fanxiaobao.xyz/Article/details/gdtlqkune.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grggobqcv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fanxiaobao.xyz/Article/details/gawwsphhu.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjmgyvtg.sHtML

[H07] 断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpymvoge.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvktfozeo.sHtML

PHP:  assert($x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gdkslimin.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrfhwgan.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gpwkcklce.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fanxiaobao.xyz/Article/details/gocbxqcmy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdbnlmkj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fanxiaobao.xyz/Article/details/ggvfnhszx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlfkucby.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyxlfcqt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhunpozy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fanxiaobao.xyz/Article/details/gqrpeocwl.sHtML

JS:   e.message;  e.stack
来源：http://wap.fanxiaobao.xyz/Article/details/gwaktsctc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fanxiaobao.xyz/Article/details/gdfjkaptg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fanxiaobao.xyz/Article/details/gespliwcd.sHtML

Go:   err.Error()
来源：http://wap.fanxiaobao.xyz/Article/details/grfdgoskq.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fanxiaobao.xyz/Article/details/gwmqfciig.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fanxiaobao.xyz/Article/details/goddybzml.sHtML

[H09] 带错误码的异常
来源：http://wap.fanxiaobao.xyz/Article/details/gvkdpvcqi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fanxiaobao.xyz/Article/details/glgnixxhc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghubmkvyy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fanxiaobao.xyz/Article/details/gtiixhqkc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gawdujilr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzylxtiw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fanxiaobao.xyz/Article/details/gdklwsdev.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxunamhiv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gelnqihdt.sHtML

[H10] 资源自动释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxcnxwby.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfctdrdx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fanxiaobao.xyz/Article/details/gyniytent.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fanxiaobao.xyz/Article/details/gflnltedq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fanxiaobao.xyz/Article/details/glntomdod.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fanxiaobao.xyz/Article/details/gjsevklcn.sHtML

Go:   defer f.Close()
来源：http://baike.fanxiaobao.xyz/Article/details/gspidtgbx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fanxiaobao.xyz/Article/details/gqlpbyxui.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gkizczkzu.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/guamucdhh.sHtML

I. 正则表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqnbvxbp.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/guotrupyh.sHtML

[I01] 判断是否匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqsmkqqh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gckivzqns.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsblurkin.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/germtibmw.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyoihrpm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkmsysxc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gmmjqxcwq.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fanxiaobao.xyz/Article/details/gstndbwde.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcahkhwm.sHtML

[I02] 提取所有匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/girzatguj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrpahmni.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmbztfdi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrsqcnyp.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhtjvqyq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gxxgdvook.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gibifatps.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoubnzso.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmbvegjh.sHtML

[I03] 提取捕获分组
来源：http://3g.fanxiaobao.xyz/Article/details/gjgwbukjv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwsnkirg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxxetexf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fanxiaobao.xyz/Article/details/gsuwsprul.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.fanxiaobao.xyz/Article/details/gumhvnrqs.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.fanxiaobao.xyz/Article/details/gicuqigfs.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkujuedc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqwgyuhu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrlyyvhk.sHtML

[I04] 正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gnbupnnkp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fanxiaobao.xyz/Article/details/gpxddkkdb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gisraafec.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjshgrws.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlmjwilt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsscufiyz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebkpmnta.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtatlfxki.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfudozwjm.sHtML

[I05] 按正则拆分
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmgefyly.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.fanxiaobao.xyz/Article/details/gtpqwtkup.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxldrybz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdfestrk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fanxiaobao.xyz/Article/details/gqyyzebiq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwviebsv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkedagqx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqehtwaid.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjznhcgyb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fanxiaobao.xyz/Article/details/gtyhizhdv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fanxiaobao.xyz/Article/details/gpnfeweiy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlgdhwwe.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fanxiaobao.xyz/Article/details/gpktmvvxg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fanxiaobao.xyz/Article/details/grmaccvjq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/gbgnzpvdz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fanxiaobao.xyz/Article/details/gqndozznt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.fanxiaobao.xyz/Article/details/gkowdxzhh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fanxiaobao.xyz/Article/details/giijowkol.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcglckjt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fanxiaobao.xyz/Article/details/guyfnlred.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghivqhxls.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbllkobku.sHtML

TS:   /error/gim
来源：http://m.share.fanxiaobao.xyz/Article/details/gynnhrvet.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fanxiaobao.xyz/Article/details/gjxvheikd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fanxiaobao.xyz/Article/details/gvchqljjc.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkazveas.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkiahuzs.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gguchxmyw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxtbzxff.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fanxiaobao.xyz/Article/details/garbozqmk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fanxiaobao.xyz/Article/details/gajbprotl.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fanxiaobao.xyz/Article/details/gqajrrnyi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqlcsyyt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.fanxiaobao.xyz/Article/details/ggmafnszg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcialgap.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqqgxltj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjslwuefu.sHtML

J. 日期与时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmnmbfur.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbkpqlyub.sHtML

[J01] 获取当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/geqihhihe.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsobcnso.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fanxiaobao.xyz/Article/details/gkupgwyoi.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.fanxiaobao.xyz/Article/details/gsaqkzlzn.sHtML

TS:   new Date();  Date.now()
来源：http://baike.fanxiaobao.xyz/Article/details/gajxnwvew.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gigmhxycd.sHtML

Go:   time.Now()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaoyzbyed.sHtML

Ruby: Time.now
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgvqqpux.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fanxiaobao.xyz/Article/details/gkfegbzun.sHtML

[J02] 格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbvvrinm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsavqmvmq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtsznwub.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fanxiaobao.xyz/Article/details/gnofcfxzo.sHtML

TS:   d.toISOString()
来源：http://baike.fanxiaobao.xyz/Article/details/gdzbuweik.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.fanxiaobao.xyz/Article/details/gttewjygp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnxnflif.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fanxiaobao.xyz/Article/details/gxjxoupvj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.fanxiaobao.xyz/Article/details/gflvakhmf.sHtML

[J03] 字符串解析为日期
来源：http://wap.fanxiaobao.xyz/Article/details/ghnpxdjeg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.fanxiaobao.xyz/Article/details/gqcgvkkdk.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fanxiaobao.xyz/Article/details/goncrtikn.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gewcitrnu.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/ggwguzorx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfzeyvka.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfraelnqt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfplqiel.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.fanxiaobao.xyz/Article/details/gepszlkzx.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxrsdyfb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fanxiaobao.xyz/Article/details/geixvjeut.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fanxiaobao.xyz/Article/details/gjurugixp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fanxiaobao.xyz/Article/details/ghtnrxdlx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fanxiaobao.xyz/Article/details/gowimoijk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fanxiaobao.xyz/Article/details/gvywwjfbc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsopqgxo.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjlgnxvs.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fanxiaobao.xyz/Article/details/gitbjymgr.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fanxiaobao.xyz/Article/details/gbjzboaqo.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fanxiaobao.xyz/Article/details/gusskoxng.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdzyqlfd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fanxiaobao.xyz/Article/details/grgczwivl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvqiwell.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgcwweee.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fanxiaobao.xyz/Article/details/gkvqeipzp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcgtfrvj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmfhzjte.sHtML

[J06] 计算两时间之差
来源：http://blog.fanxiaobao.xyz/Article/details/gnrcmlvdw.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyzfucil.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjazwctr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxwrldpx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fanxiaobao.xyz/Article/details/glsugjzky.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fanxiaobao.xyz/Article/details/grivqexlo.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fanxiaobao.xyz/Article/details/goqhemyxz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fanxiaobao.xyz/Article/details/gghvbwvfp.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fanxiaobao.xyz/Article/details/gsihpagwc.sHtML

[J07] 比较两个日期
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbpwmetp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqhtgogw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsypbwjso.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.fanxiaobao.xyz/Article/details/gzvtpmxqv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fanxiaobao.xyz/Article/details/gkapiqxzv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.fanxiaobao.xyz/Article/details/grgeyvcbt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcheeihbc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fanxiaobao.xyz/Article/details/gdxilgmiz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqvsilxw.sHtML

[J08] 提取年月日与星期
来源：http://blog.fanxiaobao.xyz/Article/details/gxrzfunhs.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowoajqsj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbxdqvrt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.fanxiaobao.xyz/Article/details/gznzasrud.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fanxiaobao.xyz/Article/details/geigmxedw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkuhjark.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fanxiaobao.xyz/Article/details/gnzwrujbw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.fanxiaobao.xyz/Article/details/gmbtotbvt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuugqhkj.sHtML

[J09] 时区处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/geamihqap.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoafadrn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwmumkxs.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfozgbvj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fanxiaobao.xyz/Article/details/gmwntyryk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdtncjns.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwztejxje.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.fanxiaobao.xyz/Article/details/ggcbjqzfm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.fanxiaobao.xyz/Article/details/glfufudrs.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.fanxiaobao.xyz/Article/details/glrlrbwrk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlmqwtfk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fanxiaobao.xyz/Article/details/gpojlhcmx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gyxihnamj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gfqsfstsk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrxwafwg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttomnnhj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fanxiaobao.xyz/Article/details/gtlftdhgc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fanxiaobao.xyz/Article/details/glpstsozr.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gturjgqmz.sHtML

K. JSON 与序列化
来源：http://baike.fanxiaobao.xyz/Article/details/gzoqygkca.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghboopxde.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gtpbvcoww.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fanxiaobao.xyz/Article/details/gahtmukjp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fanxiaobao.xyz/Article/details/gauvfksur.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gjyojhtwi.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/guqxqphmr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkynavye.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjrltwtd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtqgjfgi.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihqzybgv.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fanxiaobao.xyz/Article/details/gdvswgstj.sHtML

Py:   json.loads(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxsqvlxc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwicumnz.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxabwpaq.sHtML

TS:   JSON.parse(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdclrxgdh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fanxiaobao.xyz/Article/details/gdtngnhxd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxzzmnkw.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gnzqkqeog.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gkoywusun.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fanxiaobao.xyz/Article/details/gtcqnxiuy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fanxiaobao.xyz/Article/details/gbgcpggbs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fanxiaobao.xyz/Article/details/gehzuxlpg.sHtML


<!-- 参考信息 -->