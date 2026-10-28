代发 wailian999

[H07] 断言
来源：http://hz.jqgfzy.top/gtpealpesw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sweek.top/gtthytpnaf.html

PHP:  assert($x > 0);
来源：http://hz.guannengcc.top/gthxgoaneb.html

JS:   console.assert(x > 0);
来源：http://hz.bjfxy.top/gtivwwtrnx.html

TS:   console.assert(x > 0);
来源：http://hz.shanyushiyangkeji.top/gtiaikiwbu.html

Java: assert x > 0 : "必须为正";
来源：http://hz.mhx1999.top/gtiedspodr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hammf.cn/gtrnbawcsf.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.gzhubu.top/gtlczpnxbq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shangyingyoupin.top/gthvyfomhh.html

[H08] 获取错误信息与堆栈
来源：http://hz.smart0.xyz/gtenttpjbb.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yvedp.cn/gtfjvlxijl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yonumen.top/gtmnypyssh.html

JS:   e.message;  e.stack
来源：http://hz.jyoumei.cn/gtdhxdvphd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gzhubu.top/gtssmuqqdt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.wangshuangyany.cn/gtrdlnnqks.html

Go:   err.Error()
来源：http://hz.sxryk.cn/gtcopworxz.html

Ruby: e.message;  e.backtrace
来源：http://hz.jyoumei.cn/gtkbvqguue.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cqqwz.cn/gtrdmlsghc.html

[H09] 带错误码的异常
来源：http://hz.xuetiantiany.cn/gthqnyjndh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hysaishi.cn/gtzjrccrvb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.xuanzx.com/gtfagdsmwr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ywan-chungtsiang.top/gtgcvuvfhf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhixingplan.top/gtidlpekic.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ehwqpu.com/gtnvpxhvbm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hfpthk.cn/gttmylrror.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhaomingkeji.xyz/gthvcpnlzq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sweek.top/gtqxxwexqh.html

[H10] 资源自动释放
来源：http://hz.jqgfzy.top/gtnoqgizex.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yj20258.top/gtxgimzgdv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.c1oappe.top/gtdtejhbyu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258888.top/gtuyrfjycb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.daria6918.cn/gtuegnxggy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.cashguo.top/gtuhecjklh.html

Go:   defer f.Close()
来源：http://hz.xziqi.cn/gtgovtxtrj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.wangdashe.top/gtugjohllg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.quarkkingdee.top/gtsxltfyut.html

================================================================================
来源：http://hz.xuanzx.com/gtmthxdfnr.html

I. 正则表达式
来源：http://hz.nanxuanxn.top/gtvdwbjrvh.html

================================================================================
来源：http://hz.zdqjudy.top/gtelcxyxzs.html

[I01] 判断是否匹配
来源：http://hz.zhaomingkeji.xyz/gtshramqex.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.dashuyun.cn/gtebajkfpi.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cheryme.top/gtvzdtvxhl.html

JS:   /\d+/.test(s)
来源：http://hz.cashguo.top/gtjmdzsshl.html

TS:   /\d+/.test(s)
来源：http://hz.shzxlz.cn/gtsfdwnhdj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.aibaodan.cn/gtffsafiiw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.quarkkingdee.top/gtuntffwns.html

Ruby: s.match?(/\d+/)
来源：http://hz.yanxiufei.cn/gtkpiaokzr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.havefunace.top/gtawatwjsg.html

[I02] 提取所有匹配
来源：http://hz.ywan-chungtsiang.top/gtohzqrxyr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zdqjudy.top/gtflsetzdp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.mhx1999.top/gthqcmqdxn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xziqi.cn/gtveqqimgs.html

TS:   s.match(/\d+/g)
来源：http://hz.jlsjyb.cn/gtynnywicp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.feifeiyinyue.top/gtcxjasrej.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.redwolf501.top/gthrbgspte.html

Ruby: s.scan(/\d+/)
来源：http://hz.xziqi.cn/gtbfmayunq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jqgfzy.top/gthewiaenh.html

[I03] 提取捕获分组
来源：http://hz.jinqigfzy.top/gtrlbvlgtb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jqgfzy.top/gtozbjhvml.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xylfe.cn/gtrbwnimkb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.9152youxi.cn/gttqqzlwen.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.sysykeji.top/gtojgrdles.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yueranfly.top/gtihiwpycn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shanyushiyangkeji.top/gtnclzezey.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hnxiangtu.top/gteyiriwix.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.sufxvd.cn/gtspouhwth.html

[I04] 正则替换
来源：http://hz.sweek.top/gtpefesbqr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhoulong.xyz/gtkaqysrsl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sufxvd.cn/gtuhnwkslu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.redwolf501.top/gtetujyvbx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yuxming.cn/gtvddpwivp.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.cqqwz.cn/gtvteyshkg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.guannengcc.top/gtrmecavmn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.0kj1m.cn/gtevirfcle.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jiagoushi.top/gttosupxkh.html

[I05] 按正则拆分
来源：http://hz.aibaodan.cn/gtjdzekpsb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cucudq.cn/gtbkyqwyqk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xylfe.cn/gtmqeumcpr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hnqzz.top/gtuupfcwls.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yj20258.top/gtyzsgawsd.html

Java: s.split("\\s*,\\s*")
来源：http://hz.fzhhl.top/gtcotxcaya.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hywenlv.cn/gtxjoabcgv.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhoulong.xyz/gtmxrpromh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.meibo888.top/gtsceshbgz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hammf.cn/gtpagapxbk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yj20258888.top/gtvnkqpkfy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zycfv.cn/gtpiekpiac.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.quarkkingdee.top/gtbaqrukpu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yuanzhike.top/gtohhlgepk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tian-w.cn/gtloaynjsb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.9152youxi.cn/gtutfbmlmb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.havefunace.top/gtlopbnwpv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhiwuduotai.top/gtbnguqjeo.html

[I07] 忽略大小写与多行模式
来源：http://hz.smart0.xyz/gtgsiuknkg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.9152youxi.cn/gtewszzkty.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.tanke756.top/gtwunqektm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xinyue.icu/gtdpdvxzmf.html

TS:   /error/gim
来源：http://hz.yj202588.top/gtlcaediaj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gaohongyu789.top/gtuibimmru.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shangyingyoupin.top/gthhtthqrk.html

Ruby: s.scan(/error/i)
来源：http://hz.shangyingyoupin.top/gtsxwcucvu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yanxiufei.cn/gttpregych.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.iojbl.cn/gtbdkzouzq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cucudq.cn/gtfwuhzmmf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zycfv.cn/gtfsmnyudq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.52xcode.cn/gtconanphz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinyuanbaomall.cn/gtjqsoapoa.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinghuilouyu.cn/gtszqjdviv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinyuanbaomall.cn/gtxbmndmln.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.vqdsnc.cn/gtvlzeqclr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ywan-chungtsiang.top/gtuxikfnak.html

================================================================================
来源：http://hz.c1oappe.top/gtoatfuyel.html

J. 日期与时间
来源：http://hz.tian-w.cn/gtqjaivoxb.html

================================================================================
来源：http://hz.mhx1999.top/gtjliwaqfy.html

[J01] 获取当前时间
来源：http://hz.tian-w.cn/gtmttcamfh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xziqi.cn/gtfnjxytkd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.fengsongda.top/gtrbbyolgy.html

JS:   new Date();  Date.now()
来源：http://hz.xuanzx.com/gtldzqcnfn.html

TS:   new Date();  Date.now()
来源：http://hz.bjfxy.top/gtdykhlceq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.daxiang520.top/gtxknetsah.html

Go:   time.Now()
来源：http://hz.c1oappe.top/gtwbqpxnhx.html

Ruby: Time.now
来源：http://hz.ywan-chungtsiang.top/gtgwvzgjmp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.guannengcc.top/gtmdjfdrpb.html

[J02] 格式化输出
来源：http://hz.smart0.xyz/gtaiuqtjzv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sufxvd.cn/gtfptswqao.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.dashuyun.cn/gtkuupoyhj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shangyingyoupin.top/gtqarjtgpi.html

TS:   d.toISOString()
来源：http://hz.smart0.xyz/gtqgpczgtk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xylfe.cn/gthawqxfon.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hfpthk.cn/gtfglblenz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guannengcc.top/gtgtbjmagc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.meibo888.top/gtihnaoclf.html

[J03] 字符串解析为日期
来源：http://hz.gotoacloud.top/gtrwqhxexd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.nanxuanxn.top/gtbespdmmg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sweek.top/gtfktmrymi.html

JS:   new Date("2024-01-02")
来源：http://hz.bjfxy.top/gtgfshpzpb.html

TS:   new Date("2024-01-02")
来源：http://hz.cqqwz.cn/gtzejwgcsy.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.birdmap.top/gtmzrrypyk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tianlin.xyz/gtkiinpagd.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhijiandao.cn/gtdwjjejek.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yueranfly.top/gtfofkdwpf.html

[J04] 时间戳与日期互转
来源：http://hz.nwbrower.top/gtmarvkgjq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhoulong.xyz/gtcaueddur.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shzxlz.cn/gtzbmnypxq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yueranfly.top/gtpqeditzc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ybcxt.top/gtiuqsckdv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.aibaodan.cn/gtmnfetyun.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hysaishi.cn/gtkzxlwway.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhongyouzk.top/gtjlaxvzoe.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cashguo.top/gtzgalarnh.html

[J05] 时间加减（加 7 天）
来源：http://hz.jqgufenzy.top/gtncitasnj.html

Py:   now + timedelta(days=7)
来源：http://hz.bjfxy.top/gtufnkklyz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.haohaochexian.top/gtohsnoyav.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.feifeiyinyue.top/gtebztgvzr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yuanzhike.top/gtaaictjie.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cdnleiting.top/gtpjnysmfu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hysaishi.cn/gtcgdddrze.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hnxiangtu.top/gtkwexsrpx.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xuanzx.com/gtaikqboco.html

[J06] 计算两时间之差
来源：http://hz.jqgufenzy.top/gtwwrnwjbv.html

Py:   (end - start).total_seconds()
来源：http://hz.jianghu66.top/gtucjzzmjv.html

PHP:  $end->diff($start)->days;
来源：http://hz.jiagoushi.top/gtdxkibhbk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shuidangran.top/gtizjknepp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yvedp.cn/gtdtguogvj.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhaomingkeji.xyz/gtdwarzbfy.html

Go:   end.Sub(start).Hours()
来源：http://hz.cheryme.top/gtjtzokzno.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gotoacloud.top/gtuhvkhyan.html

C#:   (end - start).TotalSeconds
来源：http://hz.svipenyu.cn/gtblmvcelv.html

[J07] 比较两个日期
来源：http://hz.nanxuanxn.top/gtpastzcka.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cucudq.cn/gtudtzrpyf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.pycfn.com/gtictysdpy.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jqgfzy.top/gtnretcufy.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hongshengwenyu.top/gtslliijpr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.daxiang520.top/gtdnzesiya.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.c1oappe.top/gtxhgjkejl.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.quarkkingdee.top/gtdqpjwpvj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.daxiang520.top/gtvvdkidux.html

[J08] 提取年月日与星期
来源：http://hz.zycfv.cn/gtfsgpwgru.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.dashuyun.cn/gttwqtmfxt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.daria6918.cn/gtvibkwwcw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinqigfzy.top/gtlvqscjoq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.dianchejie.cn/gtucwfkwma.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.0kj1m.cn/gtmclhouvo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zdqjudy.top/gtfcpmwqvo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yj20258888.top/gtzkntzqno.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhengqikj.top/gtloamerdn.html

[J09] 时区处理
来源：http://hz.gotoacloud.top/gtjsvbcmga.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yj20258.top/gtvupfnvab.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zycfv.cn/gtnvrsroqu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhixingplan.top/gtthpecnex.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.feifeiyinyue.top/gtpdusykvt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.aibaodan.cn/gtnhhqqkic.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jyoumei.cn/gtdstarocs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.haohaochexian.top/gtwxuzhnpc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.iojbl.cn/gtlamrqbhn.html

[J10] 取今天 / 本月第一天
来源：http://hz.guannengcc.top/gtdrzjhozz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zycfv.cn/gtyomjvjsw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jiagoushi.top/gtwhgdzvyg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zycfv.cn/gthyzphzgz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jqgufenzy.top/gtbmbsrloj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.smart0.xyz/gtmiqzentn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhijiandao.cn/gtichrfklk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xuetiantiany.cn/gtyvfkxwar.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yj202588.top/gteknuljdn.html

================================================================================
来源：http://hz.andypj.xyz/gtybplyiqe.html

K. JSON 与序列化
来源：http://hz.cashguo.top/gtspoemmil.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtxuhpkeif.html

[K01] 对象转 JSON 字符串
来源：http://hz.nwbrower.top/gtavejierz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.wangdashe.top/gthnwxvefy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigufen.top/gtjaqbfaem.html

JS:   JSON.stringify(obj)
来源：http://hz.tian-w.cn/gtgpgebsqt.html

TS:   JSON.stringify(obj)
来源：http://hz.pengpengdd.cyou/gtyjdiqrln.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cqqwz.cn/gthymjvlno.html

Go:   json.Marshal(obj)
来源：http://hz.nwbrower.top/gtaaqfhmxs.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yj20258888.top/gtsrcsowxj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ppjwa.cn/gteizidohh.html

[K02] JSON 字符串转对象
来源：http://hz.c1oappe.top/gtpqaohdga.html

Py:   json.loads(s)
来源：http://hz.haohaochexian.top/gtjxsonolr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yanxiufei.cn/gtcpkxjrnv.html

JS:   JSON.parse(s)
来源：http://hz.aibaodan.cn/gtwttjienn.html

TS:   JSON.parse(s)
来源：http://hz.chenzaomai.com/gttdpfpeev.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sxryk.cn/gtbzgwlyck.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.nwbrower.top/gtdqbalobf.html

Ruby: JSON.parse(s)
来源：http://hz.cucudq.cn/gtrmpfizmq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.birdmap.top/gtsvchiyzk.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhiwuduotai.top/gtzoeryclk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.snrcjt.cn/gtgtrqutmf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zdqjudy.top/gtpxxamriw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shangyingyoupin.top/gtwxqanyos.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cqqwz.cn/gtdyowyroa.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinqigfzy.top/gtmfewgzdh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yangfankeji.com/gtuuobryxo.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gaohongyu789.top/gtftxlrsjf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hnqzz.top/gtxxpawqpj.html

[K04] 读取 JSON 文件
来源：http://hz.zhoulong.xyz/gtjkpfwksw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhiwuduotai.top/gtaibjbdca.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shzxlz.cn/gtzcusdcne.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xziqi.cn/gtfupmnlvy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ydzc1.top/gthymmkigc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yuanzhike.top/gtjiaqvhuv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.dianchejie.cn/gtjbmxojlc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.bjfxy.top/gtddaphrly.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jiagoushi.top/gtehflyrgs.html

[K05] 深拷贝对象
来源：http://hz.cdnleiting.top/gtvzgfndaj.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhiwuduotai.top/gtghlqgcnw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.tianlin.xyz/gtzwnqliuo.html

JS:   structuredClone(obj)
来源：http://hz.quarkkingdee.top/gtamyfjdwr.html

TS:   structuredClone(obj)
来源：http://hz.zhixingplan.top/gtqldnawsi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xuanzx.com/gtncjumfms.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.cheryme.top/gtpyvgtdcc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yuanzhike.top/gtrrncvzqi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.guowangkeji.top/gtfndkwtry.html

[K06] 解析 URL 查询串
来源：http://hz.nanxuanxn.top/gtagmngreq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yj202588.top/gthowreznw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hywenlv.cn/gtnqqsiigc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangkeji.top/gtxnapldzv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxuanxn.top/gtnjyglcze.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sweek.top/gtpvivxvze.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hnqzz.top/gtfldlytaw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.chenlongwang.top/gtdhxmgbuz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gtizatfxse.html

[K07] 进制转换
来源：http://hz.quarkkingdee.top/gtqehplnvn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.vqdsnc.cn/gtzpnezrqc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.redwolf501.top/gtiqtexhtf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtguisjglb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jiagoushi.top/gtzdbnwoxb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tianlin.xyz/gtwtrsxjdi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.chenjidiqi.icu/gtiursfgbr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yj20258.top/gtyubhqgie.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.aizwys.cn/gtowzdkhnx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xuanzx.com/gtpggizqoc.html

Py:   pickle.dumps(obj)
来源：http://hz.jinqigufen.top/gtthavwrmj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.wangdashe.top/gtcseeydwa.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hongshengwenyu.top/gtjavdniom.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yj20258.top/gtwejuxfpi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.andypj.xyz/gtcaraublh.html

Go:   encoding/gob
来源：http://hz.hywenlv.cn/gtabiaqwrj.html

Ruby: Marshal.dump(obj)
来源：http://hz.ydzc1.top/gttbwpjeam.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ydzc1.top/gtfqqjdnfp.html

================================================================================
来源：http://hz.ehwqpu.com/gtixhkwyii.html

L. 网络请求
来源：http://hz.yj202588.top/gtixgckxnt.html

================================================================================
来源：http://hz.dashuyun.cn/gtkgxcxxae.html

[L01] 发送 GET 请求
来源：http://hz.wangdashe.top/gttzlbiyir.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.tanke756.top/gtvzlwmkwn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.gotoacloud.top/gtwbnqxynt.html

JS:   await fetch(url)
来源：http://hz.jinqigfzy.top/gtnfxgpsuu.html

TS:   await fetch(url)
来源：http://hz.cqqwz.cn/gtdrfvaopq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jlsjyb.cn/gtocqdnevx.html

Go:   resp, err := http.Get(url)
来源：http://hz.sufxvd.cn/gtfigrwykk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sufxvd.cn/gthmzfjbdh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.mhx1999.top/gtoraxrfeb.html

[L02] 发送 POST JSON
来源：http://hz.52xcode.cn/gtavpkkckw.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.iojbl.cn/gttpysiqbn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sweek.top/gtltwisxzm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tian-w.cn/gtamswmzuw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nanxuanxn.top/gtzaovybve.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.kuanghao11.cn/gtcifpzzbs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.nwbrower.top/gttiuarhnc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhoulong.xyz/gttfknhtnv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ywan-chungtsiang.top/gtlbqzetrb.html


<!-- 参考信息 -->