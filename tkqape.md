代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yueranfly.top/gtdzgbyotg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shzxlz.cn/gttnyyitea.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xylfe.cn/gtscqxpjgv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.daria6918.cn/gtjnbqbsoi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhengqikj.top/gtiliojzxp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.smart0.xyz/gtbzrvmdgn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.vqdsnc.cn/gtzbsnddjw.html

[I05] 按正则拆分
来源：http://hz.sxryk.cn/gtwggbmhjr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cashguo.top/gtmdjhognn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.chenzaomai.com/gtkjvmejfa.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.sysykeji.top/gthrrtlelf.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhongyouzk.top/gtzneqlyus.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenlongwang.top/gteshymmpe.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.andypj.xyz/gtzmvknupx.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xuetiantiany.cn/gtqapgyvlz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.dashuyun.cn/gtsqdwrcoq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhongyouzk.top/gtvrchgsab.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.mhx1999.top/gtlrqjnchc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.kuanghao11.cn/gtlrorqjzx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.havefunace.top/gtehselmbv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gtllqzbewo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.chenjidiqi.icu/gtdztvixfb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jinqigufen.top/gtgyioemgn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shuidangran.top/gtmdwdgyhr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhoulong.xyz/gtqihyakph.html

[I07] 忽略大小写与多行模式
来源：http://hz.yanxiufei.cn/gtwsonpxtz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jinqigufen.top/gtwhbkmxaf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.gzhubu.top/gtqdrronco.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.meibo888.top/gtmnptoeze.html

TS:   /error/gim
来源：http://hz.yuanzhike.top/gtwnfnvdnr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.316326.xyz/gtkvuqdliw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shuidangran.top/gtqtbyryla.html

Ruby: s.scan(/error/i)
来源：http://hz.zhijiandao.cn/gttxsxovse.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhiwuduotai.top/gtzycnlgck.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yuanzhike.top/gtdmifwpeg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yj202588.top/gtoitlmbtm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.snrcjt.cn/gtvvzdkjnf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnxiangtu.top/gtjjhasttx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jyoumei.cn/gtbzxwsrvb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.chenlongwang.top/gtkhufyhhn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xylfe.cn/gtfmslwwwo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.wangshuangyany.cn/gtjmdbqrbg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sweek.top/gtrqrgrwvm.html

================================================================================
来源：http://hz.mhx1999.top/gtqwwcqkcs.html

J. 日期与时间
来源：http://hz.aibaodan.cn/gtoskqinkx.html

================================================================================
来源：http://hz.jinqigfzy.top/gtbgkxdpgj.html

[J01] 获取当前时间
来源：http://hz.zhengqikj.top/gtwsvoujzf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.guannengcc.top/gtardpjxrb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jqgfzy.top/gtsojwsndz.html

JS:   new Date();  Date.now()
来源：http://hz.aibaodan.cn/gtnmzsyxmz.html

TS:   new Date();  Date.now()
来源：http://hz.fengsongda.top/gtlevjrchg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.0kj1m.cn/gtuoflhlov.html

Go:   time.Now()
来源：http://hz.yuxming.cn/gtnqmhrasu.html

Ruby: Time.now
来源：http://hz.jinghuilouyu.cn/gtzwzrwjtt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.chenlongwang.top/gtefedoxeq.html

[J02] 格式化输出
来源：http://hz.hongshengwenyu.top/gtxwmtgaqa.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.c1oappe.top/gtvouclwne.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.9152youxi.cn/gtfaupnkea.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shanyushiyangtech.top/gtzxonxohm.html

TS:   d.toISOString()
来源：http://hz.sweek.top/gthztghsje.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhixingplan.top/gtucsorqfv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhijiandao.cn/gtjfxmxphs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nwbrower.top/gtnhccdgbl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.0kj1m.cn/gtbygnviqs.html

[J03] 字符串解析为日期
来源：http://hz.gzhubu.top/gtxacotsqc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.havefunace.top/gtzsehxpds.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sufxvd.cn/gtscpeisgm.html

JS:   new Date("2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtrtvvffed.html

TS:   new Date("2024-01-02")
来源：http://hz.dianchejie.cn/gteasrqgtz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hfpthk.cn/gtqrabrsnh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.redwolf501.top/gtjjtgmuru.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yuxming.cn/gtuuujpucg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hnxiangtu.top/gtrvyrreec.html

[J04] 时间戳与日期互转
来源：http://hz.ivvv.top/gtitxgsjyw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.0kj1m.cn/gttcgmhnsf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sufxvd.cn/gtfbcbgmgl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shuidangran.top/gtracvkmqm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.316326.xyz/gtvhhupqsf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ivvv.top/gtjkcnbxpi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xylfe.cn/gtmydayghj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.chenzaomai.com/gthfokhzer.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.vqdsnc.cn/gtfilnjwmv.html

[J05] 时间加减（加 7 天）
来源：http://hz.hywenlv.cn/gtqwdeuuah.html

Py:   now + timedelta(days=7)
来源：http://hz.ydzc1.top/gtzesccceh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cheryme.top/gtjmtgazao.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nanxuanxn.top/gtdexrxadv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnxiangtu.top/gtzqhhevhv.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.redwolf501.top/gtjuootrxo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hfpthk.cn/gtbtdlmffh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.redwolf501.top/gtklqiscxr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.vqdsnc.cn/gtbshiycke.html

[J06] 计算两时间之差
来源：http://hz.ydzc1.top/gtwtyfxupp.html

Py:   (end - start).total_seconds()
来源：http://hz.zhoulong.xyz/gtkturowkd.html

PHP:  $end->diff($start)->days;
来源：http://hz.yvedp.cn/gtprayrvbl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.nwbrower.top/gtwtarmqik.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.nanxuanxn.top/gtnitknizt.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xziqi.cn/gtrpwqtfsw.html

Go:   end.Sub(start).Hours()
来源：http://hz.shanyushiyangkeji.top/gtmacmtpmb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ybcxt.top/gtgnyongch.html

C#:   (end - start).TotalSeconds
来源：http://hz.dianchejie.cn/gtxkdroyfh.html

[J07] 比较两个日期
来源：http://hz.jinyuanbaomall.cn/gtvliktapl.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.smart0.xyz/gtoyuukwcf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.chenjidiqi.icu/gtmtgkrtfw.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.nwbrower.top/gtcbwmmzxa.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zycfv.cn/gtgrimjskl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yj202588.top/gtlnxscbti.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.aizwys.cn/gtpgrgirix.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xuanzx.com/gtodumrrva.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.pycfn.com/gtptuvsvyg.html

[J08] 提取年月日与星期
来源：http://hz.shanyushiyangtech.top/gtyzwtqhhl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zdqjudy.top/gttjmstudo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.guowangkeji.top/gtltphiehq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.redwolf501.top/gtxgwfidsg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinqigufen.top/gtmnjpsudf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.0kj1m.cn/gtfdrtktnf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cqqwz.cn/gterosaxin.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gzhubu.top/gtbnzykmmb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hywenlv.cn/gtssfelilj.html

[J09] 时区处理
来源：http://hz.ydjk.org.cn/gtftbdiapa.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jlsjyb.cn/gtffvfwbmi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zdqjudy.top/gtvuphifho.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tanke756.top/gtxvrevgxb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shuidangran.top/gtvvwsqfao.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.daria6918.cn/gtsnsokboz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ywan-chungtsiang.top/gtmewxmjqz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.vqdsnc.cn/gtcrlrbapn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.svipenyu.cn/gtflcdmvcb.html

[J10] 取今天 / 本月第一天
来源：http://hz.cucudq.cn/gtiephxljf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cheryme.top/gttjikqjxs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shangyingyoupin.top/gtnpmxyoei.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xuetiantiany.cn/gtikujsfxa.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cheryme.top/gtvhvbnppq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.pycfn.com/gtkuryeiqp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.sysykeji.top/gthqnfaalt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.dianchejie.cn/gtatxazvaa.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.haohaochexian.top/gtglxbhxzb.html

================================================================================
来源：http://hz.yanxiufei.cn/gtlfzrtlin.html

K. JSON 与序列化
来源：http://hz.ehwqpu.com/gtbpenqgxw.html

================================================================================
来源：http://hz.xziqi.cn/gtsppuaubk.html

[K01] 对象转 JSON 字符串
来源：http://hz.sxryk.cn/gtrfrwlorh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.gotoacloud.top/gtxfefgvos.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yuxming.cn/gtfjimqqrl.html

JS:   JSON.stringify(obj)
来源：http://hz.ywan-chungtsiang.top/gthfrtpxyo.html

TS:   JSON.stringify(obj)
来源：http://hz.yangfankeji.com/gtutzudvzs.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.gzhubu.top/gtuwgapshr.html

Go:   json.Marshal(obj)
来源：http://hz.tanke756.top/gtcmvdybzz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xylfe.cn/gtyclbexns.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.quarkkingdee.top/gtqveiaesd.html

[K02] JSON 字符串转对象
来源：http://hz.cqqwz.cn/gtoiaaxlkj.html

Py:   json.loads(s)
来源：http://hz.daria6918.cn/gtaaywzbxz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.chenlongwang.top/gtkjcydwte.html

JS:   JSON.parse(s)
来源：http://hz.zhongyouzk.top/gtgfgfjycr.html

TS:   JSON.parse(s)
来源：http://hz.fengsongda.top/gtyzjrchdg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ppjwa.cn/gtzmwvqkop.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sxryk.cn/gtqjepkzth.html

Ruby: JSON.parse(s)
来源：http://hz.aibaodan.cn/gtfsvloqvz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinqigufen.top/gtpameuihd.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.aibaodan.cn/gtpgcrkypm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhengqikj.top/gtmphnlxvn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jyoumei.cn/gtqlqzkgtn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuetiantiany.cn/gtssicqmoc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.dianchejie.cn/gtlmmtmjxj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hywenlv.cn/gtumokzcmh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.sysykeji.top/gtrrthnflp.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhixingplan.top/gtwgoajxiv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.sufxvd.cn/gtaxmwwjfs.html

[K04] 读取 JSON 文件
来源：http://hz.havefunace.top/gtiirajnay.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.daria6918.cn/gtirkuudly.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.feifeiyinyue.top/gtzuamngcn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gzhubu.top/gtmfzclxed.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.daxiang520.top/gtzuffbpkr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jqgfzy.top/gtbemwgihk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.guannengcc.top/gtlrslwjcv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ybcxt.top/gtaxafdigq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.daxiang520.top/gtwsuzpvid.html

[K05] 深拷贝对象
来源：http://hz.ywan-chungtsiang.top/gtpegstwwo.html

Py:   copy.deepcopy(obj)
来源：http://hz.52xcode.cn/gtqzryeyqw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hnxiangtu.top/gtnvbahanz.html

JS:   structuredClone(obj)
来源：http://hz.tanke756.top/gtifilhzmq.html

TS:   structuredClone(obj)
来源：http://hz.yuxming.cn/gthyfsvwnt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shangyingyoupin.top/gtsdnoauwl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yanxiufei.cn/gtjunraxnw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhaomingkeji.xyz/gtbmxemfex.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jinyuanbaomall.cn/gtardphcco.html

[K06] 解析 URL 查询串
来源：http://hz.jqgufenzy.top/gtomfdtmqg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hfpthk.cn/gtzdlwinhr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.nanxinkj.top/gthbkeuuqg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.vqdsnc.cn/gtnenabbio.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxinkj.top/gtpquzqfvw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj20258.top/gtbtzsejik.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.chenzaomai.com/gtwwdiqcks.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.pengpengdd.cyou/gtxstandxn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.wangdashe.top/gtdzoxcqey.html

[K07] 进制转换
来源：http://hz.ivvv.top/gtwonvmjpo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.dashuyun.cn/gtdhopqdao.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.0kj1m.cn/gtehctsbxt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.dashuyun.cn/gthrppqsyp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtbfqjered.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tian-w.cn/gtqfclmldt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.316326.xyz/gtlxuqttul.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.havefunace.top/gttizknduf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.316326.xyz/gtufmiftxq.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.smart0.xyz/gthrbyqxnh.html

Py:   pickle.dumps(obj)
来源：http://hz.c1oappe.top/gtjwhmffyv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.guowangkeji.top/gtaocgumhl.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.pycfn.com/gtkldomhbf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.tian-w.cn/gtfjxrgiet.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ivvv.top/gtxoqzxnpf.html

Go:   encoding/gob
来源：http://hz.jlsjyb.cn/gthlulhxjm.html

Ruby: Marshal.dump(obj)
来源：http://hz.zdqjudy.top/gtzmhofqtv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ybcxt.top/gtcobxjpfo.html

================================================================================
来源：http://hz.meibo888.top/gtgebrzspy.html

L. 网络请求
来源：http://hz.feifeiyinyue.top/gtrolevgxs.html

================================================================================
来源：http://hz.yj202588.top/gtpebhyvys.html

[L01] 发送 GET 请求
来源：http://hz.nanxinkj.top/gtkkxerdsk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.9152youxi.cn/gtbynrrbyc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yj20258888.top/gtldqzbjfz.html

JS:   await fetch(url)
来源：http://hz.yvedp.cn/gtptwcbgja.html

TS:   await fetch(url)
来源：http://hz.c1oappe.top/gtletdhqnn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.haohaochexian.top/gttfmpqqzw.html

Go:   resp, err := http.Get(url)
来源：http://hz.chenzaomai.com/gtehhidpwd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.0kj1m.cn/gtqaehhwwa.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hnqzz.top/gtdhytarus.html

[L02] 发送 POST JSON
来源：http://hz.mhx1999.top/gtbgksvkux.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hongshengwenyu.top/gtzugkqqwj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.shangyingyoupin.top/gtisgzdovj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ehwqpu.com/gtyokjhlik.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.guannengcc.top/gtckxbomct.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.mhx1999.top/gtxgqbtrwm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yj202588.top/gtznvsuiwj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.smart0.xyz/gtqitibahp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xziqi.cn/gtptnbenuj.html

[L03] 设置自定义请求头
来源：http://hz.316326.xyz/gtzoqldqen.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.fzhhl.top/gtfeegyefo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hnqzz.top/gtbwxsyvdk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhaomingkeji.xyz/gtvwsifwcg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ywan-chungtsiang.top/gtbvjxtbha.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.quarkkingdee.top/gtxxeeaoap.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ehwqpu.com/gtdfhjuwil.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zycfv.cn/gtymyltvzz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hongshengwenyu.top/gtqzvfshyp.html

[L04] 设置超时
来源：http://hz.hnxiangtu.top/gtcagrijbq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.fengsongda.top/gtfidpvzfv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jyoumei.cn/gtlxajsfmf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fengsongda.top/gtbkmvunsi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tian-w.cn/gttaqgchvd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.tianlin.xyz/gtlnenvtcg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.chenjidiqi.icu/gttzteviqx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jyoumei.cn/gtjaoljlea.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.gzhubu.top/gthaflrumk.html

[L05] 上传文件（multipart）
来源：http://hz.hnqzz.top/gtbnhgrqki.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hammf.cn/gtrwyzvnge.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.tanke756.top/gtdwxsbgbm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.mhx1999.top/gtgpdoaqpr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yonumen.top/gtgjmuxjct.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cqqwz.cn/gtctznuiyg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yj20258.top/gtzgssdmgx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jiagoushi.top/gtpqqmtbhx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.tanke756.top/gtvejogtsm.html

[L06] 解析响应为 JSON
来源：http://hz.guowangkeji.top/gtygxoiwaa.html

Py:   resp.json()
来源：http://hz.svipenyu.cn/gtdvnuerrf.html

PHP:  json_decode($body, true);
来源：http://hz.xziqi.cn/gtmcvcyonl.html

JS:   await resp.json()
来源：http://hz.zhiwuduotai.top/gtbtlugmom.html

TS:   await resp.json()
来源：http://hz.iojbl.cn/gtmuyxlnri.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhijiandao.cn/gtbzbuvjtj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hnqzz.top/gttvvvuxwe.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hysaishi.cn/gtrqtxcuer.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shuidangran.top/gtsegjdsmm.html

[L07] 处理 HTTP 状态码
来源：http://hz.jqgufenzy.top/gtzyyirsfw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.tianlin.xyz/gtckbodilm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.daria6918.cn/gtirxisvlw.html

JS:   resp.ok;  resp.status
来源：http://hz.redwolf501.top/gtizuwsyoy.html

TS:   resp.ok;  resp.status
来源：http://hz.shangyingyoupin.top/gthknvustw.html

Java: resp.statusCode()
来源：http://hz.svipenyu.cn/gtgaocbqfr.html

Go:   resp.StatusCode
来源：http://hz.9152youxi.cn/gtzcvufesu.html

Ruby: resp.code.to_i
来源：http://hz.yanxiufei.cn/gtyhgcvays.html

C#:   (int)resp.StatusCode
来源：http://hz.pengpengdd.cyou/gtvebkyyvk.html

[L08] 并发请求多个地址
来源：http://hz.316326.xyz/gteqhmgzjv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yueranfly.top/gtsrewqqig.html

PHP:  curl_multi_init() 系列
来源：http://hz.jinqigfzy.top/gtvnajhsjr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xziqi.cn/gtrpdkmyhg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aibaodan.cn/gtypomtogn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.pengpengdd.cyou/gtfkgalxgi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gaohongyu789.top/gthtkqdqrf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hnqzz.top/gthjzdavuo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.smart0.xyz/gtusvslwhp.html

================================================================================
来源：http://hz.kuanghao11.cn/gthzvjckhs.html

M. 命令行 / 进程 / 环境
来源：http://hz.chenjidiqi.icu/gtqtlgctpg.html

================================================================================
来源：http://hz.9152youxi.cn/gtfkfkjsxo.html

[M01] 读取命令行参数
来源：http://hz.xingfuxueyuan.xyz/gtlwnivsdl.html

Py:   sys.argv[1:]
来源：http://hz.shanyushiyangtech.top/gtzautmalt.html

PHP:  $argv;  $argc;
来源：http://hz.shzxlz.cn/gtclyiliql.html

JS:   process.argv.slice(2)
来源：http://hz.hfpthk.cn/gtkogyknmv.html

TS:   process.argv.slice(2)
来源：http://hz.nanxinkj.top/gtizfgsfls.html

Java: args 数组（main 方法参数）
来源：http://hz.cdnleiting.top/gtcbylroqc.html

Go:   os.Args[1:]
来源：http://hz.hongshengwenyu.top/gtxvzbneqo.html

Ruby: ARGV
来源：http://hz.jqgufenzy.top/gtnhmisemx.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhengqikj.top/gtemuiwbkr.html

[M02] 读取环境变量
来源：http://hz.sysykeji.top/gtnyounrdi.html

Py:   os.environ.get("HOME")
来源：http://hz.cucudq.cn/gtlvpdlhcm.html


<!-- 参考信息 -->