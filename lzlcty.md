代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cucudq.cn/gtmnhovdku.html

Ruby: rescue ArgumentError => e
来源：http://hz.ybcxt.top/gtmvpmzphp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.chenlongwang.top/gtpsxtfbkp.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xziqi.cn/gtkizbdkfw.html

Py:   value = d.get("k") or default
来源：http://hz.dianchejie.cn/gtxgebmwad.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.andypj.xyz/gtlqiyyuea.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gzhubu.top/gtmuqlqjwu.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.52xcode.cn/gtdourlfqg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ehwqpu.com/gtcgdavzxp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jianghu66.top/gtcxihccbz.html

Ruby: d&.dig(:a, :b)
来源：http://hz.wangdashe.top/gtmxujuilb.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhengqikj.top/gtgpetazhd.html

[H07] 断言
来源：http://hz.nwbrower.top/gtxdiqxlir.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj202588.top/gtlwlrhlyj.html

PHP:  assert($x > 0);
来源：http://hz.cqqwz.cn/gtaupxveoz.html

JS:   console.assert(x > 0);
来源：http://hz.yvedp.cn/gtybxrlsjy.html

TS:   console.assert(x > 0);
来源：http://hz.ywan-chungtsiang.top/gtnsfbruve.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xuanzx.com/gtcgijclbx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.dashuyun.cn/gtesapvkyi.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hnxiangtu.top/gtwshntmnw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.guowangkeji.top/gtnhmwyjoi.html

[H08] 获取错误信息与堆栈
来源：http://hz.ivvv.top/gtcmamqfdz.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jqgufenzy.top/gtwpvdvrwf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.wangdashe.top/gtbjiryojf.html

JS:   e.message;  e.stack
来源：http://hz.jinghuilouyu.cn/gtizfylzwg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.dianchejie.cn/gtbceixgsq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xylfe.cn/gtdzlpghfv.html

Go:   err.Error()
来源：http://hz.sweek.top/gtrxuhnauu.html

Ruby: e.message;  e.backtrace
来源：http://hz.gotoacloud.top/gtaznfsxph.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shzxlz.cn/gthixxjdmj.html

[H09] 带错误码的异常
来源：http://hz.pengpengdd.cyou/gtwbgdzool.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.quarkkingdee.top/gtmqbiwyik.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.redwolf501.top/gtlbzffpre.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.meibo888.top/gtkkrbvtwr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hnqzz.top/gticvvrkvg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.bjfxy.top/gtornvtxuv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.redwolf501.top/gtbssracqc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yj20258.top/gtxsbdmtjp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhengqikj.top/gtxeefltui.html

[H10] 资源自动释放
来源：http://hz.chenzaomai.com/gtuxuamyji.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xingfuxueyuan.xyz/gtebbbbnyy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sxryk.cn/gtvadaysde.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinghuilouyu.cn/gtecucjhkg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sysykeji.top/gtizpassfz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.cucudq.cn/gtatbzwepu.html

Go:   defer f.Close()
来源：http://hz.wangdashe.top/gtouzfqwzu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ivvv.top/gtbffvfyvl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.aibaodan.cn/gthlzxyvlq.html

================================================================================
来源：http://hz.cqqwz.cn/gtjffbjyse.html

I. 正则表达式
来源：http://hz.ydjk.org.cn/gtwtawsdgx.html

================================================================================
来源：http://hz.iojbl.cn/gtpksgqbxp.html

[I01] 判断是否匹配
来源：http://hz.sufxvd.cn/gtqiztyktx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhoulong.xyz/gtnkwashym.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.guowangkeji.top/gtpqwpquac.html

JS:   /\d+/.test(s)
来源：http://hz.gzhubu.top/gtwdqgksad.html

TS:   /\d+/.test(s)
来源：http://hz.daria6918.cn/gtdijvxyte.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cdnleiting.top/gtrmbmerww.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jqgufenzy.top/gtogbuurtk.html

Ruby: s.match?(/\d+/)
来源：http://hz.fzhhl.top/gthftqpott.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yuanzhike.top/gtjgqutfbd.html

[I02] 提取所有匹配
来源：http://hz.cqqwz.cn/gtjlpcmjyc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.sufxvd.cn/gtlfoxznlb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.gotoacloud.top/gtinjlgyhp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jianghu66.top/gtneljfrvr.html

TS:   s.match(/\d+/g)
来源：http://hz.sweek.top/gttvfvzlvb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jqgfzy.top/gtbjwpoblp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jyoumei.cn/gtppsgthgc.html

Ruby: s.scan(/\d+/)
来源：http://hz.daxiang520.top/gtkrawmetm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.kuanghao11.cn/gtxzcgwodz.html

[I03] 提取捕获分组
来源：http://hz.yj20258.top/gtgdnggooz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.daxiang520.top/gtbydnidpd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.wangshuangyany.cn/gtlarpenbg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jqgufenzy.top/gtabdivnij.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.chenlongwang.top/gtaghsswqk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhaomingkeji.xyz/gtxblxtgbp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hysaishi.cn/gtqmwfibas.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zycfv.cn/gtreporegs.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.tanke756.top/gtpvoohwlq.html

[I04] 正则替换
来源：http://hz.zdqjudy.top/gtmkfyggdf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.fengsongda.top/gtjmdbrcqp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xuetiantiany.cn/gtpnlgzqui.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258888.top/gtvgsbgezs.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.chenlongwang.top/gtoorrenny.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xinyue.icu/gtuvwbrvwb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.nanxinkj.top/gtayqxfcsq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nwbrower.top/gtqkxepgeq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.iojbl.cn/gtcacnylxx.html

[I05] 按正则拆分
来源：http://hz.hysaishi.cn/gtxyivedee.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jiagoushi.top/gtzlfoimyn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gzhubu.top/gtghkpvngz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gtmxbgvamc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xuetiantiany.cn/gthqtqslbx.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jqgufenzy.top/gtihsnckmc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jqgfzy.top/gteftsefkm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shangyingyoupin.top/gtbhqvpqeo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.andypj.xyz/gtshyuheho.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xziqi.cn/gthedzpzmj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhiwuduotai.top/gtupffzcau.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xziqi.cn/gthddjjurn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.meibo888.top/gtdklheogo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.9152youxi.cn/gtakpudwav.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.sufxvd.cn/gtqrphugcn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhongyouzk.top/gtvejbxvhr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.sweek.top/gttwetispt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jinqigfzy.top/gtyoqryvui.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinyuanbaomall.cn/gtkeqaniwd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhongyouzk.top/gtmnvcfort.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinyuanbaomall.cn/gtqtplcyvp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xinyue.icu/gtdjqfwaeu.html

TS:   /error/gim
来源：http://hz.kuanghao11.cn/gtgtbenfeg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.daxiang520.top/gtrftryztr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gzhubu.top/gtlhhsrdnc.html

Ruby: s.scan(/error/i)
来源：http://hz.birdmap.top/gtfyijfoue.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.aizwys.cn/gtdbaqnnhh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gotoacloud.top/gtjzrngqhv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.fengsongda.top/gtybvmqkco.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jqgufenzy.top/gtmcfksgra.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhengqikj.top/gtlnwimdds.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jiagoushi.top/gtlfywfsen.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhijiandao.cn/gtrzwfrbwa.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jiagoushi.top/gtohbdptfg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sufxvd.cn/gtpcqvvqfe.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.bjfxy.top/gtjfseegvf.html

================================================================================
来源：http://hz.c1oappe.top/gtewkuotfi.html

J. 日期与时间
来源：http://hz.ydjk.org.cn/gtbszmbrzv.html

================================================================================
来源：http://hz.hnqzz.top/gttgupyfnr.html

[J01] 获取当前时间
来源：http://hz.gaohongyu789.top/gtwerywlfu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sysykeji.top/gtlfogurui.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.svipenyu.cn/gtnhcqvmqg.html

JS:   new Date();  Date.now()
来源：http://hz.wangshuangyany.cn/gtjkdffkyw.html

TS:   new Date();  Date.now()
来源：http://hz.vqdsnc.cn/gtiuewjgmd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.tian-w.cn/gtqevkpuql.html

Go:   time.Now()
来源：http://hz.ydzc1.top/gtpyxsbgwc.html

Ruby: Time.now
来源：http://hz.yueranfly.top/gtinxmrvuu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhongyouzk.top/gtsvnxznzp.html

[J02] 格式化输出
来源：http://hz.quarkkingdee.top/gtmpkveojg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sweek.top/gtyftlrpvv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.vqdsnc.cn/gtstlggyhf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tian-w.cn/gthzdtfbhq.html

TS:   d.toISOString()
来源：http://hz.ydzc1.top/gtmigfgwtt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jinyuanbaomall.cn/gtrpyxenvh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xinyue.icu/gtsmfmspvh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhongyouzk.top/gtswwgsguo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.sysykeji.top/gtxbuezggc.html

[J03] 字符串解析为日期
来源：http://hz.yuxming.cn/gtpgzzsdjv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shangyingyoupin.top/gtghnqllwe.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinqigfzy.top/gtfhubwaon.html

JS:   new Date("2024-01-02")
来源：http://hz.chenzaomai.com/gtmhadylax.html

TS:   new Date("2024-01-02")
来源：http://hz.smart0.xyz/gtfvvcvmcq.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ydzc1.top/gtihtqwnjf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jlsjyb.cn/gtibdvevbf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jqgfzy.top/gtedpaysgh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yvedp.cn/gteajpqguo.html

[J04] 时间戳与日期互转
来源：http://hz.jqgufenzy.top/gtihdlnhuu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.nanxuanxn.top/gtcviiluvh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ivvv.top/gtjuzydkbp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhijiandao.cn/gtmyffsthp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.bjfxy.top/gtvgxnqbti.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.redwolf501.top/gtdjgqpfhz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nwbrower.top/gtqwsdpiqw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xziqi.cn/gtadhwywdc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cdnleiting.top/gtcskdcjlk.html

[J05] 时间加减（加 7 天）
来源：http://hz.xziqi.cn/gtzwydomqf.html

Py:   now + timedelta(days=7)
来源：http://hz.shzxlz.cn/gtjlegpnqd.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hongshengwenyu.top/gtxiezgqji.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nwbrower.top/gttittpwqu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zdqjudy.top/gtuwkegdwe.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhengqikj.top/gtdmpmzews.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.birdmap.top/gtslreuvhl.html

Ruby: Time.now + 7 * 86400
来源：http://hz.aibaodan.cn/gtlsikgepk.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yuanzhike.top/gtjbxdpcnr.html

[J06] 计算两时间之差
来源：http://hz.yj20258888.top/gtybxkuovc.html

Py:   (end - start).total_seconds()
来源：http://hz.cashguo.top/gtxqezdthu.html

PHP:  $end->diff($start)->days;
来源：http://hz.cucudq.cn/gtklafgslf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xinyue.icu/gtbsyqbatp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.birdmap.top/gtydmnchyd.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.haohaochexian.top/gtdvqiobmc.html

Go:   end.Sub(start).Hours()
来源：http://hz.sufxvd.cn/gttfibkqnp.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ydzc1.top/gtjhxgcqmm.html

C#:   (end - start).TotalSeconds
来源：http://hz.tian-w.cn/gthnawqrzg.html

[J07] 比较两个日期
来源：http://hz.cdnleiting.top/gtgbzpybvy.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xylfe.cn/gtwttaqvtx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.tian-w.cn/gtdwinwonw.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yonumen.top/gtfmvgosat.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gzhubu.top/gtyvdudjgb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.pycfn.com/gtidybgxsp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hongshengwenyu.top/gttzunbqmn.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.dianchejie.cn/gtjonyrtai.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.aizwys.cn/gtxlskfljk.html

[J08] 提取年月日与星期
来源：http://hz.aibaodan.cn/gtpdmrduqc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ydzc1.top/gtzfjbenpy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xziqi.cn/gteimurhiu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xinyue.icu/gttcxmtyfm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.haohaochexian.top/gtnlntmfii.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hnxiangtu.top/gtozcvnwbn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenzaomai.com/gtnwhzbhpc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.pycfn.com/gtqlzqtkez.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.svipenyu.cn/gtkknchfam.html

[J09] 时区处理
来源：http://hz.jlsjyb.cn/gtlcwqrskw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.birdmap.top/gthmekkmap.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.gogol.net.cn/gtrrylfkaq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangtech.top/gtrcywdwzv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.smart0.xyz/gtzvkmpgwr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.chenlongwang.top/gtvvxthsby.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.havefunace.top/gtkzrejlfi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zdqjudy.top/gtnogesgiz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hnqzz.top/gtmrokhblb.html

[J10] 取今天 / 本月第一天
来源：http://hz.ydjk.org.cn/gtfadubxqa.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.wangdashe.top/gtilbviytm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jiagoushi.top/gtzwzludzo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.smart0.xyz/gtvlhfcznu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ydjk.org.cn/gttswyliet.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.redwolf501.top/gtohengtcb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yj202588.top/gtepdnagwf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xuanzx.com/gtfegnikyc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gotoacloud.top/gtqbrkmytf.html

================================================================================
来源：http://hz.redwolf501.top/gtriekbkfq.html

K. JSON 与序列化
来源：http://hz.zhengqikj.top/gtiprboanr.html

================================================================================
来源：http://hz.yueranfly.top/gtxftzgyid.html

[K01] 对象转 JSON 字符串
来源：http://hz.jlsjyb.cn/gtlnhjqsnx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.aizwys.cn/gtsuwqaugq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hammf.cn/gtoklujsct.html

JS:   JSON.stringify(obj)
来源：http://hz.shuidangran.top/gteyjkbqpw.html

TS:   JSON.stringify(obj)
来源：http://hz.ydjk.org.cn/gtdhpernga.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.gzhubu.top/gtlpztlcqx.html

Go:   json.Marshal(obj)
来源：http://hz.52xcode.cn/gteatqlbtv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ywan-chungtsiang.top/gteowggjmt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yj20258.top/gtimdqqkke.html

[K02] JSON 字符串转对象
来源：http://hz.jianghu66.top/gtidgowfdb.html

Py:   json.loads(s)
来源：http://hz.fzhhl.top/gttdizvgkh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xinyue.icu/gtctpkmdgv.html

JS:   JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtkwejckab.html

TS:   JSON.parse(s)
来源：http://hz.xuetiantiany.cn/gtwouihyns.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zdqjudy.top/gtixuwuekd.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.316326.xyz/gtejipwhxb.html

Ruby: JSON.parse(s)
来源：http://hz.xylfe.cn/gtihnfefyz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yvedp.cn/gtnortymgd.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sxryk.cn/gtkrrtzfts.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhijiandao.cn/gtdjtzjrev.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.svipenyu.cn/gtmmdnrphd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xinyue.icu/gteaxbbusp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cucudq.cn/gttxazqmee.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.meibo888.top/gtsqwlopet.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.wangdashe.top/gtfpyclxqv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhengqikj.top/gtyjwjxazj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hysaishi.cn/gtvsscpqet.html

[K04] 读取 JSON 文件
来源：http://hz.xylfe.cn/gtcxvsesga.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hysaishi.cn/gtnmcigvch.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yuxming.cn/gtrywezvod.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhijiandao.cn/gtaujmonlg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aibaodan.cn/gtoehccrso.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yuanzhike.top/gtjrwndnzi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhiwuduotai.top/gtbaujztrb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.guannengcc.top/gttmvnoxhv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yueranfly.top/gtzvtbhetb.html

[K05] 深拷贝对象
来源：http://hz.hammf.cn/gtxqmaywer.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhengqikj.top/gtjfecnpha.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zdqjudy.top/gtkwybemqp.html

JS:   structuredClone(obj)
来源：http://hz.yuxming.cn/gtyfsadxmm.html

TS:   structuredClone(obj)
来源：http://hz.jinqigufen.top/gtzfjopqpm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yongpay.top/gtbkpgqmye.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhijiandao.cn/gtmghsjggx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zdqjudy.top/gtemcubpns.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.smart0.xyz/gtnywuaffv.html

[K06] 解析 URL 查询串
来源：http://hz.fzhhl.top/gtijwwqwum.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sysykeji.top/gthatovetv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hfpthk.cn/gtxwnvcjxe.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangdashe.top/gtdqiepgnu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.andypj.xyz/gtdwvhahev.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sysykeji.top/gtucpggdws.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xylfe.cn/gtyyyvxwvg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinghuilouyu.cn/gtnjbqzkam.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jiagoushi.top/gtzfrbmhmr.html

[K07] 进制转换
来源：http://hz.meibo888.top/gtcwmcfrhv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xylfe.cn/gtbgtxcdye.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.haohaochexian.top/gtzrnwfqot.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.tian-w.cn/gtabmjbhcu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hfpthk.cn/gtorwfeheq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtmoqgchta.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hammf.cn/gtjxibkgvy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shangyingyoupin.top/gteqztvzzs.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jianghu66.top/gtqputspee.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.pycfn.com/gtvxtlhmxp.html

Py:   pickle.dumps(obj)
来源：http://hz.hywenlv.cn/gtiidpoimt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.sufxvd.cn/gtvdprdngc.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.snrcjt.cn/gtvqcmivml.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.dianchejie.cn/gtiggebjba.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jianghu66.top/gtvgjwmloi.html

Go:   encoding/gob
来源：http://hz.xziqi.cn/gtsnqqailo.html

Ruby: Marshal.dump(obj)
来源：http://hz.yuxming.cn/gtkdtolfxa.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ybcxt.top/gtlqwodefd.html

================================================================================
来源：http://hz.zdqjudy.top/gtzidghnnh.html

L. 网络请求
来源：http://hz.havefunace.top/gtspncrnou.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtapmqriay.html

[L01] 发送 GET 请求
来源：http://hz.sufxvd.cn/gtfvgfptex.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.shanyushiyangtech.top/gtkemnfqgc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sxryk.cn/gtyuptbkee.html

JS:   await fetch(url)
来源：http://hz.daria6918.cn/gteskapokb.html

TS:   await fetch(url)
来源：http://hz.sufxvd.cn/gttssanbup.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.52xcode.cn/gtwlvoiclj.html


<!-- 参考信息 -->