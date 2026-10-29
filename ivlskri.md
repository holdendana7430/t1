代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/gxlnmdxfh.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/genxkyjop.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gbgaujaeu.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/gmuizehdl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/gcissvina.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gizqqnlda.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gzwbxsrnr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gikgkzriy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gogoqmods.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gygokzkdv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gbafgpnvf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gtheiumlt.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/getjsgnth.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gokyaqvio.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/glsguvrzi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gbuzxibqn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.zdbjq.cn/Article/details/ghhtqtnhl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gvnthgwdl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/gmhaumcpi.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/ghxqdirrk.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/gsvowssqg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/gncnsblun.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/gmkmtydil.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gmxnmoxbb.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gtbzghahz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/govabfzpf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/gjlovgqeo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/gblcstwjc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gvjylqikc.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/gwvtnnjux.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/ggmvthnuc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gshqswfmh.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/gkeztqlpj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.hesvh.cn/Article/details/gocfovymd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fehbvm.com/Article/details/gpaqahgno.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/ggubhcuia.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/gtkomxgwz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gpbfvioqc.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/gtywqtong.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.zdbjq.cn/Article/details/gwydcnlel.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/ggffjzipy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.hesvh.cn/Article/details/gvlxhfavu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gnywbfnul.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/gzbtsewdz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/gwrcitxvr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/gqglbolip.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fehbvm.com/Article/details/gjuehutwi.sHtML

[H10] 资源自动释放
来源：http://blog.zdbjq.cn/Article/details/gxsyuqdhv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.hesvh.cn/Article/details/giszytddg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.zdbjq.cn/Article/details/gsqecslme.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gwcoionfj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gzzfqjuwk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/gtlnfcmhm.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/gbkysgomd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/gwlyqkztm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gubqznctr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmsukohmf.sHtML

I. 正则表达式
来源：http://www.m.share.fehbvm.com/Article/details/goyihvoxz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqbtgcwup.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fehbvm.com/Article/details/gbnpknkkj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/ghhfatpab.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fehbvm.com/Article/details/gnblzujlc.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gppbchzrh.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkiiqmvpa.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/gmvlvbgna.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fehbvm.com/Article/details/ggqpyfamr.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gsxpbptah.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fehbvm.com/Article/details/gybrhgdxq.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.hesvh.cn/Article/details/gnzclhnqc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gtxhzvzqy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.hesvh.cn/Article/details/gxdrqrryp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/geqvsqkzu.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.hesvh.cn/Article/details/gkgeptkct.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fehbvm.com/Article/details/gcfvwteqg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.zdbjq.cn/Article/details/ggwkwlmso.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gigtrtvns.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fehbvm.com/Article/details/gnfntwuof.sHtML

[I03] 提取捕获分组
来源：http://baike.zdbjq.cn/Article/details/gmfofheri.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fehbvm.com/Article/details/gsadjklmh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.zdbjq.cn/Article/details/gjusbuloy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/giegpnppx.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fehbvm.com/Article/details/giyeokmjm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fehbvm.com/Article/details/gmcttebht.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.zdbjq.cn/Article/details/gmstdowob.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.hesvh.cn/Article/details/gjtrdujvl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.hesvh.cn/Article/details/gifstikgn.sHtML

[I04] 正则替换
来源：http://wap.hesvh.cn/Article/details/grkefoebs.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.hesvh.cn/Article/details/gpmwfilna.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gexiwcfqd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gdenqbxvn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gylinvnvc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fehbvm.com/Article/details/glhojjrds.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.hesvh.cn/Article/details/gmbgjhmjt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.hesvh.cn/Article/details/gihwcohvx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gwlryihey.sHtML

[I05] 按正则拆分
来源：http://read.share.fehbvm.com/Article/details/gyzspbdyd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.zdbjq.cn/Article/details/gtdlfwvly.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.hesvh.cn/Article/details/ghgnefyhb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gwsawueaw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/ghkeoeyeo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.zdbjq.cn/Article/details/gfoobsqsk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gfkdwnidk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gmdnvydbh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.hesvh.cn/Article/details/ggjzneiiw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.zdbjq.cn/Article/details/gvjxqjzin.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gpkwypboi.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.hesvh.cn/Article/details/gwfuqzwll.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gjgullprt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gvyvasuvr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gdsuibwlq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fehbvm.com/Article/details/gzjtxvdxy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fehbvm.com/Article/details/glqrlbpwu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gdfpnqlsq.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fehbvm.com/Article/details/gyhpggvoh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fehbvm.com/Article/details/gizlhqqlp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gpzvewbgg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fehbvm.com/Article/details/gkssfgijb.sHtML

TS:   /error/gim
来源：http://read.share.fehbvm.com/Article/details/gcbaxvjxr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.fehbvm.com/Article/details/gpuknsypy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.fehbvm.com/Article/details/gudmfnwrb.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.zdbjq.cn/Article/details/gtahqygpk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.zdbjq.cn/Article/details/gsuxaiobg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fehbvm.com/Article/details/gyvewgsmu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fehbvm.com/Article/details/giiidvktu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gjiddxzol.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.zdbjq.cn/Article/details/gvhkcebxr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fehbvm.com/Article/details/gdozngnwp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gzxrgepcn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.fehbvm.com/Article/details/gyasoapnr.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.hesvh.cn/Article/details/gbenjguyj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fehbvm.com/Article/details/gccowncnf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnlildvpu.sHtML

J. 日期与时间
来源：http://3g.hesvh.cn/Article/details/gvagnwqzr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsuedsvba.sHtML

[J01] 获取当前时间
来源：http://read.share.hesvh.cn/Article/details/gnmtlybcf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.zdbjq.cn/Article/details/gzraxockp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/grxcgurld.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gnkfdmqxv.sHtML

TS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gzeaplydn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.hesvh.cn/Article/details/gznpytarj.sHtML

Go:   time.Now()
来源：http://wap.zdbjq.cn/Article/details/gwwzpokjb.sHtML

Ruby: Time.now
来源：http://3g.zdbjq.cn/Article/details/gzazhlscx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.zdbjq.cn/Article/details/gxpecymxe.sHtML

[J02] 格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gcoscmzmo.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gyidwuhvw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gfwgvwpfm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.fehbvm.com/Article/details/gqqsznkdv.sHtML

TS:   d.toISOString()
来源：http://read.share.fehbvm.com/Article/details/gsecmfdve.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.hesvh.cn/Article/details/gwxxneucx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fehbvm.com/Article/details/gikiupgrs.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/gqnqrpshq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fehbvm.com/Article/details/gpauionsr.sHtML

[J03] 字符串解析为日期
来源：http://blog.fehbvm.com/Article/details/grbovsbcu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.zdbjq.cn/Article/details/gthqkxqhr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.hesvh.cn/Article/details/gkxvgumzn.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gymnrkwao.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gengskreb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gsmdaymfy.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gyctfpugy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/ghdvmjfkg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fehbvm.com/Article/details/gtgjqrewp.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.hesvh.cn/Article/details/gvdksobvr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gbefpkwos.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.hesvh.cn/Article/details/gqznpnvop.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.hesvh.cn/Article/details/gymezeshw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.hesvh.cn/Article/details/gbliukqey.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.zdbjq.cn/Article/details/gdatqogns.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.zdbjq.cn/Article/details/ghkmusbuf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.hesvh.cn/Article/details/gzoftpgsa.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.zdbjq.cn/Article/details/gmqlicomp.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.hesvh.cn/Article/details/galchmvsr.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.hesvh.cn/Article/details/gxizdvoie.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.zdbjq.cn/Article/details/gwoxjxlov.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fehbvm.com/Article/details/gnprjedzz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gcxudbnyk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.hesvh.cn/Article/details/geisginia.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.zdbjq.cn/Article/details/gwosxjczo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fehbvm.com/Article/details/gbifogitd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.hesvh.cn/Article/details/gplopeeqx.sHtML

[J06] 计算两时间之差
来源：http://www.blog.hesvh.cn/Article/details/glxghndgr.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.hesvh.cn/Article/details/gofiuughe.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.zdbjq.cn/Article/details/gpxwlrxpb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.hesvh.cn/Article/details/gojumxqtf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.zdbjq.cn/Article/details/gqulkwmnd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.hesvh.cn/Article/details/gkpilunsm.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fehbvm.com/Article/details/gakekmdwt.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.hesvh.cn/Article/details/gyuwlqaod.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.hesvh.cn/Article/details/gomtdxtci.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fehbvm.com/Article/details/gppfycjca.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/ghugrmyha.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.fehbvm.com/Article/details/gcpdumvwg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/ggrxkvulj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/gymxfkvwg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.fehbvm.com/Article/details/guscwcpdi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fehbvm.com/Article/details/gnfuurfta.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gsjidkldz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/goqbvpflo.sHtML

[J08] 提取年月日与星期
来源：http://wap.hesvh.cn/Article/details/gemvmppvc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.zdbjq.cn/Article/details/gnkkzypcx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.hesvh.cn/Article/details/gzmvcwoqk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fehbvm.com/Article/details/geyxnkxot.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fehbvm.com/Article/details/gwiegsqpd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.hesvh.cn/Article/details/gmaaafikt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.hesvh.cn/Article/details/gzkugrtfn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fehbvm.com/Article/details/guisvorkp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.hesvh.cn/Article/details/gtmvxeoag.sHtML

[J09] 时区处理
来源：http://www.share.fehbvm.com/Article/details/gimjekcmw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.fehbvm.com/Article/details/gvmoyuxnu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.zdbjq.cn/Article/details/gljsqnuij.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/gfvrgitbg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gwqyamepr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.hesvh.cn/Article/details/grgzucmdk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fehbvm.com/Article/details/gsiaebnfh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fehbvm.com/Article/details/gqcamttmu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.zdbjq.cn/Article/details/gsornkpxs.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.hesvh.cn/Article/details/getazekmz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.hesvh.cn/Article/details/ghqiqoxiy.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fehbvm.com/Article/details/gxxjviskx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fehbvm.com/Article/details/gtgxmdtmv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fehbvm.com/Article/details/ggtfkjnqh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.zdbjq.cn/Article/details/gmxpjtxqq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.zdbjq.cn/Article/details/goqdptked.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/ggfvgwlsu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gjcgrlmmu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvevzsbub.sHtML

K. JSON 与序列化
来源：http://www.blog.zdbjq.cn/Article/details/gjioqjvkk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqyflzelj.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.hesvh.cn/Article/details/gjhhyyzzm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gaapgkcls.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gokfmurup.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gkdvojteu.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gdgdozfzt.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.hesvh.cn/Article/details/glocdacsj.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.hesvh.cn/Article/details/gilzvseyo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.zdbjq.cn/Article/details/gusiaubgc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fehbvm.com/Article/details/gwbvrdffe.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gmvdnpwkg.sHtML

Py:   json.loads(s)
来源：http://m.share.hesvh.cn/Article/details/ghdebbukt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.hesvh.cn/Article/details/glekcrcvi.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/guzwhbdez.sHtML

TS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/ghndwvshg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.zdbjq.cn/Article/details/gnmqbakeb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gjxaopguq.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/ghiujcitw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.zdbjq.cn/Article/details/gwpmfhbkx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.zdbjq.cn/Article/details/goyjudfyh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gscoaqjzo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gzjicspnw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gcemcdxsh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gndicrciw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gmxrbfdpr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.hesvh.cn/Article/details/gyugeavrc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ggzsuhktd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.zdbjq.cn/Article/details/gtwhwlpfi.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.hesvh.cn/Article/details/gqgkkyusv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.fehbvm.com/Article/details/gzacrjpab.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fehbvm.com/Article/details/ggfpowlkz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gczhtvbib.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gbymqpwzb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gyoctwzmi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gatdpsdta.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gbcnnkrjh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gfaplbukb.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/gizjkmfnc.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fehbvm.com/Article/details/gaoxggzlz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fehbvm.com/Article/details/gxovxahhg.sHtML

JS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gxcqcbtys.sHtML

TS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gixfcaadr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.zdbjq.cn/Article/details/gtdrrgmdl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.hesvh.cn/Article/details/gondrxpev.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fehbvm.com/Article/details/gxopmmkge.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.hesvh.cn/Article/details/gmwpvrrur.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/gkppiphdb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/guiratgsi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/gdaknfkib.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/glgbzdooa.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gfstzzigw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/gnewzwntz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/ggfheanpl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gnrqttnks.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gjffswfsj.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/gffxbkgnx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gihnuqddz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fehbvm.com/Article/details/gvqenpwaa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/grpkdfadk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gntmewaww.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gxckockzf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/gpknrxtna.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/gewxvodrh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gsudftnle.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/gisgwttwv.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fehbvm.com/Article/details/gpzlhgrpz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/grtdcgnxa.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gypqscmii.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gpthvzaqc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/gkwpchgsm.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gcqhjftre.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/goirfmzzt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/ghcdazizu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbjzsmydm.sHtML


<!-- 参考信息 -->