代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.fengsongda.top/gtkfepmjhe.html

[I07] 忽略大小写与多行模式
来源：http://hz.smart0.xyz/gtuzyghiut.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.pycfn.com/gtrtexlzsm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xziqi.cn/gtfbvzqnwh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xuetiantiany.cn/gtlkvxecfq.html

TS:   /error/gim
来源：http://hz.xziqi.cn/gtgcxeoywq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhongyouzk.top/gtojzbxfzf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhixingplan.top/gtrvtlfweo.html

Ruby: s.scan(/error/i)
来源：http://hz.yuxming.cn/gtfrhxuhha.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yuxming.cn/gtcupnneng.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.nanxinkj.top/gtcmrxhglz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.redwolf501.top/gtfvcbtqgt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.nwbrower.top/gtzjopcxho.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigfzy.top/gtauykyrbo.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zdqjudy.top/gthdlorwnc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cashguo.top/gtugdvlkep.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gaohongyu789.top/gtysxscrub.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shangyingyoupin.top/gtjfayxaky.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.bjfxy.top/gtokutezsm.html

================================================================================
来源：http://hz.cdnleiting.top/gtvpijdria.html

J. 日期与时间
来源：http://hz.yj20258888.top/gtpfuqgimh.html

================================================================================
来源：http://hz.xuanzx.com/gtzoitnbbb.html

[J01] 获取当前时间
来源：http://hz.havefunace.top/gtmrcepzyh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenlongwang.top/gtrurnadve.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.haohaochexian.top/gtpznkumsa.html

JS:   new Date();  Date.now()
来源：http://hz.dianchejie.cn/gtfqbpgtxj.html

TS:   new Date();  Date.now()
来源：http://hz.hongshengwenyu.top/gtiuntsqyb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.nanxuanxn.top/gtcdsdxuao.html

Go:   time.Now()
来源：http://hz.zhoulong.xyz/gtcklzqsrg.html

Ruby: Time.now
来源：http://hz.yueranfly.top/gtxlsadnnt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yongpay.top/gtodtbuxth.html

[J02] 格式化输出
来源：http://hz.tianlin.xyz/gtakoheudr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hywenlv.cn/gtjahfffjp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yangfankeji.com/gtamswlvcn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xuetiantiany.cn/gtgtubtnvh.html

TS:   d.toISOString()
来源：http://hz.cdnleiting.top/gtnghdezpg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhongyouzk.top/gtbjrhylbg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ppjwa.cn/gtregpxtvl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yonumen.top/gtbgauzvrm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhijiandao.cn/gteogvjiqu.html

[J03] 字符串解析为日期
来源：http://hz.yj202588.top/gtezdxuqmd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shanyushiyangtech.top/gthkhmabws.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinghuilouyu.cn/gtizgowlsc.html

JS:   new Date("2024-01-02")
来源：http://hz.andypj.xyz/gtnlqeiwxg.html

TS:   new Date("2024-01-02")
来源：http://hz.chenzaomai.com/gtkfdjrvhq.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.guowangkeji.top/gtmakjqazr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.52xcode.cn/gtkgytluhv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhixingplan.top/gtjrturdut.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hnxiangtu.top/gtjujddhxx.html

[J04] 时间戳与日期互转
来源：http://hz.jinqigfzy.top/gtgpopqhdp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.nanxinkj.top/gthcokgmpg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.svipenyu.cn/gtgxbgwxfs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.daria6918.cn/gtfrkwnapy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinghuilouyu.cn/gtubhlqsza.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hysaishi.cn/gtbdmacmmf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sufxvd.cn/gtxvonbpny.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.pycfn.com/gtcdjvxzwf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yueranfly.top/gtsidksbbr.html

[J05] 时间加减（加 7 天）
来源：http://hz.xuetiantiany.cn/gtwuyncgli.html

Py:   now + timedelta(days=7)
来源：http://hz.ivvv.top/gtbuvwlkyt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ywan-chungtsiang.top/gtoghytggr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnqzz.top/gtcqzjxdzy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fengsongda.top/gtcjwavqsq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yvedp.cn/gtgightjqi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hnqzz.top/gtrheqlawd.html

Ruby: Time.now + 7 * 86400
来源：http://hz.snrcjt.cn/gtbrlpbrav.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.bjfxy.top/gtgxnqupth.html

[J06] 计算两时间之差
来源：http://hz.shanyushiyangkeji.top/gtdbtencwa.html

Py:   (end - start).total_seconds()
来源：http://hz.iojbl.cn/gtvacjbdlj.html

PHP:  $end->diff($start)->days;
来源：http://hz.cdnleiting.top/gtkgfbqcxq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.guannengcc.top/gtfculwblz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.nanxinkj.top/gtfhyuujnf.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.meibo888.top/gtmcugzzhx.html

Go:   end.Sub(start).Hours()
来源：http://hz.xingfuxueyuan.xyz/gtgwjeabiv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sysykeji.top/gtqravtwjt.html

C#:   (end - start).TotalSeconds
来源：http://hz.cqqwz.cn/gtqatczbhg.html

[J07] 比较两个日期
来源：http://hz.yj20258888.top/gtclzunqbl.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.meibo888.top/gtamlxblvz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hysaishi.cn/gtpzulzrmf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gogol.net.cn/gtiwismpal.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hywenlv.cn/gthjoqujbj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.sweek.top/gtmrapwubh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shzxlz.cn/gtdigxkykb.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ydjk.org.cn/gtzfkyfwdz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cdnleiting.top/gtrqqkvtdv.html

[J08] 提取年月日与星期
来源：http://hz.zdqjudy.top/gtgcaypaze.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.iojbl.cn/gtmavrobss.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhoulong.xyz/gtyyoephuc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.snrcjt.cn/gthmknbtyt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hywenlv.cn/gtvxsvptji.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.chenlongwang.top/gtzpetitmp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.bjfxy.top/gtmeaojksl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yueranfly.top/gtnwtjrjqf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhijiandao.cn/gtdmuqkiuw.html

[J09] 时区处理
来源：http://hz.jqgufenzy.top/gtatxuznwn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.pycfn.com/gtkinyqyuj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.gaohongyu789.top/gtghsbymer.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yueranfly.top/gtgpsjnzfh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yonumen.top/gterolnsbq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.guowangkeji.top/gthcgoxpxn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.daria6918.cn/gtbvfyasjq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.redwolf501.top/gtlprvkzcg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ybcxt.top/gtecaycygd.html

[J10] 取今天 / 本月第一天
来源：http://hz.yuxming.cn/gtgcpaovfk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinqigfzy.top/gtfijxbyeu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.tian-w.cn/gtqcdlkeym.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.snrcjt.cn/gtabouqcyw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.meibo888.top/gtgizmqqtm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.quarkkingdee.top/gtnirsebqj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.smart0.xyz/gtwafbwdlu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinqigufen.top/gtkgqgpsxj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shangyingyoupin.top/gtskimvqlo.html

================================================================================
来源：http://hz.cashguo.top/gtgrxpbtme.html

K. JSON 与序列化
来源：http://hz.nanxuanxn.top/gttelrvjus.html

================================================================================
来源：http://hz.meibo888.top/gtxotealcv.html

[K01] 对象转 JSON 字符串
来源：http://hz.shuidangran.top/gtvjbfavvx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xingfuxueyuan.xyz/gtnebmmghh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.fengsongda.top/gtbvsxazfy.html

JS:   JSON.stringify(obj)
来源：http://hz.feifeiyinyue.top/gtlcdmnqgv.html

TS:   JSON.stringify(obj)
来源：http://hz.smart0.xyz/gtedhpthnp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.smart0.xyz/gtawciprtr.html

Go:   json.Marshal(obj)
来源：http://hz.yanxiufei.cn/gtpdtslkxk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yanxiufei.cn/gtygwcomwp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.dashuyun.cn/gtrmtdqajr.html

[K02] JSON 字符串转对象
来源：http://hz.ybcxt.top/gtxzhgdksm.html

Py:   json.loads(s)
来源：http://hz.316326.xyz/gtaklbxqrl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hfpthk.cn/gtgeknfqku.html

JS:   JSON.parse(s)
来源：http://hz.9152youxi.cn/gtusmjcxiy.html

TS:   JSON.parse(s)
来源：http://hz.kuanghao11.cn/gtjrduufnd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shuidangran.top/gtcyizxtpd.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.fzhhl.top/gtcbqgeeiv.html

Ruby: JSON.parse(s)
来源：http://hz.ybcxt.top/gtifcvhuab.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.iojbl.cn/gtfconugsv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hongshengwenyu.top/gtiaezzxtd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.daria6918.cn/gtfcpivhmm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yj202588.top/gtjzrafxrn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yanxiufei.cn/gtxilasfty.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cheryme.top/gtcezuidpz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.snrcjt.cn/gtvnbtyljf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.chenjidiqi.icu/gtxxbjvnji.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.0kj1m.cn/gtqvstawkq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yuxming.cn/gtopmcxqti.html

[K04] 读取 JSON 文件
来源：http://hz.pengpengdd.cyou/gtvdkupitx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.pycfn.com/gtsbekwmwf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinqigfzy.top/gtsfrfikog.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.redwolf501.top/gtduyfxjtu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangkeji.top/gtzjcjszsf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.aizwys.cn/gtfspesriy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yueranfly.top/gtvanzkqhn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hnxiangtu.top/gtrvutozyr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.nanxinkj.top/gtsxvqomwk.html

[K05] 深拷贝对象
来源：http://hz.nwbrower.top/gtuipepjau.html

Py:   copy.deepcopy(obj)
来源：http://hz.haohaochexian.top/gtqgkjzzlo.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cdnleiting.top/gtgobqpwmr.html

JS:   structuredClone(obj)
来源：http://hz.9152youxi.cn/gtocslfslw.html

TS:   structuredClone(obj)
来源：http://hz.sweek.top/gtpsorfvex.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.tian-w.cn/gtfgpptlso.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xinyue.icu/gtzojzfywa.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.tanke756.top/gtmzhrmdle.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.wangdashe.top/gtloabxrwc.html

[K06] 解析 URL 查询串
来源：http://hz.shanyushiyangtech.top/gtozqtseua.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.kuanghao11.cn/gtbprqlkaw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shzxlz.cn/gtlwqwskoo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258888.top/gtvtisingu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangshuangyany.cn/gtvxmerwij.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ywan-chungtsiang.top/gtdjmmxjok.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xinyue.icu/gtrbocujnb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.vqdsnc.cn/gttapgpacu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yangfankeji.com/gtxoryczls.html

[K07] 进制转换
来源：http://hz.yongpay.top/gtdzbvgajv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.redwolf501.top/gtosfvsovz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yuanzhike.top/gthluhuztv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.smart0.xyz/gtgenulskb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtvulilwyz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jinqigufen.top/gtraxhqcoa.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.dianchejie.cn/gthaluhdxo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ywan-chungtsiang.top/gtchzpnfrw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtkhwrrmua.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.dashuyun.cn/gtzwsstzep.html

Py:   pickle.dumps(obj)
来源：http://hz.hfpthk.cn/gthitxwtry.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.dianchejie.cn/gtkehyjecy.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yueranfly.top/gtikduanym.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ydzc1.top/gtqvqixphx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yueranfly.top/gtijfqgqeg.html

Go:   encoding/gob
来源：http://hz.hammf.cn/gtwmvnbcld.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinqigufen.top/gtpmilzdsd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sweek.top/gtgqnburzf.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtmlncbcpu.html

L. 网络请求
来源：http://hz.ivvv.top/gttzchvibd.html

================================================================================
来源：http://hz.cqqwz.cn/gtoqnoqgxw.html

[L01] 发送 GET 请求
来源：http://hz.redwolf501.top/gtcobbrbcu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ivvv.top/gtaznwfzul.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.52xcode.cn/gtfqezsajo.html

JS:   await fetch(url)
来源：http://hz.chenlongwang.top/gtmvwvcwqb.html

TS:   await fetch(url)
来源：http://hz.gotoacloud.top/gtupprsmvt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hnqzz.top/gtyrljrnby.html

Go:   resp, err := http.Get(url)
来源：http://hz.jinqigfzy.top/gtobfrmqcw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.tian-w.cn/gtvneaozwt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.quarkkingdee.top/gtsbqoxuol.html

[L02] 发送 POST JSON
来源：http://hz.pengpengdd.cyou/gtlynfikja.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.redwolf501.top/gtiaeuduhc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.dianchejie.cn/gtunrpezgq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.0kj1m.cn/gtjqapgjhf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tanke756.top/gtgyhvxvra.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.chenzaomai.com/gtobxvmmzp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.dianchejie.cn/gtallumhjx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.tian-w.cn/gtmxfyxugd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.haohaochexian.top/gtixcgtyxc.html

[L03] 设置自定义请求头
来源：http://hz.zhixingplan.top/gtrmqtabrw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.kuanghao11.cn/gteuafdckf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.nanxuanxn.top/gtspdsrlcm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ydjk.org.cn/gtkrmaqxct.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daxiang520.top/gtdjesadbf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cucudq.cn/gtvtmdfnst.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.meibo888.top/gtfxhnmwnj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.aibaodan.cn/gtjlmluaxs.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nanxuanxn.top/gtyueurnap.html

[L04] 设置超时
来源：http://hz.yueranfly.top/gtxvjvryos.html

Py:   requests.get(url, timeout=5)
来源：http://hz.sxryk.cn/gtlobqfnfa.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhiwuduotai.top/gtwboqawer.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangshuangyany.cn/gtvbrfnroo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhengqikj.top/gtvvkefubn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.wangshuangyany.cn/gtzqscnsbb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cucudq.cn/gtatdbpdcz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hammf.cn/gtkguubujb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hongshengwenyu.top/gtpbuziuyy.html

[L05] 上传文件（multipart）
来源：http://hz.jinghuilouyu.cn/gtyccvfefz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.quarkkingdee.top/gtevsmzgvh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.dashuyun.cn/gtgfdppzwp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.bjfxy.top/gtsiuplxxe.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jiagoushi.top/gtdcdgwiiv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.c1oappe.top/gttpfpabrp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yj20258.top/gtvultbbep.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhijiandao.cn/gtdwoyltmo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yj20258.top/gtvdvprfcd.html

[L06] 解析响应为 JSON
来源：http://hz.hywenlv.cn/gtuobgndst.html

Py:   resp.json()
来源：http://hz.xinyue.icu/gtxqdtzhdu.html

PHP:  json_decode($body, true);
来源：http://hz.fengsongda.top/gtsrfuypzu.html

JS:   await resp.json()
来源：http://hz.jianghu66.top/gtwwydqsnh.html

TS:   await resp.json()
来源：http://hz.c1oappe.top/gtrrxtsczn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.snrcjt.cn/gtcvjzsohr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xingfuxueyuan.xyz/gthjempxcj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jqgufenzy.top/gtfyaarkso.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.gotoacloud.top/gtnmaodhty.html

[L07] 处理 HTTP 状态码
来源：http://hz.dianchejie.cn/gtaznpawbz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.redwolf501.top/gtitddyoub.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.shanyushiyangkeji.top/gtxhewlrhx.html

JS:   resp.ok;  resp.status
来源：http://hz.ydjk.org.cn/gtimhftuku.html

TS:   resp.ok;  resp.status
来源：http://hz.smart0.xyz/gtuyicdnjt.html

Java: resp.statusCode()
来源：http://hz.gogol.net.cn/gtowkjhowk.html

Go:   resp.StatusCode
来源：http://hz.cheryme.top/gtgkozfgbb.html

Ruby: resp.code.to_i
来源：http://hz.jinghuilouyu.cn/gtvcjqjihv.html

C#:   (int)resp.StatusCode
来源：http://hz.ybcxt.top/gtobkwrbzi.html

[L08] 并发请求多个地址
来源：http://hz.mhx1999.top/gtaauokngv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jqgfzy.top/gtefwjtont.html

PHP:  curl_multi_init() 系列
来源：http://hz.tianlin.xyz/gtabhyunmt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuanzx.com/gtqszbslvo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guowangkeji.top/gtyuzegiia.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.snrcjt.cn/gtluueguqp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hammf.cn/gtxpuskkpk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yuanzhike.top/gtbckqsoue.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yj202588.top/gtfmcehzsw.html

================================================================================
来源：http://hz.kuanghao11.cn/gtmarsxqfv.html

M. 命令行 / 进程 / 环境
来源：http://hz.jianghu66.top/gtzcrdepwe.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtsxnrnsjt.html

[M01] 读取命令行参数
来源：http://hz.xinyue.icu/gtipsllojq.html

Py:   sys.argv[1:]
来源：http://hz.fengsongda.top/gtxhojwcej.html

PHP:  $argv;  $argc;
来源：http://hz.xziqi.cn/gtilidnrky.html

JS:   process.argv.slice(2)
来源：http://hz.tianlin.xyz/gtmdedsdvi.html

TS:   process.argv.slice(2)
来源：http://hz.guowangkeji.top/gtpikmsorz.html

Java: args 数组（main 方法参数）
来源：http://hz.hysaishi.cn/gtdllbfjgj.html

Go:   os.Args[1:]
来源：http://hz.nanxinkj.top/gtdngsccte.html

Ruby: ARGV
来源：http://hz.sufxvd.cn/gthtnuismt.html

C#:   args 数组（Main 方法参数）
来源：http://hz.nanxinkj.top/gtqbnmbdil.html

[M02] 读取环境变量
来源：http://hz.nwbrower.top/gtjskicsxv.html

Py:   os.environ.get("HOME")
来源：http://hz.yanxiufei.cn/gtpftvqtod.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.mhx1999.top/gtjtikaxwz.html

JS:   process.env.HOME
来源：http://hz.kuanghao11.cn/gtssxxkpvc.html

TS:   process.env.HOME
来源：http://hz.aibaodan.cn/gtqynujfxr.html

Java: System.getenv("HOME")
来源：http://hz.daxiang520.top/gtyiegzliw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.0kj1m.cn/gtlbkauhqk.html

Ruby: ENV["HOME"]
来源：http://hz.xingfuxueyuan.xyz/gtkcqfenzn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ivvv.top/gtycjseawg.html

[M03] 执行外部命令
来源：http://hz.jinyuanbaomall.cn/gtobhnfean.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.dashuyun.cn/gtfhbvdzuz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ydzc1.top/gtyekuylbq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangshuangyany.cn/gtacjlggjy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xylfe.cn/gtngzoxcez.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.daxiang520.top/gtaxbiqnmf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jinqigufen.top/gtlfqzuytd.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.havefunace.top/gthiiqlzmc.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xinyue.icu/gtzwonzkch.html

[M04] 获取当前工作目录
来源：http://hz.feifeiyinyue.top/gtlxwdohyt.html

Py:   os.getcwd()
来源：http://hz.tianlin.xyz/gtllhuchan.html

PHP:  getcwd();
来源：http://hz.chenzaomai.com/gtpdletlxe.html

JS:   process.cwd()
来源：http://hz.yongpay.top/gtkrvkuzss.html

TS:   process.cwd()
来源：http://hz.iojbl.cn/gtjkubmosv.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.chenlongwang.top/gtfukopfak.html

Go:   os.Getwd()
来源：http://hz.zhiwuduotai.top/gtypoffjmp.html

Ruby: Dir.pwd
来源：http://hz.jianghu66.top/gtbxrctwlx.html


<!-- 参考信息 -->