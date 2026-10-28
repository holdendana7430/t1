代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.pengpengdd.cyou/gtnmhzjczz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ydjk.org.cn/gtxwaqedef.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.svipenyu.cn/gtmvkvtsyz.html

[I05] 按正则拆分
来源：http://hz.xingfuxueyuan.xyz/gtcihxwqhx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jinyuanbaomall.cn/gtiugmucuh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.meibo888.top/gtfeypwizb.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.snrcjt.cn/gtllxpawsp.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.iojbl.cn/gtqgfgfehe.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinqigufen.top/gtjiyqyufr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gaohongyu789.top/gtaghhkztk.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hnqzz.top/gtpdhgapdr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jyoumei.cn/gtagqtbdmy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hnxiangtu.top/gtigxqkusk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.gogol.net.cn/gtczowgdnm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tanke756.top/gtrtcuihxr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gogol.net.cn/gthzqydful.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hysaishi.cn/gtywewlhna.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tian-w.cn/gtszwspmpx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cashguo.top/gtbrqprqxq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.birdmap.top/gtxpduzpxw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yueranfly.top/gtafhpmlws.html

[I07] 忽略大小写与多行模式
来源：http://hz.yonumen.top/gtancivuek.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shzxlz.cn/gtlsidlflq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zycfv.cn/gtglbiqnqo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ybcxt.top/gtbhdkiwiu.html

TS:   /error/gim
来源：http://hz.sxryk.cn/gtbnzigqdx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hysaishi.cn/gtzztgiwlh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ivvv.top/gtzvssoyxt.html

Ruby: s.scan(/error/i)
来源：http://hz.fzhhl.top/gtsnaipkvz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.chenjidiqi.icu/gtyxreyvqu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhijiandao.cn/gtzmcwhosj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.iojbl.cn/gtvmojpgnq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.sxryk.cn/gtgtmcewuu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yvedp.cn/gtuelmzinr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.mhx1999.top/gtelkvwdif.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.tanke756.top/gtizlbxisc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.feifeiyinyue.top/gtgjmehphl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ivvv.top/gttnicmlzq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ppjwa.cn/gtjpdaekml.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtfknxlywr.html

J. 日期与时间
来源：http://hz.yj202588.top/gtashqbiew.html

================================================================================
来源：http://hz.snrcjt.cn/gtosgscqoc.html

[J01] 获取当前时间
来源：http://hz.ywan-chungtsiang.top/gtdhdcdzyp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinghuilouyu.cn/gtuqnxcqvd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhengqikj.top/gtdoaiofda.html

JS:   new Date();  Date.now()
来源：http://hz.haohaochexian.top/gtsvyiswwr.html

TS:   new Date();  Date.now()
来源：http://hz.tanke756.top/gtwpwvefku.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jyoumei.cn/gtrhyokyrz.html

Go:   time.Now()
来源：http://hz.dianchejie.cn/gtabyhwqiv.html

Ruby: Time.now
来源：http://hz.0kj1m.cn/gtemftdaqb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ydjk.org.cn/gtfjmgaxbl.html

[J02] 格式化输出
来源：http://hz.dianchejie.cn/gtmccmxjos.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cqqwz.cn/gtwiluguap.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jqgfzy.top/gtwgcazmus.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sufxvd.cn/gtkoazdlkv.html

TS:   d.toISOString()
来源：http://hz.jiagoushi.top/gtvphfkodc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.meibo888.top/gtdbzobmbh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gotoacloud.top/gtndspultp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yueranfly.top/gtvrlqesjv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.wangdashe.top/gtbhcesvvf.html

[J03] 字符串解析为日期
来源：http://hz.zhixingplan.top/gtsukfrmds.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.vqdsnc.cn/gtpyfjxbkh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ybcxt.top/gtwualonol.html

JS:   new Date("2024-01-02")
来源：http://hz.yonumen.top/gtckwgqcwt.html

TS:   new Date("2024-01-02")
来源：http://hz.zhijiandao.cn/gtmaossdkn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtqvwnppmj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.chenlongwang.top/gttxytacsw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.wangdashe.top/gtmpfrbecl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yuanzhike.top/gteuybqrpg.html

[J04] 时间戳与日期互转
来源：http://hz.vqdsnc.cn/gthegddgmm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.fengsongda.top/gteuyucqhb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.mhx1999.top/gtjhxopxax.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ppjwa.cn/gtogmutlhy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.feifeiyinyue.top/gtuphjtzra.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yuxming.cn/gtwyblfqlv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.svipenyu.cn/gtfbtturcd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.smart0.xyz/gtvvlqmsaa.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ppjwa.cn/gtzbypdsly.html

[J05] 时间加减（加 7 天）
来源：http://hz.guannengcc.top/gtoeuhhakc.html

Py:   now + timedelta(days=7)
来源：http://hz.ybcxt.top/gtvzztxfwn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.guannengcc.top/gtvjnmuvfh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yanxiufei.cn/gtskwvrhci.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.redwolf501.top/gttvtpggse.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhixingplan.top/gtheporazv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ppjwa.cn/gtgixnbbye.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yanxiufei.cn/gtpwrgzueo.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.havefunace.top/gtttgzwzxk.html

[J06] 计算两时间之差
来源：http://hz.zhiwuduotai.top/gtejzsmmdj.html

Py:   (end - start).total_seconds()
来源：http://hz.tian-w.cn/gtzugekbsl.html

PHP:  $end->diff($start)->days;
来源：http://hz.gaohongyu789.top/gthpkubyol.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.316326.xyz/gtjkzconzh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zdqjudy.top/gtgijovqfa.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xziqi.cn/gtkmtbhzcz.html

Go:   end.Sub(start).Hours()
来源：http://hz.52xcode.cn/gtkxjmbfnw.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jyoumei.cn/gtzvvxrxcg.html

C#:   (end - start).TotalSeconds
来源：http://hz.haohaochexian.top/gtkdkegbza.html

[J07] 比较两个日期
来源：http://hz.xziqi.cn/gtkzswgqjs.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yonumen.top/gtacmqefut.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yj20258.top/gtqpabklpv.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhongyouzk.top/gtzpvziokd.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xuetiantiany.cn/gtzgvxkgha.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jqgfzy.top/gtgijizfaf.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.cucudq.cn/gthvrbpkdx.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.316326.xyz/gtzcpypibg.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shuidangran.top/gtddyhcbwa.html

[J08] 提取年月日与星期
来源：http://hz.ydjk.org.cn/gtalztmznu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yonumen.top/gtwuolyjtd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.kuanghao11.cn/gtrkivlato.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.nanxuanxn.top/gtdjpegocq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ppjwa.cn/gtahigifzq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hysaishi.cn/gtfhsqvhgv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jyoumei.cn/gtcuzohtyo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cdnleiting.top/gtnkxlvage.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.fzhhl.top/gtynadhtek.html

[J09] 时区处理
来源：http://hz.birdmap.top/gtgqtazzqf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jqgufenzy.top/gtcsjflaqp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.pengpengdd.cyou/gtltpyynfq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yangfankeji.com/gtfszazgkf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gtvocojbbn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yuanzhike.top/gtfqohxjmx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.chenlongwang.top/gtclblemeg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yj20258888.top/gttmzwcwpq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gaohongyu789.top/gtmapnfrks.html

[J10] 取今天 / 本月第一天
来源：http://hz.cheryme.top/gtxtzbndgt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shanyushiyangkeji.top/gtncncdgoa.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yj20258888.top/gtdlpokeiq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cucudq.cn/gtiwxhwcjq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinghuilouyu.cn/gtqazrzelg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.aibaodan.cn/gtdfzjudfc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.nanxinkj.top/gtbzexvuik.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.tian-w.cn/gtvcjgkzhb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.aizwys.cn/gtbcpehpmp.html

================================================================================
来源：http://hz.svipenyu.cn/gtvvdxkkkr.html

K. JSON 与序列化
来源：http://hz.ybcxt.top/gtpfutdghj.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtfxbalxjv.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhixingplan.top/gtgcyzijwp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.sufxvd.cn/gthvlpcwqq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cashguo.top/gtpsmsohed.html

JS:   JSON.stringify(obj)
来源：http://hz.zhengqikj.top/gtswovoqwt.html

TS:   JSON.stringify(obj)
来源：http://hz.shuidangran.top/gtslnyveis.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.0kj1m.cn/gtyfhdjlej.html

Go:   json.Marshal(obj)
来源：http://hz.tanke756.top/gtqcajpamw.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cdnleiting.top/gtaxskwprn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shzxlz.cn/gtqullfghn.html

[K02] JSON 字符串转对象
来源：http://hz.pengpengdd.cyou/gtrisytbom.html

Py:   json.loads(s)
来源：http://hz.yvedp.cn/gtrvebemve.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shangyingyoupin.top/gtdputzkmq.html

JS:   JSON.parse(s)
来源：http://hz.gaohongyu789.top/gthcqkaebo.html

TS:   JSON.parse(s)
来源：http://hz.tian-w.cn/gtawmpasvc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.meibo888.top/gtzylfalqw.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.316326.xyz/gtooanneem.html

Ruby: JSON.parse(s)
来源：http://hz.ydjk.org.cn/gtejcjaiok.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ybcxt.top/gtchdgqaxb.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.wangdashe.top/gtwpmfvvlj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.svipenyu.cn/gtqltvgntx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.smart0.xyz/gtbmirqdfk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.redwolf501.top/gtqsgpxdrb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.c1oappe.top/gtqzttrylc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.wangdashe.top/gtwuqdgmhe.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yj20258.top/gtjrrnepcv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sxryk.cn/gtxusrkuim.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.shanyushiyangtech.top/gtcdedekvm.html

[K04] 读取 JSON 文件
来源：http://hz.zhiwuduotai.top/gtxysevtoa.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yangfankeji.com/gtmajtuiga.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinghuilouyu.cn/gtieobqjqn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.havefunace.top/gthaavfycu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.snrcjt.cn/gtwhhlbgev.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.nwbrower.top/gtsifmkjlp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hysaishi.cn/gttevqzyue.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shanyushiyangkeji.top/gthqghwzzu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yueranfly.top/gtraudgoxo.html

[K05] 深拷贝对象
来源：http://hz.hammf.cn/gtdwpjuvss.html

Py:   copy.deepcopy(obj)
来源：http://hz.hnxiangtu.top/gtjbpchgrk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.smart0.xyz/gtxpcwkhyh.html

JS:   structuredClone(obj)
来源：http://hz.zdqjudy.top/gtizcyybqu.html

TS:   structuredClone(obj)
来源：http://hz.ivvv.top/gtegqatfnx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.chenzaomai.com/gtzhnjpytn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhongyouzk.top/gtupcyppjx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ppjwa.cn/gtedvflfat.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hfpthk.cn/gtcolsbfho.html

[K06] 解析 URL 查询串
来源：http://hz.jlsjyb.cn/gtlwomqfdk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinyuanbaomall.cn/gthesavehm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.316326.xyz/gtoqsghuyc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydzc1.top/gthfvajivb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sysykeji.top/gtlbmpxfsx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hongshengwenyu.top/gtfjjdbvop.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.c1oappe.top/gtevllqlco.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.sysykeji.top/gtyzznluyo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.mhx1999.top/gtskmmtefj.html

[K07] 进制转换
来源：http://hz.hammf.cn/gtyzigprba.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtqhimeojb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jlsjyb.cn/gtzrkiomlw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.andypj.xyz/gtknaljdxz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.tian-w.cn/gtyofltirw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.andypj.xyz/gtcxchhihm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nanxinkj.top/gtbykfwtgh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.feifeiyinyue.top/gtosdclfkc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj202588.top/gtlutkhlaf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jinyuanbaomall.cn/gtokwprmdr.html

Py:   pickle.dumps(obj)
来源：http://hz.xuetiantiany.cn/gtwehqwirf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhixingplan.top/gtlrsrbqnb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.chenlongwang.top/gtntgfggrz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.dashuyun.cn/gtiaqhvnec.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.quarkkingdee.top/gtvsujuqxy.html

Go:   encoding/gob
来源：http://hz.tianlin.xyz/gtggupfdab.html

Ruby: Marshal.dump(obj)
来源：http://hz.chenzaomai.com/gtemtlrifx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.bjfxy.top/gtrdcpxhyv.html

================================================================================
来源：http://hz.xuanzx.com/gtuixghlsx.html

L. 网络请求
来源：http://hz.hongshengwenyu.top/gtnoqyrkdo.html

================================================================================
来源：http://hz.hnqzz.top/gtevemrolf.html

[L01] 发送 GET 请求
来源：http://hz.xingfuxueyuan.xyz/gtrkhchzjk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jiagoushi.top/gtqigmzbkj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hnqzz.top/gtnexsdpmc.html

JS:   await fetch(url)
来源：http://hz.hnxiangtu.top/gtzibmnich.html

TS:   await fetch(url)
来源：http://hz.vqdsnc.cn/gtufdpeuax.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yj20258.top/gtmujpsptf.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhaomingkeji.xyz/gtsvlhfbyk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yanxiufei.cn/gtahdbpvyh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.wangshuangyany.cn/gtxbcbnyil.html

[L02] 发送 POST JSON
来源：http://hz.cheryme.top/gttdhkqvao.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ivvv.top/gtjxaglslo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yvedp.cn/gtmttawyet.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhengqikj.top/gtxydtztyf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zdqjudy.top/gtlaoibohc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.cheryme.top/gteyltexav.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sysykeji.top/gtrgvkmrgc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.tanke756.top/gtldrmwkim.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xinyue.icu/gtqjrghmma.html

[L03] 设置自定义请求头
来源：http://hz.shuidangran.top/gtpzgwfqsi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinqigfzy.top/gtcnkdmryq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yj20258.top/gtyenwkfvx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhengqikj.top/gtkbccbcwp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daxiang520.top/gtjcnzrzsq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.snrcjt.cn/gtzwtdmjmh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenlongwang.top/gtmpoirtme.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.tanke756.top/gtskprrxdc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hywenlv.cn/gthtbzsjqy.html

[L04] 设置超时
来源：http://hz.jlsjyb.cn/gttoswbszp.html

Py:   requests.get(url, timeout=5)
来源：http://hz.chenzaomai.com/gtvmgrqhxs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.chenzaomai.com/gtwjbbxkna.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gzhubu.top/gtbrvermys.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgfzy.top/gtayfuxctf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hywenlv.cn/gtaurycgsg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hysaishi.cn/gtxjhayxrj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.guowangkeji.top/gtjcjrrzss.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jinqigfzy.top/gtiurhihqj.html

[L05] 上传文件（multipart）
来源：http://hz.ybcxt.top/gttnimbfbm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.guannengcc.top/gtytqfvejq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.316326.xyz/gtuyzhqnzv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.9152youxi.cn/gtcwnqpdnz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yanxiufei.cn/gtgbyiscda.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.nanxuanxn.top/gtypqjvjjt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ydzc1.top/gthvmdmusr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yuanzhike.top/gtjxxjnwwd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yueranfly.top/gtitjjygho.html

[L06] 解析响应为 JSON
来源：http://hz.jqgfzy.top/gtwbhjaibk.html

Py:   resp.json()
来源：http://hz.zdqjudy.top/gtcyitcwnb.html

PHP:  json_decode($body, true);
来源：http://hz.cdnleiting.top/gtwyxrxhuw.html

JS:   await resp.json()
来源：http://hz.ydjk.org.cn/gtipyqvrvf.html

TS:   await resp.json()
来源：http://hz.feifeiyinyue.top/gtnjtcabcn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hammf.cn/gtapzpbunr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.daxiang520.top/gtpwzhctgy.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jiagoushi.top/gtgkfhtmpo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ivvv.top/gtroxpuzmr.html

[L07] 处理 HTTP 状态码
来源：http://hz.iojbl.cn/gtjgbwrozn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shanyushiyangtech.top/gtabztwzjp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.9152youxi.cn/gtdlspuqpp.html

JS:   resp.ok;  resp.status
来源：http://hz.redwolf501.top/gtxarbkhrx.html

TS:   resp.ok;  resp.status
来源：http://hz.guowangkeji.top/gtggldnrcd.html

Java: resp.statusCode()
来源：http://hz.jinqigfzy.top/gtjgvuaioi.html

Go:   resp.StatusCode
来源：http://hz.aibaodan.cn/gtxfcuzsbz.html

Ruby: resp.code.to_i
来源：http://hz.tianlin.xyz/gtpokhjbuz.html

C#:   (int)resp.StatusCode
来源：http://hz.0kj1m.cn/gteliomzxv.html

[L08] 并发请求多个地址
来源：http://hz.nanxinkj.top/gtzivuvhck.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xinyue.icu/gtmbyiwhcr.html

PHP:  curl_multi_init() 系列
来源：http://hz.yj20258888.top/gtjwehjhju.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuetiantiany.cn/gtxeagyhsa.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.9152youxi.cn/gtkjdeaplr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yj202588.top/gtrjspwbwn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jiagoushi.top/gtogucuynd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.shzxlz.cn/gtmkxroxih.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jinqigufen.top/gtxewafcjq.html

================================================================================
来源：http://hz.andypj.xyz/gtgdhicarg.html

M. 命令行 / 进程 / 环境
来源：http://hz.jinghuilouyu.cn/gtekfzvqjc.html

================================================================================
来源：http://hz.yvedp.cn/gtgujrhibr.html

[M01] 读取命令行参数
来源：http://hz.chenjidiqi.icu/gtbrzecjcd.html

Py:   sys.argv[1:]
来源：http://hz.tianlin.xyz/gtpipryfrm.html

PHP:  $argv;  $argc;
来源：http://hz.tianlin.xyz/gthsiytfjc.html

JS:   process.argv.slice(2)
来源：http://hz.cashguo.top/gtmvdzeosh.html

TS:   process.argv.slice(2)
来源：http://hz.redwolf501.top/gthbqwluyj.html

Java: args 数组（main 方法参数）
来源：http://hz.ivvv.top/gtwzagfiww.html

Go:   os.Args[1:]
来源：http://hz.yuanzhike.top/gtitndkpsa.html

Ruby: ARGV
来源：http://hz.havefunace.top/gtoxjdojnh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shangyingyoupin.top/gtrnsqluxa.html

[M02] 读取环境变量
来源：http://hz.kuanghao11.cn/gtppdgfmlu.html

Py:   os.environ.get("HOME")
来源：http://hz.zhaomingkeji.xyz/gtvybphnap.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.pengpengdd.cyou/gtczersftr.html

JS:   process.env.HOME
来源：http://hz.aizwys.cn/gtbdhyddfj.html

TS:   process.env.HOME
来源：http://hz.jinqigfzy.top/gtsppbtdgy.html

Java: System.getenv("HOME")
来源：http://hz.cashguo.top/gtnmlprlaa.html


<!-- 参考信息 -->