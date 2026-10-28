代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xziqi.cn/gtrftldxgx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xylfe.cn/gtspikdocx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xinyue.icu/gtxvcdnzor.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.wangdashe.top/gtviiureds.html

[H03] 主动抛出异常
来源：http://hz.feifeiyinyue.top/gtcpkbtmpn.html

Py:   raise ValueError("错误信息")
来源：http://hz.jinqigfzy.top/gtiawowgun.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.meibo888.top/gtviacemks.html

JS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangtech.top/gthehcgoph.html

TS:   throw new Error("错误信息");
来源：http://hz.xuanzx.com/gtcqbsjyud.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hnqzz.top/gtmytkkpvg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yanxiufei.cn/gttkkbufwc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yuxming.cn/gtsmedyqyo.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtahmvsgzj.html

[H04] 自定义异常类型
来源：http://hz.jinyuanbaomall.cn/gtsvpeotfs.html

Py:   class MyError(Exception): pass
来源：http://hz.birdmap.top/gtwwclixtl.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.pycfn.com/gtgvtrsaet.html

JS:   class MyError extends Error {}
来源：http://hz.wangshuangyany.cn/gtpfmstrym.html

TS:   class MyError extends Error {}
来源：http://hz.bjfxy.top/gtkxmujkwc.html

Java: class MyException extends RuntimeException {}
来源：http://hz.chenlongwang.top/gthocszrtw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.snrcjt.cn/gtmxumyywl.html

Ruby: class MyError < StandardError; end
来源：http://hz.svipenyu.cn/gtjueedzvj.html

C#:   class MyException : Exception {}
来源：http://hz.shzxlz.cn/gtnmkzcqwy.html

[H05] 捕获特定类型
来源：http://hz.nwbrower.top/gtnnpqjjgv.html

Py:   except ValueError as e:
来源：http://hz.gotoacloud.top/gtsezsoxis.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xingfuxueyuan.xyz/gtscuswggh.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ydjk.org.cn/gtxpltovdu.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.svipenyu.cn/gtyixytgfe.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.birdmap.top/gtwcaoucdn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xuanzx.com/gtcuulmiet.html

Ruby: rescue ArgumentError => e
来源：http://hz.cucudq.cn/gtcnkerawb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinqigfzy.top/gtknoreyts.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shuidangran.top/gtjmyjecgy.html

Py:   value = d.get("k") or default
来源：http://hz.shzxlz.cn/gtrvzxqwoo.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ybcxt.top/gtrflxzsah.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.pycfn.com/gtwysgzgdq.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gogol.net.cn/gtmbmoqzvy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinyuanbaomall.cn/gtanmpoito.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xingfuxueyuan.xyz/gtjehsosev.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhongyouzk.top/gtpygyqzhx.html

C#:   obj?.A?.B ?? default
来源：http://hz.52xcode.cn/gtzuylfhoh.html

[H07] 断言
来源：http://hz.jinqigufen.top/gtaipktrlq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gaohongyu789.top/gtqmaiwsap.html

PHP:  assert($x > 0);
来源：http://hz.guannengcc.top/gtlkkashoz.html

JS:   console.assert(x > 0);
来源：http://hz.zycfv.cn/gtmkazdpxq.html

TS:   console.assert(x > 0);
来源：http://hz.sweek.top/gtrkxcynrd.html

Java: assert x > 0 : "必须为正";
来源：http://hz.dianchejie.cn/gtciohjjlr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hnqzz.top/gtqtfwfkno.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.mhx1999.top/gtwikrmkop.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ivvv.top/gtdfjdstab.html

[H08] 获取错误信息与堆栈
来源：http://hz.cdnleiting.top/gtxruidcsw.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.dashuyun.cn/gtsamlvvng.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zdqjudy.top/gtettbfnag.html

JS:   e.message;  e.stack
来源：http://hz.daria6918.cn/gtxwlcgosb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.chenjidiqi.icu/gtejeafgye.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xuanzx.com/gtasapqpnu.html

Go:   err.Error()
来源：http://hz.zhijiandao.cn/gtxbndgetg.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhijiandao.cn/gtzlblhjsn.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yj202588.top/gtsbzivcej.html

[H09] 带错误码的异常
来源：http://hz.ivvv.top/gtzldpgume.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jianghu66.top/gtmzievveh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sxryk.cn/gtmzzymaap.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xziqi.cn/gtdpklkwtr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jyoumei.cn/gtswakvnev.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cucudq.cn/gtfopvgvqc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yj20258888.top/gtrfseufhg.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ivvv.top/gtdlyujnhd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hnqzz.top/gtwauhnflx.html

[H10] 资源自动释放
来源：http://hz.pycfn.com/gtafqvnyqk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gzhubu.top/gtwpovgmxn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.snrcjt.cn/gtcjjjhesy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sxryk.cn/gtvljiufrj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jianghu66.top/gturbpdyjh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.gaohongyu789.top/gtcjiaofae.html

Go:   defer f.Close()
来源：http://hz.gzhubu.top/gtjrsitcuf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.smart0.xyz/gttzqsayax.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinyuanbaomall.cn/gtlroinwtu.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtehgfktkq.html

I. 正则表达式
来源：http://hz.zdqjudy.top/gtlziddexo.html

================================================================================
来源：http://hz.yonumen.top/gtgxubhrjo.html

[I01] 判断是否匹配
来源：http://hz.zhoulong.xyz/gtohvoxvvp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xuanzx.com/gthjwvlpqn.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shzxlz.cn/gtetlksrza.html

JS:   /\d+/.test(s)
来源：http://hz.andypj.xyz/gttnrhvmuz.html

TS:   /\d+/.test(s)
来源：http://hz.xuetiantiany.cn/gtxbxisxsc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yongpay.top/gtyjjekgor.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xuetiantiany.cn/gtaatywfet.html

Ruby: s.match?(/\d+/)
来源：http://hz.feifeiyinyue.top/gtirxnuggd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.fengsongda.top/gtvrdiyddn.html

[I02] 提取所有匹配
来源：http://hz.zhiwuduotai.top/gttyivhwny.html

Py:   re.findall(r"\d+", s)
来源：http://hz.gogol.net.cn/gtquxlqfph.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ppjwa.cn/gtxwooecvx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.52xcode.cn/gtvicdretj.html

TS:   s.match(/\d+/g)
来源：http://hz.ywan-chungtsiang.top/gtaqrehavk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.gotoacloud.top/gtyeeafcqn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shanyushiyangtech.top/gtajmlmuqr.html

Ruby: s.scan(/\d+/)
来源：http://hz.zdqjudy.top/gtvyatiywi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cdnleiting.top/gtcdqdpaqp.html

[I03] 提取捕获分组
来源：http://hz.ydzc1.top/gtramkqrxw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.havefunace.top/gtbmxibllu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhoulong.xyz/gtwujoypoa.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.sxryk.cn/gtcwwovytr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jqgfzy.top/gtjwrpklrl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.guowangkeji.top/gtesjgbgyk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cucudq.cn/gtqlmjvexe.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xinyue.icu/gtwsazilad.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jyoumei.cn/gtplqmdeed.html

[I04] 正则替换
来源：http://hz.yanxiufei.cn/gtpqmizugf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.smart0.xyz/gtqfzrcsbw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ppjwa.cn/gtffgjkwub.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.fzhhl.top/gtxasllkuq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cucudq.cn/gtdkvgwlwl.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.feifeiyinyue.top/gtbinulygr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jianghu66.top/gtiejzzqna.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shzxlz.cn/gtexepaxgp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xziqi.cn/gtcpfmuoar.html

[I05] 按正则拆分
来源：http://hz.quarkkingdee.top/gtpzcfzvad.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jqgfzy.top/gtobngvsfs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.tian-w.cn/gtptzybsuv.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.meibo888.top/gtjsxrjciz.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.snrcjt.cn/gtcbcifccf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinqigufen.top/gtycbamgtr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.9152youxi.cn/gtwescnxzk.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.wangdashe.top/gtotiieoqn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.daxiang520.top/gtsjvrlkgp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hammf.cn/gtcwxuuwdt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.feifeiyinyue.top/gtsptpkdkj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.fengsongda.top/gtyiliukes.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fzhhl.top/gtkqqiopqi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tian-w.cn/gtwatdegum.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hnqzz.top/gtjwyhxxes.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.snrcjt.cn/gtbhxcjupb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jyoumei.cn/gtjnutydoi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jinqigufen.top/gtsetwvhzr.html

[I07] 忽略大小写与多行模式
来源：http://hz.yvedp.cn/gtzyyavvus.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jyoumei.cn/gtkkksfsjd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinqigufen.top/gtfohnhlbt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xziqi.cn/gthkmzhyfj.html

TS:   /error/gim
来源：http://hz.xuetiantiany.cn/gtizktyysx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cdnleiting.top/gtzpwtrbmc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.feifeiyinyue.top/gtjzsjbshs.html

Ruby: s.scan(/error/i)
来源：http://hz.yj202588.top/gtujzjcrjb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hysaishi.cn/gtrniroasr.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jianghu66.top/gtmeamkbzf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.andypj.xyz/gtmccxbvyl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ybcxt.top/gtemsycolf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhijiandao.cn/gtbuzucplb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigfzy.top/gtvahojeuf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.kuanghao11.cn/gtevrpncdk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.iojbl.cn/gtioheimuc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cashguo.top/gtjhmeziia.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yj20258888.top/gtdowogxxm.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtdninifub.html

J. 日期与时间
来源：http://hz.chenjidiqi.icu/gtysmlwemk.html

================================================================================
来源：http://hz.xziqi.cn/gtzivexltf.html

[J01] 获取当前时间
来源：http://hz.birdmap.top/gtiwqmcnja.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.fengsongda.top/gthsrbouim.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xuanzx.com/gtrgeztudx.html

JS:   new Date();  Date.now()
来源：http://hz.zycfv.cn/gtymwugdjx.html

TS:   new Date();  Date.now()
来源：http://hz.sufxvd.cn/gtkhfoebad.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ydjk.org.cn/gtuwfqikqi.html

Go:   time.Now()
来源：http://hz.ivvv.top/gtnrgylclj.html

Ruby: Time.now
来源：http://hz.tianlin.xyz/gtscqimqsl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jqgufenzy.top/gtnqjwanen.html

[J02] 格式化输出
来源：http://hz.zycfv.cn/gtbewkxtiv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zycfv.cn/gtmzdeejcp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jyoumei.cn/gtxpfycudz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gogol.net.cn/gtmsmkcdua.html

TS:   d.toISOString()
来源：http://hz.ywan-chungtsiang.top/gtoysstefr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xuanzx.com/gtcofbvouj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yonumen.top/gtangrmanr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhiwuduotai.top/gtaddexrmz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.0kj1m.cn/gtvufwgzwa.html

[J03] 字符串解析为日期
来源：http://hz.yj202588.top/gtpourqpkt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zycfv.cn/gtlhyuuyot.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.nanxuanxn.top/gtyzmbbkrq.html

JS:   new Date("2024-01-02")
来源：http://hz.shuidangran.top/gtexfhokod.html

TS:   new Date("2024-01-02")
来源：http://hz.wangdashe.top/gtukeovuim.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yueranfly.top/gtgoasddqs.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yj20258888.top/gtctdwqxmq.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhiwuduotai.top/gtqglvvqdr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cucudq.cn/gtkpjkxmxg.html

[J04] 时间戳与日期互转
来源：http://hz.svipenyu.cn/gtbnwfdyin.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shangyingyoupin.top/gtmnhvisky.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hywenlv.cn/gtrgtvtums.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.mhx1999.top/gtlnfmcmds.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ppjwa.cn/gtzrclrxld.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.wangshuangyany.cn/gtstaasxtg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hnqzz.top/gtluaznjbb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.pycfn.com/gtotnofpga.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinqigufen.top/gttwmgyfbn.html

[J05] 时间加减（加 7 天）
来源：http://hz.iojbl.cn/gtduvdkluf.html

Py:   now + timedelta(days=7)
来源：http://hz.316326.xyz/gtfohjqiet.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ybcxt.top/gttcnwrcxd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.guannengcc.top/gteohvspri.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenzaomai.com/gtoxummgqm.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jiagoushi.top/gtostykjhe.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xuanzx.com/gteprjzacp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.aibaodan.cn/gtiwxhxrxl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.nanxuanxn.top/gteuudyxfr.html

[J06] 计算两时间之差
来源：http://hz.iojbl.cn/gtxtjeexze.html

Py:   (end - start).total_seconds()
来源：http://hz.xingfuxueyuan.xyz/gtbqvctpzn.html

PHP:  $end->diff($start)->days;
来源：http://hz.gogol.net.cn/gtxuuyzctp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.c1oappe.top/gtxeyrybgu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.guannengcc.top/gtzdklzlke.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.wangdashe.top/gtkbugderi.html

Go:   end.Sub(start).Hours()
来源：http://hz.gotoacloud.top/gtzkynphxh.html

Ruby: end - start                 # 返回秒数
来源：http://hz.guowangkeji.top/gtqkblnllc.html

C#:   (end - start).TotalSeconds
来源：http://hz.nanxinkj.top/gtdzautynd.html

[J07] 比较两个日期
来源：http://hz.meibo888.top/gttfepxcsi.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cucudq.cn/gtkkiauenf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.pycfn.com/gtsxbwyzqa.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yvedp.cn/gtugekunsj.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.52xcode.cn/gtkjbihqaf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.guowangkeji.top/gtghnflrwp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.chenjidiqi.icu/gtfegtvhhw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtycalljpi.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.pycfn.com/gtigxmkqza.html

[J08] 提取年月日与星期
来源：http://hz.zdqjudy.top/gtrrcpggss.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.aizwys.cn/gtxdcfoagw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ydzc1.top/gtqdpybuly.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.quarkkingdee.top/gtmmcepehr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.316326.xyz/gtfjtwmsoz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.sxryk.cn/gtbgvigdfq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yj202588.top/gtuehisyja.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xylfe.cn/gtuojnaynn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.c1oappe.top/gtgpdxmvzs.html

[J09] 时区处理
来源：http://hz.hysaishi.cn/gtcvxqptch.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shzxlz.cn/gthnwbmopr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.quarkkingdee.top/gtuqiuqyvo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hfpthk.cn/gtdrfsrvpf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.c1oappe.top/gtlytufauj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.52xcode.cn/gtyjajqsfh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xuanzx.com/gtrjohkgzb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinyuanbaomall.cn/gtkfkdadtv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yonumen.top/gtiulrdclt.html

[J10] 取今天 / 本月第一天
来源：http://hz.chenjidiqi.icu/gtckrnlcgl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jianghu66.top/gtikmcppot.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.wangdashe.top/gtbeabvvei.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jinghuilouyu.cn/gtombpumsh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.wangdashe.top/gtgmlgijxs.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yangfankeji.com/gtlfkphmpl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.haohaochexian.top/gtmlnppfxh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yuanzhike.top/gtokmbtgux.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zdqjudy.top/gtgonklohi.html

================================================================================
来源：http://hz.meibo888.top/gtgwkjtvtn.html

K. JSON 与序列化
来源：http://hz.wangdashe.top/gtcadfcvrk.html

================================================================================
来源：http://hz.ydzc1.top/gtqawkfxlp.html

[K01] 对象转 JSON 字符串
来源：http://hz.shangyingyoupin.top/gtblqtqhvh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yj20258.top/gtyiryfttr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhoulong.xyz/gtfqaqtjpe.html

JS:   JSON.stringify(obj)
来源：http://hz.dianchejie.cn/gttabluymr.html

TS:   JSON.stringify(obj)
来源：http://hz.gzhubu.top/gtqmaojnqc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.iojbl.cn/gtxlumhhzb.html

Go:   json.Marshal(obj)
来源：http://hz.jianghu66.top/gtmuxfvdwf.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.chenjidiqi.icu/gtyzqgugpu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.daxiang520.top/gtfmfpcjwk.html

[K02] JSON 字符串转对象
来源：http://hz.sysykeji.top/gtbvjanrqi.html

Py:   json.loads(s)
来源：http://hz.shzxlz.cn/gtwvnqshpa.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.tanke756.top/gtlmefbfwa.html

JS:   JSON.parse(s)
来源：http://hz.jqgfzy.top/gtouolxpnl.html

TS:   JSON.parse(s)
来源：http://hz.vqdsnc.cn/gtzrnioagf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xuetiantiany.cn/gtdrxkfteb.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.aizwys.cn/gthgwceowd.html

Ruby: JSON.parse(s)
来源：http://hz.ybcxt.top/gtdhshlaaa.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ehwqpu.com/gtszwruscp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.fzhhl.top/gttfnzzedz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gotoacloud.top/gtempgzuuj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shanyushiyangkeji.top/gtdfvgaxif.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhiwuduotai.top/gtnsxnufjd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sxryk.cn/gtsezsuqeh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.meibo888.top/gtauocqbda.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jianghu66.top/gtknrhfvbd.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.wangdashe.top/gtvzxrokcc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cashguo.top/gtsujrbsua.html

[K04] 读取 JSON 文件
来源：http://hz.kuanghao11.cn/gtytanmolf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jqgfzy.top/gtdiouyrgz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.0kj1m.cn/gtxckzrsyg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhongyouzk.top/gtnbbwoazz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.pengpengdd.cyou/gteupqyigd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.havefunace.top/gtbiffysve.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhijiandao.cn/gtqitrqdax.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.c1oappe.top/gtzskczriz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.chenzaomai.com/gtissolpxw.html

[K05] 深拷贝对象
来源：http://hz.gotoacloud.top/gtgtzewilq.html

Py:   copy.deepcopy(obj)
来源：http://hz.c1oappe.top/gtvbgcnoag.html

PHP:  unserialize(serialize($obj));
来源：http://hz.sufxvd.cn/gtxdmtouny.html

JS:   structuredClone(obj)
来源：http://hz.xuanzx.com/gtlpxdrbac.html

TS:   structuredClone(obj)
来源：http://hz.cdnleiting.top/gtripqagpn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.smart0.xyz/gtwsxzubnv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhongyouzk.top/gtztffeouj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.nanxuanxn.top/gtsnlvtyym.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xinyue.icu/gtyzboutoc.html

[K06] 解析 URL 查询串
来源：http://hz.cdnleiting.top/gttnsroybg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hnxiangtu.top/gtrolllwvr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yj202588.top/gtnqapfqbg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xziqi.cn/gtzbwoemye.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydzc1.top/gtdkdwbave.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yonumen.top/gtmkhuopyt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hywenlv.cn/gtpmkpzlbe.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.chenjidiqi.icu/gtvjlmgitu.html


<!-- 参考信息 -->