代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtduxvybvh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yj202588.top/gtusffwkri.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.dianchejie.cn/gtdpyueglq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gttmtxyfmh.html

[H03] 主动抛出异常
来源：http://hz.aibaodan.cn/gtviywdjfb.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj20258.top/gtgcndjosp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zycfv.cn/gtnlhrhhwo.html

JS:   throw new Error("错误信息");
来源：http://hz.ehwqpu.com/gtqtvrhsya.html

TS:   throw new Error("错误信息");
来源：http://hz.0kj1m.cn/gtivjgsbmi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xuanzx.com/gtbbyuglna.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.chenjidiqi.icu/gtedibpwfr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gogol.net.cn/gtlokcwibs.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ivvv.top/gttxnewwea.html

[H04] 自定义异常类型
来源：http://hz.yj20258.top/gtdhyfkawh.html

Py:   class MyError(Exception): pass
来源：http://hz.ybcxt.top/gtjktdtptq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhaomingkeji.xyz/gtbbfjuofw.html

JS:   class MyError extends Error {}
来源：http://hz.shanyushiyangtech.top/gtdodhmhuf.html

TS:   class MyError extends Error {}
来源：http://hz.jiagoushi.top/gtzyxklhok.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jinqigfzy.top/gtlpomsftx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xziqi.cn/gtgioupeho.html

Ruby: class MyError < StandardError; end
来源：http://hz.ppjwa.cn/gtmiofbqbf.html

C#:   class MyException : Exception {}
来源：http://hz.shanyushiyangtech.top/gthorkuqnp.html

[H05] 捕获特定类型
来源：http://hz.xingfuxueyuan.xyz/gtimxtctqw.html

Py:   except ValueError as e:
来源：http://hz.xuetiantiany.cn/gtgoeivywz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yj20258.top/gtbfhtfnnj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.vqdsnc.cn/gthmdzmkkt.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xziqi.cn/gtbkylattw.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhoulong.xyz/gtmfallgfg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.aizwys.cn/gtnxofeili.html

Ruby: rescue ArgumentError => e
来源：http://hz.iojbl.cn/gtymtnjaee.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yanxiufei.cn/gtscisvouw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yonumen.top/gtemempkgg.html

Py:   value = d.get("k") or default
来源：http://hz.jqgufenzy.top/gtxdzdgimk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gotoacloud.top/gtwdubqomv.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigufen.top/gtofpwmusr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.0kj1m.cn/gtchosujfq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.316326.xyz/gtstdicihm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.dashuyun.cn/gtdpvhcpeo.html

Ruby: d&.dig(:a, :b)
来源：http://hz.snrcjt.cn/gtsfdjyydh.html

C#:   obj?.A?.B ?? default
来源：http://hz.shanyushiyangtech.top/gtskfpshpk.html

[H07] 断言
来源：http://hz.snrcjt.cn/gtxynylucn.html

Py:   assert x > 0, "必须为正"
来源：http://hz.quarkkingdee.top/gtswpygsqu.html

PHP:  assert($x > 0);
来源：http://hz.cqqwz.cn/gtsbahkyih.html

JS:   console.assert(x > 0);
来源：http://hz.chenzaomai.com/gtpzrrynuf.html

TS:   console.assert(x > 0);
来源：http://hz.bjfxy.top/gtcoudaupl.html

Java: assert x > 0 : "必须为正";
来源：http://hz.fengsongda.top/gtxonxafrz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yueranfly.top/gtknfvtilc.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.guowangkeji.top/gtbsnqvebh.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cqqwz.cn/gtldzilsis.html

[H08] 获取错误信息与堆栈
来源：http://hz.yvedp.cn/gtcejuzqnu.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yvedp.cn/gtuihnmtqp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.aibaodan.cn/gtbiyfqakc.html

JS:   e.message;  e.stack
来源：http://hz.yuanzhike.top/gtzervpriq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yuanzhike.top/gtpqgqtist.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yangfankeji.com/gttrzeyiux.html

Go:   err.Error()
来源：http://hz.jqgufenzy.top/gtbxfufssj.html

Ruby: e.message;  e.backtrace
来源：http://hz.hywenlv.cn/gtrkjugbpp.html

C#:   e.Message;  e.StackTrace
来源：http://hz.52xcode.cn/gtoueysrjw.html

[H09] 带错误码的异常
来源：http://hz.shanyushiyangkeji.top/gtixbhulnj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.tianlin.xyz/gtedvxgema.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hammf.cn/gtnvmszlnt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shzxlz.cn/gtagevzdac.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.feifeiyinyue.top/gtqarytyyi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hnqzz.top/gtpikhtqil.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.gogol.net.cn/gtqfsgcgmb.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhengqikj.top/gtkwsaajwf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yongpay.top/gtydtrfdwu.html

[H10] 资源自动释放
来源：http://hz.wangshuangyany.cn/gtacatfxxs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.aizwys.cn/gthivwfkjh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.nanxinkj.top/gtpjvhnjox.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xinyue.icu/gtcwintewh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yueranfly.top/gtklejhahs.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.cashguo.top/gttuphrniv.html

Go:   defer f.Close()
来源：http://hz.sweek.top/gtmkirvqec.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinyuanbaomall.cn/gtkrrfbgvt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shuidangran.top/gtfyyzbhnc.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gteosuypai.html

I. 正则表达式
来源：http://hz.yj20258.top/gtkqzohpzw.html

================================================================================
来源：http://hz.aizwys.cn/gtwwyunzvp.html

[I01] 判断是否匹配
来源：http://hz.vqdsnc.cn/gtzyzdcrxn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.bjfxy.top/gtoxgrjxbk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jqgfzy.top/gtthksiabt.html

JS:   /\d+/.test(s)
来源：http://hz.jinghuilouyu.cn/gtazmrjiuh.html

TS:   /\d+/.test(s)
来源：http://hz.sweek.top/gtriclhtwk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shzxlz.cn/gtpflundbc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.aibaodan.cn/gtlhxsbmwl.html

Ruby: s.match?(/\d+/)
来源：http://hz.snrcjt.cn/gtccetauln.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinqigfzy.top/gtylvnemvu.html

[I02] 提取所有匹配
来源：http://hz.cdnleiting.top/gtlnskqelw.html

Py:   re.findall(r"\d+", s)
来源：http://hz.svipenyu.cn/gtrfrgyqxk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.fzhhl.top/gtltmajagm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj20258888.top/gthmksuzqt.html

TS:   s.match(/\d+/g)
来源：http://hz.jyoumei.cn/gtdmdazlfo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.iojbl.cn/gticzibarg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.feifeiyinyue.top/gtskmuecrr.html

Ruby: s.scan(/\d+/)
来源：http://hz.ivvv.top/gtvhbqygmx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yangfankeji.com/gtjjtjkknx.html

[I03] 提取捕获分组
来源：http://hz.tanke756.top/gtauikkafn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yueranfly.top/gtfsripyvl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jianghu66.top/gtvjmprkra.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.haohaochexian.top/gtvwkdypzc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhaomingkeji.xyz/gtiekvzgww.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.c1oappe.top/gtstcpstfi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.birdmap.top/gtebbuwnek.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhixingplan.top/gtavjjhdmx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.smart0.xyz/gttpquytkh.html

[I04] 正则替换
来源：http://hz.hnqzz.top/gtlycnnvzu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yj20258.top/gtadamnpfu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shzxlz.cn/gtvlrqmjqb.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.aizwys.cn/gtqpxbhotg.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gogol.net.cn/gtpkavzanm.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhengqikj.top/gtmxkwtqlo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yj20258888.top/gtygvsfsri.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cqqwz.cn/gtsgilxcbg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ehwqpu.com/gtnmeqbqdl.html

[I05] 按正则拆分
来源：http://hz.chenlongwang.top/gtsgupggor.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jlsjyb.cn/gtuivtejim.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.daria6918.cn/gtfrbzaddf.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yongpay.top/gtiysyfayi.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.nanxuanxn.top/gtofcqkneq.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ivvv.top/gtqcwgulil.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hnqzz.top/gtcrfnjmqu.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ydjk.org.cn/gtopwxxbjn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jinghuilouyu.cn/gtmkuexpwe.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.guannengcc.top/gtfpepbyuq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.aizwys.cn/gtxrihaotq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xylfe.cn/gtaoetrbtk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cdnleiting.top/gtljfaffaj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cqqwz.cn/gtieyutlzg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.nanxinkj.top/gtpidrnpyq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jinqigfzy.top/gtnaekdidg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.sweek.top/gtvnldscad.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gtgahjhyyu.html

[I07] 忽略大小写与多行模式
来源：http://hz.hysaishi.cn/gtyhfyajhx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.0kj1m.cn/gtosivpqvx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.dashuyun.cn/gtlkoojeqq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.tian-w.cn/gtaqdjjpza.html

TS:   /error/gim
来源：http://hz.haohaochexian.top/gtjkstmqow.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.nwbrower.top/gtarhqszra.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.c1oappe.top/gtuwpkicth.html

Ruby: s.scan(/error/i)
来源：http://hz.ppjwa.cn/gtmckzdpzi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cdnleiting.top/gtskwtwbdm.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.chenjidiqi.icu/gtxlenvtqa.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xinyue.icu/gtxwfgpfmc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.guowangkeji.top/gtneakapgz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yvedp.cn/gtbklujogu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.0kj1m.cn/gtetfezrtr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shanyushiyangkeji.top/gtxhyamybr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xuanzx.com/gtdrigdpcy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.aibaodan.cn/gtapwkvhne.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gogol.net.cn/gtwqylmnhy.html

================================================================================
来源：http://hz.gotoacloud.top/gtyhyhjiqh.html

J. 日期与时间
来源：http://hz.shuidangran.top/gthtoudwev.html

================================================================================
来源：http://hz.yanxiufei.cn/gtizeqaypi.html

[J01] 获取当前时间
来源：http://hz.guowangkeji.top/gtqlujxhid.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xylfe.cn/gtehgpfmwd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jinyuanbaomall.cn/gtjunhlocb.html

JS:   new Date();  Date.now()
来源：http://hz.zhijiandao.cn/gtorvalivy.html

TS:   new Date();  Date.now()
来源：http://hz.yj20258888.top/gtspcqrmoc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yonumen.top/gtezeghggl.html

Go:   time.Now()
来源：http://hz.nanxuanxn.top/gtcwlyyipz.html

Ruby: Time.now
来源：http://hz.xziqi.cn/gtiffufece.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shanyushiyangkeji.top/gtjfzmldjj.html

[J02] 格式化输出
来源：http://hz.jqgfzy.top/gtteiijgqz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.pengpengdd.cyou/gtlzieezgr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.c1oappe.top/gttlcgrpes.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.nwbrower.top/gtjqjmimtr.html

TS:   d.toISOString()
来源：http://hz.hywenlv.cn/gtvtcggcay.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.aibaodan.cn/gtrczszkio.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ehwqpu.com/gtdezmpdav.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenzaomai.com/gtxcmvkytg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gzhubu.top/gttltpaqmq.html

[J03] 字符串解析为日期
来源：http://hz.andypj.xyz/gtsmqdjkva.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.guowangkeji.top/gtqfpoykgk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xuanzx.com/gttsibgzqw.html

JS:   new Date("2024-01-02")
来源：http://hz.zhoulong.xyz/gtqbdcdksy.html

TS:   new Date("2024-01-02")
来源：http://hz.9152youxi.cn/gttbaiqjwd.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.daria6918.cn/gthrvzcdzv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yueranfly.top/gtramvsipw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtcxoechvy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xylfe.cn/gtzpssjwjl.html

[J04] 时间戳与日期互转
来源：http://hz.haohaochexian.top/gtwhztsrdt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yuxming.cn/gtgtbjtyvg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shuidangran.top/gtvzkzlnfp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gaohongyu789.top/gtzeznqhyp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xinyue.icu/gtskilijlx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shzxlz.cn/gtywiyfpid.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.svipenyu.cn/gtxzzjeyhq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.birdmap.top/gtvwqfaqnk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ydjk.org.cn/gtgkcrmtwx.html

[J05] 时间加减（加 7 天）
来源：http://hz.gogol.net.cn/gtvkneeahe.html

Py:   now + timedelta(days=7)
来源：http://hz.9152youxi.cn/gtdrpbxswg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xingfuxueyuan.xyz/gtdxwugbiv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenjidiqi.icu/gtpirqibjy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hysaishi.cn/gtetjuiofz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yongpay.top/gtohtkxwlz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xinyue.icu/gtfvyghcxp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinghuilouyu.cn/gtiiywxrzu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.fzhhl.top/gtiuildpnd.html

[J06] 计算两时间之差
来源：http://hz.jiagoushi.top/gtmuqfuadg.html

Py:   (end - start).total_seconds()
来源：http://hz.wangdashe.top/gtigfaeigj.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinghuilouyu.cn/gtiswjmzrm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.daria6918.cn/gthsbktsmd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jqgufenzy.top/gtiiourufw.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jinyuanbaomall.cn/gtfydwfcws.html

Go:   end.Sub(start).Hours()
来源：http://hz.gaohongyu789.top/gtyysnhkkh.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhiwuduotai.top/gtprrcbafs.html

C#:   (end - start).TotalSeconds
来源：http://hz.mhx1999.top/gtvaoxcdbf.html

[J07] 比较两个日期
来源：http://hz.cashguo.top/gtbuvvfkrs.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gttftskdyk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhengqikj.top/gtlkjpahzf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jinqigufen.top/gtwgmiosse.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shangyingyoupin.top/gtdfldbmqf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.guowangkeji.top/gtxskzqmks.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.smart0.xyz/gtvclasyks.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinqigufen.top/gttjqiryhc.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jianghu66.top/gtodoaeqxr.html

[J08] 提取年月日与星期
来源：http://hz.zhongyouzk.top/gtffpogtbn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinghuilouyu.cn/gtrwyszbnc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.gaohongyu789.top/gtienvcpts.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.haohaochexian.top/gtbluwpnsd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.guowangkeji.top/gtzeotkkci.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.fzhhl.top/gtnszpuvld.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.wangdashe.top/gtkfjzkzjl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hongshengwenyu.top/gtfucydikw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hnqzz.top/gtjyhazqyu.html

[J09] 时区处理
来源：http://hz.jinyuanbaomall.cn/gtoiqbstkn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.0kj1m.cn/gtcpaihwrh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenjidiqi.icu/gtvtvfxgjx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tanke756.top/gtrzamugqr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yanxiufei.cn/gtebqtqzwj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nanxinkj.top/gtnlfhjvlq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.havefunace.top/gtpleauwhv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.guowangkeji.top/gtymfyjxbu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinyuanbaomall.cn/gtnnezjujb.html

[J10] 取今天 / 本月第一天
来源：http://hz.cdnleiting.top/gtnkgtvjxq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj20258888.top/gtoexxdvxi.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cdnleiting.top/gtsmuualnz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhiwuduotai.top/gtshlmqhkm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.haohaochexian.top/gtenpzpeay.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.dianchejie.cn/gtsphcgrqd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.aibaodan.cn/gtyyhzcijf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinyuanbaomall.cn/gtgsypxynq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhengqikj.top/gtygugmbmd.html

================================================================================
来源：http://hz.yuxming.cn/gttvnmfgmc.html

K. JSON 与序列化
来源：http://hz.hnqzz.top/gttvsfrign.html

================================================================================
来源：http://hz.meibo888.top/gtilurhnmx.html

[K01] 对象转 JSON 字符串
来源：http://hz.nanxinkj.top/gthrocbvoe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.gaohongyu789.top/gtjfesvyma.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ydzc1.top/gtuhkesdlf.html

JS:   JSON.stringify(obj)
来源：http://hz.zhaomingkeji.xyz/gtwyiwgsuh.html

TS:   JSON.stringify(obj)
来源：http://hz.jiagoushi.top/gtnctrkjjc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.kuanghao11.cn/gtzkyqtkes.html

Go:   json.Marshal(obj)
来源：http://hz.zhiwuduotai.top/gtvuarcjgq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jiagoushi.top/gtzbagxjvw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ivvv.top/gtilkinjoq.html

[K02] JSON 字符串转对象
来源：http://hz.c1oappe.top/gtpigpoynf.html

Py:   json.loads(s)
来源：http://hz.nwbrower.top/gtdvjwsksw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.bjfxy.top/gtgecdnytx.html

JS:   JSON.parse(s)
来源：http://hz.hnqzz.top/gtdwakingu.html

TS:   JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtstqakrvy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.kuanghao11.cn/gtxwrwvdlf.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cucudq.cn/gtouffvcpb.html

Ruby: JSON.parse(s)
来源：http://hz.cucudq.cn/gtfaelqcyu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.wangshuangyany.cn/gtejuzbkrp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ydzc1.top/gtyugiegmo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.0kj1m.cn/gtnhjopymy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.aibaodan.cn/gtdfsmkacq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.nanxuanxn.top/gtfyzujivd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangshuangyany.cn/gtmswwigfk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.quarkkingdee.top/gthipyeume.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ywan-chungtsiang.top/gtvpjlmyzw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jyoumei.cn/gtmjneadkb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhaomingkeji.xyz/gtvtmtkksh.html

[K04] 读取 JSON 文件
来源：http://hz.zhaomingkeji.xyz/gtjbjjymwi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.daxiang520.top/gtgtdfejuf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.smart0.xyz/gtmdvjqoei.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aibaodan.cn/gtbruroeut.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xuetiantiany.cn/gtfatfaqik.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yj202588.top/gticlfhogu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenlongwang.top/gtykxceoxz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.mhx1999.top/gtkygxqwfc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhijiandao.cn/gtilqkylum.html

[K05] 深拷贝对象
来源：http://hz.nanxinkj.top/gtbtvyapkr.html

Py:   copy.deepcopy(obj)
来源：http://hz.birdmap.top/gtzdgplanx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cqqwz.cn/gtnpgbcwdn.html

JS:   structuredClone(obj)
来源：http://hz.ybcxt.top/gtunezlxax.html

TS:   structuredClone(obj)
来源：http://hz.svipenyu.cn/gtixzavlex.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jyoumei.cn/gtzbmgcsgm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shangyingyoupin.top/gtsobkktnm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ppjwa.cn/gtpflmyfvl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ivvv.top/gttncwvfto.html

[K06] 解析 URL 查询串
来源：http://hz.zhengqikj.top/gtbpvypkca.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xuanzx.com/gtgxgnqikk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yonumen.top/gtdnrulutg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.iojbl.cn/gtymbamdck.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sweek.top/gtfqdbffuw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xuetiantiany.cn/gtsbqnmbzi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.smart0.xyz/gtcowzegzt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gogol.net.cn/gtyeehqvsl.html


<!-- 参考信息 -->