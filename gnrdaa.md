代发 wailian999

Py:   value = d.get("k") or default
来源：http://hz.hnxiangtu.top/gtktjnsvrs.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yangfankeji.com/gtipnrheim.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ivvv.top/gtadmtrzjt.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.fengsongda.top/gtbpoglyte.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jiagoushi.top/gtrhznaksw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.guannengcc.top/gtypsnfpca.html

Ruby: d&.dig(:a, :b)
来源：http://hz.0kj1m.cn/gthqheztti.html

C#:   obj?.A?.B ?? default
来源：http://hz.dianchejie.cn/gtzaoyegii.html

[H07] 断言
来源：http://hz.quarkkingdee.top/gtqbhuzemk.html

Py:   assert x > 0, "必须为正"
来源：http://hz.nanxuanxn.top/gtfbyxxfdh.html

PHP:  assert($x > 0);
来源：http://hz.dashuyun.cn/gtpfijkuqd.html

JS:   console.assert(x > 0);
来源：http://hz.cheryme.top/gtgyerjpsn.html

TS:   console.assert(x > 0);
来源：http://hz.smart0.xyz/gtrhjdykyf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hysaishi.cn/gtubkzjpiq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.andypj.xyz/gtdmgcdxno.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.316326.xyz/gtcwuhlufz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.havefunace.top/gteendxlco.html

[H08] 获取错误信息与堆栈
来源：http://hz.ydjk.org.cn/gtqezteezv.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.daxiang520.top/gtwqaatdrf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yuxming.cn/gtxajdekxk.html

JS:   e.message;  e.stack
来源：http://hz.chenlongwang.top/gtedypqirs.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhoulong.xyz/gtkyhrenqa.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cqqwz.cn/gtbsatzfki.html

Go:   err.Error()
来源：http://hz.havefunace.top/gtyjkvalap.html

Ruby: e.message;  e.backtrace
来源：http://hz.xinyue.icu/gtvnqfuuwt.html

C#:   e.Message;  e.StackTrace
来源：http://hz.bjfxy.top/gtzrbqwmji.html

[H09] 带错误码的异常
来源：http://hz.fengsongda.top/gtuwezgsdx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.wangdashe.top/gtcpczvhqx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinqigfzy.top/gtuagubwtl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.tanke756.top/gteoiddvym.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cucudq.cn/gtnafzxivd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhixingplan.top/gtocwxfsat.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yuxming.cn/gtievkkfyf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xylfe.cn/gtouiydrjp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yvedp.cn/gtpvpeurab.html

[H10] 资源自动释放
来源：http://hz.nwbrower.top/gtvmmkxqde.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.birdmap.top/gtpchemyyz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.nwbrower.top/gtdfsqmrqf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sysykeji.top/gtpfbzgglx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.pengpengdd.cyou/gtwjqqpbku.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sysykeji.top/gtdqxhskhv.html

Go:   defer f.Close()
来源：http://hz.xuanzx.com/gtijmqmpjs.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.dashuyun.cn/gtxbpughlz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hammf.cn/gtbsvjmfvd.html

================================================================================
来源：http://hz.zhoulong.xyz/gtmsxbaovh.html

I. 正则表达式
来源：http://hz.0kj1m.cn/gtmtjwxbbf.html

================================================================================
来源：http://hz.redwolf501.top/gtarnvjmxk.html

[I01] 判断是否匹配
来源：http://hz.wangdashe.top/gtrcituqxg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jyoumei.cn/gtlijiwahh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zdqjudy.top/gtjilqqrsb.html

JS:   /\d+/.test(s)
来源：http://hz.jinghuilouyu.cn/gtncttfipt.html

TS:   /\d+/.test(s)
来源：http://hz.wangdashe.top/gtzzssmits.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.haohaochexian.top/gteybqdhfk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cucudq.cn/gthzybpeuo.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhiwuduotai.top/gtplxsfqug.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.feifeiyinyue.top/gtpbrmwrhh.html

[I02] 提取所有匹配
来源：http://hz.yueranfly.top/gtllvlkzsg.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yuanzhike.top/gtmcgizjfr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.chenlongwang.top/gtjgugvwtt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cucudq.cn/gtbbfirxlt.html

TS:   s.match(/\d+/g)
来源：http://hz.guannengcc.top/gtclindzeb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.feifeiyinyue.top/gtmwskvfbl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cucudq.cn/gtjykcabgp.html

Ruby: s.scan(/\d+/)
来源：http://hz.svipenyu.cn/gtrhplrmjh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yonumen.top/gtrgueerpu.html

[I03] 提取捕获分组
来源：http://hz.yj20258888.top/gtcifzrbwy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nanxinkj.top/gtpxvcbavd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yueranfly.top/gtgznaoaqc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xuetiantiany.cn/gtldrpgsnb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shanyushiyangkeji.top/gturyuhlrl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hnxiangtu.top/gtkjisgsgo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xylfe.cn/gtqfcloxds.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.c1oappe.top/gtwbuliauh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jinqigfzy.top/gtbbvtkkyl.html

[I04] 正则替换
来源：http://hz.guowangkeji.top/gtpfbkzrtv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.pengpengdd.cyou/gtfupofpbi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhengqikj.top/gttypknzks.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ywan-chungtsiang.top/gtvqtxugny.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258888.top/gtyndonnkc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.shangyingyoupin.top/gtpwjjehbw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yonumen.top/gtvhhzdlks.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hysaishi.cn/gtnuymxura.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nanxuanxn.top/gtvxrtgmja.html

[I05] 按正则拆分
来源：http://hz.dianchejie.cn/gtrqowppjo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.havefunace.top/gtidyticvc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.316326.xyz/gtsdmqybhm.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gzhubu.top/gtyyotlkyd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ppjwa.cn/gtzwxhbjaq.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhiwuduotai.top/gthflfnnsp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.cdnleiting.top/gtcqwcuykc.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.cheryme.top/gtdswwtuod.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hnxiangtu.top/gtfhssbwia.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.andypj.xyz/gtaqxscopn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gtfrzxolep.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hnxiangtu.top/gtaizhjfvi.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xylfe.cn/gtwlvponzz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xuetiantiany.cn/gtuwpqvwwz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.iojbl.cn/gtrgrekgqa.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.wangdashe.top/gtyfilhrzv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.chenlongwang.top/gtcgcvvxwa.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.pycfn.com/gtejpaxrgd.html

[I07] 忽略大小写与多行模式
来源：http://hz.svipenyu.cn/gtlsokvbnk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yonumen.top/gtotrxenwv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xingfuxueyuan.xyz/gtplqpzlfr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xylfe.cn/gtrmsufxjl.html

TS:   /error/gim
来源：http://hz.cucudq.cn/gtgshmxclw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hfpthk.cn/gtstgevebn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.svipenyu.cn/gtwnccqdjq.html

Ruby: s.scan(/error/i)
来源：http://hz.yonumen.top/gtvuqktlbc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jianghu66.top/gtthezjexi.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhiwuduotai.top/gtuxovqxtx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jyoumei.cn/gtjymjpbly.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.feifeiyinyue.top/gtdaddacaa.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aizwys.cn/gtdtrlbscp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xylfe.cn/gtzfdbbbvr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.snrcjt.cn/gtpntepnqp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gogol.net.cn/gthwjnhxdj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.feifeiyinyue.top/gtopacqnev.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gaohongyu789.top/gtopymetqk.html

================================================================================
来源：http://hz.316326.xyz/gtxcskzoor.html

J. 日期与时间
来源：http://hz.yuxming.cn/gtwecerptk.html

================================================================================
来源：http://hz.guannengcc.top/gtupqbumya.html

[J01] 获取当前时间
来源：http://hz.iojbl.cn/gtztpkvozo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hysaishi.cn/gtpswqfecd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jinqigfzy.top/gtpnwhvnui.html

JS:   new Date();  Date.now()
来源：http://hz.gotoacloud.top/gtkzlslwku.html

TS:   new Date();  Date.now()
来源：http://hz.ybcxt.top/gtttncnnfe.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yj20258888.top/gtviyftrcf.html

Go:   time.Now()
来源：http://hz.jqgufenzy.top/gtfxuqlolz.html

Ruby: Time.now
来源：http://hz.xuanzx.com/gtpmnchpja.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shangyingyoupin.top/gtaibslrbm.html

[J02] 格式化输出
来源：http://hz.jqgufenzy.top/gtenqmkzjd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.52xcode.cn/gtpfycazpl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shangyingyoupin.top/gtpxqhheor.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jiagoushi.top/gtckwnsodp.html

TS:   d.toISOString()
来源：http://hz.jlsjyb.cn/gtsiphvchq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.pycfn.com/gtfljcblgi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.kuanghao11.cn/gtfhvvjbwb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gzhubu.top/gtaijdojof.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zdqjudy.top/gtogjxdexf.html

[J03] 字符串解析为日期
来源：http://hz.nanxuanxn.top/gtwhkskyre.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.aibaodan.cn/gtccypbxsa.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cqqwz.cn/gtuttvciwa.html

JS:   new Date("2024-01-02")
来源：http://hz.daria6918.cn/gtndwmrpxx.html

TS:   new Date("2024-01-02")
来源：http://hz.kuanghao11.cn/gtaqcgtgqw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jinqigufen.top/gtscnenalu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hfpthk.cn/gteqrimcky.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.52xcode.cn/gtrjwklqms.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sxryk.cn/gtjiqwwihi.html

[J04] 时间戳与日期互转
来源：http://hz.ywan-chungtsiang.top/gtbfblanaw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.tian-w.cn/gtrlitdund.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.0kj1m.cn/gttuvdoijh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinqigfzy.top/gtvfkalohm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zdqjudy.top/gtamrvxvsy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cucudq.cn/gtgapusfmv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.bjfxy.top/gtjckfrigb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.wangdashe.top/gtypzeqlzd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.fengsongda.top/gtblxhggjk.html

[J05] 时间加减（加 7 天）
来源：http://hz.yj20258888.top/gtetrycmha.html

Py:   now + timedelta(days=7)
来源：http://hz.svipenyu.cn/gtsjnytyvr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yvedp.cn/gtdggutspw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenlongwang.top/gtghkkqoau.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.quarkkingdee.top/gtrcyyyxga.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shanyushiyangtech.top/gtfaygljoo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.redwolf501.top/gtksuopsob.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhengqikj.top/gtaqsyrjrs.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.mhx1999.top/gtubynvefa.html

[J06] 计算两时间之差
来源：http://hz.yvedp.cn/gtvnkohokm.html

Py:   (end - start).total_seconds()
来源：http://hz.yvedp.cn/gtvvbjngfy.html

PHP:  $end->diff($start)->days;
来源：http://hz.hammf.cn/gtrmcvklje.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xziqi.cn/gtjgjleska.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yongpay.top/gtsprxbxnf.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.9152youxi.cn/gthksyzpck.html

Go:   end.Sub(start).Hours()
来源：http://hz.wangshuangyany.cn/gtuqfgltbi.html

Ruby: end - start                 # 返回秒数
来源：http://hz.birdmap.top/gtohnvobog.html

C#:   (end - start).TotalSeconds
来源：http://hz.jyoumei.cn/gtaknjhrqd.html

[J07] 比较两个日期
来源：http://hz.gzhubu.top/gtotinglzv.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gtujpwtxji.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hysaishi.cn/gtzmucnpxm.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jianghu66.top/gthkqyaetx.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.fengsongda.top/gtvuaxmxtu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.quarkkingdee.top/gtjvihcgpy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.dashuyun.cn/gtzznqiyju.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jiagoushi.top/gtatlzqihy.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.nanxinkj.top/gtvipljgjf.html

[J08] 提取年月日与星期
来源：http://hz.tanke756.top/gtdxncyrbe.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shzxlz.cn/gtytduwzcw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.dianchejie.cn/gtutrqkzwj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hysaishi.cn/gtjhblidlm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.guowangkeji.top/gtcwmrzxfq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.andypj.xyz/gtmtqxihae.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.gaohongyu789.top/gtkgzrrlws.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yj202588.top/gtgbqfnqzt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.redwolf501.top/gtzxjbffga.html

[J09] 时区处理
来源：http://hz.hnqzz.top/gtmxjthikg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ydzc1.top/gthbyocnmu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.nwbrower.top/gtrrrcflmb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jiagoushi.top/gtwdatsfpx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gzhubu.top/gtxyljzoix.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nwbrower.top/gtlengbkat.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.quarkkingdee.top/gtwycvkizj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yongpay.top/gtodsvsknr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yuxming.cn/gtfhxsypao.html

[J10] 取今天 / 本月第一天
来源：http://hz.jqgufenzy.top/gtwmcqgyfg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cqqwz.cn/gtabgxojts.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.gaohongyu789.top/gtfjogrnnp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ydzc1.top/gtpsxakqmb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yj20258.top/gttejpvhaj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yuanzhike.top/gtjdlhcweu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.dashuyun.cn/gttabprafd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ydzc1.top/gtsvllfrwq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.fzhhl.top/gtrkmdeoab.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtchanktvy.html

K. JSON 与序列化
来源：http://hz.gaohongyu789.top/gtfthrevam.html

================================================================================
来源：http://hz.gaohongyu789.top/gtfkboheml.html

[K01] 对象转 JSON 字符串
来源：http://hz.nwbrower.top/gtkkwtceem.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yongpay.top/gtjrpykbpa.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhixingplan.top/gtigxeifkh.html

JS:   JSON.stringify(obj)
来源：http://hz.cucudq.cn/gtobnfpaie.html

TS:   JSON.stringify(obj)
来源：http://hz.gogol.net.cn/gtmscmdnpg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.dashuyun.cn/gtoignuvsz.html

Go:   json.Marshal(obj)
来源：http://hz.gogol.net.cn/gtpzdakolx.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinqigufen.top/gtzscmigvb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.daria6918.cn/gtgmaokfbs.html

[K02] JSON 字符串转对象
来源：http://hz.mhx1999.top/gtiyjuozuf.html

Py:   json.loads(s)
来源：http://hz.ywan-chungtsiang.top/gtwhqhwbmf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.tanke756.top/gtgbuikjaw.html

JS:   JSON.parse(s)
来源：http://hz.cqqwz.cn/gtxhyzxouz.html

TS:   JSON.parse(s)
来源：http://hz.chenjidiqi.icu/gtdimpylgb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jlsjyb.cn/gtghyozhsb.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.havefunace.top/gtigvkjvdf.html

Ruby: JSON.parse(s)
来源：http://hz.xingfuxueyuan.xyz/gtakcfdbyv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gaohongyu789.top/gtjfjtwewx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhengqikj.top/gtfcxzhjrp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ivvv.top/gtlukzksyq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hongshengwenyu.top/gtjvzjcvij.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.pengpengdd.cyou/gtlgsbbbhb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.feifeiyinyue.top/gtrsyolciv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.iojbl.cn/gteadgkqwm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.birdmap.top/gtuavnsusy.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.haohaochexian.top/gtjipbyxdi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hnqzz.top/gtixvsqokc.html

[K04] 读取 JSON 文件
来源：http://hz.aibaodan.cn/gtchlpafkc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.havefunace.top/gtsbncpxpr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hongshengwenyu.top/gtkvetyauv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.0kj1m.cn/gtrkqzfbyt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guannengcc.top/gtcsuxxrai.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.chenjidiqi.icu/gtodbbqqsi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.haohaochexian.top/gtkqqvsgzp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.redwolf501.top/gtbiqzkgck.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.316326.xyz/gttguzavcd.html

[K05] 深拷贝对象
来源：http://hz.havefunace.top/gtoigbeqdm.html

Py:   copy.deepcopy(obj)
来源：http://hz.ybcxt.top/gtmvlqzott.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jianghu66.top/gticpxghnc.html

JS:   structuredClone(obj)
来源：http://hz.sysykeji.top/gtegtmilqo.html

TS:   structuredClone(obj)
来源：http://hz.sysykeji.top/gtuzbmxfxd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shangyingyoupin.top/gtuddpwypz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.9152youxi.cn/gtibpphdfs.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jinyuanbaomall.cn/gturbmjuax.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.daria6918.cn/gtflepfnzd.html

[K06] 解析 URL 查询串
来源：http://hz.shanyushiyangkeji.top/gtcvzgsqjs.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.tanke756.top/gtckgxxyky.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.daria6918.cn/gtfhrevila.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xinyue.icu/gtjtareggk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.52xcode.cn/gtymqqpmzi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sufxvd.cn/gtyelodsdm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.fengsongda.top/gtyyfdxknu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.wangdashe.top/gtztbbligj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sweek.top/gteacwglsu.html

[K07] 进制转换
来源：http://hz.52xcode.cn/gtizucewoq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.pengpengdd.cyou/gttewcacvt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cdnleiting.top/gtrixlngyf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.vqdsnc.cn/gtbbpfahzb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.andypj.xyz/gtqryzizje.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hywenlv.cn/gttejcedoi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.meibo888.top/gtdipljbvr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhixingplan.top/gteqxumvom.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jyoumei.cn/gtdtkvkhyx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yangfankeji.com/gtxrimgmvi.html

Py:   pickle.dumps(obj)
来源：http://hz.jyoumei.cn/gtnpayoyts.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.svipenyu.cn/gtzptjvrqm.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jqgufenzy.top/gtbmrwoajp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xingfuxueyuan.xyz/gtskuukppy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhoulong.xyz/gttzhydbjz.html

Go:   encoding/gob
来源：http://hz.hnxiangtu.top/gtcdehbjtt.html

Ruby: Marshal.dump(obj)
来源：http://hz.cqqwz.cn/gtqzxnaigg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.chenzaomai.com/gtvnbleqtb.html

================================================================================
来源：http://hz.tianlin.xyz/gtidpmzeho.html

L. 网络请求
来源：http://hz.sxryk.cn/gtxobdcyar.html

================================================================================
来源：http://hz.xinyue.icu/gtylgvvpoj.html

[L01] 发送 GET 请求
来源：http://hz.xingfuxueyuan.xyz/gtwwzyekms.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.shangyingyoupin.top/gtyslskpqu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.iojbl.cn/gtqxjwjkhw.html

JS:   await fetch(url)
来源：http://hz.zhijiandao.cn/gtsnjzhjee.html

TS:   await fetch(url)
来源：http://hz.yvedp.cn/gttimsrwwl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yongpay.top/gtgbqypnbo.html

Go:   resp, err := http.Get(url)
来源：http://hz.chenjidiqi.icu/gtoftlbxto.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.pycfn.com/gtokecdzhq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hnqzz.top/gtrwgmfvuk.html

[L02] 发送 POST JSON
来源：http://hz.kuanghao11.cn/gtzbjbtehy.html


<!-- 参考信息 -->