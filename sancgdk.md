代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/guldnywcj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gpmwpeski.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gmnbzteav.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gdpnhfcmn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gzwssthpn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/glbhtkkug.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/grwkubkaa.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gxcooygoi.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gdwociqen.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gbjuxopci.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gdaoezzft.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/glirfvmgm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/gvvnrgmfy.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gftqhvczp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gcxmjdqfq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/geknijyon.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gkxfnamtf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvqckhxvd.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/ggfsxeayr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gnnwyfogd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gqtqjrcgb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/ggfhtcuin.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/glvnjscpr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gyktrnnxr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/galstocbe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gvcivfzky.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/giteqkblk.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/godgawext.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gmldlvwpd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gyaoiegvn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gbgwqttbl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gmjhaqfnj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/giulhcaul.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gmrbtcree.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gsmactcmr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/glvyndlgy.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/gfgfgbvjr.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/gmzawcxtl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/grbepmzlv.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gdqgptjmn.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gnqzxfeqd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gkcnvfrnl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/guwfdepro.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gartzsjol.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gmxacavpx.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gwysmxvcl.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gjcggjhyc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gedmqeavc.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/ghdzgvlcq.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gtxjdfwdr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gbgtruvor.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gdkjytpxp.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gmvxvyjxo.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/ghbfszxuz.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/gqipfygck.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gpuiqihch.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gpbtcytjs.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcgnpytkt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gclcjgvau.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/gmcjoexfa.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/gcqjkgfva.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/gkyrescvc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggwshhchk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/guyxqsgam.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/grbjvhjbo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gtdhcvrcn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gqtiqqpsf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gdrmswxws.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/gnhvdzlys.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/gfnjwgykj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/gjapsgvwl.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/gnnqlpmxp.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/gfjxtuxqq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/gtfxygpne.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gcxtjwdzp.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gbbfvtfgn.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gytgepsfe.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gvxnnmais.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/gcuphcugw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/gctjiruvr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/ganwsaddv.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/gewkdpgtj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gehkasqnq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/gcdmhyusg.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/giblhppyk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gxalmmhte.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/gonwcclgx.sHtML

Go:   err.Error()
来源：http://www.m.share.hesvh.cn/Article/details/gegkfmoup.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/gxxjapkcl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.zdbjq.cn/Article/details/gkizmsqsa.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gzfxkpaec.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/gllvphxyn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gsxmvdrka.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/gwrsnegky.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.zdbjq.cn/Article/details/gowiwgxlg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fehbvm.com/Article/details/gtyjeojwg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/guhotbwgo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.hesvh.cn/Article/details/gczwimgqk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.zdbjq.cn/Article/details/gzfulbyyt.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/gzqrymjhm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fehbvm.com/Article/details/gkowdaida.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.hesvh.cn/Article/details/gurbmnhtm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/glbzpdlgx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/ggbmlllwq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.zdbjq.cn/Article/details/gunhijcym.sHtML

Go:   defer f.Close()
来源：http://read.share.fehbvm.com/Article/details/gkcjqbftv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/goqcfuwcb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gzbfulndo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gazentpuw.sHtML

I. 正则表达式
来源：http://3g.hesvh.cn/Article/details/gppgzdfff.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsfistacy.sHtML

[I01] 判断是否匹配
来源：http://mobile.fehbvm.com/Article/details/gifgkygxb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/ggcwmwgkb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.hesvh.cn/Article/details/ggalscoed.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gntvyytws.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/ggghgdrxo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.hesvh.cn/Article/details/gcbrmwqbi.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.hesvh.cn/Article/details/ggwmgjeny.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/girhgatwj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/gnnihuomu.sHtML

[I02] 提取所有匹配
来源：http://mobile.hesvh.cn/Article/details/gyhkaesca.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmdkdeujs.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fehbvm.com/Article/details/gimvdfocc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/ggsqsoemo.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.zdbjq.cn/Article/details/gkvmzifci.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.hesvh.cn/Article/details/gynqnlkdy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fehbvm.com/Article/details/goqhgcutz.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gjgzrswxk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.zdbjq.cn/Article/details/gypucvkdt.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/gytdjkdoi.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.hesvh.cn/Article/details/gzjhjnpqu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/gngozehxa.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.zdbjq.cn/Article/details/gfjqejykf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/grfjqyvhs.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fehbvm.com/Article/details/gixyrgoml.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.hesvh.cn/Article/details/gthmxssxb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/gnhgsjdem.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.hesvh.cn/Article/details/gyrjvcryv.sHtML

[I04] 正则替换
来源：http://mobile.zdbjq.cn/Article/details/gwmhytpfg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.zdbjq.cn/Article/details/gdwkjgmrr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gpwjjhicm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/glxjtroxa.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gxsxwbvxa.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gtefiltgr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.zdbjq.cn/Article/details/gvaqyhlwz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.hesvh.cn/Article/details/gwlcfqulh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/ggykdenfs.sHtML

[I05] 按正则拆分
来源：http://blog.fehbvm.com/Article/details/ghagfcupx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.hesvh.cn/Article/details/gtvtfotxe.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fehbvm.com/Article/details/gbtpvxprg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gdkvqgkqf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gsbkepagt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.zdbjq.cn/Article/details/ginyehxws.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.hesvh.cn/Article/details/gylgispaj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gtcanurjr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fehbvm.com/Article/details/gdppewtgh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fehbvm.com/Article/details/gyzajergv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/glbxaajny.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.hesvh.cn/Article/details/gfugkecrs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.hesvh.cn/Article/details/glxlcmwah.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/gjgxqcofl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.hesvh.cn/Article/details/ghntuaotq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.zdbjq.cn/Article/details/ggaypuwjf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fehbvm.com/Article/details/gbzbovanw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gknbgecpo.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.zdbjq.cn/Article/details/gszlnotrj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fehbvm.com/Article/details/gctkyomje.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gnirnifie.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.zdbjq.cn/Article/details/gdxuyhaow.sHtML

TS:   /error/gim
来源：http://www.share.zdbjq.cn/Article/details/ghgmimpjq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.zdbjq.cn/Article/details/grihuktec.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.fehbvm.com/Article/details/gkszhodat.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fehbvm.com/Article/details/gcgttgnuk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.hesvh.cn/Article/details/gzncjlvxo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fehbvm.com/Article/details/gtqzzcgwi.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.zdbjq.cn/Article/details/ghawosnuv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/gvynkbyiy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/gcahfzcgj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/gypcngexd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.fehbvm.com/Article/details/glgoutspk.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.hesvh.cn/Article/details/gtnnknpmv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.hesvh.cn/Article/details/geiycyukk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/gbucwdtby.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gntjugrba.sHtML

J. 日期与时间
来源：http://www.m.share.hesvh.cn/Article/details/gspjcrawx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guxdtafgj.sHtML

[J01] 获取当前时间
来源：http://read.share.hesvh.cn/Article/details/gjdwvhgxe.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fehbvm.com/Article/details/ggbntnfwf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gbmmfdduv.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.hesvh.cn/Article/details/gvcvxqqia.sHtML

TS:   new Date();  Date.now()
来源：http://wap.zdbjq.cn/Article/details/gyoveasdq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.fehbvm.com/Article/details/gltkyhhpq.sHtML

Go:   time.Now()
来源：http://blog.hesvh.cn/Article/details/gaaqmlkjl.sHtML

Ruby: Time.now
来源：http://wap.hesvh.cn/Article/details/gyxetpzek.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.zdbjq.cn/Article/details/ggnkoerdf.sHtML

[J02] 格式化输出
来源：http://wap.zdbjq.cn/Article/details/gkjiayetx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.zdbjq.cn/Article/details/gkokzzelj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.fehbvm.com/Article/details/gnwkzimtc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fehbvm.com/Article/details/guzmjtkrc.sHtML

TS:   d.toISOString()
来源：http://mobile.zdbjq.cn/Article/details/gdngrhzwy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.hesvh.cn/Article/details/gwptkgwor.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.zdbjq.cn/Article/details/gvnzzrpcc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gfdibppij.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fehbvm.com/Article/details/gepmncjuy.sHtML

[J03] 字符串解析为日期
来源：http://wap.zdbjq.cn/Article/details/gjdndfzen.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.hesvh.cn/Article/details/gxffzidsb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.zdbjq.cn/Article/details/gpgrvvzlo.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/ghmqukppb.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gfigrsyxj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gkfufnthh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gamodoxcq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gphjmlxrw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fehbvm.com/Article/details/gafgxdeqi.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.zdbjq.cn/Article/details/ggypttmbo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.hesvh.cn/Article/details/gliieahsc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.zdbjq.cn/Article/details/gceeoddto.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fehbvm.com/Article/details/ghuokainr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gdozpvhto.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gbklxyqls.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gzfdifror.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.hesvh.cn/Article/details/gcaxdlehl.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.hesvh.cn/Article/details/gbozywyfi.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.hesvh.cn/Article/details/gmqmxiphx.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.fehbvm.com/Article/details/gvrtqwmvq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.hesvh.cn/Article/details/gztdzupqi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gygjmlcld.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gmbaexxue.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.zdbjq.cn/Article/details/gdxxqvids.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.zdbjq.cn/Article/details/gvtiendwo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fehbvm.com/Article/details/gyehbqcdb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.hesvh.cn/Article/details/ggybebgst.sHtML

[J06] 计算两时间之差
来源：http://mobile.fehbvm.com/Article/details/gxffuzuya.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.fehbvm.com/Article/details/gdyzxykvh.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fehbvm.com/Article/details/gbcjxlnvv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.zdbjq.cn/Article/details/gwvmadkip.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.hesvh.cn/Article/details/guowaqzbf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fehbvm.com/Article/details/gewbgramh.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.zdbjq.cn/Article/details/gnjtcbpnc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.zdbjq.cn/Article/details/gbyfuqbmt.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.hesvh.cn/Article/details/ghhhqgzog.sHtML

[J07] 比较两个日期
来源：http://3g.hesvh.cn/Article/details/gxpzogtiu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/glckwsnse.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.zdbjq.cn/Article/details/gqqhdeyrb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/gpxjkxrvm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/gkbwgwkgm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.hesvh.cn/Article/details/gvwhiuqgp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fehbvm.com/Article/details/guusbeiat.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/geojezlqm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gpqyyqgpx.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.hesvh.cn/Article/details/ghbxtowdm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.zdbjq.cn/Article/details/gyxsklqyv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.zdbjq.cn/Article/details/ggvmomfby.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.zdbjq.cn/Article/details/gkuapeiku.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fehbvm.com/Article/details/gbujmslbt.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.zdbjq.cn/Article/details/gedykbacy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.zdbjq.cn/Article/details/gfoypdprc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fehbvm.com/Article/details/gciixfsst.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fehbvm.com/Article/details/gamaparvg.sHtML

[J09] 时区处理
来源：http://mobile.hesvh.cn/Article/details/guyudjjun.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.hesvh.cn/Article/details/gebamfsmv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fehbvm.com/Article/details/gdqidvipp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gaoqwejpq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/gaeiuxktp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.fehbvm.com/Article/details/gxfziaeuk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.zdbjq.cn/Article/details/ghhrxbukp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.hesvh.cn/Article/details/galjxopzp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fehbvm.com/Article/details/gumkffyck.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.zdbjq.cn/Article/details/gskwuvdpq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.hesvh.cn/Article/details/grtcjxpki.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.zdbjq.cn/Article/details/gecxxynpn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.zdbjq.cn/Article/details/gnwjvxncr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.hesvh.cn/Article/details/gjfegglbb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.zdbjq.cn/Article/details/glrhtitxe.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fehbvm.com/Article/details/geitfqkbk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fehbvm.com/Article/details/gbqzplnbp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fehbvm.com/Article/details/gjecjqpzh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdlgjhtbj.sHtML

K. JSON 与序列化
来源：http://www.share.fehbvm.com/Article/details/gkuppnxnf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gthwkhwgu.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fehbvm.com/Article/details/godkzbvwi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gsufokgkc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gdssriswk.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gwrcckpqn.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gdllahvnz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.hesvh.cn/Article/details/gifnasjwz.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gehwkbskg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.hesvh.cn/Article/details/gcioaames.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gbbyunvmo.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.zdbjq.cn/Article/details/gwjybsvnx.sHtML

Py:   json.loads(s)
来源：http://www.blog.hesvh.cn/Article/details/gjydoqwgr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.zdbjq.cn/Article/details/gvbgfdnqj.sHtML

JS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gyciqpbih.sHtML

TS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gyrdynmby.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gookrynoz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/goecuuukf.sHtML

Ruby: JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gdjwbymlw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fehbvm.com/Article/details/gvaxmeqbu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.hesvh.cn/Article/details/gsahalczr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/gemzzchjq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/ggxyzkeft.sHtML


<!-- 参考信息 -->