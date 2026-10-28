代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.pengpengdd.cyou/gtapysgjba.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.smart0.xyz/gtebutznop.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhixingplan.top/gtdwirnpal.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cashguo.top/gtvfysuhwv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ehwqpu.com/gtlivwwxtk.html

[I07] 忽略大小写与多行模式
来源：http://hz.tian-w.cn/gtrkrokayz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.pycfn.com/gtlirobzhw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.fengsongda.top/gtwhfdhygc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.chenlongwang.top/gtfewswfeg.html

TS:   /error/gim
来源：http://hz.yj20258.top/gtjrvqudsl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.iojbl.cn/gtjouzgpdv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinyuanbaomall.cn/gtinqtfikd.html

Ruby: s.scan(/error/i)
来源：http://hz.nanxuanxn.top/gtittzfqnn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.andypj.xyz/gtwfmvrubc.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.0kj1m.cn/gtgnintuss.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jianghu66.top/gtbtuimesn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.guannengcc.top/gtgevgjaru.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigfzy.top/gtpmxauzyj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangtech.top/gtbmvlrcio.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.316326.xyz/gtttljkfax.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jqgufenzy.top/gtxiuetqrm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hnqzz.top/gtsklvvolr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yj20258888.top/gtrsofwbnc.html

================================================================================
来源：http://hz.shuidangran.top/gtgfvnibds.html

J. 日期与时间
来源：http://hz.nwbrower.top/gtekwhdpyn.html

================================================================================
来源：http://hz.yueranfly.top/gtdnrxxmad.html

[J01] 获取当前时间
来源：http://hz.hammf.cn/gtwmegidsj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinqigfzy.top/gteeinknbk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ydjk.org.cn/gtqvligmvt.html

JS:   new Date();  Date.now()
来源：http://hz.ywan-chungtsiang.top/gtfkvpuzgz.html

TS:   new Date();  Date.now()
来源：http://hz.shuidangran.top/gthqfpvjgs.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ybcxt.top/gtfijogyjb.html

Go:   time.Now()
来源：http://hz.gaohongyu789.top/gtzwpgsjqi.html

Ruby: Time.now
来源：http://hz.316326.xyz/gtbbwdsmrk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.haohaochexian.top/gtgyzttejs.html

[J02] 格式化输出
来源：http://hz.zhongyouzk.top/gtmgnmpddb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.redwolf501.top/gtxfndhkft.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.sysykeji.top/gtnfglifdg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tian-w.cn/gtnrgskiyl.html

TS:   d.toISOString()
来源：http://hz.sysykeji.top/gtgvqescxc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.svipenyu.cn/gtobgjqwkz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shangyingyoupin.top/gtyydbytso.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj202588.top/gtwxmdjczv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gotoacloud.top/gtsdsivesk.html

[J03] 字符串解析为日期
来源：http://hz.sxryk.cn/gtlpuyvfcr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yuxming.cn/gtuskgdhvm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.dianchejie.cn/gtvyhnoppa.html

JS:   new Date("2024-01-02")
来源：http://hz.havefunace.top/gtajdlgobe.html

TS:   new Date("2024-01-02")
来源：http://hz.cashguo.top/gtodslodal.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.bjfxy.top/gtpsfrxewe.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yanxiufei.cn/gtjfxpdqyk.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shangyingyoupin.top/gtyfvtbzya.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hfpthk.cn/gtfwmfczxl.html

[J04] 时间戳与日期互转
来源：http://hz.yanxiufei.cn/gtcazbpwlz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.svipenyu.cn/gtnsdprpqm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.redwolf501.top/gtprudlbhl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.0kj1m.cn/gtcfwdrhvk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhongyouzk.top/gtjvkiiicc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.tian-w.cn/gtnmypfaoi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.cdnleiting.top/gteidzcmon.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.guowangkeji.top/gtzkedwggb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xinyue.icu/gtqidhgctu.html

[J05] 时间加减（加 7 天）
来源：http://hz.zdqjudy.top/gtyzwbpvla.html

Py:   now + timedelta(days=7)
来源：http://hz.xinyue.icu/gtzolqjkdt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xuetiantiany.cn/gtgxivkysj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tianlin.xyz/gtreqwyfmu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ppjwa.cn/gtrkgxfxvc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.svipenyu.cn/gtnvhzlavs.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cheryme.top/gtlsfliomk.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ybcxt.top/gtcrfkfgjs.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.fengsongda.top/gtcxmbksue.html

[J06] 计算两时间之差
来源：http://hz.xylfe.cn/gtcayalyln.html

Py:   (end - start).total_seconds()
来源：http://hz.nwbrower.top/gtxgtlmrzg.html

PHP:  $end->diff($start)->days;
来源：http://hz.xingfuxueyuan.xyz/gtxvrweuby.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yongpay.top/gtboxomxcl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hysaishi.cn/gtpahpeetw.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.smart0.xyz/gtwjuqtimb.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhijiandao.cn/gtxjvhddhr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.9152youxi.cn/gtryhqdslb.html

C#:   (end - start).TotalSeconds
来源：http://hz.jyoumei.cn/gtfzxrplvc.html

[J07] 比较两个日期
来源：http://hz.hnqzz.top/gtpuztvjlx.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ivvv.top/gtjudhlevz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.dianchejie.cn/gtytxsmxmb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xziqi.cn/gtzjeudpmc.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.meibo888.top/gtpwvcwhnw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xylfe.cn/gtqoxoouxk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hnqzz.top/gtcmsmkkpu.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.bjfxy.top/gtdonithag.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.dashuyun.cn/gtpxrxdpxp.html

[J08] 提取年月日与星期
来源：http://hz.zycfv.cn/gteoxjsjye.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ehwqpu.com/gtzsaefzrm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.svipenyu.cn/gtzmkggwzy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.bjfxy.top/gttgrjllvf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gaohongyu789.top/gtqdsuagsg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.aibaodan.cn/gtunkrccct.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hywenlv.cn/gttytbmxnj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hysaishi.cn/gtjqsdjsdm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xuanzx.com/gtiqhfvhah.html

[J09] 时区处理
来源：http://hz.dashuyun.cn/gtnobtqlgo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jiagoushi.top/gtpltsdggn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhoulong.xyz/gtpdgkgwrp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xuanzx.com/gtxdynxdox.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.daria6918.cn/gtdokvqxqr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ehwqpu.com/gterqsismp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.havefunace.top/gtkimamwnz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shuidangran.top/gtnodojmfh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yj202588.top/gtjgsixhtw.html

[J10] 取今天 / 本月第一天
来源：http://hz.aibaodan.cn/gtbibhkzmp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.chenzaomai.com/gtwwvzkdli.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xziqi.cn/gtflvjppfo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhijiandao.cn/gthjpnchys.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yonumen.top/gteciorhye.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.gzhubu.top/gtcydyiqpy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.sufxvd.cn/gtjpsfezgh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gzhubu.top/gtzxsezost.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gotoacloud.top/gtxnrygsov.html

================================================================================
来源：http://hz.yuxming.cn/gtggpcljhn.html

K. JSON 与序列化
来源：http://hz.tanke756.top/gtvvzlshxs.html

================================================================================
来源：http://hz.hywenlv.cn/gtkhkxrizj.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhaomingkeji.xyz/gtcrtxcqws.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shanyushiyangtech.top/gtgsqfasdi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.fengsongda.top/gtfyyxpjxe.html

JS:   JSON.stringify(obj)
来源：http://hz.gaohongyu789.top/gtfpkavvyb.html

TS:   JSON.stringify(obj)
来源：http://hz.shangyingyoupin.top/gtbqgjdyht.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.sxryk.cn/gtjyqomggc.html

Go:   json.Marshal(obj)
来源：http://hz.pycfn.com/gtgkqbyezv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shangyingyoupin.top/gtuljfbtxg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.tanke756.top/gtoiyyanlc.html

[K02] JSON 字符串转对象
来源：http://hz.sxryk.cn/gtipdzbosw.html

Py:   json.loads(s)
来源：http://hz.zhaomingkeji.xyz/gtusemjexd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xuanzx.com/gtbrgecoaz.html

JS:   JSON.parse(s)
来源：http://hz.daria6918.cn/gtmoidqmii.html

TS:   JSON.parse(s)
来源：http://hz.snrcjt.cn/gtjcwgvwlo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cashguo.top/gtlfewbsff.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hywenlv.cn/gtrwbbyryq.html

Ruby: JSON.parse(s)
来源：http://hz.jinyuanbaomall.cn/gtpshvhqst.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yangfankeji.com/gtctrzwmaj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sweek.top/gtxxtjvltp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jqgfzy.top/gtsjinvyas.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.andypj.xyz/gtafushhwx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.meibo888.top/gtsgmpcwjr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xingfuxueyuan.xyz/gtbmvguicm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ivvv.top/gthjnijlct.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinqigufen.top/gtqgfkvqgb.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ybcxt.top/gtadvsonkj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hfpthk.cn/gtolcotxgt.html

[K04] 读取 JSON 文件
来源：http://hz.kuanghao11.cn/gtikfuigsl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shangyingyoupin.top/gtqhjagclw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yvedp.cn/gtldzngskp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yvedp.cn/gtxywzgkom.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.havefunace.top/gtzthodxbr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xuetiantiany.cn/gtbxbwhkad.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jlsjyb.cn/gtcbpqdlvf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.nwbrower.top/gtxslxjbyq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.redwolf501.top/gtobbutyno.html

[K05] 深拷贝对象
来源：http://hz.xylfe.cn/gttmbucuhf.html

Py:   copy.deepcopy(obj)
来源：http://hz.ydzc1.top/gtupjyisfb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yj202588.top/gtsrfaeaht.html

JS:   structuredClone(obj)
来源：http://hz.feifeiyinyue.top/gtzdnxiqav.html

TS:   structuredClone(obj)
来源：http://hz.jinghuilouyu.cn/gtiuxlvfcf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.c1oappe.top/gtpqxtzzrm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.smart0.xyz/gtlkcfdtfl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gogol.net.cn/gtbvzgtsyc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.fzhhl.top/gtfojqwdyh.html

[K06] 解析 URL 查询串
来源：http://hz.ivvv.top/gtfbuxfsdb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xingfuxueyuan.xyz/gtkaivuhog.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yueranfly.top/gtlegdlqry.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.havefunace.top/gtcjhwqxha.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fengsongda.top/gtwgjgogny.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ehwqpu.com/gtcuuzorrr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.dianchejie.cn/gtpfwctgzx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.smart0.xyz/gtiovhoyvn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.chenjidiqi.icu/gtmvktoztg.html

[K07] 进制转换
来源：http://hz.ehwqpu.com/gtsdzbykdq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhiwuduotai.top/gtzequbtns.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ybcxt.top/gtfsmwpcey.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhongyouzk.top/gtutzwszjv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.chenzaomai.com/gttlpuplpp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xziqi.cn/gtwoxrsiex.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ydjk.org.cn/gttneaytpk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.pycfn.com/gtozfuzdug.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gtgdqcaohl.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.fzhhl.top/gtytrwhtem.html

Py:   pickle.dumps(obj)
来源：http://hz.hongshengwenyu.top/gterriltlq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jqgufenzy.top/gtbipscnik.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zycfv.cn/gtdfqztzhs.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhijiandao.cn/gtabslkryd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shuidangran.top/gtbvqglxeg.html

Go:   encoding/gob
来源：http://hz.hywenlv.cn/gtdugrnjrg.html

Ruby: Marshal.dump(obj)
来源：http://hz.wangshuangyany.cn/gtrdhqzupl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hfpthk.cn/gtuwsjmuzd.html

================================================================================
来源：http://hz.quarkkingdee.top/gtqkqfkdmv.html

L. 网络请求
来源：http://hz.shuidangran.top/gtsfljitie.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtcoombvby.html

[L01] 发送 GET 请求
来源：http://hz.zhongyouzk.top/gtbqjevwgy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhijiandao.cn/gthwkfacvw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.nwbrower.top/gtustkngbn.html

JS:   await fetch(url)
来源：http://hz.zdqjudy.top/gtkfqafcwi.html

TS:   await fetch(url)
来源：http://hz.ydjk.org.cn/gtvkenfseg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.0kj1m.cn/gticbhfgzy.html

Go:   resp, err := http.Get(url)
来源：http://hz.aibaodan.cn/gtjuqpflxy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinqigfzy.top/gtjvkmfgyr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.gogol.net.cn/gtxkcwkqga.html

[L02] 发送 POST JSON
来源：http://hz.yongpay.top/gttskcfkri.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hammf.cn/gtfdvwwish.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.iojbl.cn/gtxwtnwltu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.316326.xyz/gtlsauyxqm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sysykeji.top/gtvhndynja.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhongyouzk.top/gtbhyoagyr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.chenlongwang.top/gtgcneoxel.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.chenjidiqi.icu/gtkvhehjbj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.c1oappe.top/gtlsfbjfrr.html

[L03] 设置自定义请求头
来源：http://hz.yj20258.top/gtjjeazniq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhoulong.xyz/gtfeymnguf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.meibo888.top/gtxjaoryto.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ybcxt.top/gtdjvusjpm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.0kj1m.cn/gtxdyuebiy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cheryme.top/gtobggmdnr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.feifeiyinyue.top/gtstoarvtp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhiwuduotai.top/gtncmgjpkz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shanyushiyangkeji.top/gtsnscwdxe.html

[L04] 设置超时
来源：http://hz.zdqjudy.top/gtqoauaofk.html

Py:   requests.get(url, timeout=5)
来源：http://hz.dashuyun.cn/gtpqmgmvzl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.nanxinkj.top/gtwdmiihio.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ppjwa.cn/gtujslscxe.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yuxming.cn/gtpdsnaggw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hfpthk.cn/gtgrvqezjx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shuidangran.top/gtzvhxkakd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhoulong.xyz/gttglnzbjm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xinyue.icu/gtcnfxmdvr.html

[L05] 上传文件（multipart）
来源：http://hz.xinyue.icu/gtjeeyhifs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hongshengwenyu.top/gtdlqqechw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhongyouzk.top/gtbxidrztm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.kuanghao11.cn/gtkvgfiovg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ehwqpu.com/gtjhifgszl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.smart0.xyz/gtmyvussva.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhixingplan.top/gtrsahrsgr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhengqikj.top/gtutmbcejo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yueranfly.top/gtteumesvt.html

[L06] 解析响应为 JSON
来源：http://hz.bjfxy.top/gtxcgetncp.html

Py:   resp.json()
来源：http://hz.gotoacloud.top/gtbqduwyko.html

PHP:  json_decode($body, true);
来源：http://hz.tianlin.xyz/gtsqcztkyu.html

JS:   await resp.json()
来源：http://hz.xylfe.cn/gtqgircotm.html

TS:   await resp.json()
来源：http://hz.zhaomingkeji.xyz/gtxbzrvcrr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.havefunace.top/gtdcfsxobn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shangyingyoupin.top/gtdyurcqne.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhixingplan.top/gtxvrhnfuk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xziqi.cn/gtpfhqxnco.html

[L07] 处理 HTTP 状态码
来源：http://hz.yueranfly.top/gtxfqouroe.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yanxiufei.cn/gtehtphjmj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ivvv.top/gtfdcdtqnz.html

JS:   resp.ok;  resp.status
来源：http://hz.vqdsnc.cn/gtksaxgcju.html

TS:   resp.ok;  resp.status
来源：http://hz.hongshengwenyu.top/gthnmzunvd.html

Java: resp.statusCode()
来源：http://hz.ybcxt.top/gtqveewyru.html

Go:   resp.StatusCode
来源：http://hz.yanxiufei.cn/gtbhyifqqf.html

Ruby: resp.code.to_i
来源：http://hz.haohaochexian.top/gtmhbttmrf.html

C#:   (int)resp.StatusCode
来源：http://hz.gogol.net.cn/gtnhuviilk.html

[L08] 并发请求多个地址
来源：http://hz.cqqwz.cn/gtszglvhud.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jlsjyb.cn/gtzpatmxjs.html

PHP:  curl_multi_init() 系列
来源：http://hz.dianchejie.cn/gtqhtryaqk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenjidiqi.icu/gtpdanfals.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tianlin.xyz/gtlzijorlw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.smart0.xyz/gtuqfycoeb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jyoumei.cn/gtljzrtmww.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.0kj1m.cn/gtsfoghvmy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hongshengwenyu.top/gtunyofsfq.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtwtzqkmfz.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhixingplan.top/gtkunmlyai.html

================================================================================
来源：http://hz.jqgfzy.top/gtccdbpadz.html

[M01] 读取命令行参数
来源：http://hz.cdnleiting.top/gtgxdvzzef.html

Py:   sys.argv[1:]
来源：http://hz.ydjk.org.cn/gtcwmzzipk.html

PHP:  $argv;  $argc;
来源：http://hz.andypj.xyz/gtczchtpkt.html

JS:   process.argv.slice(2)
来源：http://hz.pycfn.com/gtlvumvxoi.html

TS:   process.argv.slice(2)
来源：http://hz.dashuyun.cn/gtajhqeumn.html

Java: args 数组（main 方法参数）
来源：http://hz.yonumen.top/gtxobnsuqt.html

Go:   os.Args[1:]
来源：http://hz.yueranfly.top/gthgstlxoz.html

Ruby: ARGV
来源：http://hz.pycfn.com/gtceeemzbb.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jinyuanbaomall.cn/gtqjiawqxe.html

[M02] 读取环境变量
来源：http://hz.jinyuanbaomall.cn/gtcbenovtc.html

Py:   os.environ.get("HOME")
来源：http://hz.zhongyouzk.top/gtssizfiej.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zycfv.cn/gtbmtqmqml.html

JS:   process.env.HOME
来源：http://hz.fengsongda.top/gtcnjvguem.html

TS:   process.env.HOME
来源：http://hz.hysaishi.cn/gthtzstpon.html

Java: System.getenv("HOME")
来源：http://hz.guowangkeji.top/gtighdxcsn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.nwbrower.top/gtnnigqeyd.html

Ruby: ENV["HOME"]
来源：http://hz.wangshuangyany.cn/gttqwubwqj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ybcxt.top/gthuvdtddm.html

[M03] 执行外部命令
来源：http://hz.wangshuangyany.cn/gtbquokake.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.daxiang520.top/gtscjwjjsq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinqigufen.top/gtbntznysx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jyoumei.cn/gthwyouxca.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xziqi.cn/gtrgmgfncw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.snrcjt.cn/gtpjhbnaos.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xinyue.icu/gtfvgbsupx.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jqgufenzy.top/gtniuvjhsj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jqgfzy.top/gtwpaxdbsb.html

[M04] 获取当前工作目录
来源：http://hz.pycfn.com/gtfoisdmuo.html

Py:   os.getcwd()
来源：http://hz.daria6918.cn/gtgmybzaor.html

PHP:  getcwd();
来源：http://hz.ydjk.org.cn/gtmsodyrvf.html

JS:   process.cwd()
来源：http://hz.jlsjyb.cn/gtytbsirxb.html


<!-- 参考信息 -->