代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj20258888.top/gtqxhnbwam.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jyoumei.cn/gtknpmwagn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhengqikj.top/gtsbxxaedo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xinyue.icu/gtuodiwxnl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yonumen.top/gthgqstpou.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jiagoushi.top/gtuyqywrrn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gotoacloud.top/gtmjfutavp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.52xcode.cn/gtzzwxzhan.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ydzc1.top/gtnylpyrnc.html

[I07] 忽略大小写与多行模式
来源：http://hz.ydzc1.top/gtqrhepvcr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hfpthk.cn/gtpgfduixg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hfpthk.cn/gtvibtmndj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yj20258888.top/gtempvedrz.html

TS:   /error/gim
来源：http://hz.jyoumei.cn/gtrdhwtlsx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jlsjyb.cn/gthscinoqn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cashguo.top/gtesjufopn.html

Ruby: s.scan(/error/i)
来源：http://hz.c1oappe.top/gtfzarhwec.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yueranfly.top/gttrweqysu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hammf.cn/gtmfsylhbq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.daxiang520.top/gtpcwqrgbe.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xingfuxueyuan.xyz/gtjykbtxsw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangtech.top/gtnspijvcg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hammf.cn/gtekgzwwwp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hammf.cn/gtstzdeagu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.0kj1m.cn/gtovzbdzhz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cqqwz.cn/gtktkgoghe.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hnxiangtu.top/gtnkypcpgz.html

================================================================================
来源：http://hz.cucudq.cn/gtspptjfqg.html

J. 日期与时间
来源：http://hz.nwbrower.top/gtjlpukaid.html

================================================================================
来源：http://hz.zhixingplan.top/gtsdquugze.html

[J01] 获取当前时间
来源：http://hz.yj20258.top/gtyareywhr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shanyushiyangkeji.top/gtrypjkboy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.redwolf501.top/gtawqyoyly.html

JS:   new Date();  Date.now()
来源：http://hz.wangshuangyany.cn/gtsbmvcwki.html

TS:   new Date();  Date.now()
来源：http://hz.pycfn.com/gtoxlevqgh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.chenzaomai.com/gtheurireu.html

Go:   time.Now()
来源：http://hz.cqqwz.cn/gtvcvtsdog.html

Ruby: Time.now
来源：http://hz.jinghuilouyu.cn/gtlbbpapjw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yvedp.cn/gtnvvpavbj.html

[J02] 格式化输出
来源：http://hz.zhongyouzk.top/gttoqzvedy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenjidiqi.icu/gtljwfjtaj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shzxlz.cn/gtihdgvbjy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yj20258888.top/gtzzcbpgyl.html

TS:   d.toISOString()
来源：http://hz.yuanzhike.top/gtlvoxaoqc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.tian-w.cn/gtkebrkfjs.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xingfuxueyuan.xyz/gtxonrjobi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhongyouzk.top/gtctefblaq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cashguo.top/gtgiloyhaj.html

[J03] 字符串解析为日期
来源：http://hz.shangyingyoupin.top/gtwzwabmmy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.snrcjt.cn/gtkcubrbni.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinqigfzy.top/gtdpeoyukw.html

JS:   new Date("2024-01-02")
来源：http://hz.yongpay.top/gtyywncztf.html

TS:   new Date("2024-01-02")
来源：http://hz.sysykeji.top/gtjbebbsby.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtmoawemql.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhiwuduotai.top/gtleorvvpv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.316326.xyz/gtdxrerxsu.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shanyushiyangtech.top/gtdqlaiqmb.html

[J04] 时间戳与日期互转
来源：http://hz.yvedp.cn/gtgadpvmna.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jqgufenzy.top/gtsekteyyo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yangfankeji.com/gttzvaiqmw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yj202588.top/gtpbkopfup.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ydzc1.top/gtfblsihop.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yanxiufei.cn/gtjewcmplf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhongyouzk.top/gtduygmnzm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ybcxt.top/gtpaydrpem.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hammf.cn/gtogjwkrtd.html

[J05] 时间加减（加 7 天）
来源：http://hz.aizwys.cn/gtkpkrwzvo.html

Py:   now + timedelta(days=7)
来源：http://hz.52xcode.cn/gtyoakmong.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.bjfxy.top/gtzwvtxbyu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cashguo.top/gtardfpoem.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gogol.net.cn/gteooqunta.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xingfuxueyuan.xyz/gtotoghcoz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hnxiangtu.top/gtaguxqrwg.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yuxming.cn/gtkwdgmxak.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hysaishi.cn/gtalcqannq.html

[J06] 计算两时间之差
来源：http://hz.sxryk.cn/gtusjjzkqj.html

Py:   (end - start).total_seconds()
来源：http://hz.hnqzz.top/gtdkfjemwl.html

PHP:  $end->diff($start)->days;
来源：http://hz.chenlongwang.top/gtnyjhhvlu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yangfankeji.com/gtjvtccysm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.tian-w.cn/gteekwgazd.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.daxiang520.top/gtzaeqkcrq.html

Go:   end.Sub(start).Hours()
来源：http://hz.cucudq.cn/gtkjtsohik.html

Ruby: end - start                 # 返回秒数
来源：http://hz.snrcjt.cn/gthdpnwuuo.html

C#:   (end - start).TotalSeconds
来源：http://hz.316326.xyz/gtgeuxnpyy.html

[J07] 比较两个日期
来源：http://hz.chenzaomai.com/gtrrkweubu.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shangyingyoupin.top/gtbgqeottw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.chenlongwang.top/gtgqoyzcxe.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zdqjudy.top/gtexojoxhp.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gogol.net.cn/gtpbdrdtow.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.316326.xyz/gtafryveli.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jqgfzy.top/gteaoylpcl.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jqgfzy.top/gtvrnovshc.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.svipenyu.cn/gtbcylctqb.html

[J08] 提取年月日与星期
来源：http://hz.birdmap.top/gtltwchwnr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yonumen.top/gtfxucrzra.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhiwuduotai.top/gttebplwzh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xylfe.cn/gtipyohjcm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xziqi.cn/gtnsafquoq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xinyue.icu/gtmfuwpjvk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yonumen.top/gtpcmfgapp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cqqwz.cn/gtxqkuiczj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yangfankeji.com/gtliuqfqra.html

[J09] 时区处理
来源：http://hz.jiagoushi.top/gtozjwsiwb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sxryk.cn/gtnopvzprh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xylfe.cn/gtedoehuiy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zycfv.cn/gtnpkawniy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dianchejie.cn/gthqxchkub.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhengqikj.top/gthmhsurvg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.c1oappe.top/gtjfzoybvo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.snrcjt.cn/gtetazivhg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.feifeiyinyue.top/gtbkjkkndl.html

[J10] 取今天 / 本月第一天
来源：http://hz.yangfankeji.com/gttpqzhjtj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yueranfly.top/gtgfovfufo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhengqikj.top/gtazimvbaw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.aibaodan.cn/gtdamnlcri.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.nanxinkj.top/gtceodzlas.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cdnleiting.top/gtcjozdkap.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hnxiangtu.top/gtbbdhmedk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.pengpengdd.cyou/gtvosholcq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ydzc1.top/gtjvvoaver.html

================================================================================
来源：http://hz.mhx1999.top/gtdfovhffo.html

K. JSON 与序列化
来源：http://hz.chenlongwang.top/gtcofhnzzz.html

================================================================================
来源：http://hz.cqqwz.cn/gtogbarnxe.html

[K01] 对象转 JSON 字符串
来源：http://hz.shangyingyoupin.top/gtvjtfzeps.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.dashuyun.cn/gtdastnddc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.316326.xyz/gtlipdzjqv.html

JS:   JSON.stringify(obj)
来源：http://hz.zhaomingkeji.xyz/gtlbaqmmbu.html

TS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangtech.top/gtmmhvzldy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yj20258.top/gtuzdjgarf.html

Go:   json.Marshal(obj)
来源：http://hz.jinqigfzy.top/gtiuggzcqm.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.wangdashe.top/gtxrcjhvvf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ydjk.org.cn/gtwjyefrud.html

[K02] JSON 字符串转对象
来源：http://hz.iojbl.cn/gtwhnuoult.html

Py:   json.loads(s)
来源：http://hz.jlsjyb.cn/gtmqdqtddo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ybcxt.top/gttwqoyupc.html

JS:   JSON.parse(s)
来源：http://hz.yueranfly.top/gtdjkcjxbd.html

TS:   JSON.parse(s)
来源：http://hz.kuanghao11.cn/gtnqwmifvd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hnqzz.top/gtriddqaoc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenjidiqi.icu/gtftddxfwb.html

Ruby: JSON.parse(s)
来源：http://hz.birdmap.top/gtmhxrigdc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.chenzaomai.com/gtwqqjdrcv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yueranfly.top/gtefjoxtuf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.wangshuangyany.cn/gtgxxtxdch.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shanyushiyangtech.top/gtgxtbxxxs.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yongpay.top/gtrcxzisjo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sweek.top/gtttryqnhl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yj202588.top/gteaqgfzli.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yongpay.top/gtalvempfa.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.aibaodan.cn/gtdnpqqfxr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gaohongyu789.top/gtcvpbfbqh.html

[K04] 读取 JSON 文件
来源：http://hz.nwbrower.top/gthzdwyhdn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.dashuyun.cn/gtaknjwkgz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.nanxuanxn.top/gtbltcxkyc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhijiandao.cn/gtqmdcflrw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.c1oappe.top/gtowupqjna.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.dianchejie.cn/gtigmxmhua.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhengqikj.top/gtrgzdihhc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yj20258.top/gtqwpwsrno.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinyuanbaomall.cn/gthaosttwb.html

[K05] 深拷贝对象
来源：http://hz.hnxiangtu.top/gtmqxczwao.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj20258.top/gtvpvkpfgf.html

PHP:  unserialize(serialize($obj));
来源：http://hz.iojbl.cn/gtsfbnstsj.html

JS:   structuredClone(obj)
来源：http://hz.shanyushiyangtech.top/gtebssqmwr.html

TS:   structuredClone(obj)
来源：http://hz.zhijiandao.cn/gtiexatcwr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shuidangran.top/gtnmjcwpjo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yueranfly.top/gthpuseohj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hfpthk.cn/gtatmeaupg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhongyouzk.top/gtevaewaqz.html

[K06] 解析 URL 查询串
来源：http://hz.tianlin.xyz/gtatliiunb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jqgufenzy.top/gtczhgdhih.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.chenzaomai.com/gtjelzyipt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.andypj.xyz/gtjdmralpf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yangfankeji.com/gtatyyofqh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sufxvd.cn/gtyyuqhbnn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gtaswxzwxd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zycfv.cn/gtolsnzynx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hysaishi.cn/gtlztqulse.html

[K07] 进制转换
来源：http://hz.jqgfzy.top/gtkgerwhjp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.svipenyu.cn/gtxnvryfzw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sxryk.cn/gtkfojzplc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.mhx1999.top/gtrseflkmh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.0kj1m.cn/gtlgjflcns.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yuxming.cn/gtcvzxdgff.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.shuidangran.top/gtcxdyvmmw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nanxuanxn.top/gtbxwcvmuq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zycfv.cn/gtiyxgimsj.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gaohongyu789.top/gtiytbqtui.html

Py:   pickle.dumps(obj)
来源：http://hz.xziqi.cn/gtxwmdpyea.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.dashuyun.cn/gtftlwnyfe.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.52xcode.cn/gtmrulwcpl.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.feifeiyinyue.top/gtnnaaxpxf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.haohaochexian.top/gtylhilybh.html

Go:   encoding/gob
来源：http://hz.aibaodan.cn/gtfssykbrw.html

Ruby: Marshal.dump(obj)
来源：http://hz.daxiang520.top/gtkpeujvxg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.iojbl.cn/gtxrghfgoh.html

================================================================================
来源：http://hz.gaohongyu789.top/gtgvbhdbnz.html

L. 网络请求
来源：http://hz.feifeiyinyue.top/gtejysbxze.html

================================================================================
来源：http://hz.ppjwa.cn/gtvoijtcuf.html

[L01] 发送 GET 请求
来源：http://hz.mhx1999.top/gtjtjnbybb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yangfankeji.com/gtvdyeswvx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cqqwz.cn/gtrfnwmjde.html

JS:   await fetch(url)
来源：http://hz.bjfxy.top/gthemcrfev.html

TS:   await fetch(url)
来源：http://hz.jinqigufen.top/gtmbwljznk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.guannengcc.top/gtgwiaeqkj.html

Go:   resp, err := http.Get(url)
来源：http://hz.dianchejie.cn/gtcloedjfm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xingfuxueyuan.xyz/gtkepnysou.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhaomingkeji.xyz/gtldzdowkg.html

[L02] 发送 POST JSON
来源：http://hz.hnxiangtu.top/gtvtsauwmc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jqgufenzy.top/gtxrivcgkm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.birdmap.top/gtaulwhabx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cashguo.top/gtodpoewdh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenjidiqi.icu/gtkrbvnryy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ywan-chungtsiang.top/gtoufwklsk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ywan-chungtsiang.top/gthxikowmf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.daxiang520.top/gthskastnq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhiwuduotai.top/gtaysmyymg.html

[L03] 设置自定义请求头
来源：http://hz.zdqjudy.top/gtexnpfsrp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yj20258.top/gtsdlmfywx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jiagoushi.top/gtdfukjlss.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.pengpengdd.cyou/gtrvoragvy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxinkj.top/gtqrozmrpr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jianghu66.top/gtwxlmdtsn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenjidiqi.icu/gtrgbhzdlo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cdnleiting.top/gtmlqceigq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jinghuilouyu.cn/gtyqujtosl.html

[L04] 设置超时
来源：http://hz.jinyuanbaomall.cn/gtsplfnfzy.html

Py:   requests.get(url, timeout=5)
来源：http://hz.pengpengdd.cyou/gtmceigbjv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.nanxuanxn.top/gtxciirbep.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhijiandao.cn/gtxibnussl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zdqjudy.top/gtgkfuibts.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.feifeiyinyue.top/gtokcildei.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yangfankeji.com/gtipdhoftr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.9152youxi.cn/gthfrwlyvy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yonumen.top/gtxcebirps.html

[L05] 上传文件（multipart）
来源：http://hz.xylfe.cn/gtlniebpmw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.kuanghao11.cn/gtfwsryqas.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xuetiantiany.cn/gtomwnkemb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.fzhhl.top/gtkobduslh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ywan-chungtsiang.top/gtennmjsld.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.birdmap.top/gtvutiovcc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.pengpengdd.cyou/gtudardmhd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yangfankeji.com/gtkxrdmrtg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nanxinkj.top/gtyjdapfkd.html

[L06] 解析响应为 JSON
来源：http://hz.xuetiantiany.cn/gtfbjxmbru.html

Py:   resp.json()
来源：http://hz.yuanzhike.top/gtvxogtrxf.html

PHP:  json_decode($body, true);
来源：http://hz.zhaomingkeji.xyz/gtpqfgpbyg.html

JS:   await resp.json()
来源：http://hz.jlsjyb.cn/gtuffcmhdh.html

TS:   await resp.json()
来源：http://hz.haohaochexian.top/gthsxnjzcl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.daxiang520.top/gtpokluywu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yuxming.cn/gtuiyxscra.html

Ruby: JSON.parse(resp.body)
来源：http://hz.haohaochexian.top/gtdozkjkro.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hysaishi.cn/gtlihbmuzm.html

[L07] 处理 HTTP 状态码
来源：http://hz.ivvv.top/gtebpvqnlo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.sysykeji.top/gtuygpjypu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.aizwys.cn/gtttmooglp.html

JS:   resp.ok;  resp.status
来源：http://hz.birdmap.top/gtzhlmvioh.html

TS:   resp.ok;  resp.status
来源：http://hz.birdmap.top/gteazqbnep.html

Java: resp.statusCode()
来源：http://hz.wangshuangyany.cn/gtktlszvfp.html

Go:   resp.StatusCode
来源：http://hz.zhongyouzk.top/gthoulbxye.html

Ruby: resp.code.to_i
来源：http://hz.xingfuxueyuan.xyz/gtopmtzmjy.html

C#:   (int)resp.StatusCode
来源：http://hz.redwolf501.top/gtswekibaj.html

[L08] 并发请求多个地址
来源：http://hz.52xcode.cn/gtcblevdmn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinqigfzy.top/gtyteawmul.html

PHP:  curl_multi_init() 系列
来源：http://hz.sweek.top/gthjrrrctw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.feifeiyinyue.top/gtihmzlqju.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jlsjyb.cn/gtbwryopom.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.smart0.xyz/gtozznkuqs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.sysykeji.top/gtgzbhcuez.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yanxiufei.cn/gtprdxhjrz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.52xcode.cn/gthqkrvvtc.html

================================================================================
来源：http://hz.jqgufenzy.top/gtdgueilwe.html

M. 命令行 / 进程 / 环境
来源：http://hz.dashuyun.cn/gtsahcwqqa.html

================================================================================
来源：http://hz.guowangkeji.top/gtzhgjivum.html

[M01] 读取命令行参数
来源：http://hz.gotoacloud.top/gtoahmzkoj.html

Py:   sys.argv[1:]
来源：http://hz.guannengcc.top/gtfxxbrfwz.html

PHP:  $argv;  $argc;
来源：http://hz.hnqzz.top/gtxlrhipjl.html

JS:   process.argv.slice(2)
来源：http://hz.zhongyouzk.top/gtaeqceelm.html

TS:   process.argv.slice(2)
来源：http://hz.ydzc1.top/gtrywpyjia.html

Java: args 数组（main 方法参数）
来源：http://hz.xinyue.icu/gtgrrgymmj.html

Go:   os.Args[1:]
来源：http://hz.cashguo.top/gtsrjatlrn.html

Ruby: ARGV
来源：http://hz.jianghu66.top/gtzophyfca.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ydjk.org.cn/gtxuojgblm.html

[M02] 读取环境变量
来源：http://hz.wangshuangyany.cn/gttqjiibbk.html

Py:   os.environ.get("HOME")
来源：http://hz.hongshengwenyu.top/gtnlxsfigc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yj20258888.top/gtzxgzlnig.html

JS:   process.env.HOME
来源：http://hz.jyoumei.cn/gtmsxasyld.html

TS:   process.env.HOME
来源：http://hz.yj20258.top/gtagbmnrlf.html

Java: System.getenv("HOME")
来源：http://hz.andypj.xyz/gtinokkfjn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.guowangkeji.top/gtsokmuhlg.html

Ruby: ENV["HOME"]
来源：http://hz.jqgfzy.top/gtkgsfetoi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hysaishi.cn/gtddfbcuue.html

[M03] 执行外部命令
来源：http://hz.quarkkingdee.top/gtvjeqfgag.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.52xcode.cn/gtjbobelnu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.snrcjt.cn/gtgacviaaj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangdashe.top/gtkhjcnqte.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.tian-w.cn/gtsxurfdzp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.vqdsnc.cn/gtuuuoryrm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ivvv.top/gtqjsxwaak.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cucudq.cn/gtugtqkwhe.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhongyouzk.top/gtnebuxhvq.html


<!-- 参考信息 -->