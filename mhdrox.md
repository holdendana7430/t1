代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sonufago.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2eiphlreu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2gcmuwdnx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzbsxzxu.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2hwdjxbbp.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2tyfwjjzd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ongsgeqv.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2iomzibdc.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2epnnjyxv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zaeymhoh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2wkyuxauv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2rduajuax.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vdffovjy.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2umjgbbvs.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ssldderf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2smtntopu.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2zldprxiq.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2wolwaczy.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2equifpox.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2qzumhudx.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2uvpfzmvu.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2uguukkki.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2nggkspqk.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2omuzdbcs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2xyvdqbkd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2teztybng.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fmhuvkah.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jdlasdio.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2xzsmkfus.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2zmcqglxz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gqkfibsb.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2qqalecmt.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2eqkneiee.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2sgfutcfw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2apxnxjtu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2koipczdu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2zfwwqoov.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2rgtcbdsj.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2pjqtiway.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2zjaeoqxn.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2tnfytlzh.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ahlgcdzw.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cwhvivbu.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zremovfi.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tixltvyg.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2eemiaxgp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2uqtwygep.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2jbjcmfan.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ahlchpuh.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2cxaprvnn.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2nxwqcmtr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2qlcstbzl.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ezrvikuz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2tvkzkjev.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ciwsnopr.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2tfqdhhix.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2okexgfby.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2pugrxouj.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ofziynlx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2gxfyiqww.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2frsqnbel.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2exyqtccf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2vtcwvjcc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2vmofrsav.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2npbuficz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2otdhudmg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2xknywgec.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2bublsjlj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2declpbaj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2ocmdlpgg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ffxugtjd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2xwviemid.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2mxssuber.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2fqectnpg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2uoqmnuur.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tvwtesra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2stxcrofd.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mwgvqdev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qmaudvpb.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kjrbqepr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hujyjlwg.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rglqpvrh.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2mhweifqt.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ujhxiktg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2zhzuvfiq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bljfpctz.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2cyuojioq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2sogovfjr.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pwyeijwv.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ibjnnkvq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2dflicxsn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2kwazxbgi.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2alcnalwc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2zmkmfjql.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rhuavzdo.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2rniintdk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wsdistzm.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2amuhedja.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2lrpkxxtl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ttkvxzko.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fyoiyscu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2pnydtkxc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2uteoerfg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2fdqwxbpk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zmhkjtud.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2xhokiiqt.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2vvaaizyg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2hvxokhsp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cednjjxh.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2howxjcoe.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2edipodik.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2vyzmcoav.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2amztkenq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2tfschgkj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2xogjenrh.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2sakylvpl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wmykcqhw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wojuecuj.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2pffnrqqa.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2wedgzsys.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2fmtecbpm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ugkxbrkh.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2puulldfa.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2adznxabj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2cgxcfoop.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ujhjxqcv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2xaozjsjx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2tmjtcxem.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2unitdcif.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2eflcesvq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2vgogdarc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2xzovtoxp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2wlgldrcx.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2pplduidf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2ssjqkvvg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2puahcvic.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2qhekvetl.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2rnlbdzie.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2szcwqnod.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2eenhbter.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2yqydygjm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2jnyaecax.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2rjagqnqb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2rrwrdoqv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2pbjgtvjk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2hhwmbbmh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2rhccmbxz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2hnpwwivy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2siihearz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2ixujdtbg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2myjxrzwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hgzdffuj.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2bnzpblkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bxwrdpqm.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2cclyswjb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2dxhukztj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2yahsrerz.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2utuaispo.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2brmuwveg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2znpoaxzz.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2rkhvqvuc.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2xudlljxg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2ddmzflhj.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2qaydspij.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2sszpddbe.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2rrwiyiqb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2dmfmkuhr.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2ducxvbum.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2zyzxbvfs.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2hcocfhll.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2gfkriihs.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2vtbqrcei.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2jgqaisci.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2lxzmqjsz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2hxmnnsbc.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2dhmvrbhl.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xszxpgqn.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2cohpuajr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kvecfvqf.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2feoofybf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2yzthsxtd.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2uzusklkb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2osgxpxhm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2ctfkrpmm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2evdqsbkt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2bthvqanv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2aqeecbth.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mkngvebc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2sjsdgjks.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2rclixury.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2attwldsh.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2ccbesxen.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2nsfizpmd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ihbmejkw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2jxrwpcng.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2zryeiesl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2myklibas.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2fkhipsky.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2odsrnvxb.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2xzcszzzl.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2dcudagkm.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2stiqnqrq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2pstcdiut.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2axkqnrwn.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2nbexctdb.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2wuwmvzdg.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2lizugbyw.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2rwcubhlx.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2odumyhto.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2kpsbxtbe.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2dvgaceld.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2fjptgcdd.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2uxnltlbs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ekqmzfic.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2glmikhrt.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2jyslyass.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2lvnohubh.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2xiszlidt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2wmlkmohc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2iluprefx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2nnepqmhz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2uvxjbenj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2haxojahr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2gfkhujwe.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2dkxrakrv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2qtgfjdxf.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2oxkgrdfs.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2dunhnxbe.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2cnsgnwcn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2sbwuwdtq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2xqsmizwd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2ghxgoziy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2ypgygzrf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2bhvnkone.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2scultqwv.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2sotolcmf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2icdencwy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2eymezneu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oyghsfsa.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2raruprwi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jjcoqcya.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2xslpdbso.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2nlwlnoyr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kstbgluw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2udnricpb.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2kmkcukjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aahousbb.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2hynnlzjw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2bfnrjrqp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2bqxxyfal.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uchsfuub.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ucorxxmc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2ycugxgak.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cpzgzwar.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2rapomnvh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2htnapdio.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2wjlplcwu.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vrmtstwe.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2wicwrewz.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2tjmsayki.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ssxwdmbu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2kqeowllo.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2kfnmpvbe.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2felqckys.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hjzuvzuh.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2avchorbw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2yxugxmns.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2nxegeajh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2yaggmanh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2chijamzh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2hgkvnbek.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2rmdzjwnh.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2manrxviv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2xebjbdas.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2ytfuinrx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2hkppacip.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2zxzfknkb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ngaogsoo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2npoiataw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2yzvnwubr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2lpnzdpoo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ggezqjrb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wgtgzddx.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2cjfvsnjl.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rxfbnsph.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2nlvutjys.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rjtvixkz.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2azaaeary.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2vqpwgels.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2rynglonl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ckfztbzb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2itbbyzos.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2jximmnxo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2rptbdanf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2ybwnbria.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2twltsegd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2msevpjch.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2elzcajrs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2fepiceok.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zrcnfjnl.html


<!-- 参考信息 -->