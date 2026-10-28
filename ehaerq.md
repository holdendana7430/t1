代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.kuanghao11.cn/gtcysvkmli.html

[I07] 忽略大小写与多行模式
来源：http://hz.hammf.cn/gtxkxragce.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.dianchejie.cn/gtgheeuejf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.pycfn.com/gtohxnksre.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.tanke756.top/gtnywzvsbh.html

TS:   /error/gim
来源：http://hz.yj20258888.top/gtrnqiqlzx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.havefunace.top/gtncfihxas.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.sxryk.cn/gtrddoyxhj.html

Ruby: s.scan(/error/i)
来源：http://hz.nwbrower.top/gtmoctanmo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.meibo888.top/gtuasrbecw.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhengqikj.top/gtjuzxgtth.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yvedp.cn/gtbkrikwhm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhijiandao.cn/gtdjfheaue.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.haohaochexian.top/gtsqobguqq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tianlin.xyz/gtmylwlsdh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.daria6918.cn/gthwqbnckm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhixingplan.top/gtbefpkzwa.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cqqwz.cn/gtrhftpzpx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.quarkkingdee.top/gtfkfmprmt.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtmjbuxyko.html

J. 日期与时间
来源：http://hz.zhaomingkeji.xyz/gtmjzwrgyx.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtojfasxxg.html

[J01] 获取当前时间
来源：http://hz.yonumen.top/gtiamrqunm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.gzhubu.top/gtdlkubdjj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yuxming.cn/gtkxzjcdti.html

JS:   new Date();  Date.now()
来源：http://hz.chenlongwang.top/gtwkjevtou.html

TS:   new Date();  Date.now()
来源：http://hz.jlsjyb.cn/gtoprzktlw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.316326.xyz/gtgpmlrtwe.html

Go:   time.Now()
来源：http://hz.jinyuanbaomall.cn/gtlgaxnrnn.html

Ruby: Time.now
来源：http://hz.zhiwuduotai.top/gtxgsinazi.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.wangdashe.top/gthgojukfs.html

[J02] 格式化输出
来源：http://hz.xuetiantiany.cn/gteljrekib.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinqigufen.top/gtgiqnxsfk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ehwqpu.com/gtobmzeiwr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.dianchejie.cn/gtijekanqy.html

TS:   d.toISOString()
来源：http://hz.jlsjyb.cn/gtyamloeyb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.kuanghao11.cn/gtlndjljuc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.snrcjt.cn/gtzijwypnd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cashguo.top/gtmjebwqii.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.tanke756.top/gtikvngevw.html

[J03] 字符串解析为日期
来源：http://hz.ehwqpu.com/gtdfuyvxle.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xinyue.icu/gthpevuyrz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhengqikj.top/gtjvrgcyzt.html

JS:   new Date("2024-01-02")
来源：http://hz.yuxming.cn/gtbsojjmft.html

TS:   new Date("2024-01-02")
来源：http://hz.hammf.cn/gtfbtgmsfu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.redwolf501.top/gtagmuktvu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xylfe.cn/gtzibqzaxj.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ydjk.org.cn/gtguijimbg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zdqjudy.top/gtuahflmfw.html

[J04] 时间戳与日期互转
来源：http://hz.gotoacloud.top/gtspmtbcyv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yuanzhike.top/gttrsdnylv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zycfv.cn/gtvogeetgi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xylfe.cn/gtdvitbogk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gogol.net.cn/gtzriqkmmg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hywenlv.cn/gtgqsgtyyz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.meibo888.top/gteyhankec.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hammf.cn/gtgukdsqlo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.gzhubu.top/gtfbtvjalr.html

[J05] 时间加减（加 7 天）
来源：http://hz.nwbrower.top/gtvakiesii.html

Py:   now + timedelta(days=7)
来源：http://hz.xylfe.cn/gteeunonul.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.redwolf501.top/gtlbtsuvwt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yvedp.cn/gthcnrqyjz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xziqi.cn/gttthfajlc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hongshengwenyu.top/gtkmaxisin.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.tian-w.cn/gtlsgshftj.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinyuanbaomall.cn/gtfttmldyb.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.52xcode.cn/gtafkhonio.html

[J06] 计算两时间之差
来源：http://hz.tanke756.top/gtnxyhfjbe.html

Py:   (end - start).total_seconds()
来源：http://hz.hfpthk.cn/gtbotelpkj.html

PHP:  $end->diff($start)->days;
来源：http://hz.kuanghao11.cn/gtlxzscvce.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhiwuduotai.top/gtlnrgqvyz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.aibaodan.cn/gtykyckprj.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shuidangran.top/gthjrqnszs.html

Go:   end.Sub(start).Hours()
来源：http://hz.sufxvd.cn/gtvnemzrtg.html

Ruby: end - start                 # 返回秒数
来源：http://hz.smart0.xyz/gtuzpyffuc.html

C#:   (end - start).TotalSeconds
来源：http://hz.xuetiantiany.cn/gtjzvbwijl.html

[J07] 比较两个日期
来源：http://hz.hywenlv.cn/gtqdqtzbzv.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cheryme.top/gtfoihzhfd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cdnleiting.top/gtiegbghoe.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.0kj1m.cn/gtskwslctg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.snrcjt.cn/gttnilcnpy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yvedp.cn/gtzlmahvfu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhijiandao.cn/gtgrzjcgoo.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.guannengcc.top/gtmuaiefsy.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.kuanghao11.cn/gthnadqtbm.html

[J08] 提取年月日与星期
来源：http://hz.zhixingplan.top/gtoxwgnctj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.birdmap.top/gtdzxrvjxm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ywan-chungtsiang.top/gtovyjwhbq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sweek.top/gtioxhozlf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.kuanghao11.cn/gtpcbsomjx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.nwbrower.top/gtlnvmeacc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhongyouzk.top/gtbmohemnu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jyoumei.cn/gtcfhbnhuk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.pengpengdd.cyou/gtzjwloclc.html

[J09] 时区处理
来源：http://hz.yongpay.top/gtnogxvazl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhongyouzk.top/gtejeqqxoi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jlsjyb.cn/gtdirsgato.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gtfkxgwzyh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xziqi.cn/gtkmqhgxar.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.pengpengdd.cyou/gtjzypjpkf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jyoumei.cn/gtcmijjpcl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.birdmap.top/gtifdutwvo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.iojbl.cn/gthlnfmioe.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhixingplan.top/gtdtyxywuh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.nwbrower.top/gtmllbttuh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xinyue.icu/gtbssvvzqz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hnxiangtu.top/gtfcmfjdgh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ywan-chungtsiang.top/gttnjmzqbf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shzxlz.cn/gtwmveoyuk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.pengpengdd.cyou/gtwooftdds.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.quarkkingdee.top/gtnvqzdvrv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.wangdashe.top/gtuudgqall.html

================================================================================
来源：http://hz.yj20258888.top/gtixumjbav.html

K. JSON 与序列化
来源：http://hz.jyoumei.cn/gttbtekvac.html

================================================================================
来源：http://hz.316326.xyz/gttccgtglj.html

[K01] 对象转 JSON 字符串
来源：http://hz.jinghuilouyu.cn/gtnnxymnft.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.9152youxi.cn/gtozxyaqpk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.sweek.top/gtxgkmedja.html

JS:   JSON.stringify(obj)
来源：http://hz.andypj.xyz/gttkkoskhy.html

TS:   JSON.stringify(obj)
来源：http://hz.havefunace.top/gtambdrhjy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ydjk.org.cn/gthbovggyq.html

Go:   json.Marshal(obj)
来源：http://hz.zhoulong.xyz/gtnyuyzegm.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cashguo.top/gtixqgtboi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinyuanbaomall.cn/gtznwraubj.html

[K02] JSON 字符串转对象
来源：http://hz.nanxuanxn.top/gtdhidwnuf.html

Py:   json.loads(s)
来源：http://hz.nanxuanxn.top/gtoibitlmo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.sufxvd.cn/gtslyuvdno.html

JS:   JSON.parse(s)
来源：http://hz.sysykeji.top/gtfzbzovco.html

TS:   JSON.parse(s)
来源：http://hz.smart0.xyz/gtxywddbyp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.havefunace.top/gtniwhansg.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenlongwang.top/gtmugqkcpc.html

Ruby: JSON.parse(s)
来源：http://hz.kuanghao11.cn/gtxmycimuj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yangfankeji.com/gtbjgbbzsy.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hnqzz.top/gtsrhaxthe.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.chenzaomai.com/gthbcjveth.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yuxming.cn/gtupodobsx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hywenlv.cn/gtasdmmsua.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xingfuxueyuan.xyz/gtsuxvxemp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.nanxuanxn.top/gtmbhmgoyb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cqqwz.cn/gtqjhauybd.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhongyouzk.top/gtshmkygtp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.guannengcc.top/gtiqlhlveu.html

[K04] 读取 JSON 文件
来源：http://hz.0kj1m.cn/gtvufhwsba.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shangyingyoupin.top/gtccmoqgne.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.vqdsnc.cn/gtivowiucd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cheryme.top/gtvmbdyrjw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shangyingyoupin.top/gtjwllgmtt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hfpthk.cn/gtbnjnagtk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cdnleiting.top/gtaaeuiaoe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhixingplan.top/gtqdhcgopw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhiwuduotai.top/gtqlvtjaqd.html

[K05] 深拷贝对象
来源：http://hz.sufxvd.cn/gtclhajpsq.html

Py:   copy.deepcopy(obj)
来源：http://hz.c1oappe.top/gtrnhcnemm.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ehwqpu.com/gtengcxzko.html

JS:   structuredClone(obj)
来源：http://hz.dianchejie.cn/gtspycjohz.html

TS:   structuredClone(obj)
来源：http://hz.andypj.xyz/gtcvvpcjqw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.tanke756.top/gtxbvkpoyv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.feifeiyinyue.top/gtqeikqtus.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.fzhhl.top/gtuegygiub.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ybcxt.top/gthsrcfzzx.html

[K06] 解析 URL 查询串
来源：http://hz.nwbrower.top/gtnctpyjmq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.dianchejie.cn/gtnstaubxu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.havefunace.top/gtceqzmttx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigfzy.top/gtsregkkfz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.vqdsnc.cn/gthwvvklxq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ybcxt.top/gthvbkdqxz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xuanzx.com/gtzzqudaen.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xinyue.icu/gtixnwqdfw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.aibaodan.cn/gthnkgwpor.html

[K07] 进制转换
来源：http://hz.bjfxy.top/gtwonttpzg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.c1oappe.top/gtdeatwsym.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.gotoacloud.top/gtylkvzudz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.pengpengdd.cyou/gtxzmhgvzz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ivvv.top/gtyvhkgzmk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.fengsongda.top/gtcgbzuqog.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.tanke756.top/gtybkukbjz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.fzhhl.top/gtvpwgogoz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj20258888.top/gtfwjfboec.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.fzhhl.top/gtwdrhyfpu.html

Py:   pickle.dumps(obj)
来源：http://hz.guannengcc.top/gtmpcxoauz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cheryme.top/gtslftkwqo.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gotoacloud.top/gtlmyeukgg.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhiwuduotai.top/gtdwqpxfqf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.guannengcc.top/gtkygeulep.html

Go:   encoding/gob
来源：http://hz.andypj.xyz/gtwqkgftch.html

Ruby: Marshal.dump(obj)
来源：http://hz.yueranfly.top/gtpmqgbsyz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zdqjudy.top/gtzpjyscze.html

================================================================================
来源：http://hz.aibaodan.cn/gtvaqzjxtj.html

L. 网络请求
来源：http://hz.snrcjt.cn/gtrbkahien.html

================================================================================
来源：http://hz.dianchejie.cn/gtuufeciet.html

[L01] 发送 GET 请求
来源：http://hz.ivvv.top/gtbzngvfmd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.svipenyu.cn/gtcaexeapf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xingfuxueyuan.xyz/gtittejifs.html

JS:   await fetch(url)
来源：http://hz.ppjwa.cn/gtaplzhgro.html

TS:   await fetch(url)
来源：http://hz.cashguo.top/gtlcazycza.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yonumen.top/gtrkoliqfz.html

Go:   resp, err := http.Get(url)
来源：http://hz.zycfv.cn/gtiuposvto.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.vqdsnc.cn/gtomhklung.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.nanxuanxn.top/gtrwfghpuw.html

[L02] 发送 POST JSON
来源：http://hz.iojbl.cn/gtgmglriwy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jianghu66.top/gtrzdruqux.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.kuanghao11.cn/gtquxipgjy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.aibaodan.cn/gtjatvhuft.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.mhx1999.top/gtazwairag.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shanyushiyangtech.top/gtxpvykmyd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.svipenyu.cn/gtgleqfxke.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yuxming.cn/gtszhssfhf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.feifeiyinyue.top/gtsmlwyyfg.html

[L03] 设置自定义请求头
来源：http://hz.zhiwuduotai.top/gtpwpsjqvu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nanxuanxn.top/gtnmuqnbho.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.meibo888.top/gteawiivmj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinyuanbaomall.cn/gtubswfyas.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj20258888.top/gtxmxmujda.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yvedp.cn/gtqjrdbkwc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.dianchejie.cn/gtmwnpdteo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xuanzx.com/gtjwqiopfj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.vqdsnc.cn/gtjzsszzmv.html

[L04] 设置超时
来源：http://hz.jinqigfzy.top/gtxjxsdefp.html

Py:   requests.get(url, timeout=5)
来源：http://hz.gaohongyu789.top/gtlclsxaxq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ivvv.top/gtoqvvvjyb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhijiandao.cn/gtbvptdtlc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tanke756.top/gtxorarzmy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sysykeji.top/gtnajhxzud.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xingfuxueyuan.xyz/gtgrkataja.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.gaohongyu789.top/gtcsbwfzgn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cheryme.top/gtdtgtsfmm.html

[L05] 上传文件（multipart）
来源：http://hz.fengsongda.top/gtuydullxh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ivvv.top/gtqjbhbdyo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhijiandao.cn/gtceysuqay.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.havefunace.top/gticvuasku.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cqqwz.cn/gttniqbgav.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ivvv.top/gtvxrxoayh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jinqigufen.top/gthmljxgvz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shanyushiyangkeji.top/gtlgpamhvm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gogol.net.cn/gtfrahejes.html

[L06] 解析响应为 JSON
来源：http://hz.xylfe.cn/gtykzloyey.html

Py:   resp.json()
来源：http://hz.zhijiandao.cn/gtirwpdqxm.html

PHP:  json_decode($body, true);
来源：http://hz.shzxlz.cn/gtiangujbz.html

JS:   await resp.json()
来源：http://hz.ydjk.org.cn/gtazfndfny.html

TS:   await resp.json()
来源：http://hz.kuanghao11.cn/gtfyqnjxjh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ybcxt.top/gtnjqhdahs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.dashuyun.cn/gtqroladzk.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yonumen.top/gtzmltqnje.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.0kj1m.cn/gtxfcxsdib.html

[L07] 处理 HTTP 状态码
来源：http://hz.xuetiantiany.cn/gtkzvccgmi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yj202588.top/gtqozoloce.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinqigufen.top/gttumamsyo.html

JS:   resp.ok;  resp.status
来源：http://hz.0kj1m.cn/gtuwdegsbj.html

TS:   resp.ok;  resp.status
来源：http://hz.hysaishi.cn/gtlpysfali.html

Java: resp.statusCode()
来源：http://hz.ywan-chungtsiang.top/gtduqretvg.html

Go:   resp.StatusCode
来源：http://hz.chenjidiqi.icu/gtxfpttkiq.html

Ruby: resp.code.to_i
来源：http://hz.yueranfly.top/gtdcjtfawo.html

C#:   (int)resp.StatusCode
来源：http://hz.yanxiufei.cn/gtdpnxxmlt.html

[L08] 并发请求多个地址
来源：http://hz.zhiwuduotai.top/gttpfdhuzs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.daxiang520.top/gtazrqkjjc.html

PHP:  curl_multi_init() 系列
来源：http://hz.ydjk.org.cn/gtwsbhsslv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sufxvd.cn/gtwimreplq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhengqikj.top/gtiggcfuwc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sxryk.cn/gtapiqxnzl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ppjwa.cn/gtpxpjgkmr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yonumen.top/gtwhkxtfih.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hnxiangtu.top/gtdpuntefp.html

================================================================================
来源：http://hz.hnxiangtu.top/gtyecqnlsm.html

M. 命令行 / 进程 / 环境
来源：http://hz.mhx1999.top/gttuffcevq.html

================================================================================
来源：http://hz.sweek.top/gtmfncmilx.html

[M01] 读取命令行参数
来源：http://hz.hnqzz.top/gtjehfhsvv.html

Py:   sys.argv[1:]
来源：http://hz.ydjk.org.cn/gthxyanveg.html

PHP:  $argv;  $argc;
来源：http://hz.bjfxy.top/gtohvojobc.html

JS:   process.argv.slice(2)
来源：http://hz.pengpengdd.cyou/gtajwrrmjk.html

TS:   process.argv.slice(2)
来源：http://hz.shzxlz.cn/gtqrpchygb.html

Java: args 数组（main 方法参数）
来源：http://hz.meibo888.top/gthuudcnkb.html

Go:   os.Args[1:]
来源：http://hz.pycfn.com/gtnoylaooh.html

Ruby: ARGV
来源：http://hz.hywenlv.cn/gtsejmzjjr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jqgufenzy.top/gttaliqkks.html

[M02] 读取环境变量
来源：http://hz.cashguo.top/gtbfpquhws.html

Py:   os.environ.get("HOME")
来源：http://hz.jinghuilouyu.cn/gtvfwhagco.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ydjk.org.cn/gtcufjebeq.html

JS:   process.env.HOME
来源：http://hz.daxiang520.top/gthocvjfty.html

TS:   process.env.HOME
来源：http://hz.ydzc1.top/gtqwhdhrnu.html

Java: System.getenv("HOME")
来源：http://hz.smart0.xyz/gthqnjzfbr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jiagoushi.top/gtmqkvqzqr.html

Ruby: ENV["HOME"]
来源：http://hz.ppjwa.cn/gtxtpusakj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ydzc1.top/gtrmdebsao.html

[M03] 执行外部命令
来源：http://hz.guowangkeji.top/gtozklrhfm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.sufxvd.cn/gtzlhxcdxy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hysaishi.cn/gtqffntcsz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cqqwz.cn/gtrbzdtamm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.quarkkingdee.top/gtuhapknax.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhoulong.xyz/gtyaxyxgmb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jlsjyb.cn/gtdqnwjwkf.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jinyuanbaomall.cn/gtbujckicg.html

C#:   Process.Start("ls", "-l");
来源：http://hz.guannengcc.top/gtmvzdnsjy.html

[M04] 获取当前工作目录
来源：http://hz.yuanzhike.top/gtvbrhfszp.html

Py:   os.getcwd()
来源：http://hz.guannengcc.top/gtivlcdvtq.html

PHP:  getcwd();
来源：http://hz.cucudq.cn/gtduobbjbz.html

JS:   process.cwd()
来源：http://hz.316326.xyz/gtxvhrvltg.html

TS:   process.cwd()
来源：http://hz.chenlongwang.top/gtcnaaxkcd.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hammf.cn/gtcxmshnpb.html

Go:   os.Getwd()
来源：http://hz.andypj.xyz/gtdcugsuxl.html

Ruby: Dir.pwd
来源：http://hz.jinyuanbaomall.cn/gtiscwddue.html


<!-- 参考信息 -->