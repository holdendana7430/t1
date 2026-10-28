代发 wailian999

J. 日期与时间
来源：http://hz.52xcode.cn/gtctycjmwv.html

================================================================================
来源：http://hz.gzhubu.top/gtfadzopsl.html

[J01] 获取当前时间
来源：http://hz.fzhhl.top/gtwsrfgvxa.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinghuilouyu.cn/gthxgifdhm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xuanzx.com/gtoxmfydpl.html

JS:   new Date();  Date.now()
来源：http://hz.wangdashe.top/gtqwautoqd.html

TS:   new Date();  Date.now()
来源：http://hz.birdmap.top/gtfdhhmxqw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinghuilouyu.cn/gtplnbfngn.html

Go:   time.Now()
来源：http://hz.jinqigufen.top/gtxntyxdzw.html

Ruby: Time.now
来源：http://hz.cheryme.top/gttwfgrkiu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.sufxvd.cn/gtyeagummm.html

[J02] 格式化输出
来源：http://hz.zhijiandao.cn/gtphohubnl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangshuangyany.cn/gtygkbekfl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yongpay.top/gtvmhmhydb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.birdmap.top/gtlkxpejoa.html

TS:   d.toISOString()
来源：http://hz.yanxiufei.cn/gturwisyxj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.svipenyu.cn/gtcmhzhuyz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.sweek.top/gtdehpfjws.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sweek.top/gtpxnkzlnz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.9152youxi.cn/gtjolidacb.html

[J03] 字符串解析为日期
来源：http://hz.feifeiyinyue.top/gtffbffpbb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xuanzx.com/gtzyfkblzp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ehwqpu.com/gtapryrebx.html

JS:   new Date("2024-01-02")
来源：http://hz.zhixingplan.top/gtfarnfzfi.html

TS:   new Date("2024-01-02")
来源：http://hz.yueranfly.top/gtsjuugmeo.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.chenlongwang.top/gtezocucvw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yj20258.top/gttragfsbd.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yongpay.top/gtqdgzvume.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xuanzx.com/gtacjgwhmx.html

[J04] 时间戳与日期互转
来源：http://hz.kuanghao11.cn/gthyaqjxbo.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yongpay.top/gtuyoryeqf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhongyouzk.top/gtxqhscplu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xuetiantiany.cn/gtdiaqepvs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hnxiangtu.top/gtcwmoqhlm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.fzhhl.top/gtpfnxkcdf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.feifeiyinyue.top/gtpxakivrd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhijiandao.cn/gtqsmmuckj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.redwolf501.top/gtqurkedjb.html

[J05] 时间加减（加 7 天）
来源：http://hz.yonumen.top/gtrkuccyds.html

Py:   now + timedelta(days=7)
来源：http://hz.mhx1999.top/gtdfjuckfp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yvedp.cn/gtiulipzni.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.guowangkeji.top/gtpphzuqrf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.svipenyu.cn/gtivfptxfm.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.feifeiyinyue.top/gtkqmfvhrr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.quarkkingdee.top/gtrzfrotne.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gotoacloud.top/gtyqejlfer.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.tianlin.xyz/gtfusyxlsb.html

[J06] 计算两时间之差
来源：http://hz.zhongyouzk.top/gtejzpoent.html

Py:   (end - start).total_seconds()
来源：http://hz.gzhubu.top/gtrkvojcyv.html

PHP:  $end->diff($start)->days;
来源：http://hz.shangyingyoupin.top/gtncqatyji.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.gotoacloud.top/gtldpdgvyv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.chenlongwang.top/gtrzobnbuk.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.gogol.net.cn/gtvkubhppf.html

Go:   end.Sub(start).Hours()
来源：http://hz.yj20258.top/gtelfuidld.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ppjwa.cn/gtofdxaxbk.html

C#:   (end - start).TotalSeconds
来源：http://hz.yueranfly.top/gthfzpwnti.html

[J07] 比较两个日期
来源：http://hz.yueranfly.top/gtjpdbfpun.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.smart0.xyz/gtxfomktuf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhijiandao.cn/gtwasisiis.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.snrcjt.cn/gtelkvxpxh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.pycfn.com/gtnaaitrug.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.chenlongwang.top/gtmxinxdxm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.aibaodan.cn/gtyplkbvgb.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.52xcode.cn/gtzbqhybyh.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.c1oappe.top/gtxethnedk.html

[J08] 提取年月日与星期
来源：http://hz.nwbrower.top/gtjeijlgzr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.fzhhl.top/gttcedjsek.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ydjk.org.cn/gtpogiohgv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ivvv.top/gtqhpjmtni.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.aizwys.cn/gtkjmdbcmj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhongyouzk.top/gtrponnptp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.mhx1999.top/gtvrltcwhp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yanxiufei.cn/gtgfvcwiqx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.snrcjt.cn/gtrjzafgmb.html

[J09] 时区处理
来源：http://hz.aibaodan.cn/gtegkypmgh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yueranfly.top/gtdryluzkh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.smart0.xyz/gtwxamietu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.vqdsnc.cn/gtacrrzmno.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangdashe.top/gtvvijrktd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.sweek.top/gtunsobdza.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.chenlongwang.top/gtgjaolzdp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.sxryk.cn/gtzjudgjer.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xuanzx.com/gtssxzdqyq.html

[J10] 取今天 / 本月第一天
来源：http://hz.sxryk.cn/gtdnyqslni.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zdqjudy.top/gtkidbvkfh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.aizwys.cn/gtstttscda.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhijiandao.cn/gtzttoyzil.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yueranfly.top/gtxactxclb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cdnleiting.top/gtlouhuoxg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yonumen.top/gtufdacxqq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shanyushiyangkeji.top/gtfdhlbigm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hysaishi.cn/gtdflnrovu.html

================================================================================
来源：http://hz.aizwys.cn/gtnlluqgbb.html

K. JSON 与序列化
来源：http://hz.yvedp.cn/gtykfakxlb.html

================================================================================
来源：http://hz.xylfe.cn/gtvxtpdfvl.html

[K01] 对象转 JSON 字符串
来源：http://hz.fzhhl.top/gtseitoran.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.0kj1m.cn/gtpvqstldt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yueranfly.top/gtlltsjowt.html

JS:   JSON.stringify(obj)
来源：http://hz.mhx1999.top/gtfyniynwu.html

TS:   JSON.stringify(obj)
来源：http://hz.jinqigfzy.top/gtukzfwsse.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinqigfzy.top/gtaitkofro.html

Go:   json.Marshal(obj)
来源：http://hz.cheryme.top/gtruksssfk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.snrcjt.cn/gttwpyzhmc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.pycfn.com/gtftvotijq.html

[K02] JSON 字符串转对象
来源：http://hz.bjfxy.top/gtkurnbmay.html

Py:   json.loads(s)
来源：http://hz.52xcode.cn/gtrxjosyly.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.fzhhl.top/gteetmffjk.html

JS:   JSON.parse(s)
来源：http://hz.gaohongyu789.top/gtdtbgzntz.html

TS:   JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtkoqlzssd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.nanxuanxn.top/gtwckaytdg.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.meibo888.top/gtptfzjvlc.html

Ruby: JSON.parse(s)
来源：http://hz.chenzaomai.com/gtadawikvr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yonumen.top/gtjzlcbcpa.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cheryme.top/gtdzmgecsg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.haohaochexian.top/gtpakufsjo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yonumen.top/gtfbipbffg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigfzy.top/gtxashxjtg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.aizwys.cn/gtfxingvdz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.tanke756.top/gtgmjjznjy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jlsjyb.cn/gtwjlccgcb.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hongshengwenyu.top/gthqbpijwu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tian-w.cn/gtkrlcnezw.html

[K04] 读取 JSON 文件
来源：http://hz.jqgfzy.top/gtfczxwylf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.nanxinkj.top/gtirdxbpix.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.dianchejie.cn/gtepqawpvl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ppjwa.cn/gtorstsqeq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gzhubu.top/gtvhrkqdnv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ppjwa.cn/gtcqaodsok.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinghuilouyu.cn/gtdptbayqk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.wangdashe.top/gtxxlecoks.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yuxming.cn/gtyodckggz.html

[K05] 深拷贝对象
来源：http://hz.dashuyun.cn/gtmjpljwwd.html

Py:   copy.deepcopy(obj)
来源：http://hz.meibo888.top/gtjtvlutkp.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hywenlv.cn/gtdowsvfvd.html

JS:   structuredClone(obj)
来源：http://hz.kuanghao11.cn/gtrmkrfeso.html

TS:   structuredClone(obj)
来源：http://hz.hammf.cn/gtwlxfvjmu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hnqzz.top/gtybmjysfe.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.iojbl.cn/gtaxpiweqn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.c1oappe.top/gtuavgnelm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.daxiang520.top/gtxcrzitnu.html

[K06] 解析 URL 查询串
来源：http://hz.fengsongda.top/gtpsvfqxqq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cqqwz.cn/gtvnvpiwhu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jiagoushi.top/gtaldbxjpu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tanke756.top/gtckymzyuc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.52xcode.cn/gtveuvvlqg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.wangdashe.top/gtstooxzlo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xingfuxueyuan.xyz/gthuxnzxyg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.tian-w.cn/gtgzhmeezv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.0kj1m.cn/gtfliepmfw.html

[K07] 进制转换
来源：http://hz.shuidangran.top/gtlvgelytz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xylfe.cn/gtluefqjtp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jinqigufen.top/gtgkomwhcj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.tanke756.top/gtqqbtgclc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.iojbl.cn/gtogpzakkl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtojpcxlzi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinyuanbaomall.cn/gtzmntpkax.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.andypj.xyz/gtkzvikyqy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gthngyumov.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.daria6918.cn/gtdmyzjqex.html

Py:   pickle.dumps(obj)
来源：http://hz.yj20258888.top/gtventfnqu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shzxlz.cn/gtbqlxpikb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sysykeji.top/gtiwcmlhae.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.daria6918.cn/gtqnorpqra.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhoulong.xyz/gtoofmqvom.html

Go:   encoding/gob
来源：http://hz.sufxvd.cn/gtabarpwyk.html

Ruby: Marshal.dump(obj)
来源：http://hz.yj20258.top/gtmqjvzpqu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.tanke756.top/gtuoknufnh.html

================================================================================
来源：http://hz.yj20258888.top/gtohebnouy.html

L. 网络请求
来源：http://hz.9152youxi.cn/gtoplzbgps.html

================================================================================
来源：http://hz.nanxuanxn.top/gtsbqobsmz.html

[L01] 发送 GET 请求
来源：http://hz.hnqzz.top/gtnnshexgi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.daria6918.cn/gtsxfazhyq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.c1oappe.top/gtgwvyszde.html

JS:   await fetch(url)
来源：http://hz.jlsjyb.cn/gtewempzhn.html

TS:   await fetch(url)
来源：http://hz.gotoacloud.top/gtlalpweft.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yongpay.top/gtgohsncnq.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhixingplan.top/gtriejnuth.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.0kj1m.cn/gtnexxwnot.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.guowangkeji.top/gtgtkljzvm.html

[L02] 发送 POST JSON
来源：http://hz.zhijiandao.cn/gtwmyszgim.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jqgufenzy.top/gtbdkjfngk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.redwolf501.top/gtbctpwudw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.andypj.xyz/gtxxbthpvb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhixingplan.top/gtjzpumpjo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ivvv.top/gtydoesbau.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.daxiang520.top/gtzqtxwjmm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zycfv.cn/gtxjprhman.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.redwolf501.top/gtbwlccexf.html

[L03] 设置自定义请求头
来源：http://hz.yonumen.top/gtzqcbvdfi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhongyouzk.top/gtoextgknn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cucudq.cn/gtgzhwjczz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.fengsongda.top/gtknubfoky.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zycfv.cn/gtveyyiyjv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.nwbrower.top/gthkbtxkuc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cdnleiting.top/gtdgibcbdr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.havefunace.top/gtgixkqpux.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ivvv.top/gtxlicgdlj.html

[L04] 设置超时
来源：http://hz.tanke756.top/gtetacdqks.html

Py:   requests.get(url, timeout=5)
来源：http://hz.svipenyu.cn/gtigdlyikv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.wangshuangyany.cn/gtmbatnrdx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinqigufen.top/gtbjxgmmdj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hongshengwenyu.top/gtiziosmbe.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jinqigufen.top/gtmxnjdgqj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ivvv.top/gtbucnytiu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yuxming.cn/gttjrjgnvf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.tian-w.cn/gtlrhtlbdw.html

[L05] 上传文件（multipart）
来源：http://hz.fzhhl.top/gtjnqmqibb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zycfv.cn/gtackzfobi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.snrcjt.cn/gtfgxlpzpx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.tanke756.top/gtrbrkcsld.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.feifeiyinyue.top/gtazeqrbrb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cqqwz.cn/gtmuymgqjn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.vqdsnc.cn/gtmmrcndze.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.pengpengdd.cyou/gtzzgbvukj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shanyushiyangtech.top/gtiuizblud.html

[L06] 解析响应为 JSON
来源：http://hz.zhongyouzk.top/gtlmteeppn.html

Py:   resp.json()
来源：http://hz.jqgfzy.top/gtzvwramwt.html

PHP:  json_decode($body, true);
来源：http://hz.ydzc1.top/gtzsylkaxb.html

JS:   await resp.json()
来源：http://hz.yj20258888.top/gtwdgolvvh.html

TS:   await resp.json()
来源：http://hz.wangshuangyany.cn/gttnucpzbq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.tanke756.top/gtxkerutmc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yj20258.top/gtupvxamxz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tianlin.xyz/gtpjamdjky.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jinqigfzy.top/gtbojhwtmp.html

[L07] 处理 HTTP 状态码
来源：http://hz.havefunace.top/gtijluoqir.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yj20258.top/gtfebcywwi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.iojbl.cn/gthrleyebz.html

JS:   resp.ok;  resp.status
来源：http://hz.guannengcc.top/gtuvvusefj.html

TS:   resp.ok;  resp.status
来源：http://hz.hnqzz.top/gtyilzqvgg.html

Java: resp.statusCode()
来源：http://hz.andypj.xyz/gtvxkdemls.html

Go:   resp.StatusCode
来源：http://hz.yj20258888.top/gtauwvleic.html

Ruby: resp.code.to_i
来源：http://hz.xuetiantiany.cn/gtgrjpqdhw.html

C#:   (int)resp.StatusCode
来源：http://hz.9152youxi.cn/gttwxdsdrs.html

[L08] 并发请求多个地址
来源：http://hz.shanyushiyangkeji.top/gtevvofsvr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jqgfzy.top/gtmqutsida.html

PHP:  curl_multi_init() 系列
来源：http://hz.guannengcc.top/gtfqviiniw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.haohaochexian.top/gtnzmdonan.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.mhx1999.top/gtkmwvnces.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yj20258888.top/gtegmgybth.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shanyushiyangkeji.top/gtarwlhlea.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ivvv.top/gtexbfjjgt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jqgfzy.top/gtxbqftpwz.html

================================================================================
来源：http://hz.iojbl.cn/gtofagibph.html

M. 命令行 / 进程 / 环境
来源：http://hz.jlsjyb.cn/gtxntzdphm.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtrjtwrool.html

[M01] 读取命令行参数
来源：http://hz.ywan-chungtsiang.top/gtoezmtmnj.html

Py:   sys.argv[1:]
来源：http://hz.andypj.xyz/gtccslbnjp.html

PHP:  $argv;  $argc;
来源：http://hz.yueranfly.top/gtipanasps.html

JS:   process.argv.slice(2)
来源：http://hz.shanyushiyangkeji.top/gtcaupecwp.html

TS:   process.argv.slice(2)
来源：http://hz.hysaishi.cn/gttfcsonpa.html

Java: args 数组（main 方法参数）
来源：http://hz.yuanzhike.top/gtlukvkxgn.html

Go:   os.Args[1:]
来源：http://hz.gzhubu.top/gtmajlshdw.html

Ruby: ARGV
来源：http://hz.jiagoushi.top/gttjfgfhfl.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ydzc1.top/gtmdbyrmpg.html

[M02] 读取环境变量
来源：http://hz.wangdashe.top/gtjpskivju.html

Py:   os.environ.get("HOME")
来源：http://hz.jinqigufen.top/gtniopszak.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.bjfxy.top/gtdwcpaujk.html

JS:   process.env.HOME
来源：http://hz.jianghu66.top/gtfnaofqcp.html

TS:   process.env.HOME
来源：http://hz.hongshengwenyu.top/gtbycebose.html

Java: System.getenv("HOME")
来源：http://hz.snrcjt.cn/gtysvbdmlb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.bjfxy.top/gtiukylkhl.html

Ruby: ENV["HOME"]
来源：http://hz.tanke756.top/gtapkpspyc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.andypj.xyz/gtwbknwsbx.html

[M03] 执行外部命令
来源：http://hz.hnxiangtu.top/gtlcuuuttk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yj202588.top/gtasqextlh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.smart0.xyz/gtezetsigy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgfzy.top/gtzhwxvbyx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.havefunace.top/gtironrnlf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.gaohongyu789.top/gtsbqomztl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.gotoacloud.top/gtjbpvhzol.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.gaohongyu789.top/gteefpbaok.html

C#:   Process.Start("ls", "-l");
来源：http://hz.nanxuanxn.top/gtajacavol.html

[M04] 获取当前工作目录
来源：http://hz.yj20258888.top/gtqafccvgm.html

Py:   os.getcwd()
来源：http://hz.tianlin.xyz/gtxiypkful.html

PHP:  getcwd();
来源：http://hz.dianchejie.cn/gtnuyrknfg.html

JS:   process.cwd()
来源：http://hz.chenjidiqi.icu/gtqlnsevbg.html

TS:   process.cwd()
来源：http://hz.ywan-chungtsiang.top/gtotypswra.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.kuanghao11.cn/gtqtgvjxqf.html

Go:   os.Getwd()
来源：http://hz.vqdsnc.cn/gtfttzpgmb.html

Ruby: Dir.pwd
来源：http://hz.sxryk.cn/gtihlcfeiq.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shuidangran.top/gtrczgwgmv.html

[M05] 设置退出码
来源：http://hz.jinqigufen.top/gtpnxhwnet.html

Py:   sys.exit(1)
来源：http://hz.yuxming.cn/gtszrijjsb.html

PHP:  exit(1);
来源：http://hz.cheryme.top/gtdfqfaslv.html

JS:   process.exit(1)
来源：http://hz.gotoacloud.top/gtmwtiuxue.html

TS:   process.exit(1)
来源：http://hz.zhiwuduotai.top/gtztvhlqzj.html

Java: System.exit(1)
来源：http://hz.bjfxy.top/gtkwsgqvcj.html

Go:   os.Exit(1)
来源：http://hz.zhiwuduotai.top/gttprlrgbk.html

Ruby: exit 1
来源：http://hz.guowangkeji.top/gthmzovhjc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.mhx1999.top/gtzcrdpdjp.html

[M06] 向标准错误输出
来源：http://hz.daria6918.cn/gthtyaoors.html

Py:   print("err", file=sys.stderr)
来源：http://hz.bjfxy.top/gtoxvdfucu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yueranfly.top/gthhmzrtbe.html

JS:   console.error("err")
来源：http://hz.ppjwa.cn/gtzywyrxzs.html

TS:   console.error("err")
来源：http://hz.daria6918.cn/gtqysapdrm.html

Java: System.err.println("err")
来源：http://hz.zycfv.cn/gtavlwasui.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.gaohongyu789.top/gtmivssldj.html

Ruby: warn "err"
来源：http://hz.guowangkeji.top/gtlwlefdlv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.vqdsnc.cn/gthzaizwqm.html

[M07] 判断是否为主入口
来源：http://hz.yj20258888.top/gtxcyjtqwj.html


<!-- 参考信息 -->