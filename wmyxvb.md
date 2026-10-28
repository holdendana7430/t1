代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hfpthk.cn/gtbpvafcdp.html

Ruby: rescue ArgumentError => e
来源：http://hz.gaohongyu789.top/gtgxjwoleg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.shangyingyoupin.top/gtzusjuelq.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ydjk.org.cn/gtjopmjnoy.html

Py:   value = d.get("k") or default
来源：http://hz.zhiwuduotai.top/gtpkfaqryr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shzxlz.cn/gtkywayvda.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.dashuyun.cn/gtjwdxxaer.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cashguo.top/gtudpbagut.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jyoumei.cn/gtpwsjihkg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.pycfn.com/gtiqtirpli.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cqqwz.cn/gtswvimoir.html

C#:   obj?.A?.B ?? default
来源：http://hz.bjfxy.top/gteyglzcfr.html

[H07] 断言
来源：http://hz.hongshengwenyu.top/gtwdhxnrej.html

Py:   assert x > 0, "必须为正"
来源：http://hz.nwbrower.top/gtgpcptlbi.html

PHP:  assert($x > 0);
来源：http://hz.shanyushiyangkeji.top/gtjlcyvpxy.html

JS:   console.assert(x > 0);
来源：http://hz.ybcxt.top/gtqpplnugh.html

TS:   console.assert(x > 0);
来源：http://hz.haohaochexian.top/gtqdrefspe.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhixingplan.top/gtguecbhwe.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ivvv.top/gtpiekzxzp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.gotoacloud.top/gtvfthgueg.html

C#:   Debug.Assert(x > 0);
来源：http://hz.chenlongwang.top/gtrrebveia.html

[H08] 获取错误信息与堆栈
来源：http://hz.ywan-chungtsiang.top/gtgoonbjbr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.smart0.xyz/gthvmzyfys.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinghuilouyu.cn/gtpfrppsvp.html

JS:   e.message;  e.stack
来源：http://hz.xinyue.icu/gtzbuvyssi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhaomingkeji.xyz/gtyaixqvmu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xingfuxueyuan.xyz/gtcrmeyxkp.html

Go:   err.Error()
来源：http://hz.chenlongwang.top/gttbhvgksg.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhiwuduotai.top/gtmgpqrbrv.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhiwuduotai.top/gtcgmwvfvy.html

[H09] 带错误码的异常
来源：http://hz.jinqigufen.top/gthccamskv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.quarkkingdee.top/gtcqcytdgn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.fzhhl.top/gtfirogmba.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xuetiantiany.cn/gtenemjhgm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhaomingkeji.xyz/gtxxbpyris.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yongpay.top/gtfhzohnxu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.fengsongda.top/gtqdjpiuso.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xinyue.icu/gtwnfijidk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.wangdashe.top/gtmzemtmjv.html

[H10] 资源自动释放
来源：http://hz.hywenlv.cn/gtxlkrshup.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gogol.net.cn/gtvmpaefnv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhiwuduotai.top/gthxkexxsy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sysykeji.top/gtgoyuaoic.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.feifeiyinyue.top/gtsnzpiigg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.haohaochexian.top/gtyjadjypu.html

Go:   defer f.Close()
来源：http://hz.hammf.cn/gtwmkwmcfj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cqqwz.cn/gtauxxpmst.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jqgfzy.top/gtogdvgrpo.html

================================================================================
来源：http://hz.daxiang520.top/gttuhozrme.html

I. 正则表达式
来源：http://hz.snrcjt.cn/gtztnkvzzm.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtaregldgt.html

[I01] 判断是否匹配
来源：http://hz.jinghuilouyu.cn/gtvvjfhssq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.meibo888.top/gtfpfapmrj.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yj20258888.top/gthfibtbzi.html

JS:   /\d+/.test(s)
来源：http://hz.zdqjudy.top/gtyscdtiyp.html

TS:   /\d+/.test(s)
来源：http://hz.sweek.top/gtfnsprvux.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ywan-chungtsiang.top/gtvzuvtwsp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.wangdashe.top/gttunnbxcz.html

Ruby: s.match?(/\d+/)
来源：http://hz.xziqi.cn/gteqsgtdat.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jyoumei.cn/gtxlbiufca.html

[I02] 提取所有匹配
来源：http://hz.hysaishi.cn/gtxkcqkglh.html

Py:   re.findall(r"\d+", s)
来源：http://hz.tian-w.cn/gtvmfkknes.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.meibo888.top/gtudwgimpw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.dashuyun.cn/gtequwdrgd.html

TS:   s.match(/\d+/g)
来源：http://hz.hongshengwenyu.top/gtaiewmtpz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shanyushiyangtech.top/gthblmppmu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.c1oappe.top/gtbrchxntp.html

Ruby: s.scan(/\d+/)
来源：http://hz.yonumen.top/gtpxhhvgkm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.kuanghao11.cn/gtvlehiyvb.html

[I03] 提取捕获分组
来源：http://hz.tianlin.xyz/gtmzicostm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.guannengcc.top/gtrumjqstt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.snrcjt.cn/gtocaqpwvk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.chenzaomai.com/gtgbitqrnz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xziqi.cn/gtyzzpoejf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhongyouzk.top/gtjlmgyzhh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yongpay.top/gtybmmcbig.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xuetiantiany.cn/gtpexwqpgg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yueranfly.top/gtutxboods.html

[I04] 正则替换
来源：http://hz.guannengcc.top/gtbckjqgfi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhoulong.xyz/gtexfkroiy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinghuilouyu.cn/gtikpehasj.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ydjk.org.cn/gtruvrcamk.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.bjfxy.top/gtldqpbwys.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hnxiangtu.top/gthnajwsdp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cdnleiting.top/gtxpsonzjd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ydzc1.top/gtgrmtjwgx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jyoumei.cn/gtpkuektuz.html

[I05] 按正则拆分
来源：http://hz.aibaodan.cn/gtdjegkdtj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ybcxt.top/gtlhgwxwsk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhaomingkeji.xyz/gtxeevgqvh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.chenzaomai.com/gtqbwldqww.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cdnleiting.top/gtylmkklqw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinqigfzy.top/gteivuffbz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hnqzz.top/gtgspasoye.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jlsjyb.cn/gtewtuplpm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.tianlin.xyz/gtqttcttzk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhijiandao.cn/gtmbsqzhzp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xziqi.cn/gtffqhlyoi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.chenlongwang.top/gthomywndv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zycfv.cn/gthyptzysc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yvedp.cn/gtrduwjpom.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hywenlv.cn/gtygugcepf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.fengsongda.top/gtksrlavjg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.c1oappe.top/gttmrzwcve.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jqgufenzy.top/gtrejidmmg.html

[I07] 忽略大小写与多行模式
来源：http://hz.52xcode.cn/gtlzzxxzod.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.guowangkeji.top/gtohbomahr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yvedp.cn/gtimzzqqvs.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.snrcjt.cn/gtmbvhuqtg.html

TS:   /error/gim
来源：http://hz.gzhubu.top/gtrpuivcnz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cucudq.cn/gthndpjlln.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shzxlz.cn/gtnoygpwib.html

Ruby: s.scan(/error/i)
来源：http://hz.zhixingplan.top/gtkesvzjoh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jqgufenzy.top/gtfolalfzq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hnxiangtu.top/gtxemqjyjh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhixingplan.top/gtvhgqgcpy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.gaohongyu789.top/gtcblnpkek.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenlongwang.top/gteaprwezf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhijiandao.cn/gtxtwkceek.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jyoumei.cn/gtlzbizwbr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gogol.net.cn/gtrwjynmvy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.chenjidiqi.icu/gtojtccesd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cdnleiting.top/gtbluwmljh.html

================================================================================
来源：http://hz.jinqigfzy.top/gtcoemkcox.html

J. 日期与时间
来源：http://hz.wangshuangyany.cn/gtjubqicyu.html

================================================================================
来源：http://hz.yongpay.top/gtydhhpzvj.html

[J01] 获取当前时间
来源：http://hz.dashuyun.cn/gtgjcagugv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.iojbl.cn/gtwwmxnxyi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hnxiangtu.top/gtdkpntjkv.html

JS:   new Date();  Date.now()
来源：http://hz.daria6918.cn/gtcclkqctw.html

TS:   new Date();  Date.now()
来源：http://hz.aizwys.cn/gtopluthot.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xuanzx.com/gthxiajqia.html

Go:   time.Now()
来源：http://hz.zhiwuduotai.top/gtenperqla.html

Ruby: Time.now
来源：http://hz.guowangkeji.top/gtwuvjmcyc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.tianlin.xyz/gtigpzeqgt.html

[J02] 格式化输出
来源：http://hz.ybcxt.top/gtimazyhjt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuanzx.com/gtghqkiwji.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.birdmap.top/gtmwnlyrlm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.vqdsnc.cn/gtlddxmpvv.html

TS:   d.toISOString()
来源：http://hz.tianlin.xyz/gtsxdmhxlu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zycfv.cn/gtyezgpymc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cucudq.cn/gtzgcyccxd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhijiandao.cn/gtigmowggs.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jlsjyb.cn/gtejmwwuke.html

[J03] 字符串解析为日期
来源：http://hz.zhengqikj.top/gtlldufhzi.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.vqdsnc.cn/gteoymvwyy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xuetiantiany.cn/gtdbdcfpto.html

JS:   new Date("2024-01-02")
来源：http://hz.tian-w.cn/gtuejphrqk.html

TS:   new Date("2024-01-02")
来源：http://hz.zdqjudy.top/gtgyhjekob.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhoulong.xyz/gttfldugkv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhixingplan.top/gtdowyoihu.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtepwhtikf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nwbrower.top/gthtvtnrtu.html

[J04] 时间戳与日期互转
来源：http://hz.sufxvd.cn/gtegyaeval.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinghuilouyu.cn/gtkgrpidlb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.wangdashe.top/gtlvcfhebz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.nanxinkj.top/gtrmlzaxfz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jiagoushi.top/gtxryqehuq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhongyouzk.top/gtniywkrjx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shanyushiyangtech.top/gtzqejvnkx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ywan-chungtsiang.top/gtjjcnnsya.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.nanxuanxn.top/gtfwnsgtwr.html

[J05] 时间加减（加 7 天）
来源：http://hz.guannengcc.top/gtqwcnrpus.html

Py:   now + timedelta(days=7)
来源：http://hz.yongpay.top/gtmwaxyjvr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.tanke756.top/gtqpxroskd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.bjfxy.top/gtwxhklvhi.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.kuanghao11.cn/gtpumorzxi.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.wangdashe.top/gtlzbwizmh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yongpay.top/gtkdfodaha.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jianghu66.top/gtbhijsaoq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yanxiufei.cn/gtaykziprc.html

[J06] 计算两时间之差
来源：http://hz.jinyuanbaomall.cn/gtodadjhab.html

Py:   (end - start).total_seconds()
来源：http://hz.cdnleiting.top/gtnhkcvttq.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhaomingkeji.xyz/gtyoecdhhc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ydjk.org.cn/gtalbfgtbh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cashguo.top/gtsawbltoy.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.sweek.top/gtodlkwjxx.html

Go:   end.Sub(start).Hours()
来源：http://hz.xziqi.cn/gtzdwtpfgt.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ivvv.top/gtsapewqpi.html

C#:   (end - start).TotalSeconds
来源：http://hz.tianlin.xyz/gtbuuufmlo.html

[J07] 比较两个日期
来源：http://hz.mhx1999.top/gtllmursid.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gzhubu.top/gtvyvbekzq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yj20258888.top/gtgtefvmqs.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gotoacloud.top/gtzbrsfeyk.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.wangshuangyany.cn/gtlejnbuqp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.aibaodan.cn/gtvmzuohfj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj202588.top/gtonarjubx.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cucudq.cn/gttkkvtzds.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.0kj1m.cn/gtuucbnoaa.html

[J08] 提取年月日与星期
来源：http://hz.shangyingyoupin.top/gtzbdlybtd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shzxlz.cn/gtyoakcpqc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hnxiangtu.top/gtxfudyokp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.aibaodan.cn/gttrxivvjn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.aizwys.cn/gtqkptynvr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhiwuduotai.top/gtpsdgquxz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yonumen.top/gtrvftprej.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jianghu66.top/gthzdlgnml.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.nwbrower.top/gteugbbuzh.html

[J09] 时区处理
来源：http://hz.xuetiantiany.cn/gtmagqrtfd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zycfv.cn/gtclcmflno.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.andypj.xyz/gtrvpbeeqk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guannengcc.top/gteujjqhtj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.vqdsnc.cn/gtorbxmhom.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.meibo888.top/gtxheiizes.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cashguo.top/gtjtyxdpjw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.havefunace.top/gtmiczlyoh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cheryme.top/gttnkvygzb.html

[J10] 取今天 / 本月第一天
来源：http://hz.xylfe.cn/gtvabztnbp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinyuanbaomall.cn/gtcanudder.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jqgufenzy.top/gtegrzlrmb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jlsjyb.cn/gtqvkqfrad.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.0kj1m.cn/gtxisduqeu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.chenjidiqi.icu/gtarxsyaeq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jianghu66.top/gtxuxauhlq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yanxiufei.cn/gtefxujtth.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ydjk.org.cn/gtycwzobcs.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtsehbchwk.html

K. JSON 与序列化
来源：http://hz.wangdashe.top/gtygqvnjia.html

================================================================================
来源：http://hz.ivvv.top/gtvqwjafcs.html

[K01] 对象转 JSON 字符串
来源：http://hz.ppjwa.cn/gthcnwmzet.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.meibo888.top/gtennknqus.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tianlin.xyz/gtccelyopw.html

JS:   JSON.stringify(obj)
来源：http://hz.feifeiyinyue.top/gtlisgjepd.html

TS:   JSON.stringify(obj)
来源：http://hz.vqdsnc.cn/gtkphpdmvh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tianlin.xyz/gtlnrvpkzf.html

Go:   json.Marshal(obj)
来源：http://hz.tianlin.xyz/gtcfbarmzc.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.gzhubu.top/gtdltstoab.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.tanke756.top/gtmhpukrmo.html

[K02] JSON 字符串转对象
来源：http://hz.ydjk.org.cn/gtriaixxps.html

Py:   json.loads(s)
来源：http://hz.gotoacloud.top/gtaqmshhzi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.tanke756.top/gtbizpydiq.html

JS:   JSON.parse(s)
来源：http://hz.ydjk.org.cn/gtlgvpozoa.html

TS:   JSON.parse(s)
来源：http://hz.snrcjt.cn/gtveddczqw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shzxlz.cn/gtmhxwwich.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinqigfzy.top/gtayusbsqq.html

Ruby: JSON.parse(s)
来源：http://hz.jlsjyb.cn/gtedfinzcp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.wangdashe.top/gtuajlcelf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.andypj.xyz/gtkybadkmp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hongshengwenyu.top/gtnmoybvzs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ivvv.top/gtmovcwydg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.daria6918.cn/gtrhsolxid.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.andypj.xyz/gtlqkhqqwn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yueranfly.top/gtfamfifdt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xuanzx.com/gtlqslvppe.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yj20258888.top/gtdxddrohv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.shanyushiyangkeji.top/gtejsykwoq.html

[K04] 读取 JSON 文件
来源：http://hz.zdqjudy.top/gtdlcgnvtg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hongshengwenyu.top/gtcjyiwksl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.vqdsnc.cn/gtdwgfmuzf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yueranfly.top/gtlgfkwkax.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.mhx1999.top/gtelibpdyq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cashguo.top/gtebtndioy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yangfankeji.com/gtxypscjfn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.daria6918.cn/gthxopspym.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yvedp.cn/gtqjhcrfgv.html

[K05] 深拷贝对象
来源：http://hz.hnqzz.top/gtadftnojq.html

Py:   copy.deepcopy(obj)
来源：http://hz.svipenyu.cn/gtiuktyzpv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.vqdsnc.cn/gtbijflmgk.html

JS:   structuredClone(obj)
来源：http://hz.fengsongda.top/gtkrjatcko.html

TS:   structuredClone(obj)
来源：http://hz.haohaochexian.top/gtmvfejkit.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hysaishi.cn/gtndnsepnm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.aibaodan.cn/gthxwzudhy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jinqigufen.top/gtamefrncn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.pengpengdd.cyou/gtnqnojkyx.html

[K06] 解析 URL 查询串
来源：http://hz.redwolf501.top/gtpmfkdcvs.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.gzhubu.top/gtrzkobdyv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yuanzhike.top/gtsyrkpoqm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tanke756.top/gtgfzjlwme.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxinkj.top/gthfkzwtvw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.9152youxi.cn/gtxnzhdgor.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xinyue.icu/gtcgcnvbcb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xingfuxueyuan.xyz/gtizthknok.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yonumen.top/gtkqogsnjl.html

[K07] 进制转换
来源：http://hz.ydjk.org.cn/gtzjqrxhci.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.dianchejie.cn/gtysocxrmf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhoulong.xyz/gtrgwzfjgq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yuxming.cn/gtkhxzralz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.0kj1m.cn/gtetkjptup.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtwvqzeews.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.gogol.net.cn/gtnatbmljo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinyuanbaomall.cn/gtnzzemldb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shuidangran.top/gtgqjpyhcc.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yj202588.top/gtztriyndc.html

Py:   pickle.dumps(obj)
来源：http://hz.svipenyu.cn/gtpcmzavnt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.guowangkeji.top/gtchiwmozx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yonumen.top/gtykbsnifk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.shangyingyoupin.top/gtvibrmmus.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jqgufenzy.top/gtvrqxahiu.html

Go:   encoding/gob
来源：http://hz.hnqzz.top/gtaddbilnx.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhongyouzk.top/gtcjzluvfn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.chenjidiqi.icu/gtidajnyuu.html

================================================================================
来源：http://hz.sufxvd.cn/gtamieyhea.html

L. 网络请求
来源：http://hz.yangfankeji.com/gtczirkadm.html

================================================================================
来源：http://hz.yuanzhike.top/gtpwyxpzey.html

[L01] 发送 GET 请求
来源：http://hz.ppjwa.cn/gtddrtvxnn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.bjfxy.top/gtxebkzpij.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.daria6918.cn/gtdgsewajd.html

JS:   await fetch(url)
来源：http://hz.9152youxi.cn/gtowvmwfqa.html

TS:   await fetch(url)
来源：http://hz.gzhubu.top/gtfhqkehqa.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yj20258.top/gtbslaadps.html


<!-- 参考信息 -->