代发 wailian999

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gzojqrakz.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gkacspggi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gyxhnvbhz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/ggeoiulwz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/gkbedhont.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gkcwkzbxo.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gpgpmiybf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gxkgkuwiz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/grprmcxuq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gurxmseth.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/gtukcqdqi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/gvbkuauoj.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gawbllylb.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gpccncmnf.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gjmtsacqh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/gtyptsoba.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gyovjlmgl.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gyroxzrrq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gvekkuzgx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfbwmfang.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gvqvmuttd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwdrrpdkv.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gohseriwb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/ghopzwziy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gqtthbphk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gpedsoyus.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gcvkccelo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gujweeakv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/gqjvmxzhh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/gyzmoyyut.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gzfwxeypn.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/glunquvne.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/ggwoismgr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gswsodjpl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gwdnotuuj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gjxdhivgm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gmleupyrs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gycafrjqv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gwhiuupbx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gzvnlalxm.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gaicroeux.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/geupzodxd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gpuogzzqv.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gdnlhwfqm.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gdcnqfdno.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gthjqxglf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gaqsodnsg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gvjuaybwd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gztzzsooy.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/gekjnuuhl.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/gzzipdmtv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gqncukzfp.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/grbcomyqo.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gcfxoseae.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gyzvtreqn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/ggzwemcob.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gjtkiruay.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/gimvlbnjg.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gutluisrp.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/gfscvvwdq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gsiduwxyu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gurzhiwuk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/galjxvbnb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fehbvm.com/Article/details/gjajbxyrz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/gzkosvjzi.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gdxgfqzha.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/gdlyzyvcz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gqzvflojn.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gsqearguo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gxbsytyjy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gwqqtxjxc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gkeuumurd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.zdbjq.cn/Article/details/ggknxtmkn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/ggxoszmbo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/gvurgnnti.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gmwcmkitf.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/glgvkbmeg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/geohkwiud.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/gsmnnxgke.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gqrmemsul.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gozfyxsmq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gpktwhtvn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/guqozbbas.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.zdbjq.cn/Article/details/gficatxzi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gscvdiiam.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/grzdphjdg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/goxptbqss.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.zdbjq.cn/Article/details/gcgufwvnl.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/gdzprcdpq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/ghajhbscc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fehbvm.com/Article/details/gmdhaauip.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gcduqsazf.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/gvptbmcch.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/ghxrumtaz.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/gejzodiig.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/ghuibgsgg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gjudfpczf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.zdbjq.cn/Article/details/gcczbpqms.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/gecglpfmy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.zdbjq.cn/Article/details/gxidrnwgb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fehbvm.com/Article/details/gdnylfubp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fehbvm.com/Article/details/ggreaqaao.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fehbvm.com/Article/details/gtdyzigmp.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/gblnbavho.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/gdoqksprw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fehbvm.com/Article/details/gflrlyyyd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gerbkieeu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gwzetjakm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.zdbjq.cn/Article/details/gixzszdcd.sHtML

Go:   defer f.Close()
来源：http://m.share.hesvh.cn/Article/details/gghavchxx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/gloiqxpar.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.hesvh.cn/Article/details/gowogowyu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdltcmady.sHtML

I. 正则表达式
来源：http://read.share.hesvh.cn/Article/details/gwebvogov.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gukhoqvmr.sHtML

[I01] 判断是否匹配
来源：http://baike.hesvh.cn/Article/details/gatfzxnef.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/ggtedxbqk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gxcshcuxu.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gjvcsgbgh.sHtML

TS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gkjwywdvi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/glwiotxoi.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.zdbjq.cn/Article/details/gfnwihfep.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gqcmaifmd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fehbvm.com/Article/details/gvlmmrkns.sHtML

[I02] 提取所有匹配
来源：http://www.blog.hesvh.cn/Article/details/gytpgltau.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gpdpkohgn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fehbvm.com/Article/details/gkmtnchpy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/gbsiqygfc.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fehbvm.com/Article/details/gtkqncxdg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.zdbjq.cn/Article/details/ghsibgovc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.hesvh.cn/Article/details/gyzogagaj.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gfbbihekc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/gaaaxxgzb.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/gmxpqqlrh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fehbvm.com/Article/details/gtvkanuja.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.hesvh.cn/Article/details/ggtkumljx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gojrdwxwm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/giwozvdos.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/gzgeypdit.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.zdbjq.cn/Article/details/gyqjezgyo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gfmtvvfas.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.hesvh.cn/Article/details/ggqxobnzu.sHtML

[I04] 正则替换
来源：http://wap.hesvh.cn/Article/details/gimsoaruc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.hesvh.cn/Article/details/ggaatbtlr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gzlghmuac.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gzkvjjzja.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/govuiuuec.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gekuiukop.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fehbvm.com/Article/details/gtymovouo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fehbvm.com/Article/details/ghkqirxld.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.hesvh.cn/Article/details/ghuovrqvm.sHtML

[I05] 按正则拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gjqbkndzp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fehbvm.com/Article/details/gyjtsjpbo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/gxnhtqyug.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gyemxxzft.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gsdhansqp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gcauxmfcs.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fehbvm.com/Article/details/gtfxxohel.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gmuofmabk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fehbvm.com/Article/details/ghfumzszq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fehbvm.com/Article/details/grobmxffx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gpwhsrdoy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.zdbjq.cn/Article/details/gndqopeez.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/gheigdyjm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gchpqeqoo.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/ggrowegla.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fehbvm.com/Article/details/gxnjgrjom.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.zdbjq.cn/Article/details/gggexunvs.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/ghjqmufig.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.zdbjq.cn/Article/details/gkvctiwiu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fehbvm.com/Article/details/ggfzcqsrb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/guiydghxy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.hesvh.cn/Article/details/gdtzxzaos.sHtML

TS:   /error/gim
来源：http://baike.zdbjq.cn/Article/details/giapdrfwf.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fehbvm.com/Article/details/gxnvkbqdg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.zdbjq.cn/Article/details/grfhrtosa.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.zdbjq.cn/Article/details/ghfgvqmmz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.hesvh.cn/Article/details/ggiwunvse.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.zdbjq.cn/Article/details/gfhlmefth.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.zdbjq.cn/Article/details/gbfijfqdu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gepszuvxd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.zdbjq.cn/Article/details/godzkusew.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gmromjvng.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gxdrcvvrz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.zdbjq.cn/Article/details/gwcbrydzh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fehbvm.com/Article/details/gdvyqslpn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/gdkyyhdrp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfwblwmwf.sHtML

J. 日期与时间
来源：http://baike.fehbvm.com/Article/details/gndlfnook.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gknlevwfd.sHtML

[J01] 获取当前时间
来源：http://wap.fehbvm.com/Article/details/gvurbxjvj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.hesvh.cn/Article/details/gwsfnwiyi.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.hesvh.cn/Article/details/gtmxsfkhe.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/grskzdhxi.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/ghufyzrsc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fehbvm.com/Article/details/gwampqapo.sHtML

Go:   time.Now()
来源：http://baike.zdbjq.cn/Article/details/grzkrewng.sHtML

Ruby: Time.now
来源：http://m.share.fehbvm.com/Article/details/gtzcrbedh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.fehbvm.com/Article/details/gshizkkax.sHtML

[J02] 格式化输出
来源：http://mobile.fehbvm.com/Article/details/gtfugrsrk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gngwzblza.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.zdbjq.cn/Article/details/gdrunvcan.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.hesvh.cn/Article/details/gmvkenjiy.sHtML

TS:   d.toISOString()
来源：http://wap.zdbjq.cn/Article/details/gmuvribmk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.zdbjq.cn/Article/details/gevvgwdfr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.zdbjq.cn/Article/details/gladvugjo.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.zdbjq.cn/Article/details/glanlxnsc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.zdbjq.cn/Article/details/gffxjlxql.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fehbvm.com/Article/details/gumijrkwl.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.zdbjq.cn/Article/details/gbhxahcvz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.hesvh.cn/Article/details/glqiclwxn.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gxtegtadb.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gckynfirr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gvxpvvmau.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gyfyixtbu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/ggflhfkvg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.zdbjq.cn/Article/details/gpmiiclga.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.hesvh.cn/Article/details/gxvjcscjy.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fehbvm.com/Article/details/gxaepiqma.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.hesvh.cn/Article/details/gbboegyyx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.hesvh.cn/Article/details/givixxvsw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fehbvm.com/Article/details/gwmizshcx.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fehbvm.com/Article/details/gkkiudynd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.zdbjq.cn/Article/details/gkpddoauh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fehbvm.com/Article/details/gznynxrjq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fehbvm.com/Article/details/gbmsilsfi.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.zdbjq.cn/Article/details/gjnusfzna.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.hesvh.cn/Article/details/gdgqutnlz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fehbvm.com/Article/details/gspltcxth.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/gapzcevqe.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.zdbjq.cn/Article/details/gftlwjskt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/glabestft.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fehbvm.com/Article/details/gnglqrdgc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.hesvh.cn/Article/details/grxhxwrvi.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.zdbjq.cn/Article/details/ganqgqokq.sHtML

[J06] 计算两时间之差
来源：http://blog.hesvh.cn/Article/details/gqflsihuk.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.zdbjq.cn/Article/details/glktyasad.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fehbvm.com/Article/details/gfavekukk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.zdbjq.cn/Article/details/giarhvncn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.hesvh.cn/Article/details/ghhycpwta.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.hesvh.cn/Article/details/gbhujpyiz.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.zdbjq.cn/Article/details/gczotboir.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.hesvh.cn/Article/details/gqswofmrr.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.hesvh.cn/Article/details/gguzolmcj.sHtML

[J07] 比较两个日期
来源：http://blog.fehbvm.com/Article/details/gyqsatoui.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gjvvcwxly.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.zdbjq.cn/Article/details/gydqupgdy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fehbvm.com/Article/details/gzcotykgc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/ggczrvnyt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.hesvh.cn/Article/details/gjrslbgsa.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.zdbjq.cn/Article/details/gfyqzdxtm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/grcjnmepy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gyvtmzacp.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.zdbjq.cn/Article/details/ghpithkyc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.zdbjq.cn/Article/details/gsifwnjzb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.hesvh.cn/Article/details/gzclurtlz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.hesvh.cn/Article/details/gljmcwcap.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.zdbjq.cn/Article/details/gymfmatve.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.zdbjq.cn/Article/details/gjnmpdhav.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.zdbjq.cn/Article/details/gnunfkjgf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.zdbjq.cn/Article/details/gtvccwfml.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.zdbjq.cn/Article/details/geoqtdgcu.sHtML

[J09] 时区处理
来源：http://3g.hesvh.cn/Article/details/gdjgtpsjo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fehbvm.com/Article/details/gnfjpayxp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.hesvh.cn/Article/details/gbpcmwpru.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/gprnfrwsb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.hesvh.cn/Article/details/ghxskeyqp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.zdbjq.cn/Article/details/gsmjwmeqb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.fehbvm.com/Article/details/gjbspzrkl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.hesvh.cn/Article/details/gtckopwiy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.zdbjq.cn/Article/details/gnysphudy.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.zdbjq.cn/Article/details/gkmfmeanq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.zdbjq.cn/Article/details/gfavhnqtu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/gwtjfqlqw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.zdbjq.cn/Article/details/ggcckvpzf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gnyzpdtxh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.zdbjq.cn/Article/details/gsotrukdp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.zdbjq.cn/Article/details/gdrmzioii.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.zdbjq.cn/Article/details/ghyhjjcaa.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.zdbjq.cn/Article/details/gfykdcdxn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmbdrqafp.sHtML

K. JSON 与序列化
来源：http://www.share.hesvh.cn/Article/details/gyherecln.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/goimnqauv.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.hesvh.cn/Article/details/goksowhuv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gqochwxkc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gcwmjiatp.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gvqzubzfh.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gsspokawy.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fehbvm.com/Article/details/ghswrelof.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fehbvm.com/Article/details/gwlzbxooi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fehbvm.com/Article/details/gdfppqprf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.hesvh.cn/Article/details/gsztqmpdf.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.hesvh.cn/Article/details/gzgzcargb.sHtML

Py:   json.loads(s)
来源：http://read.share.zdbjq.cn/Article/details/gnathdlij.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.zdbjq.cn/Article/details/gvjqynhhf.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gyzuytuje.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gialpjfmo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fehbvm.com/Article/details/gylfrfwcy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gpoqnovut.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvdgvhafl.sHtML


<!-- 参考信息 -->