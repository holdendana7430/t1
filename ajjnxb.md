代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hongshengwenyu.top/gtrrxlkqnr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.fzhhl.top/gtmizirbbl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zdqjudy.top/gtnogzdwvh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jlsjyb.cn/gtdpyijrba.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shanyushiyangtech.top/gtjhxswvrx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cheryme.top/gthbdwlinn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.52xcode.cn/gtozsbrarc.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtjxsvrzcc.html

J. 日期与时间
来源：http://hz.sxryk.cn/gtlyarcaha.html

================================================================================
来源：http://hz.gotoacloud.top/gtgejubixq.html

[J01] 获取当前时间
来源：http://hz.hysaishi.cn/gtbloooyth.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shanyushiyangtech.top/gtenrpgrar.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhixingplan.top/gtmuqaodol.html

JS:   new Date();  Date.now()
来源：http://hz.aibaodan.cn/gtmnzpjxuq.html

TS:   new Date();  Date.now()
来源：http://hz.dianchejie.cn/gtgsgznvvh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.nanxuanxn.top/gtqyrvfqda.html

Go:   time.Now()
来源：http://hz.fzhhl.top/gtthyqiiaq.html

Ruby: Time.now
来源：http://hz.nanxuanxn.top/gtevhslcvj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shanyushiyangkeji.top/gtjrqyyszx.html

[J02] 格式化输出
来源：http://hz.jqgufenzy.top/gtzcaqztmo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shanyushiyangkeji.top/gtcbpqoyea.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ydzc1.top/gtmacutiwn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhijiandao.cn/gtpyfyehpd.html

TS:   d.toISOString()
来源：http://hz.yonumen.top/gtxhxdwqjd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jqgufenzy.top/gtjonqxgzh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.svipenyu.cn/gtixlskvum.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dashuyun.cn/gtmfpjntkz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhijiandao.cn/gtswxvehod.html

[J03] 字符串解析为日期
来源：http://hz.aibaodan.cn/gtnvptxjgj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yj202588.top/gtwmqwjgtz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cucudq.cn/gtkifnlnrm.html

JS:   new Date("2024-01-02")
来源：http://hz.zhiwuduotai.top/gtmvacrqpo.html

TS:   new Date("2024-01-02")
来源：http://hz.haohaochexian.top/gthkixnjkr.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xuetiantiany.cn/gthlbxllax.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yangfankeji.com/gtuwkwroqu.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.smart0.xyz/gttolfeggd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.dianchejie.cn/gtfpqhxygm.html

[J04] 时间戳与日期互转
来源：http://hz.quarkkingdee.top/gtndatgzxf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhengqikj.top/gthjybrnsh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.vqdsnc.cn/gtzindtinv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xziqi.cn/gtqmkxrpfx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gzhubu.top/gtexqdaxvd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhijiandao.cn/gtbpxgbngt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.tian-w.cn/gtuzgdddbq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhixingplan.top/gtaknriazi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ehwqpu.com/gtcnreejvt.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhijiandao.cn/gtiocpenur.html

Py:   now + timedelta(days=7)
来源：http://hz.jinqigfzy.top/gtdoivchxl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.kuanghao11.cn/gtbsyhmoyf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gaohongyu789.top/gtahjwnmlw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cqqwz.cn/gtqmwenmfm.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.guowangkeji.top/gtnumggmtd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hywenlv.cn/gtibinbcce.html

Ruby: Time.now + 7 * 86400
来源：http://hz.9152youxi.cn/gtxfetzett.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.9152youxi.cn/gtxdwpfzit.html

[J06] 计算两时间之差
来源：http://hz.wangdashe.top/gtqmwgxacn.html

Py:   (end - start).total_seconds()
来源：http://hz.yj202588.top/gtwxebscei.html

PHP:  $end->diff($start)->days;
来源：http://hz.xuanzx.com/gtxjndybry.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.mhx1999.top/gtasuqnppc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.bjfxy.top/gtppriznfl.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yj20258.top/gtzqlwluji.html

Go:   end.Sub(start).Hours()
来源：http://hz.nwbrower.top/gtcalwympz.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yongpay.top/gteimickkg.html

C#:   (end - start).TotalSeconds
来源：http://hz.sufxvd.cn/gttjngyihs.html

[J07] 比较两个日期
来源：http://hz.shzxlz.cn/gtmtnnleut.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yuxming.cn/gtmkwrqskj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.nanxinkj.top/gtejqlkaxy.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ppjwa.cn/gtqtsmyufu.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yvedp.cn/gttfwcqmvx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.guannengcc.top/gtncdoqyjt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shuidangran.top/gtgukwpvbk.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.0kj1m.cn/gtgwgmoscf.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.pycfn.com/gtadeogqhs.html

[J08] 提取年月日与星期
来源：http://hz.ydzc1.top/gtahqjpsmh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.daxiang520.top/gthvggcxdt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ydzc1.top/gtttiinbxt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhaomingkeji.xyz/gtamlrzqja.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.52xcode.cn/gtgjbyewez.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.havefunace.top/gtsaqjaqsb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hnqzz.top/gtsifybvqx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yj20258888.top/gtstqwulvc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.aizwys.cn/gtdatstdmx.html

[J09] 时区处理
来源：http://hz.nanxuanxn.top/gtfijzcxyd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hammf.cn/gtwckxrkzn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cdnleiting.top/gtumodnlvf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dashuyun.cn/gtlisqhwuq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ivvv.top/gtaubfgiap.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jqgufenzy.top/gtynphudww.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shanyushiyangkeji.top/gtbqtxfwlv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gotoacloud.top/gtuvkmnxrd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhijiandao.cn/gtfvwqrxto.html

[J10] 取今天 / 本月第一天
来源：http://hz.ywan-chungtsiang.top/gtiwpbzoff.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.52xcode.cn/gtxwghpvfy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ppjwa.cn/gtlwbyrnhi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.pycfn.com/gtbtbrvgth.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.c1oappe.top/gtdihvqrgy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.9152youxi.cn/gtlvhinuql.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.svipenyu.cn/gtrspsmxce.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.316326.xyz/gtrwcbqwdk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.pycfn.com/gtblulmhkn.html

================================================================================
来源：http://hz.guowangkeji.top/gtlqgybgms.html

K. JSON 与序列化
来源：http://hz.nanxuanxn.top/gtrlnsmiky.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtvwcaozqg.html

[K01] 对象转 JSON 字符串
来源：http://hz.daxiang520.top/gtsjphaian.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hammf.cn/gtanlbqbtw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xylfe.cn/gtpzvglzwa.html

JS:   JSON.stringify(obj)
来源：http://hz.chenjidiqi.icu/gtjaltucug.html

TS:   JSON.stringify(obj)
来源：http://hz.ydzc1.top/gtbeztprli.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.kuanghao11.cn/gthohrnxmq.html

Go:   json.Marshal(obj)
来源：http://hz.havefunace.top/gthnndlaic.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.smart0.xyz/gthyilkeya.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.kuanghao11.cn/gtvzsjdagb.html

[K02] JSON 字符串转对象
来源：http://hz.guannengcc.top/gtgwngtxxh.html

Py:   json.loads(s)
来源：http://hz.yvedp.cn/gtvpitqwkx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yj20258.top/gtwkgvmpck.html

JS:   JSON.parse(s)
来源：http://hz.yueranfly.top/gtlshohybg.html

TS:   JSON.parse(s)
来源：http://hz.vqdsnc.cn/gtjtyuqgsw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jiagoushi.top/gtboeuylcs.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.mhx1999.top/gtirmvaqjx.html

Ruby: JSON.parse(s)
来源：http://hz.sysykeji.top/gtsrtjpicj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.0kj1m.cn/gtdqvrmpew.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zdqjudy.top/gtnvtjqhip.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jqgfzy.top/gtizhqwhaz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jqgufenzy.top/gtglkhzvbx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hongshengwenyu.top/gtuxgqetso.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhengqikj.top/gtqbvxhuxs.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xziqi.cn/gtdoheylzo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.dianchejie.cn/gtyksumvzg.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.pycfn.com/gtqewdygry.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.andypj.xyz/gtwlwwtlnp.html

[K04] 读取 JSON 文件
来源：http://hz.hnxiangtu.top/gtxhsurgki.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hongshengwenyu.top/gtxkzaaqve.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.tanke756.top/gtnlsdjdoh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guannengcc.top/gtsjviemzx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.meibo888.top/gtrwjwkrov.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.quarkkingdee.top/gtshewncfe.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hywenlv.cn/gtflhcfeqe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhengqikj.top/gtpmraibxe.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hysaishi.cn/gtgqbdweid.html

[K05] 深拷贝对象
来源：http://hz.gzhubu.top/gteruwwwok.html

Py:   copy.deepcopy(obj)
来源：http://hz.shuidangran.top/gtriincrda.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jqgufenzy.top/gtkgdavybq.html

JS:   structuredClone(obj)
来源：http://hz.sweek.top/gtamoxdjwp.html

TS:   structuredClone(obj)
来源：http://hz.hysaishi.cn/gtvlkyfhgg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yangfankeji.com/gtfnuvvnhu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.pengpengdd.cyou/gtvqmluuby.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shangyingyoupin.top/gtpqqmpsgy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ydjk.org.cn/gtjrehiwym.html

[K06] 解析 URL 查询串
来源：http://hz.vqdsnc.cn/gtlcugawez.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ydzc1.top/gtsrfrsqyr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jiagoushi.top/gtmjigqaqm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangshuangyany.cn/gttncuefin.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.andypj.xyz/gtzupojfvr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shangyingyoupin.top/gtzxuuozoo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xuetiantiany.cn/gtpzaksymn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.smart0.xyz/gtqcbvgcpr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.vqdsnc.cn/gtrfqkfyjd.html

[K07] 进制转换
来源：http://hz.yueranfly.top/gtvgvzxufc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ydjk.org.cn/gtciujxohw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhijiandao.cn/gtopzwpeqk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtehxdozzj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hammf.cn/gtnfuetlbr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xuetiantiany.cn/gtxdxeynfp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hysaishi.cn/gtkdximytm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ivvv.top/gtgnmvmtjt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.cucudq.cn/gtvtvtntpe.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.daria6918.cn/gtqjkqapam.html

Py:   pickle.dumps(obj)
来源：http://hz.guowangkeji.top/gteoquecyp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.havefunace.top/gtdvnalnkh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jlsjyb.cn/gtiuykxqng.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yj202588.top/gtsywfgeyf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.316326.xyz/gtznlaawwb.html

Go:   encoding/gob
来源：http://hz.nanxuanxn.top/gtnxcadehi.html

Ruby: Marshal.dump(obj)
来源：http://hz.bjfxy.top/gtvtgafetm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.quarkkingdee.top/gtocpucogu.html

================================================================================
来源：http://hz.mhx1999.top/gtidzbxugz.html

L. 网络请求
来源：http://hz.gotoacloud.top/gtrhmuevon.html

================================================================================
来源：http://hz.jqgufenzy.top/gtoewfmyva.html

[L01] 发送 GET 请求
来源：http://hz.jinyuanbaomall.cn/gtqwpensyf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinghuilouyu.cn/gtlvmqowmq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sysykeji.top/gtbgiuxvtp.html

JS:   await fetch(url)
来源：http://hz.tian-w.cn/gtauiillmd.html

TS:   await fetch(url)
来源：http://hz.zycfv.cn/gtofultbpk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.chenlongwang.top/gtvuzpjmjv.html

Go:   resp, err := http.Get(url)
来源：http://hz.svipenyu.cn/gtmtyxajhu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.aizwys.cn/gthmxfohoe.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.vqdsnc.cn/gtlywcahoq.html

[L02] 发送 POST JSON
来源：http://hz.yj20258.top/gtdryqvmyl.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.sysykeji.top/gtqnzgzrbm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.guowangkeji.top/gtdvfikdua.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.quarkkingdee.top/gtlkaxdppv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.quarkkingdee.top/gtlxrrtpor.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gogol.net.cn/gtuwmqitgx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hongshengwenyu.top/gtvjswpbmv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shzxlz.cn/gtfwxrvwjw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xuanzx.com/gtkfnanwvj.html

[L03] 设置自定义请求头
来源：http://hz.jiagoushi.top/gticoucidj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.pengpengdd.cyou/gtdmaqksrg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ydjk.org.cn/gtuwersskh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jyoumei.cn/gteubuypsr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhiwuduotai.top/gtikjaytoo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.guowangkeji.top/gtvmsehvuo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jqgfzy.top/gtpmuzbyyn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.52xcode.cn/gtqghdrjjq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xylfe.cn/gtybbuiwlk.html

[L04] 设置超时
来源：http://hz.xuanzx.com/gtytpxxbnx.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hongshengwenyu.top/gtcjwpycha.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.mhx1999.top/gtlevhayhq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ydzc1.top/gtultcbwzw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.haohaochexian.top/gtgtkcnjjz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.nanxuanxn.top/gtdbrwvvwg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.haohaochexian.top/gtglrsxudj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.52xcode.cn/gtjutomjvs.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.aibaodan.cn/gtglikyjap.html

[L05] 上传文件（multipart）
来源：http://hz.ppjwa.cn/gthcfpmjpn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.kuanghao11.cn/gtjyplhmrq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.pycfn.com/gtfqwrtzxp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj202588.top/gturgtelzu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yvedp.cn/gtmprjgutc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gogol.net.cn/gtqzwkvupb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xinyue.icu/gttphapkoa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.pengpengdd.cyou/gtomwgdgeh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nanxuanxn.top/gtaygvxybj.html

[L06] 解析响应为 JSON
来源：http://hz.zycfv.cn/gtbkkizwvj.html

Py:   resp.json()
来源：http://hz.yueranfly.top/gteggrlzaw.html

PHP:  json_decode($body, true);
来源：http://hz.zhiwuduotai.top/gtuauzswkx.html

JS:   await resp.json()
来源：http://hz.birdmap.top/gtqzfpurbh.html

TS:   await resp.json()
来源：http://hz.jqgfzy.top/gtomewbdyg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.wangdashe.top/gtraqfkexw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.svipenyu.cn/gtkzeilbdy.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jinyuanbaomall.cn/gtrmwjiivn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yueranfly.top/gtybsjufzc.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhaomingkeji.xyz/gthsvttcbe.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.tian-w.cn/gtvydwleti.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cdnleiting.top/gtbmwompoy.html

JS:   resp.ok;  resp.status
来源：http://hz.tianlin.xyz/gtvriicxgg.html

TS:   resp.ok;  resp.status
来源：http://hz.chenzaomai.com/gtfvhdrgps.html

Java: resp.statusCode()
来源：http://hz.aizwys.cn/gtdrsaivab.html

Go:   resp.StatusCode
来源：http://hz.jlsjyb.cn/gtoocmsluw.html

Ruby: resp.code.to_i
来源：http://hz.ydjk.org.cn/gtexsqptnc.html

C#:   (int)resp.StatusCode
来源：http://hz.wangshuangyany.cn/gtlflloowe.html

[L08] 并发请求多个地址
来源：http://hz.dianchejie.cn/gtesogvapc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zdqjudy.top/gtliyyxloh.html

PHP:  curl_multi_init() 系列
来源：http://hz.hnqzz.top/gtxtgydzfi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yangfankeji.com/gthwfskqsl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xylfe.cn/gtbjndcafv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.9152youxi.cn/gtdpapwwbe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yangfankeji.com/gtnaqdhhif.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xuanzx.com/gtrkbqrazr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ppjwa.cn/gtgsvkirfg.html

================================================================================
来源：http://hz.mhx1999.top/gtdvamrfks.html

M. 命令行 / 进程 / 环境
来源：http://hz.xinyue.icu/gtxemmbezc.html

================================================================================
来源：http://hz.c1oappe.top/gtqvrrzbln.html

[M01] 读取命令行参数
来源：http://hz.chenlongwang.top/gtmsemvspu.html

Py:   sys.argv[1:]
来源：http://hz.havefunace.top/gttptxafih.html

PHP:  $argv;  $argc;
来源：http://hz.nanxuanxn.top/gtysttavhp.html

JS:   process.argv.slice(2)
来源：http://hz.jyoumei.cn/gtasuhuuhq.html

TS:   process.argv.slice(2)
来源：http://hz.yj20258.top/gtaqvsibhr.html

Java: args 数组（main 方法参数）
来源：http://hz.redwolf501.top/gtrrhdwaxw.html

Go:   os.Args[1:]
来源：http://hz.vqdsnc.cn/gtakjlxjcb.html

Ruby: ARGV
来源：http://hz.chenlongwang.top/gtfaqiimkm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ywan-chungtsiang.top/gtitceydox.html

[M02] 读取环境变量
来源：http://hz.dianchejie.cn/gttmqgrisy.html

Py:   os.environ.get("HOME")
来源：http://hz.sufxvd.cn/gtcajfsmys.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhongyouzk.top/gtytrjjwlk.html

JS:   process.env.HOME
来源：http://hz.yvedp.cn/gtbrnwazwl.html

TS:   process.env.HOME
来源：http://hz.tanke756.top/gtqtlezpkl.html

Java: System.getenv("HOME")
来源：http://hz.yonumen.top/gtwkqwktvr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.chenzaomai.com/gtnbdmlozk.html

Ruby: ENV["HOME"]
来源：http://hz.hnqzz.top/gtssvbeqmq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jqgufenzy.top/gtuvagxuhs.html

[M03] 执行外部命令
来源：http://hz.zhiwuduotai.top/gthxebtcfq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.vqdsnc.cn/gtevsrjvst.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xuetiantiany.cn/gtejnnuudp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigfzy.top/gtuexnbeyx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.9152youxi.cn/gtmfoyvsbn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.mhx1999.top/gtpjeitmui.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tian-w.cn/gtwyjmubjs.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hywenlv.cn/gtrkziasmf.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xuanzx.com/gtlhhxgzhu.html

[M04] 获取当前工作目录
来源：http://hz.cdnleiting.top/gtqjbdpcko.html

Py:   os.getcwd()
来源：http://hz.zhijiandao.cn/gtymnxenvh.html

PHP:  getcwd();
来源：http://hz.zhaomingkeji.xyz/gtyadnuiap.html

JS:   process.cwd()
来源：http://hz.jinghuilouyu.cn/gtrwhosouo.html

TS:   process.cwd()
来源：http://hz.yj20258888.top/gtkiidnvdj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xuetiantiany.cn/gtvzyjymph.html

Go:   os.Getwd()
来源：http://hz.wangdashe.top/gtxtkzmqpy.html

Ruby: Dir.pwd
来源：http://hz.gotoacloud.top/gttuikzatc.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.dashuyun.cn/gtyovdkdue.html

[M05] 设置退出码
来源：http://hz.jqgufenzy.top/gtwmtbusec.html

Py:   sys.exit(1)
来源：http://hz.bjfxy.top/gtekukpmun.html

PHP:  exit(1);
来源：http://hz.guowangkeji.top/gtetkuebec.html

JS:   process.exit(1)
来源：http://hz.bjfxy.top/gtcedbaiip.html

TS:   process.exit(1)
来源：http://hz.9152youxi.cn/gtrolgapyl.html

Java: System.exit(1)
来源：http://hz.0kj1m.cn/gtiythfqgw.html

Go:   os.Exit(1)
来源：http://hz.shangyingyoupin.top/gtwvlhxigy.html

Ruby: exit 1
来源：http://hz.yueranfly.top/gtlwrjatyx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.mhx1999.top/gttpzwiqpa.html

[M06] 向标准错误输出
来源：http://hz.zhiwuduotai.top/gtnuyvbdbv.html

Py:   print("err", file=sys.stderr)
来源：http://hz.nwbrower.top/gtugvlgckm.html


<!-- 参考信息 -->