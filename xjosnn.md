代发 wailian999

[J03] 字符串解析为日期
来源：http://hz.zycfv.cn/gtuddnrrxd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.aibaodan.cn/gtgkphpeuq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinqigfzy.top/gtraninraz.html

JS:   new Date("2024-01-02")
来源：http://hz.9152youxi.cn/gttlrflowz.html

TS:   new Date("2024-01-02")
来源：http://hz.shuidangran.top/gthipxgyem.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhongyouzk.top/gtywbyrlio.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jianghu66.top/gteubwnaya.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.316326.xyz/gtlmkwysdy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.kuanghao11.cn/gtibokjkvr.html

[J04] 时间戳与日期互转
来源：http://hz.gotoacloud.top/gtmcvbvdur.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.havefunace.top/gtpsrpmyka.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jinqigfzy.top/gtyhlspmni.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinyuanbaomall.cn/gtiviafsrc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yanxiufei.cn/gtzsqdmapd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.aibaodan.cn/gttohbpsvp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.haohaochexian.top/gtnsacbuue.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.meibo888.top/gtlpbvidbu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.redwolf501.top/gtzuzctort.html

[J05] 时间加减（加 7 天）
来源：http://hz.ydzc1.top/gtoyiikkwc.html

Py:   now + timedelta(days=7)
来源：http://hz.pycfn.com/gttuwsxdch.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.guannengcc.top/gtdqqevhzs.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.havefunace.top/gtrjjlgzuf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangdashe.top/gtjvuooekb.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.andypj.xyz/gtcnldjvom.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xingfuxueyuan.xyz/gtidrxcqip.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gotoacloud.top/gtfzwhkhnx.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhaomingkeji.xyz/gtzpmusbew.html

[J06] 计算两时间之差
来源：http://hz.gaohongyu789.top/gthzephuli.html

Py:   (end - start).total_seconds()
来源：http://hz.yj20258.top/gtnaaxipnq.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinyuanbaomall.cn/gtvlkglyrl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ydjk.org.cn/gtrcjkolek.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.chenzaomai.com/gtvaildmec.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.316326.xyz/gtbyplfyuq.html

Go:   end.Sub(start).Hours()
来源：http://hz.smart0.xyz/gtcazhijkf.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhixingplan.top/gtyyoqxuln.html

C#:   (end - start).TotalSeconds
来源：http://hz.mhx1999.top/gtwtovwgks.html

[J07] 比较两个日期
来源：http://hz.jinyuanbaomall.cn/gtmfshcokg.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jinqigfzy.top/gtwahlbjnv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhiwuduotai.top/gtqabsiryf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.chenjidiqi.icu/gtwjbhigni.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.feifeiyinyue.top/gtzlqzgaks.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yueranfly.top/gtwvgphgmj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.pycfn.com/gtsqqiaawn.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zdqjudy.top/gtwuqelxux.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yonumen.top/gtchkizwqf.html

[J08] 提取年月日与星期
来源：http://hz.cdnleiting.top/gttfjydqxv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.iojbl.cn/gtmaxxxkmi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hongshengwenyu.top/gtpufbkebb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cashguo.top/gtaousyngz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.haohaochexian.top/gtqnyuvrmy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.52xcode.cn/gtijemjiuo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hongshengwenyu.top/gtqkidcdio.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenzaomai.com/gtacrixgsv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jiagoushi.top/gtoxolbzbz.html

[J09] 时区处理
来源：http://hz.smart0.xyz/gtpqclielp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ivvv.top/gtpluyrwvc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.nwbrower.top/gtnmkssiwd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.birdmap.top/gtizdjtifb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dianchejie.cn/gtnqutzbvr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nanxuanxn.top/gtwmyzchss.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xinyue.icu/gtjhaixyhq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.daxiang520.top/gtthqieicb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.dianchejie.cn/gthxwzzsao.html

[J10] 取今天 / 本月第一天
来源：http://hz.meibo888.top/gttrrelesk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jyoumei.cn/gtzvreikse.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.svipenyu.cn/gtoubumrkb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.tian-w.cn/gtejklfbil.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinyuanbaomall.cn/gtmxkdfccl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.0kj1m.cn/gtozsneeqx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xuetiantiany.cn/gtlmuiwzcc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhongyouzk.top/gtvrioqiej.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yvedp.cn/gtisklppos.html

================================================================================
来源：http://hz.hnqzz.top/gtksfvdatv.html

K. JSON 与序列化
来源：http://hz.hongshengwenyu.top/gtfqcpthkm.html

================================================================================
来源：http://hz.xinyue.icu/gtqyakgflb.html

[K01] 对象转 JSON 字符串
来源：http://hz.dashuyun.cn/gtuquhdnmj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.wangshuangyany.cn/gtxyuyoixs.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.0kj1m.cn/gttmzgiyzd.html

JS:   JSON.stringify(obj)
来源：http://hz.kuanghao11.cn/gtdqmftcwn.html

TS:   JSON.stringify(obj)
来源：http://hz.jiagoushi.top/gtxlaotkwr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.316326.xyz/gtbjipsgqj.html

Go:   json.Marshal(obj)
来源：http://hz.sweek.top/gtuwysrkgn.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xuetiantiany.cn/gtsljxaxtu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.fzhhl.top/gtkaufeqek.html

[K02] JSON 字符串转对象
来源：http://hz.cheryme.top/gtzrbhfpxh.html

Py:   json.loads(s)
来源：http://hz.jinghuilouyu.cn/gtpyrvekud.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shanyushiyangtech.top/gtooxlazdm.html

JS:   JSON.parse(s)
来源：http://hz.yj20258.top/gtnpihfgun.html

TS:   JSON.parse(s)
来源：http://hz.wangdashe.top/gtgllezjdv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cheryme.top/gteqekzlps.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.tanke756.top/gtqepljiuv.html

Ruby: JSON.parse(s)
来源：http://hz.tian-w.cn/gtoguyuctj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zycfv.cn/gtzyqsquqs.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.dashuyun.cn/gttpqtazgr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xingfuxueyuan.xyz/gtqpfnoqii.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.guannengcc.top/gttecirryj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cashguo.top/gtwbxelcwo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.snrcjt.cn/gtfxdumzaf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yanxiufei.cn/gtoyzodmkz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ybcxt.top/gtttaxmhrt.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hfpthk.cn/gtmzewkhla.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhengqikj.top/gtozwztbfu.html

[K04] 读取 JSON 文件
来源：http://hz.yonumen.top/gtenanzwcs.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jqgufenzy.top/gtyxvzrohh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ppjwa.cn/gtfkwfjlrq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dashuyun.cn/gtrvfkyafr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hywenlv.cn/gtxktirkup.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shuidangran.top/gtuvgtqkmx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ehwqpu.com/gtzloiwhdb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yanxiufei.cn/gtkwojfkxy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.gaohongyu789.top/gtedoncqsc.html

[K05] 深拷贝对象
来源：http://hz.cheryme.top/gtssjkbriu.html

Py:   copy.deepcopy(obj)
来源：http://hz.ywan-chungtsiang.top/gtzcyesxuw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhijiandao.cn/gtdwarikgp.html

JS:   structuredClone(obj)
来源：http://hz.smart0.xyz/gtngkxxbob.html

TS:   structuredClone(obj)
来源：http://hz.sweek.top/gtbjgcbpzt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.chenzaomai.com/gtnpwudzaf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhijiandao.cn/gtysiiaeae.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.sxryk.cn/gtvxpjyqrw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.wangshuangyany.cn/gtliwvhuyg.html

[K06] 解析 URL 查询串
来源：http://hz.mhx1999.top/gtvrbguedj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.tanke756.top/gtkxijygih.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.iojbl.cn/gtiqmikovx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.haohaochexian.top/gtqipktvvv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangdashe.top/gtgzasxjin.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hysaishi.cn/gteislcanw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.iojbl.cn/gtbaicvgqh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.nwbrower.top/gtojluuxgl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.havefunace.top/gtymcfcfwt.html

[K07] 进制转换
来源：http://hz.jianghu66.top/gtiqolldsq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtgywzhtph.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.vqdsnc.cn/gtcxvflfve.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhiwuduotai.top/gtlsnsbmvc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.dianchejie.cn/gtasumeech.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.sxryk.cn/gtlmzeczda.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yvedp.cn/gtabfrjxdj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ywan-chungtsiang.top/gtwoqnsezn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yangfankeji.com/gtwhkagnws.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xingfuxueyuan.xyz/gtldqaupyk.html

Py:   pickle.dumps(obj)
来源：http://hz.guannengcc.top/gtoghnzbzz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinyuanbaomall.cn/gtlxdjkmvt.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cqqwz.cn/gtigtcojzh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.feifeiyinyue.top/gtesqhwwyw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenzaomai.com/gtveiprxtl.html

Go:   encoding/gob
来源：http://hz.jqgfzy.top/gttngsivmg.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinqigfzy.top/gtiyqofppo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhijiandao.cn/gttszkfrwe.html

================================================================================
来源：http://hz.0kj1m.cn/gtfaykwruo.html

L. 网络请求
来源：http://hz.jyoumei.cn/gthdkshdgi.html

================================================================================
来源：http://hz.yongpay.top/gtsdrmbtti.html

[L01] 发送 GET 请求
来源：http://hz.zhiwuduotai.top/gtnczcrtkl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gaohongyu789.top/gtiqqxdkjn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shanyushiyangtech.top/gtybjitbgc.html

JS:   await fetch(url)
来源：http://hz.hysaishi.cn/gtrcbplens.html

TS:   await fetch(url)
来源：http://hz.jlsjyb.cn/gtwwuhtfvl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.redwolf501.top/gtkttwkpoq.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhoulong.xyz/gtxssnvduf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.birdmap.top/gtrsxxprry.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ppjwa.cn/gtiomrllhk.html

[L02] 发送 POST JSON
来源：http://hz.xingfuxueyuan.xyz/gtrriwmdsh.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hnqzz.top/gtlvyckcrh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hongshengwenyu.top/gtctzxvhse.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sysykeji.top/gtxzsiudfs.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hfpthk.cn/gtcidefyqk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ybcxt.top/gtgzvcmzjv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhiwuduotai.top/gtytwvqoof.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ydjk.org.cn/gtbbnfngms.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ydjk.org.cn/gtarwstden.html

[L03] 设置自定义请求头
来源：http://hz.nanxinkj.top/gtyaqfnzat.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jqgufenzy.top/gtrrxixnni.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ppjwa.cn/gtkgkcuqtx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhiwuduotai.top/gtowldlnxp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tian-w.cn/gttyszbmtl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhijiandao.cn/gtmsyykegl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jqgufenzy.top/gtkooemmhi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.mhx1999.top/gtjglnmqbt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.vqdsnc.cn/gtagobznoh.html

[L04] 设置超时
来源：http://hz.birdmap.top/gtwonumirb.html

Py:   requests.get(url, timeout=5)
来源：http://hz.mhx1999.top/gtojfenhux.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sysykeji.top/gtwzkdtobh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.0kj1m.cn/gtkwvijzaj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258.top/gtwqbicdyj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.vqdsnc.cn/gtsgwooqds.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj202588.top/gtbdpezzhw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.52xcode.cn/gtqmpcpeub.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.tanke756.top/gttkfjvlrk.html

[L05] 上传文件（multipart）
来源：http://hz.ybcxt.top/gtjqzxznms.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.fzhhl.top/gtoxtroadj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.guannengcc.top/gtzilhjsqw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.mhx1999.top/gtywtjgyty.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj20258888.top/gtmtxylrcp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hysaishi.cn/gtpiwhskhf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xingfuxueyuan.xyz/gtxaopthio.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ybcxt.top/gtjwlvtmha.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hnxiangtu.top/gthrpaxnkp.html

[L06] 解析响应为 JSON
来源：http://hz.yvedp.cn/gteoyieoem.html

Py:   resp.json()
来源：http://hz.cdnleiting.top/gtacoxjzrq.html

PHP:  json_decode($body, true);
来源：http://hz.zhongyouzk.top/gtsfnjnyfg.html

JS:   await resp.json()
来源：http://hz.sweek.top/gtgwhdcvjo.html

TS:   await resp.json()
来源：http://hz.ybcxt.top/gtxjukotrm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.daxiang520.top/gthufnmrns.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jlsjyb.cn/gtltsfunre.html

Ruby: JSON.parse(resp.body)
来源：http://hz.daxiang520.top/gtszuulbuo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.meibo888.top/gtdlyqymao.html

[L07] 处理 HTTP 状态码
来源：http://hz.xylfe.cn/gtlqrcgtie.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jinghuilouyu.cn/gtjzftsefr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yongpay.top/gtrxluglir.html

JS:   resp.ok;  resp.status
来源：http://hz.cdnleiting.top/gtuhqlodro.html

TS:   resp.ok;  resp.status
来源：http://hz.chenlongwang.top/gtzrhcofbr.html

Java: resp.statusCode()
来源：http://hz.gogol.net.cn/gtfrfpwuyt.html

Go:   resp.StatusCode
来源：http://hz.hammf.cn/gtfywtzvrv.html

Ruby: resp.code.to_i
来源：http://hz.ppjwa.cn/gtbylrcmvj.html

C#:   (int)resp.StatusCode
来源：http://hz.gotoacloud.top/gteskpsmvj.html

[L08] 并发请求多个地址
来源：http://hz.zhengqikj.top/gtxpqqvsfp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.shuidangran.top/gtslxeauac.html

PHP:  curl_multi_init() 系列
来源：http://hz.cqqwz.cn/gtklmxaona.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hammf.cn/gtzaxihzpk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shuidangran.top/gtogxkshfj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhijiandao.cn/gttuapsvot.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yonumen.top/gtqfyblsqk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cdnleiting.top/gtutmyyana.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yonumen.top/gtmszjsguj.html

================================================================================
来源：http://hz.aizwys.cn/gtyhlflyus.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhoulong.xyz/gtorgnkfyv.html

================================================================================
来源：http://hz.ydzc1.top/gtdairiubo.html

[M01] 读取命令行参数
来源：http://hz.hnxiangtu.top/gtbsazvskr.html

Py:   sys.argv[1:]
来源：http://hz.ydzc1.top/gtbvpdhkhl.html

PHP:  $argv;  $argc;
来源：http://hz.hysaishi.cn/gtfzyouwtj.html

JS:   process.argv.slice(2)
来源：http://hz.yj202588.top/gteaongjya.html

TS:   process.argv.slice(2)
来源：http://hz.zhaomingkeji.xyz/gtvrzczvlc.html

Java: args 数组（main 方法参数）
来源：http://hz.hongshengwenyu.top/gtrpfgzfnf.html

Go:   os.Args[1:]
来源：http://hz.zhaomingkeji.xyz/gtuidkrazw.html

Ruby: ARGV
来源：http://hz.yvedp.cn/gtxjbunube.html

C#:   args 数组（Main 方法参数）
来源：http://hz.guannengcc.top/gtfppcasyo.html

[M02] 读取环境变量
来源：http://hz.yonumen.top/gtxehtnnxp.html

Py:   os.environ.get("HOME")
来源：http://hz.cdnleiting.top/gtnmgfcwpu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.daria6918.cn/gtafbuwepz.html

JS:   process.env.HOME
来源：http://hz.316326.xyz/gtegdflkyg.html

TS:   process.env.HOME
来源：http://hz.cdnleiting.top/gtavezygwm.html

Java: System.getenv("HOME")
来源：http://hz.jinghuilouyu.cn/gtpudblcjs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yvedp.cn/gtbubdirzq.html

Ruby: ENV["HOME"]
来源：http://hz.yuanzhike.top/gtkqncfgik.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenjidiqi.icu/gtihjfhlhn.html

[M03] 执行外部命令
来源：http://hz.jinyuanbaomall.cn/gtxetspgpc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yueranfly.top/gtatugbytr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.nwbrower.top/gtoputkxyl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cqqwz.cn/gtjpetlqyw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.vqdsnc.cn/gtjybuizdu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yj20258.top/gtxszdtxga.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yuxming.cn/gttqiptpqy.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.haohaochexian.top/gtqfdmyyoy.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ywan-chungtsiang.top/gtmflvxboz.html

[M04] 获取当前工作目录
来源：http://hz.tanke756.top/gtcjwplgao.html

Py:   os.getcwd()
来源：http://hz.yuxming.cn/gtuxcjfyxo.html

PHP:  getcwd();
来源：http://hz.zhongyouzk.top/gtesjfyqby.html

JS:   process.cwd()
来源：http://hz.jinyuanbaomall.cn/gtaxajenaz.html

TS:   process.cwd()
来源：http://hz.sxryk.cn/gtjpwycfyq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yanxiufei.cn/gtmshuzlun.html

Go:   os.Getwd()
来源：http://hz.gogol.net.cn/gtogzmoyne.html

Ruby: Dir.pwd
来源：http://hz.jqgfzy.top/gtezjrmrqv.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.daxiang520.top/gtmcktbole.html

[M05] 设置退出码
来源：http://hz.fzhhl.top/gttgtwdqjz.html

Py:   sys.exit(1)
来源：http://hz.xziqi.cn/gtsbyxzfun.html

PHP:  exit(1);
来源：http://hz.yonumen.top/gthqrxmxgc.html

JS:   process.exit(1)
来源：http://hz.tian-w.cn/gtmsregkkn.html

TS:   process.exit(1)
来源：http://hz.tanke756.top/gtykjcbycn.html

Java: System.exit(1)
来源：http://hz.hammf.cn/gtzpyweggr.html

Go:   os.Exit(1)
来源：http://hz.chenlongwang.top/gtzizefbky.html

Ruby: exit 1
来源：http://hz.tian-w.cn/gtotxozjci.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.kuanghao11.cn/gtrtsvfthg.html

[M06] 向标准错误输出
来源：http://hz.gzhubu.top/gtwaqufvpg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.vqdsnc.cn/gtlofgwvgm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.wangdashe.top/gtrttfbfsq.html

JS:   console.error("err")
来源：http://hz.dianchejie.cn/gtlfjdpfac.html

TS:   console.error("err")
来源：http://hz.shangyingyoupin.top/gtlwfdydvw.html

Java: System.err.println("err")
来源：http://hz.tian-w.cn/gtucdupjyn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhongyouzk.top/gtpbjivaoy.html

Ruby: warn "err"
来源：http://hz.gzhubu.top/gtpqggwybu.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yangfankeji.com/gtgqfkdmhv.html

[M07] 判断是否为主入口
来源：http://hz.feifeiyinyue.top/gtgkmxmgcz.html

Py:   if __name__ == "__main__":
来源：http://hz.c1oappe.top/gtiexqklwn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhongyouzk.top/gtvzdukpap.html

JS:   require.main === module
来源：http://hz.shanyushiyangkeji.top/gtsghoksnf.html

TS:   require.main === module
来源：http://hz.dianchejie.cn/gtrgdvxrko.html

Java: public static void main(String[] args)
来源：http://hz.gotoacloud.top/gtkrqjsjki.html

Go:   func main()
来源：http://hz.yvedp.cn/gtbbgfwxyg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.redwolf501.top/gtetmkalfk.html

C#:   static void Main(string[] args)
来源：http://hz.cheryme.top/gtqpejkapg.html

[M08] 获取系统与运行时信息
来源：http://hz.gaohongyu789.top/gthdtukxba.html

Py:   platform.system();  platform.python_version()
来源：http://hz.daxiang520.top/gtipkdveuf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.redwolf501.top/gtkfbqdtee.html

JS:   process.platform;  process.version
来源：http://hz.shuidangran.top/gtohdrmgua.html

TS:   process.platform;  process.version
来源：http://hz.sweek.top/gthektvppi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.guowangkeji.top/gttihqznom.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.haohaochexian.top/gtmjydeamk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hywenlv.cn/gtlyccillp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.gaohongyu789.top/gtdqrxbbts.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtqyaftouq.html

N. 数据结构与算法
来源：http://hz.yueranfly.top/gtrhvgjfus.html

================================================================================
来源：http://hz.meibo888.top/gtpdypwhnl.html


<!-- 参考信息 -->