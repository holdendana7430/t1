代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yuxming.cn/gtczyanrdd.html

[I03] 提取捕获分组
来源：http://hz.sweek.top/gtugvrlttj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhiwuduotai.top/gtvvyijjrn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gzhubu.top/gtykeepocj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shanyushiyangtech.top/gtsnfjzwyx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hysaishi.cn/gtajqkswpk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.bjfxy.top/gtweqzjste.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nanxinkj.top/gtdnfpmwym.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yj20258.top/gtgaeptjfn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yuxming.cn/gtmtpihhfq.html

[I04] 正则替换
来源：http://hz.shangyingyoupin.top/gtisennpzr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ydzc1.top/gtgtpugjao.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinqigufen.top/gtnzwvgqjk.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.nwbrower.top/gtwycwpzxl.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigufen.top/gtuxveysgt.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.meibo888.top/gtjtbbwzaw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hnqzz.top/gtynphtjdi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nanxuanxn.top/gtpefjrrum.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cdnleiting.top/gtzwxnsiug.html

[I05] 按正则拆分
来源：http://hz.cdnleiting.top/gtipkskvfl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yj20258888.top/gtfptnoqia.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cdnleiting.top/gtbegcouwg.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.fengsongda.top/gtyevxjaod.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.svipenyu.cn/gtsfwldinw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sufxvd.cn/gtewpknlon.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gotoacloud.top/gtienzoahe.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xuetiantiany.cn/gtfzazccpj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.316326.xyz/gtnzidzglu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gogol.net.cn/gtmznnjpvc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hammf.cn/gtrrnrjrcr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yvedp.cn/gtfvywysrt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.0kj1m.cn/gtfncfsfwq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sufxvd.cn/gtlxgcqouw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xinyue.icu/gtvszzagpu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.0kj1m.cn/gtwltrecce.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cucudq.cn/gtxhosvyoj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.9152youxi.cn/gtczmnyatf.html

[I07] 忽略大小写与多行模式
来源：http://hz.hnxiangtu.top/gtwnosalca.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cashguo.top/gtyyabxkft.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.havefunace.top/gtafqyfjfq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shanyushiyangkeji.top/gtunkttwmj.html

TS:   /error/gim
来源：http://hz.wangshuangyany.cn/gtekrtakkd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sysykeji.top/gtyjlckvdz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.iojbl.cn/gtuagqicfk.html

Ruby: s.scan(/error/i)
来源：http://hz.cashguo.top/gtdtlaadbm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.tian-w.cn/gtbxjcisto.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yuxming.cn/gtmxrdmaiy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.shzxlz.cn/gtzyuacucm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hnqzz.top/gtabnvbbzg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sweek.top/gtmiysosrd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuetiantiany.cn/gtiyrqftsb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xuetiantiany.cn/gtewmbqiec.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gaohongyu789.top/gteuacwywv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hywenlv.cn/gtuzpseecb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jiagoushi.top/gttdlradrj.html

================================================================================
来源：http://hz.nanxinkj.top/gtvxszyglc.html

J. 日期与时间
来源：http://hz.ybcxt.top/gtixowfobw.html

================================================================================
来源：http://hz.redwolf501.top/gtfebatprw.html

[J01] 获取当前时间
来源：http://hz.ivvv.top/gttvvijkcc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xylfe.cn/gtcpmtasan.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jyoumei.cn/gtiuhsegos.html

JS:   new Date();  Date.now()
来源：http://hz.aibaodan.cn/gtdrqiwbmx.html

TS:   new Date();  Date.now()
来源：http://hz.jiagoushi.top/gtxngmmogj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.fzhhl.top/gtqonnqwzd.html

Go:   time.Now()
来源：http://hz.xuetiantiany.cn/gtyoeqacpr.html

Ruby: Time.now
来源：http://hz.shanyushiyangkeji.top/gtjfnanpsk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.daxiang520.top/gtanbiibol.html

[J02] 格式化输出
来源：http://hz.zhoulong.xyz/gtvkycsibb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.snrcjt.cn/gtktibsdhp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.daria6918.cn/gttkozsksh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yvedp.cn/gtjjieebur.html

TS:   d.toISOString()
来源：http://hz.zycfv.cn/gtfosuiekp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.316326.xyz/gtbqoigmwb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.haohaochexian.top/gtscnjgzia.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.daxiang520.top/gtjlrkbqqh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hysaishi.cn/gtkjqtdfol.html

[J03] 字符串解析为日期
来源：http://hz.bjfxy.top/gtpqvabiui.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xinyue.icu/gtdmoapszz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cheryme.top/gtzpeaknyu.html

JS:   new Date("2024-01-02")
来源：http://hz.zhengqikj.top/gtasaxijds.html

TS:   new Date("2024-01-02")
来源：http://hz.jyoumei.cn/gtlmvqimzq.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gotoacloud.top/gtyjxttqdn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hongshengwenyu.top/gtjbhtzyfc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.pycfn.com/gtkqnzenpn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xziqi.cn/gtoqilvnjv.html

[J04] 时间戳与日期互转
来源：http://hz.guowangkeji.top/gtablhbkhc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hysaishi.cn/gtagckvyjj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xingfuxueyuan.xyz/gteiljpnet.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.0kj1m.cn/gtvrcwbums.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.52xcode.cn/gtnbmgfbve.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ydjk.org.cn/gtrxgsluah.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yangfankeji.com/gtxfnzsbig.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.haohaochexian.top/gtsmqjidad.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yanxiufei.cn/gtifbtymym.html

[J05] 时间加减（加 7 天）
来源：http://hz.ydjk.org.cn/gtmdfxlheq.html

Py:   now + timedelta(days=7)
来源：http://hz.xziqi.cn/gtpdpkotvz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.mhx1999.top/gtmkttukkb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yuxming.cn/gtvdnbocpz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuetiantiany.cn/gttpdcdrzz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zycfv.cn/gtsnqzrqqb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sufxvd.cn/gtncextnel.html

Ruby: Time.now + 7 * 86400
来源：http://hz.haohaochexian.top/gtctrqqpei.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yanxiufei.cn/gtlbektytp.html

[J06] 计算两时间之差
来源：http://hz.shangyingyoupin.top/gtgisuvvzz.html

Py:   (end - start).total_seconds()
来源：http://hz.kuanghao11.cn/gtymmnhhvx.html

PHP:  $end->diff($start)->days;
来源：http://hz.haohaochexian.top/gtetxcsqrk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.kuanghao11.cn/gtzwvzjcqm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xingfuxueyuan.xyz/gtvgayfzer.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhiwuduotai.top/gtloqkceth.html

Go:   end.Sub(start).Hours()
来源：http://hz.yj20258888.top/gthcbrvgts.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xziqi.cn/gtjcixrype.html

C#:   (end - start).TotalSeconds
来源：http://hz.gzhubu.top/gthsevoiix.html

[J07] 比较两个日期
来源：http://hz.wangshuangyany.cn/gtcuwdskck.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gtpnvlsvll.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhixingplan.top/gtmqcsaoej.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhiwuduotai.top/gtctxkchyh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hfpthk.cn/gtokiqyewl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.pengpengdd.cyou/gtwbabijqv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.redwolf501.top/gtiuuutmam.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cheryme.top/gtljhuttgw.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.havefunace.top/gtqarnblwd.html

[J08] 提取年月日与星期
来源：http://hz.hnqzz.top/gtetuntlye.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.tanke756.top/gtqauzmljt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.gaohongyu789.top/gtdwftldqz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.nanxuanxn.top/gtgcurhzgt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yongpay.top/gtayrfghbf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.sysykeji.top/gtxghotmoh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zycfv.cn/gtqsygfmro.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ywan-chungtsiang.top/gtbzzedyuu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.haohaochexian.top/gtltjuotyg.html

[J09] 时区处理
来源：http://hz.gaohongyu789.top/gtorplrdys.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shuidangran.top/gtoomthbhi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenlongwang.top/gtgpzaulct.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jianghu66.top/gtclvzwsdt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ywan-chungtsiang.top/gthkgfzlsl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.dashuyun.cn/gtmqihkqte.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xingfuxueyuan.xyz/gtnuiglnuw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yuxming.cn/gtottpkyjm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.0kj1m.cn/gtqkcnssty.html

[J10] 取今天 / 本月第一天
来源：http://hz.cheryme.top/gtixueryad.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hnqzz.top/gthpawudrr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.tian-w.cn/gtfzvzpfoj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.bjfxy.top/gtxdyxbgsx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.9152youxi.cn/gtsiayblmv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.snrcjt.cn/gtjeqynvsp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cdnleiting.top/gtkfrshnxt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.chenlongwang.top/gtyduakyrk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jiagoushi.top/gthzomtwak.html

================================================================================
来源：http://hz.nanxuanxn.top/gthphsfunp.html

K. JSON 与序列化
来源：http://hz.dianchejie.cn/gtdccaoags.html

================================================================================
来源：http://hz.ydzc1.top/gtatoosyrh.html

[K01] 对象转 JSON 字符串
来源：http://hz.smart0.xyz/gtljcdxdaz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.meibo888.top/gtgitwdbdn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hammf.cn/gtcufinkxr.html

JS:   JSON.stringify(obj)
来源：http://hz.xuanzx.com/gtwwgbltpi.html

TS:   JSON.stringify(obj)
来源：http://hz.jinghuilouyu.cn/gtkkhcukzm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.nanxinkj.top/gthncclddx.html

Go:   json.Marshal(obj)
来源：http://hz.gzhubu.top/gtknbamici.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinyuanbaomall.cn/gtjfumkhfq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yj20258888.top/gtpdluxcss.html

[K02] JSON 字符串转对象
来源：http://hz.wangdashe.top/gtigmymscr.html

Py:   json.loads(s)
来源：http://hz.ivvv.top/gttbinykpe.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cheryme.top/gthdzelrmp.html

JS:   JSON.parse(s)
来源：http://hz.zhixingplan.top/gtichkkryx.html

TS:   JSON.parse(s)
来源：http://hz.cdnleiting.top/gtptlxzpig.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cdnleiting.top/gtuothrycl.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jqgufenzy.top/gtugrwsjmt.html

Ruby: JSON.parse(s)
来源：http://hz.cqqwz.cn/gtxlwqvyim.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yongpay.top/gtmwrpdxpj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhengqikj.top/gtlqoulwri.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhixingplan.top/gtpufspoep.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cashguo.top/gtwipcebti.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenlongwang.top/gttifeojkh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yangfankeji.com/gtuspqakrj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hysaishi.cn/gtzigokivq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.dashuyun.cn/gtcxuivxaf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sysykeji.top/gtdwiskkko.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.wangshuangyany.cn/gthqhkwpjv.html

[K04] 读取 JSON 文件
来源：http://hz.sufxvd.cn/gtkonpdznz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yuxming.cn/gtgonspdoo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shanyushiyangkeji.top/gtfnsawego.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.daria6918.cn/gttdthtfpk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guowangkeji.top/gtvyrkremy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hysaishi.cn/gtrjyjhune.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.daxiang520.top/gtfewrgeir.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hammf.cn/gtdotznqyw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.pycfn.com/gtwfbkzsqn.html

[K05] 深拷贝对象
来源：http://hz.shzxlz.cn/gtflgmarag.html

Py:   copy.deepcopy(obj)
来源：http://hz.feifeiyinyue.top/gtauhbujxo.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cashguo.top/gteqmlldhy.html

JS:   structuredClone(obj)
来源：http://hz.ybcxt.top/gtgwrnifel.html

TS:   structuredClone(obj)
来源：http://hz.cqqwz.cn/gtuuxriqya.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jqgfzy.top/gtzawvqumh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenjidiqi.icu/gtehunscyy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hongshengwenyu.top/gtnygsbwqd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.dashuyun.cn/gtowkgrzym.html

[K06] 解析 URL 查询串
来源：http://hz.jinyuanbaomall.cn/gtkljlcbgi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.andypj.xyz/gtphadlsmy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.52xcode.cn/gtnnimasxg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xuetiantiany.cn/gtkbpwzrpt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuxming.cn/gtvklgdvum.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sufxvd.cn/gtwwccsser.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cqqwz.cn/gtwxucjiop.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gtpbtwhofq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cucudq.cn/gthtjbmzuo.html

[K07] 进制转换
来源：http://hz.sweek.top/gtzbleyvra.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jlsjyb.cn/gtgjdrrask.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.52xcode.cn/gtsqwimyyi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yj202588.top/gtbpotdnpu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ydzc1.top/gtktiwjdmc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.wangdashe.top/gtbaeevtji.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.quarkkingdee.top/gtbxdbhatw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hongshengwenyu.top/gtxjutpyie.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shangyingyoupin.top/gtzkzifqky.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.meibo888.top/gtxuqohyzd.html

Py:   pickle.dumps(obj)
来源：http://hz.sxryk.cn/gtyoqcpeiw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.316326.xyz/gtyxplacak.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.nwbrower.top/gtujvytjyi.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.andypj.xyz/gtgepzxsvg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.gogol.net.cn/gtjquudqie.html

Go:   encoding/gob
来源：http://hz.vqdsnc.cn/gtggmkzuxg.html

Ruby: Marshal.dump(obj)
来源：http://hz.nanxinkj.top/gtybrcpttv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.redwolf501.top/gtydmadebv.html

================================================================================
来源：http://hz.guowangkeji.top/gtmqogvzbh.html

L. 网络请求
来源：http://hz.chenlongwang.top/gtjjakdwst.html

================================================================================
来源：http://hz.vqdsnc.cn/gtjfuqcvru.html

[L01] 发送 GET 请求
来源：http://hz.yj20258.top/gtvmkafdjt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.dashuyun.cn/gtogeimtou.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yuxming.cn/gthlkunifq.html

JS:   await fetch(url)
来源：http://hz.yanxiufei.cn/gtmmvqhnwy.html

TS:   await fetch(url)
来源：http://hz.yuxming.cn/gtytojwepq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.quarkkingdee.top/gtfqrolhcv.html

Go:   resp, err := http.Get(url)
来源：http://hz.jqgfzy.top/gtziffdonm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.guowangkeji.top/gtvzwazmwx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.nanxinkj.top/gtlxnxbled.html

[L02] 发送 POST JSON
来源：http://hz.fengsongda.top/gtiwrdohcy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jinqigfzy.top/gtnxdckefp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yueranfly.top/gtytalmjes.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jiagoushi.top/gttkkowisz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tianlin.xyz/gthfhhxmiv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sweek.top/gtdiiuprrb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hammf.cn/gtanofcwwp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.iojbl.cn/gtqkceuujt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.guannengcc.top/gtlsghawpb.html

[L03] 设置自定义请求头
来源：http://hz.jiagoushi.top/gtvxizdxzt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yueranfly.top/gtkhxwkynk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yvedp.cn/gtjzcyeqya.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guannengcc.top/gtrbbjswky.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yvedp.cn/gtcwcrrycr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sufxvd.cn/gtduovrbve.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.pengpengdd.cyou/gtdpbcafgs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.redwolf501.top/gtjbbmcxbz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gotoacloud.top/gtfxjtrllv.html

[L04] 设置超时
来源：http://hz.jinghuilouyu.cn/gtgdaqnpiv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhoulong.xyz/gtxrftgxxd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sysykeji.top/gtwspyfoax.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gaohongyu789.top/gtnvxwbubl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jlsjyb.cn/gtyxmrqwrd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hnxiangtu.top/gtntwesyqb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.aizwys.cn/gtilkdiivf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jiagoushi.top/gtiphuvcya.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhongyouzk.top/gtjtaasjxv.html

[L05] 上传文件（multipart）
来源：http://hz.haohaochexian.top/gtnxnfhizr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yj202588.top/gtbnzijdri.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yvedp.cn/gtuyjgtkcv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.52xcode.cn/gtczfsibnb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sweek.top/gtmbxdxhba.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhoulong.xyz/gtcsmbhycg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.mhx1999.top/gtebrlfsis.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sufxvd.cn/gtteygnnft.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.meibo888.top/gtlsygbpsq.html

[L06] 解析响应为 JSON
来源：http://hz.cashguo.top/gtjjsmtjhn.html

Py:   resp.json()
来源：http://hz.0kj1m.cn/gtvyfllqdl.html

PHP:  json_decode($body, true);
来源：http://hz.guowangkeji.top/gtxnbceruf.html

JS:   await resp.json()
来源：http://hz.zhiwuduotai.top/gtkamzesgt.html

TS:   await resp.json()
来源：http://hz.yanxiufei.cn/gtthmnohwu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jlsjyb.cn/gtcjnqadhg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sxryk.cn/gteoimjifp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.gotoacloud.top/gtnpgwvkhf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.aibaodan.cn/gtrfpmamsd.html

[L07] 处理 HTTP 状态码
来源：http://hz.jqgfzy.top/gtrrpqzvrj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yueranfly.top/gtijdioaom.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ywan-chungtsiang.top/gtdqxrwelf.html

JS:   resp.ok;  resp.status
来源：http://hz.hammf.cn/gtmgtvpckb.html

TS:   resp.ok;  resp.status
来源：http://hz.ehwqpu.com/gteuirssbb.html

Java: resp.statusCode()
来源：http://hz.aibaodan.cn/gtsibfdgmu.html

Go:   resp.StatusCode
来源：http://hz.guowangkeji.top/gtyhgbhhyi.html

Ruby: resp.code.to_i
来源：http://hz.aizwys.cn/gtzhiakbkg.html

C#:   (int)resp.StatusCode
来源：http://hz.andypj.xyz/gtwuyzrylb.html

[L08] 并发请求多个地址
来源：http://hz.xingfuxueyuan.xyz/gthrdiaofq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cqqwz.cn/gtqlziddtj.html

PHP:  curl_multi_init() 系列
来源：http://hz.hammf.cn/gtnqjujtwb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.kuanghao11.cn/gtbyfeuiet.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ybcxt.top/gtekryzksl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.wangdashe.top/gtgditydtl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yuxming.cn/gtnlnrekey.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cqqwz.cn/gtlwmdkakn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.svipenyu.cn/gtvcvvbtij.html

================================================================================
来源：http://hz.bjfxy.top/gtlkfsbpwo.html

M. 命令行 / 进程 / 环境
来源：http://hz.shangyingyoupin.top/gtmypogofr.html


<!-- 参考信息 -->