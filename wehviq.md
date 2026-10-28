代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.chenzaomai.com/gtcqybldqn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.wangdashe.top/gtrpippyws.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hongshengwenyu.top/gtnvcjbnap.html

[I05] 按正则拆分
来源：http://hz.ehwqpu.com/gtwlbnrdhq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shangyingyoupin.top/gtouitsueb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.pycfn.com/gtzfhdkubs.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.mhx1999.top/gtvhovadmp.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gtfhxybfae.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zycfv.cn/gtzbbscswm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hysaishi.cn/gtbwsnqhji.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.wangdashe.top/gtydzqadvr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhengqikj.top/gthomafwlz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jiagoushi.top/gtumqhmepg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.tianlin.xyz/gtkftlltgv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zdqjudy.top/gtlujaglsv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aibaodan.cn/gtamijtdgo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.haohaochexian.top/gtnzrivnad.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.52xcode.cn/gtiuuhttkj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.aibaodan.cn/gtygtbsogf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.aibaodan.cn/gtxhvqakeh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.chenzaomai.com/gthaacxaxq.html

[I07] 忽略大小写与多行模式
来源：http://hz.xuetiantiany.cn/gtaudgbbqc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yanxiufei.cn/gtxbvtqrmq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.feifeiyinyue.top/gtxuobyvgj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yj20258.top/gtcshkeqgn.html

TS:   /error/gim
来源：http://hz.cashguo.top/gtonugrlxc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yj202588.top/gtqoekaqyx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.nwbrower.top/gtfeyygnam.html

Ruby: s.scan(/error/i)
来源：http://hz.andypj.xyz/gtqpzopolk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.daxiang520.top/gtfsprpwuw.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.quarkkingdee.top/gtuiadrhjv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sysykeji.top/gthvtlbrzc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhongyouzk.top/gtrcnjipae.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhongyouzk.top/gtgiglrlpc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shangyingyoupin.top/gtqzgcgrul.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hfpthk.cn/gtxbsnyrsb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jiagoushi.top/gtrhjyirpi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhijiandao.cn/gtwxhhvumb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.52xcode.cn/gtfukjwvsu.html

================================================================================
来源：http://hz.fengsongda.top/gtcrezupgr.html

J. 日期与时间
来源：http://hz.yongpay.top/gtstzcwhrx.html

================================================================================
来源：http://hz.zhijiandao.cn/gtnujtqwvn.html

[J01] 获取当前时间
来源：http://hz.xuanzx.com/gtjbtcquhz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.svipenyu.cn/gtoxdwsayc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cheryme.top/gtvqzvkzyb.html

JS:   new Date();  Date.now()
来源：http://hz.nanxinkj.top/gtmnkqtyfz.html

TS:   new Date();  Date.now()
来源：http://hz.birdmap.top/gtbmxgvtpi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.c1oappe.top/gttjymrfhm.html

Go:   time.Now()
来源：http://hz.snrcjt.cn/gtjwkmmabn.html

Ruby: Time.now
来源：http://hz.yangfankeji.com/gtstewicys.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xylfe.cn/gtuzezvpbq.html

[J02] 格式化输出
来源：http://hz.aizwys.cn/gtcutngsrg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangdashe.top/gtynfqnood.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.birdmap.top/gtsokcjauc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ehwqpu.com/gtmaccfldy.html

TS:   d.toISOString()
来源：http://hz.shanyushiyangkeji.top/gttpjldhfd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xuetiantiany.cn/gtwctrumzx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.kuanghao11.cn/gthkuhqdeb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhoulong.xyz/gtrtkduycy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gogol.net.cn/gtalsbubey.html

[J03] 字符串解析为日期
来源：http://hz.iojbl.cn/gtibwtiwsx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yonumen.top/gtjuanwkzr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.quarkkingdee.top/gtluymbxfj.html

JS:   new Date("2024-01-02")
来源：http://hz.jinqigufen.top/gtynvczaxs.html

TS:   new Date("2024-01-02")
来源：http://hz.svipenyu.cn/gtrtussfde.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jqgufenzy.top/gthtfdxxbx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shuidangran.top/gtyljioycl.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xuanzx.com/gtrnwgtwjq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yueranfly.top/gtpjrdpmoe.html

[J04] 时间戳与日期互转
来源：http://hz.9152youxi.cn/gttpwobnpw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhongyouzk.top/gtzzulochp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhongyouzk.top/gtarjhxqzt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.chenjidiqi.icu/gtwpfgicap.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.0kj1m.cn/gtshsrbuhy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.daxiang520.top/gtlhkyqwpq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.dashuyun.cn/gtjrhqsvcm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gaohongyu789.top/gtttoninxw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yueranfly.top/gttbqcyzwv.html

[J05] 时间加减（加 7 天）
来源：http://hz.quarkkingdee.top/gtoycpapfm.html

Py:   now + timedelta(days=7)
来源：http://hz.jinqigufen.top/gtotskzide.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hongshengwenyu.top/gtvccroplb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhiwuduotai.top/gtnrazbojg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jlsjyb.cn/gtvnvpbcep.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xuanzx.com/gtbyoxbzmp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.chenlongwang.top/gtuupeiraq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ppjwa.cn/gtfffrtuse.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ydjk.org.cn/gtqeiokxno.html

[J06] 计算两时间之差
来源：http://hz.zhijiandao.cn/gtviwjsrqy.html

Py:   (end - start).total_seconds()
来源：http://hz.wangdashe.top/gtqrdlmged.html

PHP:  $end->diff($start)->days;
来源：http://hz.xingfuxueyuan.xyz/gtdocjjaiz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.fengsongda.top/gtdtokwbnc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ydjk.org.cn/gtfcrzjggl.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yonumen.top/gthwobfqjj.html

Go:   end.Sub(start).Hours()
来源：http://hz.tian-w.cn/gtyztdjpvp.html

Ruby: end - start                 # 返回秒数
来源：http://hz.fengsongda.top/gtubmfhxam.html

C#:   (end - start).TotalSeconds
来源：http://hz.hywenlv.cn/gtxwpuwfxd.html

[J07] 比较两个日期
来源：http://hz.gaohongyu789.top/gtelcigjpm.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.pycfn.com/gtmvmuahgz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.gotoacloud.top/gthahpkzva.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yvedp.cn/gtwjuvjjoh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jlsjyb.cn/gtzrmeydpq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yj20258.top/gtqesmazgp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hammf.cn/gtxhamawwk.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xuanzx.com/gthrbhwzve.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cucudq.cn/gtrvzgdyyj.html

[J08] 提取年月日与星期
来源：http://hz.shuidangran.top/gtmpsvcsfc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.guannengcc.top/gtrdmqbyhx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.haohaochexian.top/gtlxsymwvw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.bjfxy.top/gtmrrquitf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.kuanghao11.cn/gtdipafcbg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hnxiangtu.top/gtchcvebfp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ydzc1.top/gttefheidf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xuetiantiany.cn/gtzjdpqtvt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.tianlin.xyz/gtnrxibfww.html

[J09] 时区处理
来源：http://hz.xingfuxueyuan.xyz/gtvmahaeag.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yuanzhike.top/gtssyczeze.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shzxlz.cn/gtiaitmxnu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sufxvd.cn/gtvaccuoil.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.fzhhl.top/gtwoajghun.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.316326.xyz/gtxffaszeo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ywan-chungtsiang.top/gtsjqhvszs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shanyushiyangtech.top/gthbqpoxvx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yj202588.top/gtuqovlpbf.html

[J10] 取今天 / 本月第一天
来源：http://hz.nanxinkj.top/gtiemsiupq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhiwuduotai.top/gtrscrxykt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinghuilouyu.cn/gthotctjfx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cdnleiting.top/gtelbioqzq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.meibo888.top/gtpcqwsdmi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cucudq.cn/gthvkkbpbo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zdqjudy.top/gteduzazty.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shanyushiyangtech.top/gtrqyhqcis.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yanxiufei.cn/gtthceuauo.html

================================================================================
来源：http://hz.yonumen.top/gtqxtmlebv.html

K. JSON 与序列化
来源：http://hz.xinyue.icu/gtfceovukn.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtsqjwfpgv.html

[K01] 对象转 JSON 字符串
来源：http://hz.gogol.net.cn/gtngznlbrl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ywan-chungtsiang.top/gtozceppfq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.chenjidiqi.icu/gtzcwdsyjf.html

JS:   JSON.stringify(obj)
来源：http://hz.havefunace.top/gtpqignzqq.html

TS:   JSON.stringify(obj)
来源：http://hz.gzhubu.top/gtpbydfnbn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zdqjudy.top/gthfanvlfe.html

Go:   json.Marshal(obj)
来源：http://hz.nanxinkj.top/gtyvmmblvd.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ydzc1.top/gtwnipfqrp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhengqikj.top/gtzzempdqp.html

[K02] JSON 字符串转对象
来源：http://hz.jiagoushi.top/gtorizppuu.html

Py:   json.loads(s)
来源：http://hz.zhixingplan.top/gtbqunuqmr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yvedp.cn/gteqclydoi.html

JS:   JSON.parse(s)
来源：http://hz.svipenyu.cn/gtporlcyat.html

TS:   JSON.parse(s)
来源：http://hz.jyoumei.cn/gttpsullwf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.52xcode.cn/gtbsyrhngl.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gzhubu.top/gtlyomsorb.html

Ruby: JSON.parse(s)
来源：http://hz.sysykeji.top/gtuyhiljdy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sufxvd.cn/gtvxuxsgsq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.bjfxy.top/gtmnnvebet.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.snrcjt.cn/gtimljmhsi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.fengsongda.top/gttryqswdi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.pengpengdd.cyou/gtwcrtmtyb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.nanxuanxn.top/gtygruqtis.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yonumen.top/gteptfhjrs.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhaomingkeji.xyz/gtgivwdrff.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xuetiantiany.cn/gtcbzicrrp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.daria6918.cn/gtuoorjpvp.html

[K04] 读取 JSON 文件
来源：http://hz.redwolf501.top/gttnycdixf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.guannengcc.top/gtbflugmrd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.c1oappe.top/gtbxebfull.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shangyingyoupin.top/gtynkaageb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dianchejie.cn/gtkaslymor.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cucudq.cn/gttvuwgvwn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jqgufenzy.top/gthddotqnv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gogol.net.cn/gttegxibwp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.mhx1999.top/gtkihtileb.html

[K05] 深拷贝对象
来源：http://hz.sysykeji.top/gtseejpnyn.html

Py:   copy.deepcopy(obj)
来源：http://hz.ppjwa.cn/gtyotfkmri.html

PHP:  unserialize(serialize($obj));
来源：http://hz.guannengcc.top/gtoledcwng.html

JS:   structuredClone(obj)
来源：http://hz.birdmap.top/gtbfidjeww.html

TS:   structuredClone(obj)
来源：http://hz.jiagoushi.top/gtdehsscjq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.feifeiyinyue.top/gtgawrmfgh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.fzhhl.top/gtklztbtpz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.wangshuangyany.cn/gtiarvrtei.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.smart0.xyz/gtfxsyjrua.html

[K06] 解析 URL 查询串
来源：http://hz.jiagoushi.top/gtocsnjgsl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.bjfxy.top/gtrvixtgyx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jqgufenzy.top/gtasvlgsux.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xuanzx.com/gtejlekhth.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.svipenyu.cn/gtcfkubmwm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.meibo888.top/gtfrppfqqf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.tanke756.top/gtiglqdnjm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.fzhhl.top/gtfdupsptr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cdnleiting.top/gtjufuqjwf.html

[K07] 进制转换
来源：http://hz.gotoacloud.top/gtmrabcwpd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.gaohongyu789.top/gtfkrhcjrd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shanyushiyangtech.top/gtofmgaswk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.cheryme.top/gtwxvhdjqo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.tanke756.top/gtzumkdldt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtyagjrpqm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.shanyushiyangkeji.top/gtrizdoixz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sweek.top/gteouuqfng.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hywenlv.cn/gtqkiarcfv.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.aibaodan.cn/gtoigubblv.html

Py:   pickle.dumps(obj)
来源：http://hz.yueranfly.top/gtkilizlig.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinyuanbaomall.cn/gtawcppiae.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jiagoushi.top/gtgdmvkksu.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.c1oappe.top/gtljmyvuak.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yangfankeji.com/gthfsssqxm.html

Go:   encoding/gob
来源：http://hz.cheryme.top/gtlkdrnaxq.html

Ruby: Marshal.dump(obj)
来源：http://hz.pengpengdd.cyou/gtgxrjejfz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xinyue.icu/gtumlnimkd.html

================================================================================
来源：http://hz.jianghu66.top/gtfthzypbz.html

L. 网络请求
来源：http://hz.pycfn.com/gtikxgpebj.html

================================================================================
来源：http://hz.smart0.xyz/gtdhyqnpui.html

[L01] 发送 GET 请求
来源：http://hz.pengpengdd.cyou/gtthnhwkch.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.chenzaomai.com/gtrxxvpndu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.fengsongda.top/gtqoaaikih.html

JS:   await fetch(url)
来源：http://hz.gzhubu.top/gtmlmdfsvi.html

TS:   await fetch(url)
来源：http://hz.shzxlz.cn/gtkgdkaxlv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.quarkkingdee.top/gtcttkyayh.html

Go:   resp, err := http.Get(url)
来源：http://hz.xinyue.icu/gtjvnapkkt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sysykeji.top/gtxqaotzxy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yueranfly.top/gtdknalwsl.html

[L02] 发送 POST JSON
来源：http://hz.yvedp.cn/gtrmylhmtb.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.andypj.xyz/gtdvgngesd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ydjk.org.cn/gtyefslbym.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.svipenyu.cn/gtvxlrlfkl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cashguo.top/gtlsrrdohj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ydzc1.top/gtcrlpzhtg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jlsjyb.cn/gtsjgokugi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.pengpengdd.cyou/gtmhcaoroh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jyoumei.cn/gtrwuvanei.html

[L03] 设置自定义请求头
来源：http://hz.ivvv.top/gtzzeyaans.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.chenzaomai.com/gtlfpdeimd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hfpthk.cn/gtjhtxkoqr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ehwqpu.com/gtchrshoty.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cdnleiting.top/gtzhqroyun.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zdqjudy.top/gtguwejzmb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ivvv.top/gtnorpojkh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cdnleiting.top/gtnqtaczna.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.guannengcc.top/gtgixsgriv.html

[L04] 设置超时
来源：http://hz.ivvv.top/gtqpzwovsq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.tanke756.top/gtkguayulm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xziqi.cn/gtcwhgbgvs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhiwuduotai.top/gtzwyavtyf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenlongwang.top/gtmitqarvp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yueranfly.top/gtngafsxxw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.tianlin.xyz/gtqoemzhlk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ybcxt.top/gtbyypumxm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.feifeiyinyue.top/gtbaayewpt.html

[L05] 上传文件（multipart）
来源：http://hz.yj20258.top/gtvvqlphwo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hongshengwenyu.top/gtxgaxcaup.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhijiandao.cn/gthfkzrawd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.fengsongda.top/gtwbiaxvia.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.feifeiyinyue.top/gthokiltzf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yuanzhike.top/gtxhqrilng.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jqgfzy.top/gtmvjvhbtk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yonumen.top/gttogyuzeo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yanxiufei.cn/gtledrtxev.html

[L06] 解析响应为 JSON
来源：http://hz.yuxming.cn/gtbnrpqgee.html

Py:   resp.json()
来源：http://hz.pengpengdd.cyou/gtwygyarry.html

PHP:  json_decode($body, true);
来源：http://hz.birdmap.top/gtgsbykygz.html

JS:   await resp.json()
来源：http://hz.hywenlv.cn/gtvmuewxva.html

TS:   await resp.json()
来源：http://hz.hammf.cn/gtcisdiyuw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.pengpengdd.cyou/gtlzasxyxm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sysykeji.top/gtnczxkuhv.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tianlin.xyz/gtvcckyuwx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xziqi.cn/gtyhtdpvdg.html

[L07] 处理 HTTP 状态码
来源：http://hz.shuidangran.top/gtifhncszq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhaomingkeji.xyz/gtcnrrocsc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.tian-w.cn/gtynljllpy.html

JS:   resp.ok;  resp.status
来源：http://hz.tianlin.xyz/gtpdehiskv.html

TS:   resp.ok;  resp.status
来源：http://hz.guowangkeji.top/gtzgswekmc.html

Java: resp.statusCode()
来源：http://hz.shanyushiyangtech.top/gtkycqrlml.html

Go:   resp.StatusCode
来源：http://hz.shanyushiyangkeji.top/gtjiapdqgm.html

Ruby: resp.code.to_i
来源：http://hz.sweek.top/gtzuqxzvuu.html

C#:   (int)resp.StatusCode
来源：http://hz.tian-w.cn/gtinyipmet.html

[L08] 并发请求多个地址
来源：http://hz.sxryk.cn/gtxaelanuk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhongyouzk.top/gtkdrwcdco.html

PHP:  curl_multi_init() 系列
来源：http://hz.fzhhl.top/gtfcjexnhp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhengqikj.top/gteyaultoc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pycfn.com/gtoqvklfzl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ywan-chungtsiang.top/gtwhgzuisl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yongpay.top/gtzoxsftvs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhixingplan.top/gtoljjmurt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.nanxinkj.top/gtkxwvipcs.html

================================================================================
来源：http://hz.ybcxt.top/gtcalfdcng.html

M. 命令行 / 进程 / 环境
来源：http://hz.hfpthk.cn/gtjhkhaqbp.html

================================================================================
来源：http://hz.zdqjudy.top/gtexklchfs.html

[M01] 读取命令行参数
来源：http://hz.chenzaomai.com/gtahxmianu.html

Py:   sys.argv[1:]
来源：http://hz.zhoulong.xyz/gtchbjylyb.html

PHP:  $argv;  $argc;
来源：http://hz.sysykeji.top/gtxyrpoles.html

JS:   process.argv.slice(2)
来源：http://hz.hnqzz.top/gtcprlszik.html

TS:   process.argv.slice(2)
来源：http://hz.zycfv.cn/gtpbnavqiv.html

Java: args 数组（main 方法参数）
来源：http://hz.tianlin.xyz/gtpmqzogsz.html

Go:   os.Args[1:]
来源：http://hz.cheryme.top/gtczgwyozc.html

Ruby: ARGV
来源：http://hz.birdmap.top/gtushjodqg.html

C#:   args 数组（Main 方法参数）
来源：http://hz.smart0.xyz/gtcfqkdriv.html

[M02] 读取环境变量
来源：http://hz.xylfe.cn/gtqckubugk.html

Py:   os.environ.get("HOME")
来源：http://hz.yj20258888.top/gtcgagrbyf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zycfv.cn/gtfhigvsbd.html

JS:   process.env.HOME
来源：http://hz.jianghu66.top/gtyhcpjjiv.html

TS:   process.env.HOME
来源：http://hz.feifeiyinyue.top/gtqsacdwcp.html

Java: System.getenv("HOME")
来源：http://hz.vqdsnc.cn/gtzdhrthkm.html


<!-- 参考信息 -->