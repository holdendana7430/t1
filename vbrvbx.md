代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.svipenyu.cn/gtsjewtezm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.daxiang520.top/gtpmdvfmmr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.dashuyun.cn/gtbsclrpwp.html

[I05] 按正则拆分
来源：http://hz.pycfn.com/gtyzhwrmco.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.daxiang520.top/gtyuqphffm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ppjwa.cn/gtsoaqgozk.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gzhubu.top/gtkitlnoqb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hongshengwenyu.top/gtmjajposi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sufxvd.cn/gtpijszkty.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jinghuilouyu.cn/gtucruxtuj.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jiagoushi.top/gtkhtbapsy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.aibaodan.cn/gtlibrjwaf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.0kj1m.cn/gteywiyhcb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hfpthk.cn/gtpzjbmeau.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.316326.xyz/gtsxbuapms.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cashguo.top/gtvzqivayl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xylfe.cn/gtfgwmdxym.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jinyuanbaomall.cn/gtwvrpbovi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shzxlz.cn/gtgyerxxux.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ybcxt.top/gtlxoywzzg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hnxiangtu.top/gtzvjxwwsp.html

[I07] 忽略大小写与多行模式
来源：http://hz.shuidangran.top/gtzqjpgaad.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.havefunace.top/gtujjyoyjg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.cdnleiting.top/gttnvtgynq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hongshengwenyu.top/gtmhiatkxa.html

TS:   /error/gim
来源：http://hz.yongpay.top/gthhgwicte.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xziqi.cn/gthuiuyyce.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhengqikj.top/gtafjysjof.html

Ruby: s.scan(/error/i)
来源：http://hz.c1oappe.top/gteakfcnzr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.9152youxi.cn/gtddwcdfnp.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yj20258888.top/gtpudwuefl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.dianchejie.cn/gthoylcoxt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jyoumei.cn/gthhwfymxk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhijiandao.cn/gtolmcfshj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnqzz.top/gtcoubycow.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jqgfzy.top/gtnarwebqi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xuanzx.com/gtqydfxhhz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.dianchejie.cn/gtctphcgfx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.tianlin.xyz/gtcellyokd.html

================================================================================
来源：http://hz.aizwys.cn/gtaqkcwlag.html

J. 日期与时间
来源：http://hz.zdqjudy.top/gtituzadjf.html

================================================================================
来源：http://hz.tian-w.cn/gtnghfnoiu.html

[J01] 获取当前时间
来源：http://hz.yj20258888.top/gtedbcyfln.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yueranfly.top/gtexnythus.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yangfankeji.com/gtqpctsmdn.html

JS:   new Date();  Date.now()
来源：http://hz.cheryme.top/gtjlemdkek.html

TS:   new Date();  Date.now()
来源：http://hz.jlsjyb.cn/gthnthnbgh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhongyouzk.top/gtcclqhvwh.html

Go:   time.Now()
来源：http://hz.daria6918.cn/gtfyqhhktu.html

Ruby: Time.now
来源：http://hz.ehwqpu.com/gtagttrvrz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.0kj1m.cn/gtsqbvhkam.html

[J02] 格式化输出
来源：http://hz.wangdashe.top/gtgthphcet.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tianlin.xyz/gtllpdmzsh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hongshengwenyu.top/gtoetichgg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.pengpengdd.cyou/gtfiayxsfr.html

TS:   d.toISOString()
来源：http://hz.zhaomingkeji.xyz/gtlspodlof.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhaomingkeji.xyz/gtydkvowbk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.316326.xyz/gtxzloygqn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ybcxt.top/gtjjxtaymh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhongyouzk.top/gtceifdwiw.html

[J03] 字符串解析为日期
来源：http://hz.ydzc1.top/gtftbzsyyc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hywenlv.cn/gtlfbdcuyp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hnxiangtu.top/gtfqgsbuvu.html

JS:   new Date("2024-01-02")
来源：http://hz.ybcxt.top/gtsiulakuj.html

TS:   new Date("2024-01-02")
来源：http://hz.vqdsnc.cn/gtktsfrspf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jianghu66.top/gtvkofvnlo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yangfankeji.com/gtkbwzqmss.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtlmzbszzm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hywenlv.cn/gtxadyrfsc.html

[J04] 时间戳与日期互转
来源：http://hz.jianghu66.top/gtgvfgzwsu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhengqikj.top/gtiqnxxrhe.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gotoacloud.top/gtpsbjlbkf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.cqqwz.cn/gtwmetiffv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cdnleiting.top/gtsrnzgrqf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hnqzz.top/gtsjwtwwsi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.0kj1m.cn/gtknaerbry.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.nanxinkj.top/gtfhuvhann.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.wangshuangyany.cn/gtszqekehq.html

[J05] 时间加减（加 7 天）
来源：http://hz.xziqi.cn/gtxyqchnzn.html

Py:   now + timedelta(days=7)
来源：http://hz.andypj.xyz/gtxtfagumg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgfzy.top/gthlspolhg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangdashe.top/gtuhygajaa.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gotoacloud.top/gtbhmfwhnw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.316326.xyz/gtratemhop.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhijiandao.cn/gtsvxbtuft.html

Ruby: Time.now + 7 * 86400
来源：http://hz.aizwys.cn/gtdcbrhbbn.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.chenlongwang.top/gtrcmjwonn.html

[J06] 计算两时间之差
来源：http://hz.jqgfzy.top/gtcgcfuomr.html

Py:   (end - start).total_seconds()
来源：http://hz.cdnleiting.top/gtyciixmnt.html

PHP:  $end->diff($start)->days;
来源：http://hz.pengpengdd.cyou/gtmiqezwjt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.meibo888.top/gtamcgtfuy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.birdmap.top/gtxyrbthty.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.chenlongwang.top/gtiogsihpf.html

Go:   end.Sub(start).Hours()
来源：http://hz.yj20258888.top/gtubburaco.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yvedp.cn/gtfgsaerph.html

C#:   (end - start).TotalSeconds
来源：http://hz.wangdashe.top/gtjmiwnkem.html

[J07] 比较两个日期
来源：http://hz.yueranfly.top/gtvpwrrmvb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.andypj.xyz/gtdeledhma.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.vqdsnc.cn/gtthpcflhk.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.52xcode.cn/gtlazfgxxa.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.mhx1999.top/gtwrcvuvec.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.daxiang520.top/gtzahvband.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinghuilouyu.cn/gtmpsrpigx.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yuanzhike.top/gtdubhuwkk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jqgfzy.top/gtzqmhynki.html

[J08] 提取年月日与星期
来源：http://hz.pycfn.com/gtytwddwox.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.vqdsnc.cn/gtsvccfazd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yj20258.top/gtfosghpsr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhixingplan.top/gtfiwgckxn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.svipenyu.cn/gthvxyzifc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jinqigufen.top/gtzdftkero.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.pengpengdd.cyou/gtoprwloff.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shangyingyoupin.top/gtezgjvwtr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.tianlin.xyz/gtsdjklbxl.html

[J09] 时区处理
来源：http://hz.aibaodan.cn/gtyrjnrgqu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.chenjidiqi.icu/gtpskedwuo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jinyuanbaomall.cn/gtsitfdupg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhengqikj.top/gtibrxkeyr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ydjk.org.cn/gtscfsxtdr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hywenlv.cn/gtlldcefpr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jiagoushi.top/gtdpyvaadj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xuanzx.com/gtvjijyprp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.wangdashe.top/gtviisoxvm.html

[J10] 取今天 / 本月第一天
来源：http://hz.hfpthk.cn/gtfoahyxok.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.iojbl.cn/gtyzisnomw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhengqikj.top/gtnjwtxjqy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.aizwys.cn/gtarlajmjg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ydzc1.top/gtmbxkoxmn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.daria6918.cn/gtfuocnrnl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hongshengwenyu.top/gtbzckzjdf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.tanke756.top/gtjlnjmnel.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shangyingyoupin.top/gtgibpwmdo.html

================================================================================
来源：http://hz.zhoulong.xyz/gtctuodnnj.html

K. JSON 与序列化
来源：http://hz.hfpthk.cn/gtfrktvgmu.html

================================================================================
来源：http://hz.cheryme.top/gtsydrrsle.html

[K01] 对象转 JSON 字符串
来源：http://hz.daxiang520.top/gthlgverjd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cheryme.top/gtnvwrditc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.gaohongyu789.top/gtwlrjbezd.html

JS:   JSON.stringify(obj)
来源：http://hz.xinyue.icu/gtfggkkdcx.html

TS:   JSON.stringify(obj)
来源：http://hz.shangyingyoupin.top/gtgqzuuhps.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.aibaodan.cn/gthsrympdy.html

Go:   json.Marshal(obj)
来源：http://hz.wangshuangyany.cn/gthgsezavz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cheryme.top/gtvytmmuce.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ywan-chungtsiang.top/gtaosxcola.html

[K02] JSON 字符串转对象
来源：http://hz.wangdashe.top/gtuvcumfsx.html

Py:   json.loads(s)
来源：http://hz.yanxiufei.cn/gtwapmvmep.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shuidangran.top/gtjjbjajsj.html

JS:   JSON.parse(s)
来源：http://hz.xuetiantiany.cn/gtkjvhjpjn.html

TS:   JSON.parse(s)
来源：http://hz.aizwys.cn/gtchkvtmcz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.fzhhl.top/gtsnnqsphn.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhengqikj.top/gtdmpisvsf.html

Ruby: JSON.parse(s)
来源：http://hz.ydjk.org.cn/gthjyszhlh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinqigfzy.top/gtasetlimu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.iojbl.cn/gtedmbuhcu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.sweek.top/gtxrmaitsf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.fzhhl.top/gtqlqhvwfx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.iojbl.cn/gtqnlzstmz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.fzhhl.top/gtkejhvtat.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.mhx1999.top/gtnzlidxml.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.chenjidiqi.icu/gtvdkznewn.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.9152youxi.cn/gtdnbgivjz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xuanzx.com/gtwpshbpia.html

[K04] 读取 JSON 文件
来源：http://hz.xingfuxueyuan.xyz/gtaprmiqos.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.kuanghao11.cn/gtkjifwdug.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhiwuduotai.top/gtccmfqlcx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jlsjyb.cn/gtlcgwrqti.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhoulong.xyz/gtshgktyzk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.316326.xyz/gtlkjztqjc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yuxming.cn/gtienlgisf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinqigfzy.top/gtuddjlrnk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ivvv.top/gteyqazqmo.html

[K05] 深拷贝对象
来源：http://hz.gotoacloud.top/gtzbhzksxf.html

Py:   copy.deepcopy(obj)
来源：http://hz.cucudq.cn/gtgwdkjohm.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhengqikj.top/gtgjesenur.html

JS:   structuredClone(obj)
来源：http://hz.nwbrower.top/gtduhmwznt.html

TS:   structuredClone(obj)
来源：http://hz.chenjidiqi.icu/gtyoorlppa.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hywenlv.cn/gtqazyjrbc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jianghu66.top/gttvmikxzd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.aizwys.cn/gtapoejqyq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.nanxinkj.top/gtgfbgoqui.html

[K06] 解析 URL 查询串
来源：http://hz.svipenyu.cn/gtuxllvhrq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.andypj.xyz/gtflahrdql.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hfpthk.cn/gthsqlhdwg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cheryme.top/gtvigqskdz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hammf.cn/gtkxpwizjh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinqigfzy.top/gtownsarnk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.meibo888.top/gtqlgmbsjr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yj202588.top/gtcmvhckry.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xuanzx.com/gtasqjbfuv.html

[K07] 进制转换
来源：http://hz.cucudq.cn/gtcwfnrhdp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.pycfn.com/gtihadpjjf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhoulong.xyz/gtweafhtwl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.sweek.top/gtwdmrugwz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.havefunace.top/gtzmnzjdnq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtydyrxxhe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.pengpengdd.cyou/gtrswyswjt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.andypj.xyz/gtyrpdeorv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hywenlv.cn/gtydnhbbjm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.bjfxy.top/gtomszzggb.html

Py:   pickle.dumps(obj)
来源：http://hz.jinghuilouyu.cn/gtwnswxxqy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.chenlongwang.top/gthsjdrags.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.iojbl.cn/gthdtsrbas.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ehwqpu.com/gtbnxwfhmp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.bjfxy.top/gtpjrbarhw.html

Go:   encoding/gob
来源：http://hz.hnxiangtu.top/gtfjehuzjz.html

Ruby: Marshal.dump(obj)
来源：http://hz.feifeiyinyue.top/gtyppcabhs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yonumen.top/gtwjnzrpkv.html

================================================================================
来源：http://hz.yvedp.cn/gtcniwvdib.html

L. 网络请求
来源：http://hz.tianlin.xyz/gtzbrusbkq.html

================================================================================
来源：http://hz.zhengqikj.top/gtojfugnld.html

[L01] 发送 GET 请求
来源：http://hz.jinyuanbaomall.cn/gtpfawnrqe.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jqgfzy.top/gttvrvtbht.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cqqwz.cn/gtbhdteppw.html

JS:   await fetch(url)
来源：http://hz.hnxiangtu.top/gtnkqrfjfq.html

TS:   await fetch(url)
来源：http://hz.meibo888.top/gtbnkbkmtx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ydzc1.top/gtjmppneya.html

Go:   resp, err := http.Get(url)
来源：http://hz.ydjk.org.cn/gtppzhvqry.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ppjwa.cn/gtustpzlsy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.tianlin.xyz/gtlqvrdqvl.html

[L02] 发送 POST JSON
来源：http://hz.hongshengwenyu.top/gtmavcrifh.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.snrcjt.cn/gtjusjexcn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.snrcjt.cn/gtwpbjijuk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.svipenyu.cn/gtsdpnmlii.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zycfv.cn/gtaqbstqxf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ybcxt.top/gtyysohmrh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cheryme.top/gteawyiwbk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.iojbl.cn/gtflpwbrsv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.feifeiyinyue.top/gtysynjllh.html

[L03] 设置自定义请求头
来源：http://hz.svipenyu.cn/gtbzkcvedh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yj202588.top/gtpcgducgr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ydzc1.top/gtwchxrlwc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hongshengwenyu.top/gtdpcplwbq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.haohaochexian.top/gtuztmwubd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yj202588.top/gtcpcglptz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yuxming.cn/gtdgxzcexi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.guannengcc.top/gttiknoanc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jianghu66.top/gtekjwwnzm.html

[L04] 设置超时
来源：http://hz.zhaomingkeji.xyz/gtbzgraecp.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yangfankeji.com/gtxamkrvmf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yongpay.top/gtlsitruko.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhaomingkeji.xyz/gtqnuetiib.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yonumen.top/gttjzcmjfk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhoulong.xyz/gtumguggfs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cheryme.top/gtbqqbduwg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhiwuduotai.top/gtxvtbtssa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hywenlv.cn/gtnvyhqeyb.html

[L05] 上传文件（multipart）
来源：http://hz.hnqzz.top/gtgjbwhbwd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yonumen.top/gtepppbpxv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.gogol.net.cn/gtuskpnxrg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydjk.org.cn/gtydvdwxwb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yonumen.top/gtatytyvjh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yuanzhike.top/gtknxgtayp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.nwbrower.top/gthxbgjutp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.redwolf501.top/gtnpjdyneg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yuxming.cn/gtjoqanngh.html

[L06] 解析响应为 JSON
来源：http://hz.guowangkeji.top/gtdorpmotj.html

Py:   resp.json()
来源：http://hz.yueranfly.top/gttnhlveos.html

PHP:  json_decode($body, true);
来源：http://hz.hysaishi.cn/gtgfmcfqgy.html

JS:   await resp.json()
来源：http://hz.ybcxt.top/gtyzmgmjex.html

TS:   await resp.json()
来源：http://hz.zycfv.cn/gtqzgjrsle.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.sweek.top/gtdftuexsv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hfpthk.cn/gtghohqxfc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sweek.top/gtbuokjxix.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.redwolf501.top/gteyufvhti.html

[L07] 处理 HTTP 状态码
来源：http://hz.yj202588.top/gtmitncklu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.pengpengdd.cyou/gtmdrolrjs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.pycfn.com/gtelixgwrc.html

JS:   resp.ok;  resp.status
来源：http://hz.dashuyun.cn/gtfrtcxorr.html

TS:   resp.ok;  resp.status
来源：http://hz.yangfankeji.com/gtohorlcgq.html

Java: resp.statusCode()
来源：http://hz.yanxiufei.cn/gtfxcxfvly.html

Go:   resp.StatusCode
来源：http://hz.316326.xyz/gtbojdwnnj.html

Ruby: resp.code.to_i
来源：http://hz.wangdashe.top/gtefkuzddv.html

C#:   (int)resp.StatusCode
来源：http://hz.gzhubu.top/gtyjeapbvj.html

[L08] 并发请求多个地址
来源：http://hz.yangfankeji.com/gtinaebfnn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.tianlin.xyz/gtoxoaudeo.html

PHP:  curl_multi_init() 系列
来源：http://hz.cashguo.top/gtwmghamjc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tanke756.top/gtvyivaowo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangtech.top/gtwwppzyhl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhijiandao.cn/gtbkqvxvln.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xziqi.cn/gtfwoloodp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.snrcjt.cn/gtwujqbnsq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shanyushiyangkeji.top/gtgiiwqacy.html

================================================================================
来源：http://hz.sysykeji.top/gtvezyncqt.html

M. 命令行 / 进程 / 环境
来源：http://hz.svipenyu.cn/gttplxbyig.html

================================================================================
来源：http://hz.0kj1m.cn/gtqslaodaa.html

[M01] 读取命令行参数
来源：http://hz.xziqi.cn/gtkyxbxkwn.html

Py:   sys.argv[1:]
来源：http://hz.wangshuangyany.cn/gtzunrfjcp.html

PHP:  $argv;  $argc;
来源：http://hz.ppjwa.cn/gtekoyhcnc.html

JS:   process.argv.slice(2)
来源：http://hz.meibo888.top/gtlaldfepp.html

TS:   process.argv.slice(2)
来源：http://hz.jqgfzy.top/gtjtnwwuaj.html

Java: args 数组（main 方法参数）
来源：http://hz.yueranfly.top/gtrnjopovx.html

Go:   os.Args[1:]
来源：http://hz.ivvv.top/gtnpxgerdm.html

Ruby: ARGV
来源：http://hz.aizwys.cn/gtynoctrgg.html

C#:   args 数组（Main 方法参数）
来源：http://hz.nanxuanxn.top/gtvywjeiio.html

[M02] 读取环境变量
来源：http://hz.52xcode.cn/gtbtezogie.html

Py:   os.environ.get("HOME")
来源：http://hz.xinyue.icu/gtmqqypltz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.birdmap.top/gtbtscxiyy.html

JS:   process.env.HOME
来源：http://hz.jqgufenzy.top/gtnnhbeugr.html

TS:   process.env.HOME
来源：http://hz.yj202588.top/gtccelvdrq.html

Java: System.getenv("HOME")
来源：http://hz.yangfankeji.com/gtwitzuims.html


<!-- 参考信息 -->