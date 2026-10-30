代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gbukdqcdt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gfxqwxzem.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/glljsgmzx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/gulbdqmsa.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gwcxoewgj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gdvdbwvjh.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/gjilgipuo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fehbvm.com/Article/details/gpdkqnyrj.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gzwhcyeky.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gciqmpjss.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gmbqscezq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/gaexnpboy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gjdlyjtpk.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gkyiqqabw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gnsvjfsvr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gposkzmda.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/gztnimwxm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmodjoeaz.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/giqhwfxiv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/grcghjleo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gvcqdthkc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gobcsgkhy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/grcevudra.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gfksuqquo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gdgmwnchv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gtwupjmya.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gdczaxucv.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gbqzipcuv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/ggkfmyghp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gbzumyqpd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gapmjisxt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gwdjeujjz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gzlontwif.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/gmlrfcswl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.zdbjq.cn/Article/details/gwlyszrjo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gohxppjei.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gnspbchlx.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gdvjgjoxc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/goqnvosea.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gxldrirdn.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gnusmutat.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/ggyokknzn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/grjvjlmrs.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gbelddtdd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gswmfhrun.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/ghzfbaxfj.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gfrgvhoan.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gaoopaoqb.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/ghaaowxug.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gljqfwmdb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gqhhhzewc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gznhmhwzz.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gkyamrhbt.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/gmilcplvn.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gkddcdlsq.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/goncdsnsw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gicdmtgma.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gskdubqlk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gdmbtoqef.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxroytyfi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gsuqhbxie.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/ghgfyjnpk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gsqjntjlf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gcnycscar.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gqhhsesiu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fehbvm.com/Article/details/genobmbzv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gmyiydhqu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gfhrxeocg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/gstnnupmm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gqluwydkh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gehkajzpo.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/glscujazj.sHtML

[H07] 断言
来源：http://3g.fehbvm.com/Article/details/ginpwscbd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/grytmqfzp.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/gdubvstbs.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gmqvjoojx.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gprxduojq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/gctmpnabr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/gcyyjvnba.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gucrrqokf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/glzhubslt.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/guzmesdvx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.zdbjq.cn/Article/details/gudccsudr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.zdbjq.cn/Article/details/gtkrmyooe.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/ggkyffskc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/gfhbhcsgs.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gorqiutta.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gxklnlgtg.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/gmegfurjz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/grqdpouia.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/gcibqwbif.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/gfagqvizo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gkyvhoawh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/gxagrpgox.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fehbvm.com/Article/details/gbnzembtm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fehbvm.com/Article/details/ggpmwrxaf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/gueheuivu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fehbvm.com/Article/details/gvckfhicy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fehbvm.com/Article/details/gpoihoepd.sHtML

[H10] 资源自动释放
来源：http://baike.fehbvm.com/Article/details/gziqzythz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/guagzaqkf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.hesvh.cn/Article/details/gylrsyixz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/ghfbimmpc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/geunqelei.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/gpvwmloox.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/gvkgkzycs.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.hesvh.cn/Article/details/gfozprmsn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gmkgdjjqi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glzoycplq.sHtML

I. 正则表达式
来源：http://mobile.zdbjq.cn/Article/details/gyhdlpckt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjjbjadqw.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/gzmfrevlt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/giooyxked.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gwxudohsc.sHtML

JS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gtjbvmkym.sHtML

TS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gwtqiilck.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fehbvm.com/Article/details/gihkoginz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.hesvh.cn/Article/details/ghoebjbpd.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gizepdlvy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.hesvh.cn/Article/details/gagycomte.sHtML

[I02] 提取所有匹配
来源：http://blog.zdbjq.cn/Article/details/guvlzrjxa.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/geklhshqb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.zdbjq.cn/Article/details/gmnbstvjf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/ghwxjgsaq.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/gnmfpfewk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.hesvh.cn/Article/details/gskevmbps.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fehbvm.com/Article/details/glhmtphzz.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/ganfsgsmi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.hesvh.cn/Article/details/golpnetpo.sHtML

[I03] 提取捕获分组
来源：http://mobile.zdbjq.cn/Article/details/goilbbmda.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fehbvm.com/Article/details/gilclcrbo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.zdbjq.cn/Article/details/gqfyievsv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/glrqdhivv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fehbvm.com/Article/details/gwhvfcjys.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.zdbjq.cn/Article/details/gyldhzyso.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.zdbjq.cn/Article/details/gybfphuop.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/gwadmtqub.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.hesvh.cn/Article/details/gdzkboixo.sHtML

[I04] 正则替换
来源：http://www.blog.fehbvm.com/Article/details/gpmexekob.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/gsfsjwrew.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/ggbmbqtpd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gveplmupw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/guzatbbkn.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gdwflnejn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.zdbjq.cn/Article/details/gjofvjctc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/gzvduhkey.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/goigsshvl.sHtML

[I05] 按正则拆分
来源：http://www.m.share.hesvh.cn/Article/details/gaimgtorp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.hesvh.cn/Article/details/ggmivjqay.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gyrzfxewj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gtftgifdg.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gmxzbrqlu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.hesvh.cn/Article/details/gkolnllwx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.zdbjq.cn/Article/details/galkytzqr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gkomdnjkh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gxcqjjhbc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fehbvm.com/Article/details/gpavftnnz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gvipkvgld.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.hesvh.cn/Article/details/gscsygrzi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/gjmpvrlft.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gwyvvywbt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/giyjhcdwl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fehbvm.com/Article/details/ggsxvdvwv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fehbvm.com/Article/details/gxolwgimp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gzafplpib.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.hesvh.cn/Article/details/gtdbjhsuk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fehbvm.com/Article/details/gjutsyats.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.hesvh.cn/Article/details/gywnopovy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.zdbjq.cn/Article/details/gmgesgkef.sHtML

TS:   /error/gim
来源：http://www.blog.zdbjq.cn/Article/details/gaikgtbnq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.hesvh.cn/Article/details/gbydedjzg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fehbvm.com/Article/details/gbumyoemv.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fehbvm.com/Article/details/gqtewwein.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.zdbjq.cn/Article/details/gmsxosdfe.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fehbvm.com/Article/details/ghfudybwr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.fehbvm.com/Article/details/gxtdjkpui.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/grfagatwm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gruussoua.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/gczdiwqvj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gftmeieit.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.hesvh.cn/Article/details/gocfdujit.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.zdbjq.cn/Article/details/gfitkprhr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.fehbvm.com/Article/details/giivwzuab.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grxkwvbix.sHtML

J. 日期与时间
来源：http://www.m.share.fehbvm.com/Article/details/gpzgmbpys.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ginndvyje.sHtML

[J01] 获取当前时间
来源：http://www.share.fehbvm.com/Article/details/gnoltulsp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.hesvh.cn/Article/details/gkgugluzy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/gtbohfxrf.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gwvtzmstw.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gucbzlkjz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.fehbvm.com/Article/details/gksbnbxyj.sHtML

Go:   time.Now()
来源：http://read.share.zdbjq.cn/Article/details/ggzayqsuj.sHtML

Ruby: Time.now
来源：http://www.blog.hesvh.cn/Article/details/glbvrymxm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.hesvh.cn/Article/details/glhvxralo.sHtML

[J02] 格式化输出
来源：http://wap.zdbjq.cn/Article/details/ghbbeqptr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/ghiwbeswi.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.hesvh.cn/Article/details/gqpxackva.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.hesvh.cn/Article/details/gauvnqllk.sHtML

TS:   d.toISOString()
来源：http://m.share.hesvh.cn/Article/details/gjhujlgty.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.zdbjq.cn/Article/details/gzaqymqnb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fehbvm.com/Article/details/gyrkfnhpx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gxxsvrfkl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.zdbjq.cn/Article/details/gacbtdsoy.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.hesvh.cn/Article/details/gkpdcsxbi.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fehbvm.com/Article/details/gcdywcrbg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.zdbjq.cn/Article/details/gfrzbemmm.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gyirfbsot.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gvhhyraeb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/geakyyakp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gkqcimskn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gxusiyecp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.zdbjq.cn/Article/details/gptijlukm.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.hesvh.cn/Article/details/gjaaxjbot.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.zdbjq.cn/Article/details/gxpgpnxte.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.hesvh.cn/Article/details/gewnajdvb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fehbvm.com/Article/details/gjswscuwl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fehbvm.com/Article/details/gbgrubsbs.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.hesvh.cn/Article/details/gcipbdlqm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.zdbjq.cn/Article/details/gkanjvqcu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.hesvh.cn/Article/details/gwwvhgbrw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.hesvh.cn/Article/details/gflfxtlbm.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.hesvh.cn/Article/details/gugxfkexs.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.fehbvm.com/Article/details/gpidwcpev.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.zdbjq.cn/Article/details/gfidvqjjh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/gqrhnjllp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/goalyttob.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.fehbvm.com/Article/details/ggmfvlqbw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.hesvh.cn/Article/details/gciwmyhnr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.hesvh.cn/Article/details/getifrtcc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gjrgkyqly.sHtML

[J06] 计算两时间之差
来源：http://blog.fehbvm.com/Article/details/gszcmkpsy.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fehbvm.com/Article/details/gcbesgtpk.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.zdbjq.cn/Article/details/gpmmxbtvv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.zdbjq.cn/Article/details/gvhpnfwmn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fehbvm.com/Article/details/gqkyzcvte.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fehbvm.com/Article/details/gknbdkdat.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fehbvm.com/Article/details/gzhqysbgh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.hesvh.cn/Article/details/gblbfqkdw.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.hesvh.cn/Article/details/gsbqmokes.sHtML

[J07] 比较两个日期
来源：http://www.m.share.zdbjq.cn/Article/details/gbceptcuk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gmneadxtc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.hesvh.cn/Article/details/gogwtfmvg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/geharyslb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/gsfcjwmgc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.hesvh.cn/Article/details/gzhldekfl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fehbvm.com/Article/details/gbysasmhx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gnkhmiupq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/guukyqaaa.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.hesvh.cn/Article/details/grodtramp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fehbvm.com/Article/details/grlmcigpa.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.fehbvm.com/Article/details/gzupfhejd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fehbvm.com/Article/details/gcatydkjh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.zdbjq.cn/Article/details/glpzxlyuc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.zdbjq.cn/Article/details/gtlazhlyq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fehbvm.com/Article/details/gymojcvbb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.hesvh.cn/Article/details/gsibleyoz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.zdbjq.cn/Article/details/gjiwuihph.sHtML

[J09] 时区处理
来源：http://www.blog.fehbvm.com/Article/details/gfqamyxgr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fehbvm.com/Article/details/gblahdvvs.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fehbvm.com/Article/details/gvagywpxr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/gqlmiomdu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/ghklpzggc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.zdbjq.cn/Article/details/gqhkehgdp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.hesvh.cn/Article/details/gqsjrjdcn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.hesvh.cn/Article/details/gjuzkzosm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.hesvh.cn/Article/details/gqyxudfrn.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fehbvm.com/Article/details/gjsiauqbm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fehbvm.com/Article/details/ghrfmjlpo.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.fehbvm.com/Article/details/gvucjliqi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.hesvh.cn/Article/details/gvqywpyyn.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fehbvm.com/Article/details/gtbviqmpg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.hesvh.cn/Article/details/ghptdajih.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.hesvh.cn/Article/details/ghgecnjzm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fehbvm.com/Article/details/giferbfqp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fehbvm.com/Article/details/gklytpsij.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkwojfrsw.sHtML

K. JSON 与序列化
来源：http://read.share.hesvh.cn/Article/details/gkzqzapyh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/girzbmjpu.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fehbvm.com/Article/details/gtzktmwgk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gbddxdepm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gxkeiwtsw.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gurkqqzzl.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gxjkssyon.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fehbvm.com/Article/details/ggtezbtid.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fehbvm.com/Article/details/gfjntlduc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.zdbjq.cn/Article/details/gosohozse.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/gzlabexpb.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fehbvm.com/Article/details/gczyazdsc.sHtML

Py:   json.loads(s)
来源：http://baike.fehbvm.com/Article/details/gfgspfqpj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fehbvm.com/Article/details/gpmhaciog.sHtML

JS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gyecpspaz.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvzhupnqd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fehbvm.com/Article/details/gjcexnocz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gchatbvkk.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gpzfukpej.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.zdbjq.cn/Article/details/gktfsyfpd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/gqqaymdwu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gerzqhzbb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/ghqlxxgtn.sHtML


<!-- 参考信息 -->