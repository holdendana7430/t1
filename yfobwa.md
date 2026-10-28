代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.smart0.xyz/gtkxghaxnw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jiagoushi.top/gtikqcctym.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jiagoushi.top/gtzhnhnomj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cqqwz.cn/gttpfpmimf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.shangyingyoupin.top/gtvxzwvkzk.html

[I07] 忽略大小写与多行模式
来源：http://hz.yuxming.cn/gtlkmksdzx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yuanzhike.top/gtcxnpxiey.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhijiandao.cn/gtifadhxvl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yj202588.top/gtpkhxpyux.html

TS:   /error/gim
来源：http://hz.sxryk.cn/gtyoiirnzk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.0kj1m.cn/gtunitkvpw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhongyouzk.top/gttxubozmj.html

Ruby: s.scan(/error/i)
来源：http://hz.sweek.top/gttmparqht.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sufxvd.cn/gtnjdsoolb.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yonumen.top/gtoksvbyxv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sweek.top/gtmszvzcvz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.guowangkeji.top/gtastzrvvs.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.52xcode.cn/gtuoyusgkn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gotoacloud.top/gtdptwkkxc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.dashuyun.cn/gteexfcykh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.dianchejie.cn/gtasyryxip.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.9152youxi.cn/gtritulpgq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hnxiangtu.top/gtoidpoguv.html

================================================================================
来源：http://hz.birdmap.top/gtpntupbel.html

J. 日期与时间
来源：http://hz.jqgfzy.top/gtzlblciuv.html

================================================================================
来源：http://hz.ppjwa.cn/gtlpvgkitq.html

[J01] 获取当前时间
来源：http://hz.aibaodan.cn/gttkmjaspz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hywenlv.cn/gtxoeaiaro.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yuanzhike.top/gtzsarrfma.html

JS:   new Date();  Date.now()
来源：http://hz.xziqi.cn/gthfwytfzp.html

TS:   new Date();  Date.now()
来源：http://hz.shanyushiyangtech.top/gtynshmhmq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cdnleiting.top/gtjctskllh.html

Go:   time.Now()
来源：http://hz.gogol.net.cn/gteqczkaux.html

Ruby: Time.now
来源：http://hz.ywan-chungtsiang.top/gtewxsirze.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xylfe.cn/gtwufiqyog.html

[J02] 格式化输出
来源：http://hz.ydzc1.top/gtacxivatf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.feifeiyinyue.top/gtyawokkak.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xingfuxueyuan.xyz/gtswsucwtn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.0kj1m.cn/gtmrihzojd.html

TS:   d.toISOString()
来源：http://hz.jinghuilouyu.cn/gtfjgybffp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.c1oappe.top/gtlqexryoa.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yueranfly.top/gtjurgnjud.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gogol.net.cn/gtrqkvgjdz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cqqwz.cn/gtycvpvoge.html

[J03] 字符串解析为日期
来源：http://hz.pycfn.com/gtfddyqpcx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.tanke756.top/gttqojdidn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hywenlv.cn/gteddimrwk.html

JS:   new Date("2024-01-02")
来源：http://hz.jianghu66.top/gtymumihqo.html

TS:   new Date("2024-01-02")
来源：http://hz.andypj.xyz/gtllqxlxob.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jiagoushi.top/gtyjmgrtgt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.pycfn.com/gtptlkwbqa.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.daria6918.cn/gtvkggutlp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.0kj1m.cn/gtbkveygjd.html

[J04] 时间戳与日期互转
来源：http://hz.havefunace.top/gtyzynbwut.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.nwbrower.top/gtilkuqqbt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ehwqpu.com/gtmvxmjmeo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xuanzx.com/gtblpurlpj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jqgufenzy.top/gthfonjdil.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jqgufenzy.top/gtmwummvhu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xinyue.icu/gtdqhirass.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.fengsongda.top/gtzstrjdut.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj20258888.top/gtdwuxunoh.html

[J05] 时间加减（加 7 天）
来源：http://hz.wangdashe.top/gtnwmuycsq.html

Py:   now + timedelta(days=7)
来源：http://hz.wangdashe.top/gtrkwthkes.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hnxiangtu.top/gtltrgibhp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jianghu66.top/gtpdwfoyns.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shuidangran.top/gtiemldbhc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cheryme.top/gtnooptiov.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.52xcode.cn/gtdzyejcwc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hysaishi.cn/gthdjiysll.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.pengpengdd.cyou/gtzgftohbu.html

[J06] 计算两时间之差
来源：http://hz.52xcode.cn/gtvwakdmnx.html

Py:   (end - start).total_seconds()
来源：http://hz.jqgfzy.top/gtywumvfgx.html

PHP:  $end->diff($start)->days;
来源：http://hz.ywan-chungtsiang.top/gtwftymkfw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.guowangkeji.top/gtdywzaivn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.nwbrower.top/gtvspkizrz.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.chenlongwang.top/gtbxuyrenm.html

Go:   end.Sub(start).Hours()
来源：http://hz.pengpengdd.cyou/gtpjbyoffl.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yueranfly.top/gthsoplxov.html

C#:   (end - start).TotalSeconds
来源：http://hz.daria6918.cn/gtxbtyydle.html

[J07] 比较两个日期
来源：http://hz.dianchejie.cn/gtfcelcuun.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ydjk.org.cn/gtulohhdin.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.daxiang520.top/gtazcxqooj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ywan-chungtsiang.top/gtberhkvdf.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.haohaochexian.top/gtlposceph.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yvedp.cn/gtmfyhevaj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhijiandao.cn/gtpdjphlxt.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.daxiang520.top/gtlqmiixfy.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zdqjudy.top/gtztvontsj.html

[J08] 提取年月日与星期
来源：http://hz.jlsjyb.cn/gtgtaigkkz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinghuilouyu.cn/gtwgeillsa.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shzxlz.cn/gtjhnedklb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yonumen.top/gtmwacljuv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ivvv.top/gttvmdvvwo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xuanzx.com/gtlttdwdsy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhijiandao.cn/gtpqsaaoxh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.dashuyun.cn/gtytooccjq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.daxiang520.top/gtgwglosig.html

[J09] 时区处理
来源：http://hz.shanyushiyangkeji.top/gtiyrtotye.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.fzhhl.top/gtdzznavxq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.guowangkeji.top/gtdlcotixf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.quarkkingdee.top/gtoyazqccj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tianlin.xyz/gtrhftfkun.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.52xcode.cn/gtbkdlbzuz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xingfuxueyuan.xyz/gtzigrtexh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenlongwang.top/gthkrutbbq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shzxlz.cn/gtlwedaxyu.html

[J10] 取今天 / 本月第一天
来源：http://hz.daria6918.cn/gtlwbjtlpb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.tanke756.top/gtuiwsgwnx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yangfankeji.com/gtnnwwfizf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhongyouzk.top/gtivvaqkrc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.pycfn.com/gtxzayyzss.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jqgufenzy.top/gtylpasgwx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yuanzhike.top/gtmpojhvwq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cheryme.top/gteboclkuo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jqgufenzy.top/gtuqxujyjl.html

================================================================================
来源：http://hz.aizwys.cn/gtgbsmktqz.html

K. JSON 与序列化
来源：http://hz.aizwys.cn/gtdfqosyeq.html

================================================================================
来源：http://hz.jinqigufen.top/gthmaedemf.html

[K01] 对象转 JSON 字符串
来源：http://hz.vqdsnc.cn/gtosavifmd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.daxiang520.top/gtgtxjerqh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yj202588.top/gtdvtityhd.html

JS:   JSON.stringify(obj)
来源：http://hz.zhiwuduotai.top/gtflidgedc.html

TS:   JSON.stringify(obj)
来源：http://hz.snrcjt.cn/gtmqptgwcl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.9152youxi.cn/gttdfvjmvz.html

Go:   json.Marshal(obj)
来源：http://hz.guowangkeji.top/gtlmtnfxdx.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yuxming.cn/gtpqzsalfw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.pycfn.com/gtqbcjdfan.html

[K02] JSON 字符串转对象
来源：http://hz.quarkkingdee.top/gtxqgaioyb.html

Py:   json.loads(s)
来源：http://hz.yuxming.cn/gtoybjvpmq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cheryme.top/gtftylwrcp.html

JS:   JSON.parse(s)
来源：http://hz.sufxvd.cn/gtpvenjccq.html

TS:   JSON.parse(s)
来源：http://hz.guannengcc.top/gtnonldkwj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhongyouzk.top/gttdnjdoqz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shzxlz.cn/gtocljbzdr.html

Ruby: JSON.parse(s)
来源：http://hz.gzhubu.top/gtptugtfkf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jqgufenzy.top/gtimtrmedc.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cqqwz.cn/gtzhkflccs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jiagoushi.top/gtimopjbiu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shzxlz.cn/gttgpztvqi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenlongwang.top/gtyvdfccmt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xziqi.cn/gtddmhagts.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dianchejie.cn/gtzzjdrohk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yuanzhike.top/gtbnpfzonz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ydzc1.top/gtebztlcsn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cdnleiting.top/gtnhrousuq.html

[K04] 读取 JSON 文件
来源：http://hz.nanxuanxn.top/gtxdloprqp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.havefunace.top/gtrwvuvfaa.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhixingplan.top/gtcfhzwnkn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gogol.net.cn/gtzyuabqdn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aibaodan.cn/gtfgriekdo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ydzc1.top/gtqateoaje.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.vqdsnc.cn/gtbkigxjth.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.chenjidiqi.icu/gtsadqzalz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.guowangkeji.top/gttmswmxme.html

[K05] 深拷贝对象
来源：http://hz.yj202588.top/gtdpzxuvrq.html

Py:   copy.deepcopy(obj)
来源：http://hz.fengsongda.top/gtssdshion.html

PHP:  unserialize(serialize($obj));
来源：http://hz.nanxuanxn.top/gteqmsdqzb.html

JS:   structuredClone(obj)
来源：http://hz.yonumen.top/gtrykwdwjl.html

TS:   structuredClone(obj)
来源：http://hz.vqdsnc.cn/gtgaqebhcb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ybcxt.top/gtpcaxfrmb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yanxiufei.cn/gtipzyrhrx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.quarkkingdee.top/gtycmdzvno.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yanxiufei.cn/gtxeewypox.html

[K06] 解析 URL 查询串
来源：http://hz.ivvv.top/gtoxhsissu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sysykeji.top/gtzauvqxsn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xylfe.cn/gtmsfyface.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.9152youxi.cn/gtvlfdxztb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yanxiufei.cn/gtoxaatlhu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jlsjyb.cn/gtfkkhibaq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hammf.cn/gtioiujspk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhongyouzk.top/gtgxwvqzxy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hywenlv.cn/gteosksxia.html

[K07] 进制转换
来源：http://hz.feifeiyinyue.top/gthyzvrbcu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yvedp.cn/gthgxpdpkf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yueranfly.top/gtzrmhxvvq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhiwuduotai.top/gtbreguzml.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yj20258888.top/gtzhtphmbk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.fengsongda.top/gtyvpvyclh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.chenlongwang.top/gtfdqrhwgg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yangfankeji.com/gtihqpdvsm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinghuilouyu.cn/gteuvraobt.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ybcxt.top/gtsgsvwnpt.html

Py:   pickle.dumps(obj)
来源：http://hz.xuanzx.com/gtuiytcisv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.wangdashe.top/gtccvcrkqm.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jinyuanbaomall.cn/gtvfsbepde.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gotoacloud.top/gtvpxxoaye.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yj20258.top/gthhyvliag.html

Go:   encoding/gob
来源：http://hz.iojbl.cn/gtgbwaddcf.html

Ruby: Marshal.dump(obj)
来源：http://hz.iojbl.cn/gtpqrplcyy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.feifeiyinyue.top/gtbhrtqdte.html

================================================================================
来源：http://hz.wangdashe.top/gtklefezpe.html

L. 网络请求
来源：http://hz.shuidangran.top/gthznzgyoe.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtbxeyftou.html

[L01] 发送 GET 请求
来源：http://hz.shanyushiyangtech.top/gtlccpuoio.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cheryme.top/gtctvaviri.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.chenlongwang.top/gtfhqduwlp.html

JS:   await fetch(url)
来源：http://hz.xylfe.cn/gtzxxmlpfl.html

TS:   await fetch(url)
来源：http://hz.nanxinkj.top/gtuxzonidn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.mhx1999.top/gtkdcokmrz.html

Go:   resp, err := http.Get(url)
来源：http://hz.zycfv.cn/gtvjmojjma.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.nanxuanxn.top/gtmungbptr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.aizwys.cn/gtsjnkfwgk.html

[L02] 发送 POST JSON
来源：http://hz.52xcode.cn/gtnrkmyeoi.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hywenlv.cn/gtuzrpqnrq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ywan-chungtsiang.top/gtperqaqcx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hammf.cn/gtkainlath.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnqzz.top/gtjlizzjuf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xinyue.icu/gtzhwqfdnw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhongyouzk.top/gteipxdygd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.mhx1999.top/gtmtzxxjlq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.pengpengdd.cyou/gtenailuqb.html

[L03] 设置自定义请求头
来源：http://hz.redwolf501.top/gtkyjigntc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xingfuxueyuan.xyz/gtguwybuos.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.svipenyu.cn/gtclwfdcyp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aibaodan.cn/gtvyagpctu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shanyushiyangtech.top/gtasfjiwbj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.quarkkingdee.top/gtpztwloon.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.tianlin.xyz/gtjnzhuskr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hysaishi.cn/gtmmrufafu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuanzhike.top/gtgussppjw.html

[L04] 设置超时
来源：http://hz.hysaishi.cn/gtyyulpiyp.html

Py:   requests.get(url, timeout=5)
来源：http://hz.feifeiyinyue.top/gtrosorwcv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yj202588.top/gtqkhkzynw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zycfv.cn/gtxlygslke.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yongpay.top/gtvessqprm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yueranfly.top/gthlyfauae.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.tian-w.cn/gtdxlqefms.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xuetiantiany.cn/gtcfjadzlh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.chenjidiqi.icu/gtazjtnrsw.html

[L05] 上传文件（multipart）
来源：http://hz.chenzaomai.com/gtiimrzvnd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.dashuyun.cn/gtbcbfznqp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.smart0.xyz/gtbhwkeuxv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xylfe.cn/gtbvvhdwfd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.aizwys.cn/gtdvhizcwc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gzhubu.top/gtiwlajrvz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jyoumei.cn/gtgvclvirm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ehwqpu.com/gtqocpfeyz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yj202588.top/gtiiaytyoo.html

[L06] 解析响应为 JSON
来源：http://hz.gogol.net.cn/gtnsuuflvh.html

Py:   resp.json()
来源：http://hz.iojbl.cn/gtoccxpocg.html

PHP:  json_decode($body, true);
来源：http://hz.0kj1m.cn/gtrhnlqmlk.html

JS:   await resp.json()
来源：http://hz.jinqigufen.top/gtpvpmayzx.html

TS:   await resp.json()
来源：http://hz.yuxming.cn/gtepiashci.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.mhx1999.top/gtibhzdfhw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hfpthk.cn/gtfgwaotoa.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sxryk.cn/gthywofyhg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ybcxt.top/gtdmunomkv.html

[L07] 处理 HTTP 状态码
来源：http://hz.yj20258888.top/gtzavnwpsu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ppjwa.cn/gtjysjoylf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jqgufenzy.top/gttuedoapa.html

JS:   resp.ok;  resp.status
来源：http://hz.cashguo.top/gttvfcbchp.html

TS:   resp.ok;  resp.status
来源：http://hz.havefunace.top/gtnkejhxvd.html

Java: resp.statusCode()
来源：http://hz.sweek.top/gtjwmpqfly.html

Go:   resp.StatusCode
来源：http://hz.ydjk.org.cn/gtiysoxndr.html

Ruby: resp.code.to_i
来源：http://hz.zhixingplan.top/gtnwueksdd.html

C#:   (int)resp.StatusCode
来源：http://hz.yangfankeji.com/gtybyqfdjn.html

[L08] 并发请求多个地址
来源：http://hz.jqgufenzy.top/gtwlldwimh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.quarkkingdee.top/gtnidswrzt.html

PHP:  curl_multi_init() 系列
来源：http://hz.guowangkeji.top/gtxqxpctbk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.smart0.xyz/gttnjagvdq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj20258888.top/gtfxzgeani.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.mhx1999.top/gtpryhoztw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.kuanghao11.cn/gtksdfswlu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yj20258.top/gthmevhfhl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jiagoushi.top/gtvhrvjzlq.html

================================================================================
来源：http://hz.jyoumei.cn/gtkjcqinpf.html

M. 命令行 / 进程 / 环境
来源：http://hz.sysykeji.top/gtgdwudhrg.html

================================================================================
来源：http://hz.fengsongda.top/gtftnyxvki.html

[M01] 读取命令行参数
来源：http://hz.wangshuangyany.cn/gtdoysjdbx.html

Py:   sys.argv[1:]
来源：http://hz.yj20258.top/gtebtlpiyt.html

PHP:  $argv;  $argc;
来源：http://hz.zhixingplan.top/gtvotvuavi.html

JS:   process.argv.slice(2)
来源：http://hz.hongshengwenyu.top/gtcwqmtjjo.html

TS:   process.argv.slice(2)
来源：http://hz.nwbrower.top/gtpfugiatm.html

Java: args 数组（main 方法参数）
来源：http://hz.zhijiandao.cn/gtiylonixk.html

Go:   os.Args[1:]
来源：http://hz.guowangkeji.top/gtsxwxvdup.html

Ruby: ARGV
来源：http://hz.sufxvd.cn/gtvmczpshn.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jinqigufen.top/gtnyoakuoz.html

[M02] 读取环境变量
来源：http://hz.yangfankeji.com/gtthhytkeh.html

Py:   os.environ.get("HOME")
来源：http://hz.hongshengwenyu.top/gtighiqidu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinyuanbaomall.cn/gtvzayebjc.html

JS:   process.env.HOME
来源：http://hz.zhijiandao.cn/gtoqusjbks.html

TS:   process.env.HOME
来源：http://hz.shanyushiyangtech.top/gthoyfszxx.html

Java: System.getenv("HOME")
来源：http://hz.yj20258.top/gtutrnvnjq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.guannengcc.top/gtmzouuiez.html

Ruby: ENV["HOME"]
来源：http://hz.jiagoushi.top/gtbatmdbat.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhengqikj.top/gtechxkfuk.html

[M03] 执行外部命令
来源：http://hz.9152youxi.cn/gtfiepiugp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shanyushiyangkeji.top/gtzmupmdjv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.sysykeji.top/gtjyoaygzq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yongpay.top/gtdbfgtxpw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuanzhike.top/gtlirewmjw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sxryk.cn/gtuolbkutm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xingfuxueyuan.xyz/gtduiuzcin.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hysaishi.cn/gtqpjcgpli.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jinqigufen.top/gtgrewoukx.html

[M04] 获取当前工作目录
来源：http://hz.pengpengdd.cyou/gtnqivjamr.html

Py:   os.getcwd()
来源：http://hz.ppjwa.cn/gtebebprlr.html

PHP:  getcwd();
来源：http://hz.jinqigfzy.top/gtcovaorxx.html

JS:   process.cwd()
来源：http://hz.yangfankeji.com/gteuxwzasy.html


<!-- 参考信息 -->