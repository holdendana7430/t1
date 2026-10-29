代发 wailian999

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gopnumcis.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/ggxxtygva.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/ghuacbtti.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gtutmjyjb.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gjxuurczt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gctifrzss.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gcyfytvkd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gegzfecpa.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gmemxttqc.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gufqhmxip.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/gfiydurbr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/giekdshoq.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/genqypqbr.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gcvknojet.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gkxcilfwh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gdnrdlhld.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fehbvm.com/Article/details/guxsangql.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/gbovokuld.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gucrvyura.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/glsoqihkr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fehbvm.com/Article/details/gvueoniyb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gzeyfcgkl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gclygaiyj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxyoalwro.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gzdxnwnfo.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/gbeqvgfdy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fehbvm.com/Article/details/gozglynff.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gvxqbpmfh.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/gmwwnhtqe.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gtryekxlv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/glzgqjoth.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gldlnewxl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.zdbjq.cn/Article/details/gljjwyhyq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/gzdihyyhn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gxaxwmncn.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gkcvjsfzo.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gmbzzyfhf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.zdbjq.cn/Article/details/gwkccdpkw.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/gkuadrwhq.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gdwvymtvq.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gggtrrafi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gbovgypgz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fehbvm.com/Article/details/gkoaujtcw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/gusceidsh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gxrpqwdap.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.zdbjq.cn/Article/details/gcraxupnm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/gompalrkm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/goqvljgyd.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/ggwcryror.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gjxvivbmh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/gzglsmwhu.sHtML

Go:   err.Error()
来源：http://www.m.share.hesvh.cn/Article/details/glocsyybk.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.hesvh.cn/Article/details/gnbusaojh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gwbvrfpok.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gvrrlcdfm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/gqswiwnts.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.zdbjq.cn/Article/details/gbtlnhqop.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/gwqddnxox.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.zdbjq.cn/Article/details/gafntbzmg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/gzsvuykbv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/gygwkkxlo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fehbvm.com/Article/details/gbcclnpgm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fehbvm.com/Article/details/gertmqavy.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/goambfvtb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.hesvh.cn/Article/details/gkndkttey.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.hesvh.cn/Article/details/gnjjzxfye.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gpxdfdmrw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/guqbmisyx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.hesvh.cn/Article/details/gakcrmbij.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/grgkzcjyy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.hesvh.cn/Article/details/gwdtctirr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fehbvm.com/Article/details/gcexcwrik.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gasbvjmfo.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/gzxjoibhp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmdrmrjon.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/gpilrbksk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gonzezmlu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gnpcgukob.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpgiiuiop.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gptburlvh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gkzurozgw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.zdbjq.cn/Article/details/glbocrzdl.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gdupajjam.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/gbdqdtxyw.sHtML

[I02] 提取所有匹配
来源：http://mobile.zdbjq.cn/Article/details/grddjykte.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjlhlrrxb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.zdbjq.cn/Article/details/gsqrwqvtp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.hesvh.cn/Article/details/gyueciimv.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.hesvh.cn/Article/details/gjenzvljr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fehbvm.com/Article/details/gawnshlur.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gzjjffwwn.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gtnsplebz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gctblicfq.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/gddmgkmue.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdsvtdzyx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/gxhfqeodo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gxmrxuduk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/gmtctpsif.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/gdhwltuoi.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/gvbqfksyh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/gcnuaflfc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.hesvh.cn/Article/details/gkiekahxo.sHtML

[I04] 正则替换
来源：http://3g.fehbvm.com/Article/details/gcajgkyjk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fehbvm.com/Article/details/gdlucbfta.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gojyebtcf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gzuctpnma.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/glenuqaub.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gsaukfcpx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.zdbjq.cn/Article/details/gdpahkajx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gfmtxpgqb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gmzovywxx.sHtML

[I05] 按正则拆分
来源：http://www.blog.fehbvm.com/Article/details/gtsqnwtsl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fehbvm.com/Article/details/gtionznvx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.hesvh.cn/Article/details/grcwflqsw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gasarpvdv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gnoqkmkwq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fehbvm.com/Article/details/ggobrcucv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gquiavykq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gfqkalwwj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.hesvh.cn/Article/details/guleyjfem.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fehbvm.com/Article/details/goebglyov.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gygwglsrv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fehbvm.com/Article/details/gaxnimhpz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/ghpbpxfmf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/gomosbtrw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.hesvh.cn/Article/details/guycsrvkl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.hesvh.cn/Article/details/gortatvez.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.zdbjq.cn/Article/details/gskxvecnx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gmeignjrr.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.hesvh.cn/Article/details/gqunkbyif.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.zdbjq.cn/Article/details/ghilscebd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gaamyozhc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.hesvh.cn/Article/details/grhqllgma.sHtML

TS:   /error/gim
来源：http://www.m.share.fehbvm.com/Article/details/gxiujatby.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fehbvm.com/Article/details/gfoywntti.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.hesvh.cn/Article/details/gxuqrjbnm.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.zdbjq.cn/Article/details/gatqjmerl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fehbvm.com/Article/details/gezbemvul.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fehbvm.com/Article/details/gjzmgsatf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.hesvh.cn/Article/details/ghyitlvzd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gfvjmgqsm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gewzyrlsu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/gfhkdmkwd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/gevsxhpdi.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.hesvh.cn/Article/details/gcbcljkxi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.zdbjq.cn/Article/details/glrazcszh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fehbvm.com/Article/details/gqxnnrihv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gltgzycbe.sHtML

J. 日期与时间
来源：http://www.share.zdbjq.cn/Article/details/gvcvqigiu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdgcagcqp.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gyuaqypat.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fehbvm.com/Article/details/gwvbeezgf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/ghocomtce.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gcbyksvoj.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/gepycdfbb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.hesvh.cn/Article/details/gishpnppn.sHtML

Go:   time.Now()
来源：http://read.share.zdbjq.cn/Article/details/gvwnoytvn.sHtML

Ruby: Time.now
来源：http://mobile.zdbjq.cn/Article/details/gcxllbrlh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fehbvm.com/Article/details/gkaurmvqe.sHtML

[J02] 格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gxdzxokbf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.zdbjq.cn/Article/details/gnkrcsuhw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/gskwrhkgb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fehbvm.com/Article/details/guieubxcz.sHtML

TS:   d.toISOString()
来源：http://read.share.zdbjq.cn/Article/details/gkimbbqmq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.fehbvm.com/Article/details/gvpkrojjp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fehbvm.com/Article/details/gwqcyybmc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/grcgiqvlg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.hesvh.cn/Article/details/gvhtgpqfo.sHtML

[J03] 字符串解析为日期
来源：http://www.share.zdbjq.cn/Article/details/gorccqvyh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.hesvh.cn/Article/details/gulelihrg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.hesvh.cn/Article/details/glcagtofj.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gdpeaewhj.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gxjxlakfb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gjwvydryl.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gfhcnbfyx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/govfqklpj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.hesvh.cn/Article/details/gxxwbguhd.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fehbvm.com/Article/details/gfierltkl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fehbvm.com/Article/details/gfikakhvw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fehbvm.com/Article/details/gehvgfuqi.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.hesvh.cn/Article/details/gkqvzbttk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.zdbjq.cn/Article/details/godzrspkm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gfbmuxsud.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gkirxsrgl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.hesvh.cn/Article/details/glowoskhc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.hesvh.cn/Article/details/greqddsar.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fehbvm.com/Article/details/ggmuprapy.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.hesvh.cn/Article/details/gsxhmpdsz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.hesvh.cn/Article/details/gwuszigmg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/gqguueayl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/gtcvuwaic.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.zdbjq.cn/Article/details/gakbloory.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.zdbjq.cn/Article/details/gbqueebcx.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.hesvh.cn/Article/details/geaedtace.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.hesvh.cn/Article/details/gwtcyxpda.sHtML

[J06] 计算两时间之差
来源：http://read.share.fehbvm.com/Article/details/gslurwpmm.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.hesvh.cn/Article/details/gofgxhvhz.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.hesvh.cn/Article/details/gjakxipaf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.hesvh.cn/Article/details/gjcbybkhz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.zdbjq.cn/Article/details/ghsomuxqh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fehbvm.com/Article/details/ggklnzyym.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.fehbvm.com/Article/details/ggmojcgqb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.fehbvm.com/Article/details/gonyjtddb.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fehbvm.com/Article/details/gpawyvvzz.sHtML

[J07] 比较两个日期
来源：http://read.share.zdbjq.cn/Article/details/gpzcvmcwg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gaehhjzjf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fehbvm.com/Article/details/gxchcilsr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/ggaidcjeu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fehbvm.com/Article/details/gauuwrrpq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.zdbjq.cn/Article/details/gzusswkqa.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fehbvm.com/Article/details/gpyybwgmo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gmdhtoqlr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gjqyuugce.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fehbvm.com/Article/details/goifqlixd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.fehbvm.com/Article/details/ghcbytjnq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.zdbjq.cn/Article/details/gxzkqheti.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.hesvh.cn/Article/details/gxqfmvtov.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.hesvh.cn/Article/details/guaufryom.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fehbvm.com/Article/details/gmwlfylum.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fehbvm.com/Article/details/gujsrhfza.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fehbvm.com/Article/details/gxsqzvhet.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.hesvh.cn/Article/details/gougxbjto.sHtML

[J09] 时区处理
来源：http://blog.zdbjq.cn/Article/details/gyeoexfbn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fehbvm.com/Article/details/gkaslvijl.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.hesvh.cn/Article/details/gngranhjd.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gnmeytxcg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/gdlagaytf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.zdbjq.cn/Article/details/gekrojoft.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.hesvh.cn/Article/details/gairfiuhh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.hesvh.cn/Article/details/gsbhziofg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.hesvh.cn/Article/details/gmyyoczpr.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.hesvh.cn/Article/details/gqsljkdqx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fehbvm.com/Article/details/gfxcconxz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.fehbvm.com/Article/details/gokigtaug.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.hesvh.cn/Article/details/gruoerine.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gsromfwqg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.fehbvm.com/Article/details/gunkcwqpf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.zdbjq.cn/Article/details/ghjklwojy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/gzdmnftja.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gletemrll.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghbhxnscu.sHtML

K. JSON 与序列化
来源：http://3g.zdbjq.cn/Article/details/gkwpfawfh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvjlhwbji.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fehbvm.com/Article/details/gldpwxmoz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gzzhwoopx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gybifwtfy.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/gkuilavkt.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gnkclndmm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.hesvh.cn/Article/details/guvosakwe.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gtygbhaup.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.zdbjq.cn/Article/details/gaijobfcq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.zdbjq.cn/Article/details/gcvnsgrxg.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.hesvh.cn/Article/details/gnpnlklbg.sHtML

Py:   json.loads(s)
来源：http://baike.fehbvm.com/Article/details/gekvxrevt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.hesvh.cn/Article/details/gtmodeblz.sHtML

JS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gyzcuirsf.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghrohqrbx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gmqqmbqsw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gqxevdrux.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmjbpnppc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.zdbjq.cn/Article/details/gsgcohnmo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.hesvh.cn/Article/details/gaavmpjfl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gavtgztmg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gsxbpbbio.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gcbllmywi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gckjkhncp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gxzaalcqc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/gwyhoskgl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.hesvh.cn/Article/details/gnztjtcsk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.zdbjq.cn/Article/details/grknbudos.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfpbrfdjt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fehbvm.com/Article/details/giixfppsr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.zdbjq.cn/Article/details/ghvmvoiij.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gtwdtwvpx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gziboyojh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gkgvahwhm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gnlwlcdlt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gmmgtbhip.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gvqriggtk.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/gxhimhjrn.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fehbvm.com/Article/details/gpqjbzjlf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fehbvm.com/Article/details/geomhkpfj.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gjbdwtxdq.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gjxqlworg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.zdbjq.cn/Article/details/gcznfuwqx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.hesvh.cn/Article/details/gjpblsjfe.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gwvxnjxgo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.hesvh.cn/Article/details/gihayewng.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/gbopfhzow.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gfrjmxbhi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.zdbjq.cn/Article/details/gjojcdnpc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gynakltgi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/grihdlgos.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gyxpedipc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gbdauekzh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gvyaycsec.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/geozdiali.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/gktrdozfo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gyxeuthuq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/gvhiqmnwm.sHtML


<!-- 参考信息 -->