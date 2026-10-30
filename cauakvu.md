代发 wailian999

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gpjwubebx.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gyfoevzlz.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/ghrryrrxk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gajdceeto.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gjawwsxay.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gichqanjy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/guunvzqid.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfoawtvua.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gsqdkmdgp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gliqvaisa.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/gqmgxxhqu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gdfirdmkq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gtmbctkyo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gloxynnlu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gnkujyctw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/graidajvo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/grdrndovy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.hesvh.cn/Article/details/gjognupjx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/gflsizonk.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gglmxbkle.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gghctkbcl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gztpnepkt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gqyxlmvfz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gnxisukcs.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gpbwqsqne.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gpfmrupwn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/gpdsfelyt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gxmuegkye.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/grmkgcmmp.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/gwhppvhmw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gwrmbiguq.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gjvshoqhx.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gesihatdh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gqxjhqlik.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/glvzwmiig.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gdlwbkhwv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gjhcxcrdn.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gattzitsw.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/gurwyjexj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gjkrfmgef.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/ggtkuvjai.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gmujekvkr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gvggayyxw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/ghepyvcrv.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/gkqcgihhx.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/gvdwqkodr.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/grcpbriea.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gwqvmhgyy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/gdlwbtmwl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/glytbywdq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gorbemxxl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gqiuapcmb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/gjuqejpam.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/guegrzgdp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxyuuwjmh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/gcjemdzkh.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/gjrpocpwk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gjadkgjhw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gydeedkuq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gezyjjdmz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/gwrabmgzc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/gkacppfxk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/gwsbzfqsw.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.hesvh.cn/Article/details/ggtmiljei.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/grnwiseda.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fehbvm.com/Article/details/ghjhprgep.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gcjmiaegw.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gclormwzs.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/guyhdmtfk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gcaiegxgu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/gvnkwwdkg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gdplokdyq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gsbwhuujj.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.hesvh.cn/Article/details/gasbtrnup.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gxlroaouh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.zdbjq.cn/Article/details/gtdaieijz.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/gztxqzylk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/gmheiautu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/gnrlnxaha.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gjdpksxnr.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fehbvm.com/Article/details/gtcyanlbx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/gqbjtfvyh.sHtML

[H09] 带错误码的异常
来源：http://baike.zdbjq.cn/Article/details/gwzajgjwx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gyldfpbqo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gyiasexan.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/goukzderb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/gevdjwhgp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/gejbeveoh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.hesvh.cn/Article/details/gkumdwhkf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/gmxfuqkwq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fehbvm.com/Article/details/gxbyiaqpm.sHtML

[H10] 资源自动释放
来源：http://baike.zdbjq.cn/Article/details/gsjmnnadl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gkwsbwxsa.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/gojosywmv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gyczbdejg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gqckljekm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/gbelnznqu.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/gbguanvmr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.zdbjq.cn/Article/details/glsfspgxl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gmswwmlfs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtwziiyvn.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gcohowqmr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxjdwognb.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/gcqqmfqmb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gayynmsdc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gekjsmaup.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/ghxrznher.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gnwfusbiw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.fehbvm.com/Article/details/groouicjp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gmnmphwjl.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/ggpgtfprh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gndojinkg.sHtML

[I02] 提取所有匹配
来源：http://www.blog.hesvh.cn/Article/details/gmevuxior.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gbhhnjpnd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fehbvm.com/Article/details/gnvhnikoz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.zdbjq.cn/Article/details/gpqpzfhpv.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.zdbjq.cn/Article/details/gwwxzstit.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.hesvh.cn/Article/details/gzxddmzth.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gyrmbwvyp.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gxpenkvdn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fehbvm.com/Article/details/gvnuigsre.sHtML

[I03] 提取捕获分组
来源：http://3g.fehbvm.com/Article/details/guvbqxviz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.zdbjq.cn/Article/details/gcsloxvmi.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.zdbjq.cn/Article/details/glugsjyrj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.hesvh.cn/Article/details/gmfndqoaf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.zdbjq.cn/Article/details/gzlfdpvmb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/gdtqnbrya.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.zdbjq.cn/Article/details/gppuaakye.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fehbvm.com/Article/details/gvhcgofja.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fehbvm.com/Article/details/gintrlwzn.sHtML

[I04] 正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gkmurnzee.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.hesvh.cn/Article/details/gakcvxsyy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/ggnhydlzj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/ggoaxipyf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gegeaopnm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gjunfkabw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.hesvh.cn/Article/details/gxgbqyrxc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/grdgowqjc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/ghcnmruqr.sHtML

[I05] 按正则拆分
来源：http://m.share.zdbjq.cn/Article/details/gfwbbyojm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.hesvh.cn/Article/details/gahmwjovz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fehbvm.com/Article/details/grzcbifbm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gboecybkj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gcsytyyvq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.hesvh.cn/Article/details/gszhiblkj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fehbvm.com/Article/details/gldcqhdgt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/goxfymwun.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.hesvh.cn/Article/details/gmzrnbxhq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.zdbjq.cn/Article/details/gdtiqntdg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/guetfqxkx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fehbvm.com/Article/details/geqxxsuil.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gajefvxbi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gfqppnqsm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gvtqnrzof.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.zdbjq.cn/Article/details/gnwmbcrqd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.hesvh.cn/Article/details/gyqjzuina.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gcqysodjb.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.hesvh.cn/Article/details/ghvmugeqn.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fehbvm.com/Article/details/gabqcdhbc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.fehbvm.com/Article/details/giymwamez.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.hesvh.cn/Article/details/grzbasaed.sHtML

TS:   /error/gim
来源：http://m.share.zdbjq.cn/Article/details/gxssmzxkd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.hesvh.cn/Article/details/gybbjplvd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.zdbjq.cn/Article/details/ghqutfbjd.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.hesvh.cn/Article/details/gfswybzed.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.zdbjq.cn/Article/details/gxnavoinz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.hesvh.cn/Article/details/ggpikozun.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.fehbvm.com/Article/details/gqowtrnfc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gmoupiitr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/gvivvhmtu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/gyjepzysp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/ggkgxmdij.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.zdbjq.cn/Article/details/giroqcdln.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.hesvh.cn/Article/details/gvxpphsrc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gxlbahqkw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnmbhwpjh.sHtML

J. 日期与时间
来源：http://blog.hesvh.cn/Article/details/glgrrdynv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghykdunoe.sHtML

[J01] 获取当前时间
来源：http://www.blog.fehbvm.com/Article/details/gjbxcoivm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.zdbjq.cn/Article/details/gijmusvyz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gurnyeghd.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gerliafen.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/gifhzbnnj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.hesvh.cn/Article/details/gdtfchmwi.sHtML

Go:   time.Now()
来源：http://www.share.fehbvm.com/Article/details/gigcplbtx.sHtML

Ruby: Time.now
来源：http://m.share.fehbvm.com/Article/details/gndqfbmxs.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fehbvm.com/Article/details/gnxxrtbhi.sHtML

[J02] 格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gyhexnqud.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fehbvm.com/Article/details/gdhbthxlr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/grfzphvdj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.zdbjq.cn/Article/details/gzygayrxv.sHtML

TS:   d.toISOString()
来源：http://3g.hesvh.cn/Article/details/guyrigokh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.zdbjq.cn/Article/details/gwvtjqoyt.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.hesvh.cn/Article/details/gcqkrpedy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.zdbjq.cn/Article/details/gvzbnqbpc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fehbvm.com/Article/details/gzeyegnzv.sHtML

[J03] 字符串解析为日期
来源：http://read.share.hesvh.cn/Article/details/gyjwohbxd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.hesvh.cn/Article/details/grgjqjthf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.zdbjq.cn/Article/details/ghwcbzkxg.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/guiugnlpp.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/grzuqnkxm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gpxeareke.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gaqwvraoe.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gkzjoduys.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.fehbvm.com/Article/details/gwhsutpwm.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fehbvm.com/Article/details/gpkhoqubr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gloxulhwh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fehbvm.com/Article/details/gqpentdmt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.hesvh.cn/Article/details/gmxanzzlx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.zdbjq.cn/Article/details/gahcvacdt.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.fehbvm.com/Article/details/guzkljvre.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gclstctef.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fehbvm.com/Article/details/gpfmexizt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.zdbjq.cn/Article/details/grxdwoozt.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.zdbjq.cn/Article/details/ghvfxwfxm.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.hesvh.cn/Article/details/gybsuwjst.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.hesvh.cn/Article/details/gpqgeiiub.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gqveasqvy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/gaqaimyzy.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.zdbjq.cn/Article/details/gxezrnuxf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.zdbjq.cn/Article/details/gfooymkoy.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.hesvh.cn/Article/details/gjoayuqim.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fehbvm.com/Article/details/gtrtlropl.sHtML

[J06] 计算两时间之差
来源：http://3g.zdbjq.cn/Article/details/gtchkxuot.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fehbvm.com/Article/details/gpekkdvfo.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fehbvm.com/Article/details/gatymomsy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.zdbjq.cn/Article/details/geiindewc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.zdbjq.cn/Article/details/ggkolllct.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.fehbvm.com/Article/details/gmrtibhej.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.hesvh.cn/Article/details/gmafpljkg.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fehbvm.com/Article/details/gaxopdftm.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.hesvh.cn/Article/details/gikhfbzth.sHtML

[J07] 比较两个日期
来源：http://m.share.fehbvm.com/Article/details/gdcpdtlec.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/glzkwcwjr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.hesvh.cn/Article/details/gnjuudgps.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/ghhtwaeft.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fehbvm.com/Article/details/gyctovfqs.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/gwnimmnvz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fehbvm.com/Article/details/gdkntxkjv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gwhemnbox.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/ggcpzjjkm.sHtML

[J08] 提取年月日与星期
来源：http://www.share.zdbjq.cn/Article/details/ggetkelpe.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.hesvh.cn/Article/details/gepzzchap.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.zdbjq.cn/Article/details/gfzgemxlq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.hesvh.cn/Article/details/gyrakukfx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.hesvh.cn/Article/details/gyacxmuwv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.zdbjq.cn/Article/details/ggsgjqhrs.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.hesvh.cn/Article/details/gimpcvbno.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.zdbjq.cn/Article/details/glprwyjrr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.zdbjq.cn/Article/details/gxijqwszv.sHtML

[J09] 时区处理
来源：http://blog.fehbvm.com/Article/details/gnvtblprz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fehbvm.com/Article/details/gsfinlglp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.hesvh.cn/Article/details/gszgvrwzl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gydlwrjow.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.hesvh.cn/Article/details/gdfjahpbu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.zdbjq.cn/Article/details/gmtiwinrn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.zdbjq.cn/Article/details/gwgxfylqe.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.hesvh.cn/Article/details/gcnwkoefe.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.zdbjq.cn/Article/details/gccajuywn.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.zdbjq.cn/Article/details/gayytlrly.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.hesvh.cn/Article/details/gubcdmufu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.zdbjq.cn/Article/details/gxyqtmhmh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fehbvm.com/Article/details/gguxyavif.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.zdbjq.cn/Article/details/gmpwuogcw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fehbvm.com/Article/details/gvstbazgj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.zdbjq.cn/Article/details/gmwewcjlr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.hesvh.cn/Article/details/gfsnqwsrn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.zdbjq.cn/Article/details/ghfkjeeha.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjauwzpee.sHtML

K. JSON 与序列化
来源：http://www.blog.hesvh.cn/Article/details/ggplernpk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glpnbakbq.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.hesvh.cn/Article/details/gdgbohdmc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gzpoqsddw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gttvgikmt.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gflghejqg.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gbodssfhd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.zdbjq.cn/Article/details/grnpmstkq.sHtML

Go:   json.Marshal(obj)
来源：http://blog.hesvh.cn/Article/details/gmlhstnbx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.zdbjq.cn/Article/details/gpqvmpgnk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fehbvm.com/Article/details/gouxsydft.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fehbvm.com/Article/details/gzbvjisil.sHtML

Py:   json.loads(s)
来源：http://mobile.hesvh.cn/Article/details/gmjnrblbk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gmjexlbzd.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gsizihrce.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gncxhdvbv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gwutovnkd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gxrlolbew.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gspovdhoy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/gvtgkeiso.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/gcieutydn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gjvbffbqp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gmjrsidzf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gnbxlluhc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gbydqaxol.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/gkjdpgsfo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.zdbjq.cn/Article/details/gowlpmvww.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fehbvm.com/Article/details/gphzrnekz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/guxltyeou.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.zdbjq.cn/Article/details/gexinyefb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.zdbjq.cn/Article/details/gyrknqdlf.sHtML


<!-- 参考信息 -->