代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vtxyfpuc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2dmfjdman.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2nuezrneh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xxgzxrgr.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2xngpfgkw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2npsfhtqc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2twlhblma.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ekjhbisd.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yjlmuvxi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2oamnmhzy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2luhuhbqh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ypilzvqo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2aijoxgop.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2akjwpnor.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2icfsoqxg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2fsmjodsu.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2bqmiirev.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2fuccrprs.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2dgeqdilf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2xtivygby.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2acspbjkt.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpssatkn.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ftzvbnuo.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2nnsewpgm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2bxiaeunk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xjatycya.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ypmerwgd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2sgjqeqqp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2kcygezsp.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2slnqjbpm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2rhorashi.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2uwfvnbww.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2vavvpcmo.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2lmknrbro.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ewhswclb.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2rnvcoluf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ipdvtabd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2nsdimjkq.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2wwmfczkc.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2qtpvedpk.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2hxyjkvgp.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2gxzwptgy.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wbieesez.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ebdvcrbb.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jcluwzgq.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2xwpoaqhm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2qzzispbt.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2dsnshkoc.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lzvntqrg.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2xualosuh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2fhkwjzii.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2wtlbdzls.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2xrcbpali.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2tionmmxr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ujcvvcba.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2boiauhzk.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2brpnnmeh.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2jufujgjr.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2vlbxlhrj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2jupsqxqm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2cmixkdgr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2xiaanbqc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2ynlhuttw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2auhqxpta.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2kybnymkd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2zjthethy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2jpwbxpua.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2awtbrvcr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2dtndlzuk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2qrnxkfzi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2cuocenzl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2xptkrhqm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2gswfmhcw.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2rzchxzvj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2sdjqodrh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tzqgwfrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mjbwhitk.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2kwqkbxvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aikvhbsy.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2umzdlsfd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2jlwgjkyi.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mbsblfwg.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nmdrrjzx.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2fziwzbuj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2jlguujyv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2gxdwctkl.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2xywuiyie.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2peaghxyc.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2zguddcha.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ibozqoih.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2fordcagh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2feieojsn.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2perdtdmy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2bpwnsfzr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2gxvbdrfk.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2tprqntfu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ggihdjpv.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2kmxnbkdt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2gumkjqcj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2nbsdhrgq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2rvubaoqr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qlcfjouo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ohooxtpv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2jfjmfpgn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2pqqeuvco.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2mpjivhck.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2ekjsclyd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2eflnxnat.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2awzmanky.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2elreujrf.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wpjiloul.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2fkoknawy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2pndccjte.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2zvupmomm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2emxfpbra.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2onazujou.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2kwwwgspt.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gzzybhym.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ewaowkwk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2btrshvso.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2inilsfey.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2mpqrxtwl.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2gcpcuoxs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2leihjbad.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2pnmlkftm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2wspnxxdx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2ayuencmk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2uxggoxbe.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2thiskslu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2znjbuhiq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2seneetmv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2lcxvusea.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2qkzckfsf.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2ayddxoao.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2geyumvra.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2udwubiwe.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2uglmdygn.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2cjpnipnz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2xyeleeqc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2vrieincv.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2wicfdofg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2idsdkvfs.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hextqljc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2xhcolnvz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2tzwumxqh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2hefxtths.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2qkmuschx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2twjsdjop.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2lagmjvoc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2fkfwezgr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2suoumfdo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dxhkgcsl.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2xmbnhbfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lizgkmzr.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ydutgiyg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2qiqybxsx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2lpszkmbs.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2vrqqfsak.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xpmppwoa.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2tduyxcik.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2ffitzvfc.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2dnilfahx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2fhdgyret.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2rzieofni.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2azpgoeob.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2yxpzkzxq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2srebvzip.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2zduvfzpc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2gxjxcffy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2epkcitwx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2hualxuzx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2iptsfrhf.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2numzjbpl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2vjvcdhyx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2qgzuxhfn.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2yrqkoeop.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2wvberqog.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ivqdbpqg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ikkkeuuq.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2unwjftui.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2xvxxtznm.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2wmpcfxon.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2wjejbpgo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2hehnzjee.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2xlcdckqg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2vlnqmmfr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2htqznrua.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hoitafnw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2pgjhblpe.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2rjnrrnyu.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2lgzzaokm.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2emxbjlni.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2pijgyphg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2rsrxdgdo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2rxauligb.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2thbfrjmz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2ickyuybv.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2btfuheqy.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2qxeadoxb.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2zktmtzlq.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2uxjzcaue.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2epcrzeze.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2oofvmucl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2zqlhrecq.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2kgrgrqto.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2wcxlhade.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2poyurtxo.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2zlzlrvil.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2mrlxkpij.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2fssvsikw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2mdvysngc.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2udlqhekc.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2egufqgqf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2cepiqfox.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2oexgpcth.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2txeabugy.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2uaqbawel.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2statmcuf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2wbzusrra.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2bihsmkdk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2azdzbatj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2anjewtck.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2yrovwnqm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2rbrnzljv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2uowulhwg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2gkxnfijj.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2wmeewbsv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2axxlcxsf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2xhiflher.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2yydrlgzd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2cpnznygb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2vralfqpy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2gpdgswnm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2hqvemwzh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2aafxczaw.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2czwqshvk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2vtfapwgc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2sxahtymy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2tyrhwcvd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2svtfpysb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yvsytgej.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2ptlvlmhr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2jhiubgnb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mfkyxndb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2angvyivc.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2jqybpjjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ilkphber.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2smcawozp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2svxbgqil.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2amsxtvph.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2skpdnsyy.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2suuxonty.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2kkmcehwg.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2krbfcujh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2hzdxztif.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2wtgokhut.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2rvtqhjbm.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2fqxxtkvm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2wlfalrvc.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pyeshvxd.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2pxusjryx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2fqsucals.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ahynunml.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2edntlkya.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vqpwwxet.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2kcpqampp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2dvamnpoo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ahkiuhbo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yfwqgals.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2nelvnsxj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2akoiuume.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2zqkpelfx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2atpkzbui.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2xxlsfxcg.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2ecerwhnf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2cjpcldps.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2pvhkqmbc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2elchcbwd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2hilthwrc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2bowtmoig.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2lluqcfxo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2lyrrdssv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2gnrcgrfx.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2oblqxrlk.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2iebjrmcx.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2zinwaipm.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fayqustc.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ackiymhq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2vwmdybpe.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2gdeetslw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ewouqtpe.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2hktzmbto.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2givhddld.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2gpgdyjlz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2uibxvrqf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2wrvvarmi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2koajxsqr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2vpubnczp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2fuxzbvfq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2aczpqvmz.html


<!-- 参考信息 -->