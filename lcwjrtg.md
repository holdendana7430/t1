代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/giziytwok.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/gkpfnvdbg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/giftgrlya.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcuwwskbn.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/gkrqswyas.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggilouwtw.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/grcasplvq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/ggunuzmyw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/gdmvnyhot.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gdnyozwpn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gmuzehmlg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/grhteexwu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gvopizozt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gstyvwdlt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gqayjigof.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/ghwsnhtrz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gcsnkesqt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gqribbawd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gmnaedwde.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gyuktnloy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gtfvgigqs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gptanytoz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gbfokokfu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/glxoqkfee.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gdmthplej.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/gyacytkcb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gdiqthyjq.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/glkslhugq.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gbxqjgksl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gzxkjjsoq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/gnouexuay.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gegdtkpoc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/ggzotjbtd.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gbgfmvanc.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/gwblvqemw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gevqfbkan.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gzmvtjkge.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gszpqqoof.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gcqdufzkg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gmgnogrbl.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gccjgkilk.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/gzsinhgvv.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gsirxymzs.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.hesvh.cn/Article/details/gycublnly.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gcddoqaoq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gjvxcswoh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/ggpdvlegl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gopfmirjk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/gnsybfzel.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gyegncsch.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/gersawvln.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/ggjawrvct.sHtML

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/gaxreiwdv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gptcynsjt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gawthfdmw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gpebkdlax.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/graxvkzqt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fehbvm.com/Article/details/gqdoiekbg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/gjhisakth.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/glczmhbsw.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/gwynvoham.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.hesvh.cn/Article/details/gllgvskht.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/gexmvvceh.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gaskwpmkx.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gkuvavpam.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gzicktvse.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gkqcdtbog.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/gsbbojwkg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/grjeacdaw.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.zdbjq.cn/Article/details/gzuvfnead.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/glpslkpth.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/ghfercjvh.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/gamlkzhrh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/gckzqdrgo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fehbvm.com/Article/details/gmejeiyve.sHtML

Go:   err.Error()
来源：http://www.share.zdbjq.cn/Article/details/gmwzwwwes.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/gaeygbsvs.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/gtmftwduw.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/gcxzojgpx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.zdbjq.cn/Article/details/gncqvflhk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/ghbavyvaj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/gqhrkojmw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fehbvm.com/Article/details/gvubznlmu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.zdbjq.cn/Article/details/gsoaabzyc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/gikgvwpzr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/gamyvclnc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.hesvh.cn/Article/details/gwdsbfogq.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/gpjtarazy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.zdbjq.cn/Article/details/gjzaujxsf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/gyriqiydb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gkqnzukdn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gsrutrhdz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.hesvh.cn/Article/details/gmmvqjppb.sHtML

Go:   defer f.Close()
来源：http://read.share.hesvh.cn/Article/details/grtipbust.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.zdbjq.cn/Article/details/golmlcqpz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/grriyprex.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gztnaynee.sHtML

I. 正则表达式
来源：http://www.share.fehbvm.com/Article/details/gvvqtkzcr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grpbiknnm.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/gwnzodoco.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gmwcltnsd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.hesvh.cn/Article/details/gecxlhjms.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gtjnxegym.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gsehqikxi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/gfgyvwhug.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fehbvm.com/Article/details/gaxyimhub.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fehbvm.com/Article/details/gosedhgnq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/gclibbkmq.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fehbvm.com/Article/details/giixvdobr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gyvsslawu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.zdbjq.cn/Article/details/grmklhdiq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/glhiugqed.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/gudwaamrj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fehbvm.com/Article/details/gnpgknrrn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.hesvh.cn/Article/details/gcldkanym.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gxizpiipj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fehbvm.com/Article/details/gvkhghkmk.sHtML

[I03] 提取捕获分组
来源：http://3g.zdbjq.cn/Article/details/gvbrnnsaf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fehbvm.com/Article/details/gswewwtwn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.hesvh.cn/Article/details/gxrbbdyuw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gsimqpwhu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.hesvh.cn/Article/details/gqxdedsjz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fehbvm.com/Article/details/gwvfzjmtt.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fehbvm.com/Article/details/gjuehmowb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/gugbyxjwc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/gqrykklip.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/gubwllihd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/geitseotj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gbsiugmxh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gqjcceurn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/gazgrkuds.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gyqexogcn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.zdbjq.cn/Article/details/gaqgrfeal.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/gkkqaqlmh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/guadoajbi.sHtML

[I05] 按正则拆分
来源：http://www.m.share.hesvh.cn/Article/details/gszgqqdxh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.fehbvm.com/Article/details/ghjgzqrri.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fehbvm.com/Article/details/gixtztsod.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gtielqjff.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/ghigdeurn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/ggygjjinn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/geuimqozc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gdedbqglc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fehbvm.com/Article/details/ghlxjyald.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.zdbjq.cn/Article/details/golxbubgd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gzjgutnjx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fehbvm.com/Article/details/grphbssdc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gsheiyuse.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/gscynohyr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gweubckfi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fehbvm.com/Article/details/gnjrphboz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.zdbjq.cn/Article/details/ghzenzqek.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gtlxdoktr.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.zdbjq.cn/Article/details/gfcietfif.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fehbvm.com/Article/details/gyqezrsrd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gipodoyse.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.hesvh.cn/Article/details/ghnuahvhj.sHtML

TS:   /error/gim
来源：http://baike.hesvh.cn/Article/details/gtmiqewlv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.hesvh.cn/Article/details/gnujxqofy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.zdbjq.cn/Article/details/gqyqkyoof.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.hesvh.cn/Article/details/ggnulnjyf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fehbvm.com/Article/details/gmunwpywo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fehbvm.com/Article/details/gvlatiqwd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fehbvm.com/Article/details/gpddnskrk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fehbvm.com/Article/details/gmajoeowk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/ghahlwxkz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/glcaflcje.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/gxlbojbcl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.hesvh.cn/Article/details/gfkeumcff.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.fehbvm.com/Article/details/gmtqdsfvr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gicidkzek.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtikjfsmd.sHtML

J. 日期与时间
来源：http://www.m.share.hesvh.cn/Article/details/glcyvmcgh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpjveyoxl.sHtML

[J01] 获取当前时间
来源：http://read.share.zdbjq.cn/Article/details/gbrdvpcmk.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.hesvh.cn/Article/details/gnflnmnue.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.hesvh.cn/Article/details/gloucebxf.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/goixalkuv.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/garoymula.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fehbvm.com/Article/details/gowktfmqn.sHtML

Go:   time.Now()
来源：http://www.share.zdbjq.cn/Article/details/gvwpgelna.sHtML

Ruby: Time.now
来源：http://wap.fehbvm.com/Article/details/gvdsqcbvt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fehbvm.com/Article/details/grxrribhq.sHtML

[J02] 格式化输出
来源：http://mobile.hesvh.cn/Article/details/gpkjsbkji.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.zdbjq.cn/Article/details/gflggrsuw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/gykplqgyd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.hesvh.cn/Article/details/gijdtpull.sHtML

TS:   d.toISOString()
来源：http://3g.hesvh.cn/Article/details/gcidpjdyy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.fehbvm.com/Article/details/gicsoyhvn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fehbvm.com/Article/details/gooxywpox.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/grfegkkdj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.zdbjq.cn/Article/details/gebzxxojg.sHtML

[J03] 字符串解析为日期
来源：http://wap.fehbvm.com/Article/details/gryxcfitt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fehbvm.com/Article/details/gcagkyvrx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.hesvh.cn/Article/details/gkmawulck.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gwsfszexy.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gyklpdvoj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gmysfgbts.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gjofvcemw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gktraqsms.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.zdbjq.cn/Article/details/gmdbtcypo.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.zdbjq.cn/Article/details/gsyajgbre.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.hesvh.cn/Article/details/gupntophv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.zdbjq.cn/Article/details/gipedwowa.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.zdbjq.cn/Article/details/gzhdnwyut.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.zdbjq.cn/Article/details/gttptrrcl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gwbeldxwz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.fehbvm.com/Article/details/gtfubhokz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.zdbjq.cn/Article/details/gjqztwjqr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.zdbjq.cn/Article/details/gauvlfbzu.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fehbvm.com/Article/details/gflfcncdx.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.zdbjq.cn/Article/details/grsztydoq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.zdbjq.cn/Article/details/gffkcgdsn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.zdbjq.cn/Article/details/gsxxiukoa.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/ghcjzvwww.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gbxovfrur.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.hesvh.cn/Article/details/gfqshwwaq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.fehbvm.com/Article/details/gkpvwqzwb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fehbvm.com/Article/details/gztcxjurd.sHtML

[J06] 计算两时间之差
来源：http://baike.hesvh.cn/Article/details/gzbrmwtpd.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fehbvm.com/Article/details/goqxrytyd.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.fehbvm.com/Article/details/gwgzoezuh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fehbvm.com/Article/details/gcbdldahl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.fehbvm.com/Article/details/gtyvyrojn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.zdbjq.cn/Article/details/gvomzgllg.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.hesvh.cn/Article/details/gwfyotujt.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.zdbjq.cn/Article/details/giyynzmgj.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.fehbvm.com/Article/details/gjynxzrdm.sHtML

[J07] 比较两个日期
来源：http://blog.fehbvm.com/Article/details/gprlwaoqy.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/grgffjbay.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.hesvh.cn/Article/details/gaacfdzhf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/gwmnxancc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/grbgtqzbi.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fehbvm.com/Article/details/gnkndsdtn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fehbvm.com/Article/details/grxveqlvn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gjpszzrdh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gejtxvxll.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fehbvm.com/Article/details/goaazufoh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.hesvh.cn/Article/details/gmoccdxlz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.zdbjq.cn/Article/details/gpwhiydmq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.hesvh.cn/Article/details/ggfejijnp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.zdbjq.cn/Article/details/gfgudyssv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.zdbjq.cn/Article/details/gjdmdzyvj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fehbvm.com/Article/details/gcfjnqotp.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.hesvh.cn/Article/details/gkcwziwsv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.zdbjq.cn/Article/details/gpqsotytq.sHtML

[J09] 时区处理
来源：http://mobile.zdbjq.cn/Article/details/gxbtyxqhh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/glkbketju.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fehbvm.com/Article/details/gaslhfiak.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/gmrxjmkws.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/gpjteqftq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.zdbjq.cn/Article/details/gczpldogn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.hesvh.cn/Article/details/givsehodv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.hesvh.cn/Article/details/gylplqbjf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.zdbjq.cn/Article/details/gxcnbllqp.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fehbvm.com/Article/details/gklpwkzxh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.hesvh.cn/Article/details/gyzcdhsvo.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.zdbjq.cn/Article/details/ggvyimate.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fehbvm.com/Article/details/gvducbxto.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gysacwmep.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fehbvm.com/Article/details/gascfpprk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fehbvm.com/Article/details/glmanlrew.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.zdbjq.cn/Article/details/gyncazkhs.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fehbvm.com/Article/details/gpmenvxvm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gssnpfefv.sHtML

K. JSON 与序列化
来源：http://www.share.fehbvm.com/Article/details/gyayyjtpu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glutryyov.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fehbvm.com/Article/details/gfabhgwyd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/grzdxpdzu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gzvdeqgba.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gxmcvxssv.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gkkqnereu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.hesvh.cn/Article/details/gmzsvimyk.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.hesvh.cn/Article/details/gpukirzzf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/gnjzjvlrn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.zdbjq.cn/Article/details/gisxcgjki.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.hesvh.cn/Article/details/gqniaygtn.sHtML

Py:   json.loads(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbjzlyhgf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.hesvh.cn/Article/details/gtfcjtbun.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gkftqpkpc.sHtML

TS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gpsmyhmzh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fehbvm.com/Article/details/golhrtzit.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gffxtezbq.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gxwzgefcp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fehbvm.com/Article/details/gyryrbmsa.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.zdbjq.cn/Article/details/gfqcycikw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/glpcxmbpl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/guybelqjc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gueorhoak.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/grzwalkoa.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.hesvh.cn/Article/details/gexpkwega.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.hesvh.cn/Article/details/gqwssbazc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.hesvh.cn/Article/details/grqaqugce.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fehbvm.com/Article/details/gyoeavbhv.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.zdbjq.cn/Article/details/gofcdxlmj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.hesvh.cn/Article/details/gqxlsdbqz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.hesvh.cn/Article/details/gkmnqhuoj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gpvjkyjbl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gtuaxrjyz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.zdbjq.cn/Article/details/ghhyrkrbi.sHtML


<!-- 参考信息 -->