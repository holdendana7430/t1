代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.gogol.net.cn/gtbyycgcvg.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ydzc1.top/gtqhzsctze.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhiwuduotai.top/gtgezhfcmu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhijiandao.cn/gtappckezw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.tanke756.top/gtlkyhaliw.html

Ruby: rescue ArgumentError => e
来源：http://hz.ybcxt.top/gtdeunqtvs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zdqjudy.top/gtporhzjqd.html

[H06] 可选值 / 空值安全访问
来源：http://hz.meibo888.top/gtfkdqovfy.html

Py:   value = d.get("k") or default
来源：http://hz.nanxinkj.top/gtsgmwhrxt.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yuxming.cn/gtyhtusmtx.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.meibo888.top/gtzoqciykx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.dashuyun.cn/gtoyhwqdhw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yuxming.cn/gthacvvxqx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yuxming.cn/gtvlklqpbg.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jiagoushi.top/gteyaqyzbw.html

C#:   obj?.A?.B ?? default
来源：http://hz.cucudq.cn/gtjrbvhvwu.html

[H07] 断言
来源：http://hz.sysykeji.top/gtdbsyczaj.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hammf.cn/gtsamafeyn.html

PHP:  assert($x > 0);
来源：http://hz.yvedp.cn/gtbggkqdrs.html

JS:   console.assert(x > 0);
来源：http://hz.shuidangran.top/gtbssziceg.html

TS:   console.assert(x > 0);
来源：http://hz.zhixingplan.top/gtqbnkmdlf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yanxiufei.cn/gtjitgaskq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yvedp.cn/gtlrlcwmxa.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hfpthk.cn/gtnouegenm.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhengqikj.top/gtlphhjuex.html

[H08] 获取错误信息与堆栈
来源：http://hz.hysaishi.cn/gtufyxvttm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ywan-chungtsiang.top/gtrqvfffeu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ehwqpu.com/gtmvycnsyj.html

JS:   e.message;  e.stack
来源：http://hz.haohaochexian.top/gtqhllrpcg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhongyouzk.top/gtwquuwlkr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.smart0.xyz/gtjhwvvase.html

Go:   err.Error()
来源：http://hz.yuanzhike.top/gtgbwmxiou.html

Ruby: e.message;  e.backtrace
来源：http://hz.andypj.xyz/gtncikxhzo.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hywenlv.cn/gtdylrpvnl.html

[H09] 带错误码的异常
来源：http://hz.ywan-chungtsiang.top/gtfotmyexr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jqgfzy.top/gtvlwvafcu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cdnleiting.top/gttvpjbvch.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jyoumei.cn/gtythnmyzd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.kuanghao11.cn/gtphpbnbgg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.nanxuanxn.top/gtxnpfdvxf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.svipenyu.cn/gtqpkljqfl.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.dashuyun.cn/gtgiozwxuh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.pengpengdd.cyou/gtnwnyrovc.html

[H10] 资源自动释放
来源：http://hz.andypj.xyz/gthckmcdiz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yonumen.top/gttsroydff.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.316326.xyz/gttemdtazq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.meibo888.top/gtmpiiwvpt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.guowangkeji.top/gtcnpeqisj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.shanyushiyangkeji.top/gtkpdkkplt.html

Go:   defer f.Close()
来源：http://hz.mhx1999.top/gtfyvfhklc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shanyushiyangkeji.top/gtqrbewkpb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.nanxinkj.top/gtouvpxfnz.html

================================================================================
来源：http://hz.iojbl.cn/gtklxbrnck.html

I. 正则表达式
来源：http://hz.havefunace.top/gtpwinocsc.html

================================================================================
来源：http://hz.yanxiufei.cn/gtiacipyuy.html

[I01] 判断是否匹配
来源：http://hz.vqdsnc.cn/gtcfdyxhic.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.andypj.xyz/gtfiswjblx.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yuanzhike.top/gtmnsccvdm.html

JS:   /\d+/.test(s)
来源：http://hz.mhx1999.top/gtyrgryauo.html

TS:   /\d+/.test(s)
来源：http://hz.zhiwuduotai.top/gtozwbvwtg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.iojbl.cn/gtwetprhpg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zycfv.cn/gtkufmjphg.html

Ruby: s.match?(/\d+/)
来源：http://hz.52xcode.cn/gtvyqchvyb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.quarkkingdee.top/gtyywfuffc.html

[I02] 提取所有匹配
来源：http://hz.daria6918.cn/gtdaxylcwa.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ppjwa.cn/gtuhgtfucb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.sufxvd.cn/gtntipjdvv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhengqikj.top/gthnupqtgu.html

TS:   s.match(/\d+/g)
来源：http://hz.tanke756.top/gtacllmfwa.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhongyouzk.top/gtdcduivkl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.pengpengdd.cyou/gtfuagkcwr.html

Ruby: s.scan(/\d+/)
来源：http://hz.fzhhl.top/gtypqvanax.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ywan-chungtsiang.top/gtftoiwqmq.html

[I03] 提取捕获分组
来源：http://hz.fengsongda.top/gtxsbdtkze.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.0kj1m.cn/gtrljiarbd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.nanxuanxn.top/gtmfsqbtno.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jqgfzy.top/gtcrjszjji.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.sufxvd.cn/gtssdrkcdk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.daxiang520.top/gtjsykyjom.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ybcxt.top/gtxmxllcon.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shanyushiyangkeji.top/gtbbjydjlv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.0kj1m.cn/gtmgmdoqej.html

[I04] 正则替换
来源：http://hz.tanke756.top/gtwgdmvajx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yanxiufei.cn/gtxzcxexbm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gogol.net.cn/gtxjnhkgzp.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.birdmap.top/gtmnczvwxq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.316326.xyz/gtimviyzyr.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.tianlin.xyz/gtcetmcpus.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hysaishi.cn/gtgaarhhlj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.pengpengdd.cyou/gtllglpyms.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.wangshuangyany.cn/gtutmuvmtw.html

[I05] 按正则拆分
来源：http://hz.hfpthk.cn/gtzaiamogy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhaomingkeji.xyz/gtfpgqrsir.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yj20258888.top/gtyuosekfv.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hysaishi.cn/gtgzevwozz.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jianghu66.top/gtmfaecolp.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhaomingkeji.xyz/gterzqdwxh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.iojbl.cn/gtoyqxubwe.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj20258.top/gtcgwuaxha.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhiwuduotai.top/gtastgwxqa.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.chenjidiqi.icu/gtfvnifotv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.guowangkeji.top/gtqectwjiq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.havefunace.top/gtfzvbsbek.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgufenzy.top/gtujzllcdr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ybcxt.top/gtrfkswbdn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yonumen.top/gtfxyujwjx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xingfuxueyuan.xyz/gtouoytegi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.feifeiyinyue.top/gteawxscji.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.bjfxy.top/gthnikmoku.html

[I07] 忽略大小写与多行模式
来源：http://hz.ywan-chungtsiang.top/gtblqyhpli.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hysaishi.cn/gtvmgpinbr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xziqi.cn/gtvwzmwers.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinghuilouyu.cn/gtgewunloa.html

TS:   /error/gim
来源：http://hz.yj202588.top/gtinpgvfct.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xuetiantiany.cn/gthwwnpchj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xinyue.icu/gtlfkxmrdp.html

Ruby: s.scan(/error/i)
来源：http://hz.pengpengdd.cyou/gtzmvdakun.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.0kj1m.cn/gteeklhrjn.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.chenzaomai.com/gtjeghuepv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.feifeiyinyue.top/gtqsslfzfi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cheryme.top/gtufcabysx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuetiantiany.cn/gtdxzgedzj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgufenzy.top/gteyiibmbh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xuetiantiany.cn/gtaxsfyhbl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhiwuduotai.top/gtegjgweon.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhaomingkeji.xyz/gttrohjxxl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yangfankeji.com/gttkabmqvf.html

================================================================================
来源：http://hz.yj20258888.top/gtzjvijopq.html

J. 日期与时间
来源：http://hz.hnxiangtu.top/gtzzchqmhb.html

================================================================================
来源：http://hz.fengsongda.top/gtjmagcpsd.html

[J01] 获取当前时间
来源：http://hz.yj20258888.top/gtcygsdwaz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenjidiqi.icu/gtansqkvqx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cdnleiting.top/gtgaousodo.html

JS:   new Date();  Date.now()
来源：http://hz.shangyingyoupin.top/gtucevcslm.html

TS:   new Date();  Date.now()
来源：http://hz.chenlongwang.top/gteihvsxts.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hywenlv.cn/gtspzpcdmv.html

Go:   time.Now()
来源：http://hz.yj20258888.top/gtuzadutwu.html

Ruby: Time.now
来源：http://hz.9152youxi.cn/gtblcytsjv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ehwqpu.com/gtpqfwuumq.html

[J02] 格式化输出
来源：http://hz.cqqwz.cn/gtdzrrvjgq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenjidiqi.icu/gtijsubjej.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hnxiangtu.top/gthagxxvky.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.chenzaomai.com/gtonptdbmp.html

TS:   d.toISOString()
来源：http://hz.xuetiantiany.cn/gtlzqjytvj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shanyushiyangtech.top/gtnixwqett.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.havefunace.top/gtzdsvmqpi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.316326.xyz/gtsqkmmaas.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ybcxt.top/gtzkiptslr.html

[J03] 字符串解析为日期
来源：http://hz.cashguo.top/gtfkcykkls.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ywan-chungtsiang.top/gtusgbuzzm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xziqi.cn/gtbibjgyvw.html

JS:   new Date("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtjuejfypp.html

TS:   new Date("2024-01-02")
来源：http://hz.mhx1999.top/gtcrsdthfi.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.guannengcc.top/gtsyvcqfkt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhixingplan.top/gtereaznos.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yj20258.top/gtfhkuhkog.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yanxiufei.cn/gtrwcukegt.html

[J04] 时间戳与日期互转
来源：http://hz.jqgfzy.top/gtmsqalhty.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hammf.cn/gtxjtjylkz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yuanzhike.top/gtlhsylawm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhengqikj.top/gtvagdjbne.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yuxming.cn/gtaccsqsjr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hnqzz.top/gtfcfdbuot.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.feifeiyinyue.top/gtififzbpa.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.316326.xyz/gtxsginqjb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.wangdashe.top/gtyrinfiiu.html

[J05] 时间加减（加 7 天）
来源：http://hz.dianchejie.cn/gtqzshhswa.html

Py:   now + timedelta(days=7)
来源：http://hz.havefunace.top/gtufayroiz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xuetiantiany.cn/gtubhgphfr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aibaodan.cn/gtkjtelovq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ivvv.top/gtwzksvlnp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jqgufenzy.top/gtazdjrzag.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ehwqpu.com/gtyktqfydt.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gaohongyu789.top/gtbvyeljtq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.fengsongda.top/gtvchqvrjk.html

[J06] 计算两时间之差
来源：http://hz.yangfankeji.com/gtrbrnfumg.html

Py:   (end - start).total_seconds()
来源：http://hz.sweek.top/gtlofsfhuf.html

PHP:  $end->diff($start)->days;
来源：http://hz.tanke756.top/gtrdnxymed.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hnqzz.top/gtxmtuyjfd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.dashuyun.cn/gtltaangjl.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.9152youxi.cn/gtlfexsabd.html

Go:   end.Sub(start).Hours()
来源：http://hz.quarkkingdee.top/gtmxjncnax.html

Ruby: end - start                 # 返回秒数
来源：http://hz.c1oappe.top/gtpifzsgxp.html

C#:   (end - start).TotalSeconds
来源：http://hz.shzxlz.cn/gtcgrhzrog.html

[J07] 比较两个日期
来源：http://hz.ydjk.org.cn/gtnoxoavsi.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yuanzhike.top/gttrxanlwh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.svipenyu.cn/gtweqnfwxm.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.guannengcc.top/gtkmssizfr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gzhubu.top/gtpkcjdxgv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.gzhubu.top/gtabwzbnbn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.birdmap.top/gtsnhzolte.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jiagoushi.top/gtioouwyxs.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.wangdashe.top/gtjomqxmdc.html

[J08] 提取年月日与星期
来源：http://hz.nanxinkj.top/gtlesvmzdb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hywenlv.cn/gthtsgmgwm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhixingplan.top/gtspfmcvxm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.wangshuangyany.cn/gtabmcuqsh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhengqikj.top/gtaxhdeezy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.tian-w.cn/gtciqzooqc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cdnleiting.top/gtxsxmhfrb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xingfuxueyuan.xyz/gtkniqqzju.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ivvv.top/gtkbhstbor.html

[J09] 时区处理
来源：http://hz.yuxming.cn/gtxttynfut.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sysykeji.top/gtyldwlkny.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhijiandao.cn/gtijvnxucx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.redwolf501.top/gtuzmtjwzj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shzxlz.cn/gtjmfomczt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ybcxt.top/gtykoijrex.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.0kj1m.cn/gtwjvfeoyo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shangyingyoupin.top/gtlesnxgdo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.316326.xyz/gtklhgvdsy.html

[J10] 取今天 / 本月第一天
来源：http://hz.sxryk.cn/gtpwhftcep.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jqgufenzy.top/gtmgzwevhh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jyoumei.cn/gtwrunspmf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yj20258888.top/gtcnryzxgo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.quarkkingdee.top/gtcmsxvpmz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhixingplan.top/gtgdmqvwei.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hongshengwenyu.top/gtmamdogpg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hammf.cn/gtxjyuocfe.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jqgufenzy.top/gttvvwchwx.html

================================================================================
来源：http://hz.hysaishi.cn/gtwlcxzkvd.html

K. JSON 与序列化
来源：http://hz.yueranfly.top/gtlphytrlc.html

================================================================================
来源：http://hz.sweek.top/gtasiwchqu.html

[K01] 对象转 JSON 字符串
来源：http://hz.ppjwa.cn/gtualxogpn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jqgfzy.top/gtartsrylh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xylfe.cn/gtpaxzoruz.html

JS:   JSON.stringify(obj)
来源：http://hz.havefunace.top/gtyomnkdxz.html

TS:   JSON.stringify(obj)
来源：http://hz.gzhubu.top/gtrtyipdsi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.nwbrower.top/gthkqvofjc.html

Go:   json.Marshal(obj)
来源：http://hz.yangfankeji.com/gtgzdspszt.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhoulong.xyz/gtzuirbami.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.bjfxy.top/gtpkxobozj.html

[K02] JSON 字符串转对象
来源：http://hz.sysykeji.top/gtqgnyfxjq.html

Py:   json.loads(s)
来源：http://hz.jqgfzy.top/gtlvzflcpr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yuxming.cn/gtmkogchnd.html

JS:   JSON.parse(s)
来源：http://hz.kuanghao11.cn/gtpvukmfwk.html

TS:   JSON.parse(s)
来源：http://hz.jqgfzy.top/gtcwouecrn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.andypj.xyz/gtfkusgwrp.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hongshengwenyu.top/gtgnsxhjdz.html

Ruby: JSON.parse(s)
来源：http://hz.jqgfzy.top/gtpysgsvdt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.daria6918.cn/gtsmnbrccs.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.mhx1999.top/gtacdxubvf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.svipenyu.cn/gtwltcasud.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.daxiang520.top/gtrdubatws.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yvedp.cn/gtrxnuxwlu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydzc1.top/gtrjumodsv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dashuyun.cn/gttvxzioar.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.daxiang520.top/gtifyezekv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.svipenyu.cn/gthgvzjgnm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.guannengcc.top/gtwyocfzdj.html

[K04] 读取 JSON 文件
来源：http://hz.jinyuanbaomall.cn/gtpgcqlsna.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhixingplan.top/gthuixrllg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.nanxuanxn.top/gtkeezeimp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hammf.cn/gttnaiuxht.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangtech.top/gtwbzwsgvx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.fengsongda.top/gtzustlncs.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sxryk.cn/gtizpmgnqp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ydzc1.top/gtxuimcffl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.gotoacloud.top/gtvckwyfxy.html

[K05] 深拷贝对象
来源：http://hz.zycfv.cn/gtevlfiisq.html

Py:   copy.deepcopy(obj)
来源：http://hz.hysaishi.cn/gtqxnerpxb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhaomingkeji.xyz/gtlqhdmavp.html

JS:   structuredClone(obj)
来源：http://hz.ppjwa.cn/gtahogihmx.html

TS:   structuredClone(obj)
来源：http://hz.aibaodan.cn/gtgsasvtmy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.0kj1m.cn/gtwpiwvpnc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.daxiang520.top/gtaudxfihd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jlsjyb.cn/gtjxaydgnc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.c1oappe.top/gtbmgmzkjw.html

[K06] 解析 URL 查询串
来源：http://hz.iojbl.cn/gtquxstoxx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cucudq.cn/gtouwyndxd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.mhx1999.top/gtcymwxmoh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigufen.top/gtuguihjlv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnxiangtu.top/gtvsajyvvp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jqgfzy.top/gtwoefcrck.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ywan-chungtsiang.top/gtdkenyufs.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.wangshuangyany.cn/gtwxmkrxca.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.vqdsnc.cn/gtzovoqigf.html

[K07] 进制转换
来源：http://hz.hnxiangtu.top/gtbizcojsr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.chenjidiqi.icu/gtioenniui.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.birdmap.top/gtwjokmvmw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtphsalyxj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.guowangkeji.top/gtviushinr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.snrcjt.cn/gtoedserlt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.9152youxi.cn/gtbmctyutg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ivvv.top/gtuovfhnmw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.aizwys.cn/gtdgixlkne.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.nwbrower.top/gtpaxxbniq.html

Py:   pickle.dumps(obj)
来源：http://hz.pycfn.com/gtlerelwqi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gotoacloud.top/gtbiuxrdyk.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.haohaochexian.top/gtiyvjddhh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gotoacloud.top/gtbfkwhmaj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hfpthk.cn/gthzbnyrpw.html

Go:   encoding/gob
来源：http://hz.shanyushiyangkeji.top/gtcsjptemp.html

Ruby: Marshal.dump(obj)
来源：http://hz.yj202588.top/gtxchzjpcb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinqigufen.top/gtknfjtdkg.html

================================================================================
来源：http://hz.wangdashe.top/gtueiujyox.html

L. 网络请求
来源：http://hz.tian-w.cn/gtenpukjko.html

================================================================================
来源：http://hz.sweek.top/gtbrqefgma.html

[L01] 发送 GET 请求
来源：http://hz.chenzaomai.com/gtprqjgcyo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yj202588.top/gtisjdqkyw.html


<!-- 参考信息 -->