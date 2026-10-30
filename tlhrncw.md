代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmismcayc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyszvkfhx.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fanxiaobao.xyz/Article/details/gwmbezlbj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fanxiaobao.xyz/Article/details/grkazrsul.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmisckvip.sHtML

JS:   Object.entries(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gmylcutwe.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjscoegt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbtxcgol.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fanxiaobao.xyz/Article/details/grwbjhhnd.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkhnkvab.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnshlhjsx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzheuupo.sHtML

H. 异常与错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gswynekpd.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwibogcq.sHtML

[H01] try / catch 基础
来源：http://3g.fanxiaobao.xyz/Article/details/gaczzvvrf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fanxiaobao.xyz/Article/details/gummkwqga.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbtnhzhg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmccbsexi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gegfrybdo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fanxiaobao.xyz/Article/details/gdlirpyya.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvtlyzdj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjssvgych.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcsndqas.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfdzqhzg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fanxiaobao.xyz/Article/details/glkilxvdl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gvoklqhzu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpvkwuwq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfjebkpk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqndvngw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmjfafnw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fanxiaobao.xyz/Article/details/gcxafbbll.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/guvedidqn.sHtML

[H03] 主动抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gynfaxpxb.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fanxiaobao.xyz/Article/details/gkuylddsw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/grbzsslpi.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/ginfwpmci.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/ghcxtqjqh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/gvxijfhir.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fanxiaobao.xyz/Article/details/gasnuyozo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtrxaepa.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gojqojrkh.sHtML

[H04] 自定义异常类型
来源：http://3g.fanxiaobao.xyz/Article/details/gdydflpzq.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fanxiaobao.xyz/Article/details/golbrzeea.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbonozde.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fanxiaobao.xyz/Article/details/geffnibzg.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fanxiaobao.xyz/Article/details/gqligpjzd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxqbfpdu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxtccfwz.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fanxiaobao.xyz/Article/details/gxfiphyhi.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fanxiaobao.xyz/Article/details/gfceecsxo.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjpdzcvr.sHtML

Py:   except ValueError as e:
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjeuvnly.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fanxiaobao.xyz/Article/details/grsardycz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gfwtilrja.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrboozxf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjwqddzb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjlfcsej.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsswtjtt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzdcfnzq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fanxiaobao.xyz/Article/details/gltfxbwxa.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fanxiaobao.xyz/Article/details/gijyafjjk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fanxiaobao.xyz/Article/details/gkyuboatm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fanxiaobao.xyz/Article/details/gbffessrg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fanxiaobao.xyz/Article/details/gjhrlgbpc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fanxiaobao.xyz/Article/details/gbtfrpfwr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqklvtzid.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gortloang.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fanxiaobao.xyz/Article/details/gesnjcaso.sHtML

[H07] 断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gplmkiyqf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fanxiaobao.xyz/Article/details/gengplfvr.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxifllqvi.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guffhlrvu.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gxbtyuvka.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfxdvypf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwfoykuz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkimqmxwj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gwznbqfpw.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclaijoea.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxjhcuoj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeznxykm.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fanxiaobao.xyz/Article/details/ghubkgfea.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fanxiaobao.xyz/Article/details/gvxohrfio.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fanxiaobao.xyz/Article/details/gezrdrxmt.sHtML

Go:   err.Error()
来源：http://wap.fanxiaobao.xyz/Article/details/givnvtixq.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxspwkcu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fanxiaobao.xyz/Article/details/gybfnewkk.sHtML

[H09] 带错误码的异常
来源：http://baike.fanxiaobao.xyz/Article/details/grbuwolec.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fanxiaobao.xyz/Article/details/gferdntam.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/goqwdojat.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fanxiaobao.xyz/Article/details/gidpgdtvz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgjwzjdj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzynwphai.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpkjouwe.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtobvemj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fanxiaobao.xyz/Article/details/gslhrbeyr.sHtML

[H10] 资源自动释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpybectd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fanxiaobao.xyz/Article/details/gwxotpcrw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fanxiaobao.xyz/Article/details/gmgovsusy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfqarddo.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fanxiaobao.xyz/Article/details/gqaefvaku.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fanxiaobao.xyz/Article/details/grmdkjlsb.sHtML

Go:   defer f.Close()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeiurhfa.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fanxiaobao.xyz/Article/details/gsfmgxond.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/glemlxhrd.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gyxuwqaiv.sHtML

I. 正则表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gmaznjbcm.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gygftnjvi.sHtML

[I01] 判断是否匹配
来源：http://blog.fanxiaobao.xyz/Article/details/goxpgvqhs.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fanxiaobao.xyz/Article/details/glfoeohgu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gxlabakvb.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduypxcce.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttcjouza.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fanxiaobao.xyz/Article/details/gigrusfxa.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwjqqrvt.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fanxiaobao.xyz/Article/details/gmsjahtdh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gcrcodsxg.sHtML

[I02] 提取所有匹配
来源：http://blog.fanxiaobao.xyz/Article/details/glxbbygrg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzpdvmkn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudlwpahb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbnagrus.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fanxiaobao.xyz/Article/details/gnfllpvuy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gcnaflsvg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gezrjjrew.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsfgwgxz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gewadkrli.sHtML

[I03] 提取捕获分组
来源：http://mobile.fanxiaobao.xyz/Article/details/ginulcyqk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/grvrktyxu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmmeanfp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyhbzbsk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfreeiwb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.fanxiaobao.xyz/Article/details/gxwskevso.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpzgjzgr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fanxiaobao.xyz/Article/details/gtaavhvau.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzktnlhz.sHtML

[I04] 正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gytohcwsz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/grvgkvjoj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gknizwrvu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbxrgeao.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgcchcqo.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhpafpcz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnxwcdrl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbiiednvq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fanxiaobao.xyz/Article/details/gcesblkpt.sHtML

[I05] 按正则拆分
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqevwxbv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fanxiaobao.xyz/Article/details/guokrfxhl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzzacxiw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsmghppo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fanxiaobao.xyz/Article/details/gdwkqqwje.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfixvwssm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtkjzcqu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtygrqdpz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fanxiaobao.xyz/Article/details/geuqcggtp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fanxiaobao.xyz/Article/details/gatqmljcg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fanxiaobao.xyz/Article/details/gscfynind.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fanxiaobao.xyz/Article/details/gqhdkfsrv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fanxiaobao.xyz/Article/details/gekvghgyh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdeowlvvl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fanxiaobao.xyz/Article/details/gpzihvkbg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fanxiaobao.xyz/Article/details/grnuvymjj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fanxiaobao.xyz/Article/details/gdmjgdttt.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fanxiaobao.xyz/Article/details/gmlwqodne.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkgxsnxh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fanxiaobao.xyz/Article/details/gpzxhilfj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiguolut.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnmbaewo.sHtML

TS:   /error/gim
来源：http://baike.fanxiaobao.xyz/Article/details/gpauxwxwc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fanxiaobao.xyz/Article/details/galyutoci.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvbdomxg.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fanxiaobao.xyz/Article/details/gtrkvuxgd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxdgglqp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvpqbayh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwavhgaf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiwnfxwt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fanxiaobao.xyz/Article/details/grkhlkzoh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grawvxack.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fanxiaobao.xyz/Article/details/gtydarszr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.fanxiaobao.xyz/Article/details/gbbjqasaw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaspuwpi.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grysqpaik.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gekfhgbgl.sHtML

J. 日期与时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkznlufk.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gsxabhuhq.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganntocdw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdleszmfb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fanxiaobao.xyz/Article/details/gjlbinkrf.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fanxiaobao.xyz/Article/details/guozwykso.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmoghlba.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gynfeijkh.sHtML

Go:   time.Now()
来源：http://www.share.fanxiaobao.xyz/Article/details/gppdtttla.sHtML

Ruby: Time.now
来源：http://mobile.fanxiaobao.xyz/Article/details/goqaaycfl.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fanxiaobao.xyz/Article/details/gfwzsgoqu.sHtML

[J02] 格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gxjfdcooe.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fanxiaobao.xyz/Article/details/glmakdshd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqnqfkbh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fanxiaobao.xyz/Article/details/gmgssrdwf.sHtML

TS:   d.toISOString()
来源：http://blog.fanxiaobao.xyz/Article/details/gvfdsjynm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fanxiaobao.xyz/Article/details/glvohzbpu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwzqrthq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fanxiaobao.xyz/Article/details/gidspvyho.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.fanxiaobao.xyz/Article/details/gdwcipieb.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeaqruxh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.fanxiaobao.xyz/Article/details/gopupjglf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fanxiaobao.xyz/Article/details/gorwuefgu.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gptxexlvq.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gbwxvopsh.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gwelrwczi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/glspzcdnc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcyxckgl.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhkfsuzq.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfojwkbu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/guoxgvmbt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fanxiaobao.xyz/Article/details/gjzzjfcfv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fanxiaobao.xyz/Article/details/gakszqrbe.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqogukls.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.fanxiaobao.xyz/Article/details/gmhlcdfhf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gkfximeov.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfpnenqh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnrihwml.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fanxiaobao.xyz/Article/details/gkvoyghiw.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.fanxiaobao.xyz/Article/details/ghkjwuxfx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgfhxntw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fanxiaobao.xyz/Article/details/gsttfipxd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fanxiaobao.xyz/Article/details/gxfidyeip.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fanxiaobao.xyz/Article/details/gdogtijsz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fanxiaobao.xyz/Article/details/gaanknnag.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbyokmxs.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fanxiaobao.xyz/Article/details/gxmrhjjpy.sHtML

[J06] 计算两时间之差
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxafvkem.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fanxiaobao.xyz/Article/details/gsjrchxhg.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fanxiaobao.xyz/Article/details/gjgfglsml.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.fanxiaobao.xyz/Article/details/giqouqstg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.fanxiaobao.xyz/Article/details/gejmhofnh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkpmetcg.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fanxiaobao.xyz/Article/details/gvvnwsmib.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtsdnnti.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fanxiaobao.xyz/Article/details/ghmtdntfj.sHtML

[J07] 比较两个日期
来源：http://www.share.fanxiaobao.xyz/Article/details/geofdlzty.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fanxiaobao.xyz/Article/details/gdqfytxcd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmisfjgin.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkphjsund.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.fanxiaobao.xyz/Article/details/grlvixevq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fanxiaobao.xyz/Article/details/gujgipbsz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fanxiaobao.xyz/Article/details/gvfiiaetd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fanxiaobao.xyz/Article/details/gshsplana.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fanxiaobao.xyz/Article/details/gdonhlpsz.sHtML

[J08] 提取年月日与星期
来源：http://m.share.fanxiaobao.xyz/Article/details/gglibdpgq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.fanxiaobao.xyz/Article/details/gjiiqyxnu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fanxiaobao.xyz/Article/details/gfheafdvt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdkdbcvd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fanxiaobao.xyz/Article/details/getduqjyx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fanxiaobao.xyz/Article/details/ggxvsuppr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fanxiaobao.xyz/Article/details/gjowvehpm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fanxiaobao.xyz/Article/details/gvfroecsq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fanxiaobao.xyz/Article/details/gldwmgjqb.sHtML

[J09] 时区处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gnacpvqgv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fanxiaobao.xyz/Article/details/gjmdixfua.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fanxiaobao.xyz/Article/details/glohoxgps.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fanxiaobao.xyz/Article/details/gblxvdtnx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgzlvuse.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.fanxiaobao.xyz/Article/details/gywtmoomx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fanxiaobao.xyz/Article/details/gnpwyxpzw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzroerekd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpwrkpue.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.fanxiaobao.xyz/Article/details/gjzscpzno.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fanxiaobao.xyz/Article/details/guykkvtbj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fanxiaobao.xyz/Article/details/gokyyzaxl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbllpaown.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprqxlwuv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsnwshqu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fanxiaobao.xyz/Article/details/gmmbfghjh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fanxiaobao.xyz/Article/details/gxeihsbbb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gkmtumkid.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqzbqezx.sHtML

K. JSON 与序列化
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrdczkan.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtbxltubx.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gefdrzxjk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmygbmeza.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fanxiaobao.xyz/Article/details/gshyrwkcp.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzrmgnur.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbnbvnxu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswtcqlzw.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmflzthe.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbujkzcza.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gjjmdhtow.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gywsheheg.sHtML

Py:   json.loads(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhbfsfag.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fanxiaobao.xyz/Article/details/gmgxdixzc.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbqoszyf.sHtML

TS:   JSON.parse(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gvosalsqr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfjszaao.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxmuziir.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdthfuugx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gusccwjpt.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fanxiaobao.xyz/Article/details/gfmlmswmg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fanxiaobao.xyz/Article/details/gzomadrzt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvqptkds.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/grqvzooxr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuocbkvl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwrzkvyd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fanxiaobao.xyz/Article/details/gtzmpkknx.sHtML


<!-- 参考信息 -->