代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yongpay.top/gtslabfvnq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yongpay.top/gtznmfxmxc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jlsjyb.cn/gtzgfqdhid.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.mhx1999.top/gtcdsgxtym.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hywenlv.cn/gtqftyvfdp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.iojbl.cn/gtnqdrcgpt.html

[I04] 正则替换
来源：http://hz.wangshuangyany.cn/gthndfeukd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yuanzhike.top/gteadszzss.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jiagoushi.top/gttpetzhoi.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.pengpengdd.cyou/gtjmilxdzn.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigfzy.top/gtzsyvzcya.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.daxiang520.top/gtvhlctpdo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yangfankeji.com/gttchfnkhy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.aibaodan.cn/gtjghlrnbv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.chenjidiqi.icu/gtquyzcpgb.html

[I05] 按正则拆分
来源：http://hz.snrcjt.cn/gtdvshoamo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yonumen.top/gtsqgrtkdo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cheryme.top/gtgijxltca.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yuanzhike.top/gtlggfnszf.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhijiandao.cn/gtlrhmdldo.html

Java: s.split("\\s*,\\s*")
来源：http://hz.fzhhl.top/gtbjuymsik.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hnxiangtu.top/gttvbdcwzw.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nwbrower.top/gtwwypkudb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhaomingkeji.xyz/gtzoebwjtv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.meibo888.top/gtwkqsqpat.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cashguo.top/gtpeqaccsp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.havefunace.top/gtlzwfmzyw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yongpay.top/gtpubpwesb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258888.top/gtqqbxshmg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hnqzz.top/gtyuzceylz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.0kj1m.cn/gtzfprynnd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.chenzaomai.com/gtijypcfdy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xziqi.cn/gtqstfsttp.html

[I07] 忽略大小写与多行模式
来源：http://hz.hysaishi.cn/gtjtbtiijd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.wangshuangyany.cn/gtsjxgisro.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.cucudq.cn/gtrkinjixv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhengqikj.top/gtvivivepi.html

TS:   /error/gim
来源：http://hz.guowangkeji.top/gtqevnqevg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.feifeiyinyue.top/gtpnpsvkbk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.haohaochexian.top/gtpkdqftpf.html

Ruby: s.scan(/error/i)
来源：http://hz.pycfn.com/gtwwitxbyc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinghuilouyu.cn/gtybhozsse.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.meibo888.top/gtfmfuyvrw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.nanxuanxn.top/gtbyfbocfd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xuanzx.com/gtghzpajvv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dashuyun.cn/gtyinyaoqr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xylfe.cn/gtpjaeggjj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhongyouzk.top/gtknxepncy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.vqdsnc.cn/gtrlajwbam.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ehwqpu.com/gtxojzwevm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.aizwys.cn/gtfzfhucvq.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtcsuipnyy.html

J. 日期与时间
来源：http://hz.jinghuilouyu.cn/gtshyukpoj.html

================================================================================
来源：http://hz.guannengcc.top/gtuvavwbgi.html

[J01] 获取当前时间
来源：http://hz.yanxiufei.cn/gtdfsjcsav.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.andypj.xyz/gtstbwbwsj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.pycfn.com/gtgoyqozdf.html

JS:   new Date();  Date.now()
来源：http://hz.hnqzz.top/gtldpplkau.html

TS:   new Date();  Date.now()
来源：http://hz.yuxming.cn/gttmsgtycm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zdqjudy.top/gtxaofjojl.html

Go:   time.Now()
来源：http://hz.316326.xyz/gtnyuqqrhv.html

Ruby: Time.now
来源：http://hz.cdnleiting.top/gtnsvgtlfl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jianghu66.top/gtnmzuuqdx.html

[J02] 格式化输出
来源：http://hz.pycfn.com/gtubetaysr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cheryme.top/gtarsksfhg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.havefunace.top/gtbcqwyppf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.pycfn.com/gtamhtaqix.html

TS:   d.toISOString()
来源：http://hz.vqdsnc.cn/gtrtqejhww.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.dashuyun.cn/gtangopqvw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ywan-chungtsiang.top/gtuutmhpan.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yangfankeji.com/gtptirgfqx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jiagoushi.top/gtctuetagw.html

[J03] 字符串解析为日期
来源：http://hz.aibaodan.cn/gtiqfbxzzg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ywan-chungtsiang.top/gtdniyngfy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hnxiangtu.top/gtwdixrruj.html

JS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtxhxvusxe.html

TS:   new Date("2024-01-02")
来源：http://hz.cashguo.top/gthjvbmzub.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.nwbrower.top/gtwsdwwffj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cashguo.top/gtwrmhlgwr.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhijiandao.cn/gturcmbutv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.meibo888.top/gtqsluhcsu.html

[J04] 时间戳与日期互转
来源：http://hz.shzxlz.cn/gtycelbjpz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.andypj.xyz/gtihwowtcm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.guannengcc.top/gtlvmyozmq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.nwbrower.top/gtjiceowby.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nanxinkj.top/gtzhgcbpjg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.andypj.xyz/gtfuajswiv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jyoumei.cn/gtxnvhdpsn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.wangdashe.top/gtczqhaptw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cheryme.top/gtphxwsotc.html

[J05] 时间加减（加 7 天）
来源：http://hz.cheryme.top/gtipwqaiqg.html

Py:   now + timedelta(days=7)
来源：http://hz.jiagoushi.top/gtluwscnib.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.gzhubu.top/gtsvuxtedl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hysaishi.cn/gtjnqznzbg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dashuyun.cn/gtsrhmueye.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hammf.cn/gtpaflstia.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sysykeji.top/gtlwhqioud.html

Ruby: Time.now + 7 * 86400
来源：http://hz.meibo888.top/gtovpmhiya.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.9152youxi.cn/gtsdslltpp.html

[J06] 计算两时间之差
来源：http://hz.ywan-chungtsiang.top/gtcicifcxb.html

Py:   (end - start).total_seconds()
来源：http://hz.shzxlz.cn/gtbnovblcf.html

PHP:  $end->diff($start)->days;
来源：http://hz.jlsjyb.cn/gtolhcgdwj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shanyushiyangtech.top/gtpjnabdbh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.c1oappe.top/gtfwsztumo.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.aizwys.cn/gtgoxpzton.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhoulong.xyz/gtmdetzngc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.snrcjt.cn/gtgukdwhjy.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhiwuduotai.top/gtkdlpidvr.html

[J07] 比较两个日期
来源：http://hz.ehwqpu.com/gtwdluzsih.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtkncfhusb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.nanxinkj.top/gtnffknpfh.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.chenlongwang.top/gthsaujmus.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.haohaochexian.top/gtqmqtpljf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xuanzx.com/gthaplkqql.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yuanzhike.top/gtpluuuzdv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gtervounkx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.aizwys.cn/gtkxxlvmwk.html

[J08] 提取年月日与星期
来源：http://hz.snrcjt.cn/gtjmeagzwe.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.svipenyu.cn/gtaoqkamji.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sweek.top/gtfppjjjfw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.tian-w.cn/gtjkiguuqy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.bjfxy.top/gtvdiedxpz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.haohaochexian.top/gtcrqhjmjf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.fzhhl.top/gtdbgkbdsy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.snrcjt.cn/gtlcvimmdb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinqigfzy.top/gtypivwxns.html

[J09] 时区处理
来源：http://hz.wangshuangyany.cn/gtckzjlqlo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.aizwys.cn/gtuaanldkw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yj202588.top/gtrqicjgfo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guannengcc.top/gtgibhwttj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yangfankeji.com/gtjiztgdhq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.aibaodan.cn/gtkfvspeit.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cucudq.cn/gtzlvwjitl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.daxiang520.top/gtykbjnvsa.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.wangdashe.top/gtvignzvar.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinghuilouyu.cn/gtpxpbdkgz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.dianchejie.cn/gtbohtrurf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.bjfxy.top/gtretgpnlh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhengqikj.top/gtxvnoaiuq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cucudq.cn/gttaaudjlq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shuidangran.top/gtbrginciy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.wangdashe.top/gtfvxjqbfx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xylfe.cn/gtfzixzaeu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yuxming.cn/gtlagalhdu.html

================================================================================
来源：http://hz.xinyue.icu/gthstttorq.html

K. JSON 与序列化
来源：http://hz.yueranfly.top/gtdyhucdff.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtydggjywf.html

[K01] 对象转 JSON 字符串
来源：http://hz.iojbl.cn/gtnvoajblz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shangyingyoupin.top/gtytdltcwx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.guowangkeji.top/gtpqoirhtt.html

JS:   JSON.stringify(obj)
来源：http://hz.dianchejie.cn/gtczvxwbum.html

TS:   JSON.stringify(obj)
来源：http://hz.yanxiufei.cn/gtngydwsls.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yj20258888.top/gtvrwtpfus.html

Go:   json.Marshal(obj)
来源：http://hz.nwbrower.top/gtucvznnml.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yonumen.top/gthtoiqgdu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.gaohongyu789.top/gtfsrzxmln.html

[K02] JSON 字符串转对象
来源：http://hz.jianghu66.top/gtnzoefwhh.html

Py:   json.loads(s)
来源：http://hz.cucudq.cn/gtzafutuyf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xylfe.cn/gtkyhagpgy.html

JS:   JSON.parse(s)
来源：http://hz.yuxming.cn/gtlpyxxadt.html

TS:   JSON.parse(s)
来源：http://hz.ydzc1.top/gtjxpwcjhu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gaohongyu789.top/gtwowrltzv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ydzc1.top/gtkuynofwn.html

Ruby: JSON.parse(s)
来源：http://hz.jyoumei.cn/gtbgzymcxj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.tian-w.cn/gtlramjiqz.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.gzhubu.top/gtjkuuvuos.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ybcxt.top/gtonkcbhnq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.9152youxi.cn/gtwocgzfrt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj202588.top/gtdzwbxvmd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.smart0.xyz/gtmzosswad.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.9152youxi.cn/gtuogkljqt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yuxming.cn/gtnajxheby.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.vqdsnc.cn/gtognbknns.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jqgfzy.top/gtvuryzhqh.html

[K04] 读取 JSON 文件
来源：http://hz.zhijiandao.cn/gtihpfuuvx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hnxiangtu.top/gthejxiodl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.chenjidiqi.icu/gtobntqeyj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.birdmap.top/gtujuxqayr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tianlin.xyz/gtvnuitkjd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gogol.net.cn/gtxqcphwcs.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.feifeiyinyue.top/gtwsbwdbrg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.birdmap.top/gtptfnznlr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jianghu66.top/gtdfpefjib.html

[K05] 深拷贝对象
来源：http://hz.yj202588.top/gtppahitnl.html

Py:   copy.deepcopy(obj)
来源：http://hz.daria6918.cn/gtmgmhaczv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.feifeiyinyue.top/gtomhdjdcc.html

JS:   structuredClone(obj)
来源：http://hz.c1oappe.top/gtjmdzqjgh.html

TS:   structuredClone(obj)
来源：http://hz.52xcode.cn/gtdltufcjv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.chenzaomai.com/gtvxeraaiz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.wangdashe.top/gtdwhmoygh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.nanxuanxn.top/gtnpevgpmx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhongyouzk.top/gtiyghufkm.html

[K06] 解析 URL 查询串
来源：http://hz.ehwqpu.com/gtdwlkjzjc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.0kj1m.cn/gtkstrieun.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.dashuyun.cn/gtsbiegjom.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.smart0.xyz/gtqmbuxfap.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xylfe.cn/gtynwfxibc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jianghu66.top/gtspqcskde.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.0kj1m.cn/gtcknsdbiy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.feifeiyinyue.top/gtlsojnvve.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.chenjidiqi.icu/gtwyfmvgaa.html

[K07] 进制转换
来源：http://hz.sxryk.cn/gthklsxnyv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ydzc1.top/gtdymrwjkk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.daxiang520.top/gtxzosbgok.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.iojbl.cn/gtjhriirqj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jyoumei.cn/gtjladjgqw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gtopmevfzu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.fengsongda.top/gtotnhbwye.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yj202588.top/gtlcysmsdb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhijiandao.cn/gtxxmoeuje.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yvedp.cn/gtzbouhidz.html

Py:   pickle.dumps(obj)
来源：http://hz.fzhhl.top/gtonwmodto.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.vqdsnc.cn/gtgcdbgbsa.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hysaishi.cn/gtksnqmxba.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.nwbrower.top/gtloijwnsq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.gotoacloud.top/gtiyqgptvi.html

Go:   encoding/gob
来源：http://hz.vqdsnc.cn/gtbnmgrnwy.html

Ruby: Marshal.dump(obj)
来源：http://hz.yongpay.top/gtawlwlunv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.chenlongwang.top/gthvksbozj.html

================================================================================
来源：http://hz.cashguo.top/gtcbsgqxsp.html

L. 网络请求
来源：http://hz.shzxlz.cn/gtyermuiys.html

================================================================================
来源：http://hz.zhoulong.xyz/gtfxkxvmvp.html

[L01] 发送 GET 请求
来源：http://hz.xziqi.cn/gthyxztxuo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.guannengcc.top/gtjdhyuoqf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hysaishi.cn/gtxntnboif.html

JS:   await fetch(url)
来源：http://hz.pengpengdd.cyou/gtxotwyoay.html

TS:   await fetch(url)
来源：http://hz.mhx1999.top/gtzfyygmqd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.chenjidiqi.icu/gtcgukrlct.html

Go:   resp, err := http.Get(url)
来源：http://hz.cucudq.cn/gtwxblkvtb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhengqikj.top/gtbhyofkko.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.chenlongwang.top/gtdzziwned.html

[L02] 发送 POST JSON
来源：http://hz.cdnleiting.top/gthijubtps.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.sysykeji.top/gtchhhylgo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhiwuduotai.top/gtayaglszt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.9152youxi.cn/gtpnzaqoqo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhengqikj.top/gtkimxlyue.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.c1oappe.top/gtzuqurcel.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shuidangran.top/gtxioisylb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shanyushiyangkeji.top/gtkxevrpag.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.wangshuangyany.cn/gtqcezjsnt.html

[L03] 设置自定义请求头
来源：http://hz.jinghuilouyu.cn/gtctjvolzi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hammf.cn/gtipqhvofd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.52xcode.cn/gtnysssbuq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.pycfn.com/gtyzafipft.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinghuilouyu.cn/gtjdvsyykz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.chenjidiqi.icu/gtbnppmack.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhengqikj.top/gtrawflnny.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sxryk.cn/gtapfejose.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.pycfn.com/gteqpxemvi.html

[L04] 设置超时
来源：http://hz.jinqigfzy.top/gtvnnuphip.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jyoumei.cn/gtgszfmdiq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhengqikj.top/gteaakocdt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cheryme.top/gtcqjzedmb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuetiantiany.cn/gtkgvsnbih.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.bjfxy.top/gtjpqisusp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jianghu66.top/gtnykutgfx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinqigufen.top/gtqnofzhbn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ivvv.top/gtfbmglzcz.html

[L05] 上传文件（multipart）
来源：http://hz.aibaodan.cn/gtzxbsypgf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.0kj1m.cn/gtloeexjvb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xuetiantiany.cn/gthklgxyrf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yvedp.cn/gtojeznbdw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sufxvd.cn/gtguxyuwni.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.iojbl.cn/gtqvfbbpxp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xingfuxueyuan.xyz/gtrbonpwan.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ydjk.org.cn/gtyvcbiktc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhiwuduotai.top/gtuiyancxs.html

[L06] 解析响应为 JSON
来源：http://hz.chenlongwang.top/gtivrdheyn.html

Py:   resp.json()
来源：http://hz.chenzaomai.com/gttqgfkfxg.html

PHP:  json_decode($body, true);
来源：http://hz.nanxuanxn.top/gtreayzvoo.html

JS:   await resp.json()
来源：http://hz.yonumen.top/gtwgptzjoz.html

TS:   await resp.json()
来源：http://hz.ybcxt.top/gtnarvdhgt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.dashuyun.cn/gtlibgheei.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.dianchejie.cn/gtgsmqjcbf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.snrcjt.cn/gthxdvzxju.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.feifeiyinyue.top/gtqdtimhxx.html

[L07] 处理 HTTP 状态码
来源：http://hz.jyoumei.cn/gtmzrwyvxl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.vqdsnc.cn/gttzgjojpi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.9152youxi.cn/gttktvuvrp.html

JS:   resp.ok;  resp.status
来源：http://hz.fzhhl.top/gtxdeuleyv.html

TS:   resp.ok;  resp.status
来源：http://hz.guowangkeji.top/gtaaxyirvw.html

Java: resp.statusCode()
来源：http://hz.hysaishi.cn/gtgrazmwxo.html

Go:   resp.StatusCode
来源：http://hz.sufxvd.cn/gtcfrztdkr.html

Ruby: resp.code.to_i
来源：http://hz.aibaodan.cn/gtpasnsjrj.html

C#:   (int)resp.StatusCode
来源：http://hz.haohaochexian.top/gtlxfgipdo.html

[L08] 并发请求多个地址
来源：http://hz.ivvv.top/gtbqppdwxm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.meibo888.top/gtxxgymsli.html

PHP:  curl_multi_init() 系列
来源：http://hz.sxryk.cn/gthzcitxtw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenlongwang.top/gtajrrmeye.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.smart0.xyz/gtfuwdipft.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jianghu66.top/gtiajsmneq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jyoumei.cn/gtbxvqnijd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.aizwys.cn/gthwbasrxt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.guannengcc.top/gtebodmorf.html

================================================================================
来源：http://hz.birdmap.top/gtbsboqgyj.html

M. 命令行 / 进程 / 环境
来源：http://hz.jqgufenzy.top/gtqhovhiqp.html

================================================================================
来源：http://hz.shuidangran.top/gtowvlczzl.html

[M01] 读取命令行参数
来源：http://hz.gaohongyu789.top/gtkdnfimjw.html

Py:   sys.argv[1:]
来源：http://hz.hongshengwenyu.top/gtjhymcoop.html

PHP:  $argv;  $argc;
来源：http://hz.xylfe.cn/gtaaoognms.html


<!-- 参考信息 -->