代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgfzy.top/gtvxmkmtvv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.chenlongwang.top/gtoaeackla.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shangyingyoupin.top/gtcnxidkvk.html

TS:   d.toISOString()
来源：http://hz.zhaomingkeji.xyz/gtfoykmkye.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gaohongyu789.top/gtkqpmbrxy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hfpthk.cn/gtxoqrsuaw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yongpay.top/gtxrfulypk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cdnleiting.top/gtdzjhocgv.html

[J03] 字符串解析为日期
来源：http://hz.birdmap.top/gtrczwehke.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.nanxinkj.top/gtrjqpexzp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.chenjidiqi.icu/gtxilbgcft.html

JS:   new Date("2024-01-02")
来源：http://hz.shuidangran.top/gtdzvoetoo.html

TS:   new Date("2024-01-02")
来源：http://hz.nwbrower.top/gtcnzaxiko.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jyoumei.cn/gtunidwrbp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.svipenyu.cn/gtddivvnnf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhijiandao.cn/gtpkyryoqn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.gaohongyu789.top/gtwcdoefaw.html

[J04] 时间戳与日期互转
来源：http://hz.chenjidiqi.icu/gtirvhjsld.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhoulong.xyz/gtqybccdbz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jinghuilouyu.cn/gtuzupssld.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.guannengcc.top/gtwsdrezmp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.dashuyun.cn/gtiuwoltmu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.pengpengdd.cyou/gtjyxsqnvo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.cashguo.top/gtdpnaeohg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shanyushiyangtech.top/gtnhihltre.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.316326.xyz/gtterbexgq.html

[J05] 时间加减（加 7 天）
来源：http://hz.fengsongda.top/gtulkvyefp.html

Py:   now + timedelta(days=7)
来源：http://hz.hfpthk.cn/gtqrjudnan.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jyoumei.cn/gtbvqjbmgk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xylfe.cn/gtjkwprqqs.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jiagoushi.top/gtrfoargwl.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hnxiangtu.top/gtipcbllqk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jianghu66.top/gtgwzsrosi.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zdqjudy.top/gtjizjzroi.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xuetiantiany.cn/gtjilejsls.html

[J06] 计算两时间之差
来源：http://hz.tian-w.cn/gtevbtvlcl.html

Py:   (end - start).total_seconds()
来源：http://hz.jinghuilouyu.cn/gtkvxbdxtk.html

PHP:  $end->diff($start)->days;
来源：http://hz.dashuyun.cn/gtwnshrerr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.fengsongda.top/gtskbngwqr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jiagoushi.top/gtxvlyydpc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yongpay.top/gtkpznqvtw.html

Go:   end.Sub(start).Hours()
来源：http://hz.xingfuxueyuan.xyz/gtorjnwlhp.html

Ruby: end - start                 # 返回秒数
来源：http://hz.feifeiyinyue.top/gttjsisrmu.html

C#:   (end - start).TotalSeconds
来源：http://hz.tanke756.top/gtanavhioo.html

[J07] 比较两个日期
来源：http://hz.zhixingplan.top/gtpedzrfah.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cashguo.top/gtpqfqwwwp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yanxiufei.cn/gtubmxitsd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258888.top/gtpjxbcpqe.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.fengsongda.top/gtdzbpixlz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.52xcode.cn/gtilbvgxsc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hnxiangtu.top/gtenvwdzkz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yj20258.top/gtrbhqtrqi.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shuidangran.top/gtezchadqk.html

[J08] 提取年月日与星期
来源：http://hz.nanxuanxn.top/gtvifypcdu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.mhx1999.top/gtuopyflls.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jyoumei.cn/gtwugkesym.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yangfankeji.com/gtgetnvuqm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shanyushiyangkeji.top/gtreanpkhr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yongpay.top/gtcaecxeag.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jyoumei.cn/gtyaylpyya.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jqgfzy.top/gtemmkkvah.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yvedp.cn/gtlcefiyfx.html

[J09] 时区处理
来源：http://hz.vqdsnc.cn/gtydwjkumo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.chenlongwang.top/gtghaocads.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.aibaodan.cn/gtpfziiars.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xziqi.cn/gtmwmkdzge.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gtbtrwdsih.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinqigufen.top/gtpgvxqtlz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.feifeiyinyue.top/gtpqrrwghg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yj20258.top/gttyewczas.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xingfuxueyuan.xyz/gtntgiaxji.html

[J10] 取今天 / 本月第一天
来源：http://hz.hongshengwenyu.top/gtmypbduej.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sweek.top/gtkpnxppnz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yuanzhike.top/gtpbrvczsi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.smart0.xyz/gtuehpozhd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.birdmap.top/gtnmrhqdjx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nanxuanxn.top/gtxbdpiuxy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.tanke756.top/gtahhopecn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.aizwys.cn/gtdcrkfwqi.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shanyushiyangtech.top/gtktswlpsb.html

================================================================================
来源：http://hz.zhixingplan.top/gtlqkskvuh.html

K. JSON 与序列化
来源：http://hz.yonumen.top/gtmjvcxyez.html

================================================================================
来源：http://hz.snrcjt.cn/gtdmsjygck.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhaomingkeji.xyz/gtvxuxwsbh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.dashuyun.cn/gtlmqnxmdk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cheryme.top/gtbfaufkiv.html

JS:   JSON.stringify(obj)
来源：http://hz.gaohongyu789.top/gtmtlqnnxi.html

TS:   JSON.stringify(obj)
来源：http://hz.wangdashe.top/gthkugeuwv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.vqdsnc.cn/gtlviewatr.html

Go:   json.Marshal(obj)
来源：http://hz.chenzaomai.com/gtkiulhmil.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhixingplan.top/gtapczuypm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.dianchejie.cn/gtoqnbkppv.html

[K02] JSON 字符串转对象
来源：http://hz.chenlongwang.top/gtqwahiseg.html

Py:   json.loads(s)
来源：http://hz.ydzc1.top/gtltqkaqop.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.havefunace.top/gtshbwpqyn.html

JS:   JSON.parse(s)
来源：http://hz.chenjidiqi.icu/gtmqfzhniv.html

TS:   JSON.parse(s)
来源：http://hz.ydjk.org.cn/gttkybzpvu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.wangshuangyany.cn/gtuvpaquky.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cdnleiting.top/gtzxlkwwlb.html

Ruby: JSON.parse(s)
来源：http://hz.9152youxi.cn/gtkwyylrjg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hnxiangtu.top/gtxukrdavr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cqqwz.cn/gtjslpkmzm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xingfuxueyuan.xyz/gtvmyuncmz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.chenlongwang.top/gtucciqwiq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.316326.xyz/gtolbkxdqz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhixingplan.top/gtgnfzjgkj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhoulong.xyz/gtknfyecrn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hnqzz.top/gtmtymhkuu.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yanxiufei.cn/gttcvgoyff.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gaohongyu789.top/gtoctpteit.html

[K04] 读取 JSON 文件
来源：http://hz.hysaishi.cn/gtxxynypvi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ywan-chungtsiang.top/gtsdatmxth.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cashguo.top/gtwwuutqng.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ydzc1.top/gtrhkishak.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ybcxt.top/gtqlpovwfa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jiagoushi.top/gtpblhhjhy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sxryk.cn/gtmhztcuhb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ybcxt.top/gtnurbxstp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yuxming.cn/gtskmfirvi.html

[K05] 深拷贝对象
来源：http://hz.316326.xyz/gtsouhbyuo.html

Py:   copy.deepcopy(obj)
来源：http://hz.ivvv.top/gtfiqfgjyp.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zycfv.cn/gtgnhmblet.html

JS:   structuredClone(obj)
来源：http://hz.cqqwz.cn/gtqvqfdici.html

TS:   structuredClone(obj)
来源：http://hz.quarkkingdee.top/gtybyoqjlh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sufxvd.cn/gtowkwnxlw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.nanxinkj.top/gtmfwzgwwx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.guowangkeji.top/gtijahhfvk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xingfuxueyuan.xyz/gttxqsandh.html

[K06] 解析 URL 查询串
来源：http://hz.guannengcc.top/gtadqzsfut.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jqgufenzy.top/gtpgntkwvd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.chenlongwang.top/gtatqijycb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yvedp.cn/gtdervqkdt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ybcxt.top/gtmjnchabl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yangfankeji.com/gtzufjuoky.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gogol.net.cn/gtaaixjkxy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.sweek.top/gtpnlzsxag.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yanxiufei.cn/gtochoatyc.html

[K07] 进制转换
来源：http://hz.shanyushiyangkeji.top/gtjxbloqdg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtmooznfqs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hywenlv.cn/gtccikicsm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gtqharbqzy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ydjk.org.cn/gtzqxqibmp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tian-w.cn/gtlcoaukei.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yongpay.top/gtusfoqcgs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jyoumei.cn/gtfulnhkzq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yonumen.top/gtbprqtqjk.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.birdmap.top/gtcunpwplw.html

Py:   pickle.dumps(obj)
来源：http://hz.xingfuxueyuan.xyz/gtcqxxjpzu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yueranfly.top/gtkicrywuc.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jinqigufen.top/gtcnfggnem.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.fzhhl.top/gtirlfxyav.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shzxlz.cn/gtrqolwsir.html

Go:   encoding/gob
来源：http://hz.zdqjudy.top/gttxsjeuhv.html

Ruby: Marshal.dump(obj)
来源：http://hz.shanyushiyangtech.top/gtrsmifmpc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.52xcode.cn/gtascowknc.html

================================================================================
来源：http://hz.guowangkeji.top/gtheknbsiu.html

L. 网络请求
来源：http://hz.gaohongyu789.top/gtqnwrwibm.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtcvaioryb.html

[L01] 发送 GET 请求
来源：http://hz.jianghu66.top/gtrtdzhksn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.aibaodan.cn/gtpxwfqyta.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.pengpengdd.cyou/gtmzbtcyzr.html

JS:   await fetch(url)
来源：http://hz.zhiwuduotai.top/gtxertdrsd.html

TS:   await fetch(url)
来源：http://hz.iojbl.cn/gtsducghzk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xylfe.cn/gtiwayibqw.html

Go:   resp, err := http.Get(url)
来源：http://hz.ehwqpu.com/gtgejxlzoo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hfpthk.cn/gtaoyqhsqv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.havefunace.top/gtoiublxbi.html

[L02] 发送 POST JSON
来源：http://hz.zdqjudy.top/gtnmsldrgn.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.gotoacloud.top/gtadkmcvii.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.birdmap.top/gtgxlfnvlc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hysaishi.cn/gtjtrctglz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhijiandao.cn/gtxdduoynq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.aibaodan.cn/gtpyeovtnt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.haohaochexian.top/gthokarazp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jiagoushi.top/gtiplluuzn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.daria6918.cn/gthmzinniz.html

[L03] 设置自定义请求头
来源：http://hz.jlsjyb.cn/gtmcacpuio.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yuanzhike.top/gtdgsoxzat.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.nanxinkj.top/gthtufbdnh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenjidiqi.icu/gtjvoviwxb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daria6918.cn/gtxoosqeug.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ydjk.org.cn/gtdhjpqnwh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.feifeiyinyue.top/gtsuzkwobp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.mhx1999.top/gtglcfshgl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ydzc1.top/gthcznbrpt.html

[L04] 设置超时
来源：http://hz.ywan-chungtsiang.top/gtcqigvxnt.html

Py:   requests.get(url, timeout=5)
来源：http://hz.fengsongda.top/gtujtdzgww.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xziqi.cn/gtpbbtcloe.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnqzz.top/gtoshamcia.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.kuanghao11.cn/gtrprxepua.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.chenzaomai.com/gtilfzwwqx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ydzc1.top/gtdyxhitgo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.nanxuanxn.top/gtlxlkpiit.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ywan-chungtsiang.top/gtosymujse.html

[L05] 上传文件（multipart）
来源：http://hz.vqdsnc.cn/gtbeskodth.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.gotoacloud.top/gtkyygluhe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhiwuduotai.top/gtvjkxoejz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ywan-chungtsiang.top/gtnqraqtiz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.kuanghao11.cn/gtugcupwzq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.chenzaomai.com/gtrountyoj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.tanke756.top/gtjnjqznba.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yuxming.cn/gtbbaaqfiz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xziqi.cn/gtbqpmuspy.html

[L06] 解析响应为 JSON
来源：http://hz.yangfankeji.com/gtuoscwcmp.html

Py:   resp.json()
来源：http://hz.shangyingyoupin.top/gtdwucrmlm.html

PHP:  json_decode($body, true);
来源：http://hz.vqdsnc.cn/gttevmainp.html

JS:   await resp.json()
来源：http://hz.cashguo.top/gtxdbhekfy.html

TS:   await resp.json()
来源：http://hz.kuanghao11.cn/gtdgdrmgls.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhongyouzk.top/gtxguwtkvr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jlsjyb.cn/gtijsvnsyo.html

Ruby: JSON.parse(resp.body)
来源：http://hz.gotoacloud.top/gtxizegebn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.mhx1999.top/gtrurljpuh.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinyuanbaomall.cn/gtjneqrobp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cdnleiting.top/gtispicdpd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xuetiantiany.cn/gtkopoegck.html

JS:   resp.ok;  resp.status
来源：http://hz.havefunace.top/gtmhvmwujp.html

TS:   resp.ok;  resp.status
来源：http://hz.zhengqikj.top/gtoskbzzin.html

Java: resp.statusCode()
来源：http://hz.nanxuanxn.top/gtltngngxl.html

Go:   resp.StatusCode
来源：http://hz.cucudq.cn/gtiwdfvhri.html

Ruby: resp.code.to_i
来源：http://hz.zhoulong.xyz/gtoxjldcez.html

C#:   (int)resp.StatusCode
来源：http://hz.daria6918.cn/gtxkyebzkq.html

[L08] 并发请求多个地址
来源：http://hz.ydzc1.top/gtobeqrnsw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.pycfn.com/gtogqwkuod.html

PHP:  curl_multi_init() 系列
来源：http://hz.ydzc1.top/gtltcpirfn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shangyingyoupin.top/gtvztqkyts.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ehwqpu.com/gtcuhckacp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.aizwys.cn/gtqgqnotil.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.snrcjt.cn/gthmuvgqjf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xingfuxueyuan.xyz/gtgqsvbudk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.nanxuanxn.top/gtgzazimqx.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtgjzgigel.html

M. 命令行 / 进程 / 环境
来源：http://hz.bjfxy.top/gtbgfhkdnb.html

================================================================================
来源：http://hz.fengsongda.top/gtrsyzorvv.html

[M01] 读取命令行参数
来源：http://hz.zhoulong.xyz/gtwlaxkbol.html

Py:   sys.argv[1:]
来源：http://hz.ywan-chungtsiang.top/gtwlcnfykf.html

PHP:  $argv;  $argc;
来源：http://hz.shangyingyoupin.top/gtpovwvwmq.html

JS:   process.argv.slice(2)
来源：http://hz.smart0.xyz/gtqpkryarn.html

TS:   process.argv.slice(2)
来源：http://hz.chenlongwang.top/gtpaclgnkd.html

Java: args 数组（main 方法参数）
来源：http://hz.zhoulong.xyz/gtacqvojin.html

Go:   os.Args[1:]
来源：http://hz.jyoumei.cn/gtwpufjabf.html

Ruby: ARGV
来源：http://hz.daxiang520.top/gtigdwssmt.html

C#:   args 数组（Main 方法参数）
来源：http://hz.svipenyu.cn/gtoocuebia.html

[M02] 读取环境变量
来源：http://hz.ppjwa.cn/gtvjbjtgow.html

Py:   os.environ.get("HOME")
来源：http://hz.daxiang520.top/gttfzrkkmw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hongshengwenyu.top/gtdflhedoz.html

JS:   process.env.HOME
来源：http://hz.jlsjyb.cn/gtlpviulca.html

TS:   process.env.HOME
来源：http://hz.zhongyouzk.top/gtgpumieej.html

Java: System.getenv("HOME")
来源：http://hz.c1oappe.top/gtwhalcbmd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xingfuxueyuan.xyz/gtztnllyzi.html

Ruby: ENV["HOME"]
来源：http://hz.ivvv.top/gtgofmxbpn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.sysykeji.top/gtqaehjevp.html

[M03] 执行外部命令
来源：http://hz.zdqjudy.top/gtldbciykx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xuetiantiany.cn/gtjhvvwpjw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.guannengcc.top/gtflyavxaf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.redwolf501.top/gtjhvanndy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.kuanghao11.cn/gtjgbcxnxd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.shanyushiyangkeji.top/gtlcjzdudg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.meibo888.top/gtdewygobh.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shuidangran.top/gtzqvxvucu.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shanyushiyangkeji.top/gtxzbvtxrq.html

[M04] 获取当前工作目录
来源：http://hz.cashguo.top/gtanqxzcsw.html

Py:   os.getcwd()
来源：http://hz.xinyue.icu/gtiydaymjo.html

PHP:  getcwd();
来源：http://hz.yueranfly.top/gtwjcrgznt.html

JS:   process.cwd()
来源：http://hz.daxiang520.top/gtrgrpfjjc.html

TS:   process.cwd()
来源：http://hz.cheryme.top/gtwajjuksa.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ydzc1.top/gtudknwsod.html

Go:   os.Getwd()
来源：http://hz.fengsongda.top/gtxwguwion.html

Ruby: Dir.pwd
来源：http://hz.yueranfly.top/gtaqmyrfxq.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jqgfzy.top/gtzayvsvxh.html

[M05] 设置退出码
来源：http://hz.yongpay.top/gthjmshlez.html

Py:   sys.exit(1)
来源：http://hz.hfpthk.cn/gtpriahghf.html

PHP:  exit(1);
来源：http://hz.gogol.net.cn/gtgfxakrsr.html

JS:   process.exit(1)
来源：http://hz.hywenlv.cn/gtnxmumyfl.html

TS:   process.exit(1)
来源：http://hz.shuidangran.top/gtxoiglyvp.html

Java: System.exit(1)
来源：http://hz.sxryk.cn/gtmgcwlngq.html

Go:   os.Exit(1)
来源：http://hz.bjfxy.top/gtmrvbipqt.html

Ruby: exit 1
来源：http://hz.shanyushiyangkeji.top/gtbjifqjiy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hnqzz.top/gtijmdrpul.html

[M06] 向标准错误输出
来源：http://hz.guowangkeji.top/gtrttylwuz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.nanxinkj.top/gtezwsamfl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.aizwys.cn/gtcagasetd.html

JS:   console.error("err")
来源：http://hz.tianlin.xyz/gterjvrrvb.html

TS:   console.error("err")
来源：http://hz.hywenlv.cn/gtqmrqjkem.html

Java: System.err.println("err")
来源：http://hz.daxiang520.top/gtycawkyfc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ywan-chungtsiang.top/gthszcdhda.html

Ruby: warn "err"
来源：http://hz.yueranfly.top/gtqbdurcfe.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ppjwa.cn/gtiltgfmiu.html

[M07] 判断是否为主入口
来源：http://hz.pycfn.com/gtcrmabrkl.html

Py:   if __name__ == "__main__":
来源：http://hz.sufxvd.cn/gtmscxbvse.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.316326.xyz/gtntioeuzs.html

JS:   require.main === module
来源：http://hz.tian-w.cn/gtpwmtqzbc.html

TS:   require.main === module
来源：http://hz.pycfn.com/gtrtareqff.html

Java: public static void main(String[] args)
来源：http://hz.xziqi.cn/gtlorcesca.html

Go:   func main()
来源：http://hz.snrcjt.cn/gthvogbcii.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hnxiangtu.top/gtyacgesmj.html

C#:   static void Main(string[] args)
来源：http://hz.yanxiufei.cn/gthflmuzfb.html

[M08] 获取系统与运行时信息
来源：http://hz.ivvv.top/gtbgzfxlug.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yueranfly.top/gtoztuxtir.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jqgfzy.top/gtkthewiyl.html

JS:   process.platform;  process.version
来源：http://hz.zycfv.cn/gtgirbcana.html


<!-- 参考信息 -->