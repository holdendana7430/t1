代发 wailian999

[J03] 字符串解析为日期
来源：http://hz.kuanghao11.cn/gtoiotduub.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.pycfn.com/gthjplqikh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinyuanbaomall.cn/gtisxhzmaw.html

JS:   new Date("2024-01-02")
来源：http://hz.zhijiandao.cn/gtrbqcctnz.html

TS:   new Date("2024-01-02")
来源：http://hz.aibaodan.cn/gtouqzyxte.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cashguo.top/gtukjfpacq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gtmozkvsmy.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtzuzrojyg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.kuanghao11.cn/gtgsuqmtrp.html

[J04] 时间戳与日期互转
来源：http://hz.sufxvd.cn/gtanogiibl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ydzc1.top/gtqlqnpnxv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sweek.top/gtvemncmju.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hammf.cn/gtyztxshok.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhongyouzk.top/gtwkjnegvc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xingfuxueyuan.xyz/gthhlwjquy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yuanzhike.top/gtgsgyrttd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.andypj.xyz/gtvydnxhko.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.snrcjt.cn/gtmpetbnui.html

[J05] 时间加减（加 7 天）
来源：http://hz.sweek.top/gtvthesagj.html

Py:   now + timedelta(days=7)
来源：http://hz.xuetiantiany.cn/gtwbkmcfqt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhiwuduotai.top/gtdxodfbcc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhiwuduotai.top/gtfjiikrxc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cucudq.cn/gtgotxzlux.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hammf.cn/gtnhorkhov.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.daria6918.cn/gtvzaephdz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ydjk.org.cn/gtgyufgwbf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.chenzaomai.com/gttzliueuj.html

[J06] 计算两时间之差
来源：http://hz.meibo888.top/gtgmchlzrx.html

Py:   (end - start).total_seconds()
来源：http://hz.hongshengwenyu.top/gtjyqdywsi.html

PHP:  $end->diff($start)->days;
来源：http://hz.xylfe.cn/gtutnrvjbj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.fengsongda.top/gtxwqaxjkj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cashguo.top/gtlcpthrbr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.gzhubu.top/gtvxdipxuu.html

Go:   end.Sub(start).Hours()
来源：http://hz.yuanzhike.top/gtkcarghdl.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yangfankeji.com/gtdpvwrufc.html

C#:   (end - start).TotalSeconds
来源：http://hz.sxryk.cn/gtiwrcqqbc.html

[J07] 比较两个日期
来源：http://hz.wangdashe.top/gtjqvgoiex.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhoulong.xyz/gtqgxabxly.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xylfe.cn/gtmnepedbq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ehwqpu.com/gtybjawctv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ppjwa.cn/gtcxwjynxx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jqgufenzy.top/gtgsswczks.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.wangdashe.top/gtebikioyq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.shuidangran.top/gtrjdkasrj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yuxming.cn/gtcteyhysy.html

[J08] 提取年月日与星期
来源：http://hz.daxiang520.top/gtmpyvvjmj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hnqzz.top/gtjcwzosxg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zycfv.cn/gtzywrafqr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.dashuyun.cn/gtpsykqrpo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yj20258.top/gtwcjmlyux.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.sxryk.cn/gtyxdefrnx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hammf.cn/gtwtynnedi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cucudq.cn/gtonxxkzkg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.fzhhl.top/gtnaupbofv.html

[J09] 时区处理
来源：http://hz.jyoumei.cn/gtncaoqkoi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.smart0.xyz/gtjdgrpjmr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.havefunace.top/gticokuqdd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinyuanbaomall.cn/gtestbnzmv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.bjfxy.top/gtljlvhaci.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.fengsongda.top/gtdpgsvwhc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhoulong.xyz/gtkxqovyjn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ybcxt.top/gtdcbjzmon.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yvedp.cn/gtuaavqufd.html

[J10] 取今天 / 本月第一天
来源：http://hz.yvedp.cn/gtppcngtfd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ppjwa.cn/gtbiojdppz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ppjwa.cn/gtoxrkictz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.quarkkingdee.top/gtgnnhhxot.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.chenzaomai.com/gtsppzrcmk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.aibaodan.cn/gtnlmteoet.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.dianchejie.cn/gtoalvcslw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.vqdsnc.cn/gtkifaapyq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.redwolf501.top/gtzmqjphtq.html

================================================================================
来源：http://hz.meibo888.top/gtmjmruxcg.html

K. JSON 与序列化
来源：http://hz.chenlongwang.top/gtmrduszvg.html

================================================================================
来源：http://hz.aibaodan.cn/gtwcurbjeb.html

[K01] 对象转 JSON 字符串
来源：http://hz.zycfv.cn/gtjdkvyyll.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.nwbrower.top/gtaujvrwpy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ivvv.top/gtudsspgcq.html

JS:   JSON.stringify(obj)
来源：http://hz.jinqigfzy.top/gtvxqeuzvq.html

TS:   JSON.stringify(obj)
来源：http://hz.shzxlz.cn/gtwlkjiqxl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.sxryk.cn/gtiohkeazb.html

Go:   json.Marshal(obj)
来源：http://hz.hnxiangtu.top/gtzakmheuy.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jqgfzy.top/gtdknhjzkh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.52xcode.cn/gtsqoswdik.html

[K02] JSON 字符串转对象
来源：http://hz.shuidangran.top/gttyvqspnj.html

Py:   json.loads(s)
来源：http://hz.nwbrower.top/gtertbtoui.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.nanxuanxn.top/gtwszavjog.html

JS:   JSON.parse(s)
来源：http://hz.jinqigufen.top/gtrxvdjrhy.html

TS:   JSON.parse(s)
来源：http://hz.0kj1m.cn/gtkgkexwmm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.aizwys.cn/gtmtsczspo.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yueranfly.top/gtonfanwsc.html

Ruby: JSON.parse(s)
来源：http://hz.9152youxi.cn/gtycaduzyi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xingfuxueyuan.xyz/gtgrkuoukw.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinyuanbaomall.cn/gtieutkpee.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cdnleiting.top/gtnigbebax.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gaohongyu789.top/gtzfvzoadx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigufen.top/gtbyazesak.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangtech.top/gtvtwzewlt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.birdmap.top/gtvymlljoi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xuanzx.com/gtvzimwttq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhixingplan.top/gtvbrdrxgf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hammf.cn/gtupxfasrg.html

[K04] 读取 JSON 文件
来源：http://hz.xinyue.icu/gtprlekdfl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.iojbl.cn/gtxzqsenzv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cqqwz.cn/gtlfmxgpse.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.kuanghao11.cn/gtvhmkawem.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xinyue.icu/gtsufgfjfe.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ivvv.top/gtdookdjya.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shuidangran.top/gtdlfzmadc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ybcxt.top/gtfubjrxul.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yvedp.cn/gtsbxcrvev.html

[K05] 深拷贝对象
来源：http://hz.zhaomingkeji.xyz/gtaklztcam.html

Py:   copy.deepcopy(obj)
来源：http://hz.52xcode.cn/gtyvapvbpj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.52xcode.cn/gtjkrlycet.html

JS:   structuredClone(obj)
来源：http://hz.xinyue.icu/gtcrrzdjrj.html

TS:   structuredClone(obj)
来源：http://hz.chenzaomai.com/gtscmpzeqe.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yanxiufei.cn/gtoqygqamk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yvedp.cn/gtqljomdob.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zdqjudy.top/gtgpgaismc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jinqigfzy.top/gtttxkmunc.html

[K06] 解析 URL 查询串
来源：http://hz.yuxming.cn/gtjqcvrgoq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.pengpengdd.cyou/gtlexnkahs.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.bjfxy.top/gtzjslqfit.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.daria6918.cn/gtwltxxlfl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sufxvd.cn/gtzmuwiixo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.wangshuangyany.cn/gtzngfkchi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sufxvd.cn/gtmpbrvssp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.fzhhl.top/gtfkgbwqew.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sxryk.cn/gtmmgqqnbb.html

[K07] 进制转换
来源：http://hz.zdqjudy.top/gtkabkouza.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.sufxvd.cn/gtmpcdehfk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sufxvd.cn/gtjfmjcwby.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.c1oappe.top/gtmqwjhepa.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gotoacloud.top/gtkbpgctjs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.sxryk.cn/gtdbrtondn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sysykeji.top/gtlfndiigc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jyoumei.cn/gtzwzitwtv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.fengsongda.top/gtthjysvta.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.nanxuanxn.top/gtzttyuzpm.html

Py:   pickle.dumps(obj)
来源：http://hz.hnqzz.top/gtbeyvcjkn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.fengsongda.top/gtkhtxukid.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ehwqpu.com/gtkvmybgyx.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ybcxt.top/gturskpivo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hywenlv.cn/gtwxqlazrj.html

Go:   encoding/gob
来源：http://hz.zdqjudy.top/gtpiropqlf.html

Ruby: Marshal.dump(obj)
来源：http://hz.c1oappe.top/gttxwjwmeh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.9152youxi.cn/gtadziocde.html

================================================================================
来源：http://hz.shuidangran.top/gtgrikxstg.html

L. 网络请求
来源：http://hz.smart0.xyz/gtdhmubqxx.html

================================================================================
来源：http://hz.zhixingplan.top/gtecdkujag.html

[L01] 发送 GET 请求
来源：http://hz.hnqzz.top/gtywiygpfj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.dianchejie.cn/gtzrcdtwno.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hnqzz.top/gtftohdthr.html

JS:   await fetch(url)
来源：http://hz.sweek.top/gtmjudkodp.html

TS:   await fetch(url)
来源：http://hz.andypj.xyz/gtcskpskav.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhaomingkeji.xyz/gtcpsrxfwn.html

Go:   resp, err := http.Get(url)
来源：http://hz.jqgufenzy.top/gtjnofquml.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.dashuyun.cn/gtpfzhjauh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.vqdsnc.cn/gtnzjlksvp.html

[L02] 发送 POST JSON
来源：http://hz.xuetiantiany.cn/gthaiwzwrr.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.dianchejie.cn/gtoevxrmfi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.mhx1999.top/gtiheconhk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shzxlz.cn/gtgubuxrwl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.iojbl.cn/gtrsmnjntz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jianghu66.top/gtkvnzsprq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.wangdashe.top/gtxpbspbxm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xuetiantiany.cn/gtiqldrbkz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.andypj.xyz/gtegdaeoqp.html

[L03] 设置自定义请求头
来源：http://hz.cucudq.cn/gtkckdfwhv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.haohaochexian.top/gtoarepjdu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ivvv.top/gtmbgekwsz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shuidangran.top/gtarmfohjw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxinkj.top/gtfmmwwszf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.chenjidiqi.icu/gtzcdnegle.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jiagoushi.top/gtyycklemr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.fzhhl.top/gtpqlahnct.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hnxiangtu.top/gtbhakwqco.html

[L04] 设置超时
来源：http://hz.chenjidiqi.icu/gteqcyekfx.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hywenlv.cn/gtkzyraqta.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.redwolf501.top/gtnotydmnv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fzhhl.top/gtapyxbyjq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cqqwz.cn/gtovdnsouy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ehwqpu.com/gtrqmlnsdl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yueranfly.top/gtgmbaqqfy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ivvv.top/gtbrfabaxk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhaomingkeji.xyz/gtsmtroytf.html

[L05] 上传文件（multipart）
来源：http://hz.guannengcc.top/gtgckiaqtm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinyuanbaomall.cn/gtcdjccpfy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yangfankeji.com/gtxnylflhg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shzxlz.cn/gtibaavjvw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydzc1.top/gtljgidkpx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cdnleiting.top/gtpqgjodjf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yuanzhike.top/gtikdvsiep.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinqigfzy.top/gtrlqcrqsh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ppjwa.cn/gtqdbpvbre.html

[L06] 解析响应为 JSON
来源：http://hz.cheryme.top/gtdunxszxw.html

Py:   resp.json()
来源：http://hz.sweek.top/gtshlneqrs.html

PHP:  json_decode($body, true);
来源：http://hz.pengpengdd.cyou/gtxrbuoykl.html

JS:   await resp.json()
来源：http://hz.yj202588.top/gtoemwdyja.html

TS:   await resp.json()
来源：http://hz.meibo888.top/gttigbimlb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cashguo.top/gtrwphpnkg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ppjwa.cn/gtddhuixsp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yonumen.top/gtrlyypazv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ydjk.org.cn/gtmockecfe.html

[L07] 处理 HTTP 状态码
来源：http://hz.yj202588.top/gtoalmxzgy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.iojbl.cn/gtoixjfvtj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sysykeji.top/gtjjtzynns.html

JS:   resp.ok;  resp.status
来源：http://hz.yj202588.top/gtgypwsbdb.html

TS:   resp.ok;  resp.status
来源：http://hz.sweek.top/gtqghatznv.html

Java: resp.statusCode()
来源：http://hz.pengpengdd.cyou/gtdrxfxzry.html

Go:   resp.StatusCode
来源：http://hz.smart0.xyz/gtrozxjxxi.html

Ruby: resp.code.to_i
来源：http://hz.zhixingplan.top/gtzxjnmsbi.html

C#:   (int)resp.StatusCode
来源：http://hz.ydzc1.top/gtlntrlyww.html

[L08] 并发请求多个地址
来源：http://hz.aibaodan.cn/gtxqohoanv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.dianchejie.cn/gtxyygngme.html

PHP:  curl_multi_init() 系列
来源：http://hz.52xcode.cn/gtwcqvdiql.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangshuangyany.cn/gtxyygblry.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yonumen.top/gtbkbzcpjg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hnxiangtu.top/gtdauhxpaq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhijiandao.cn/gtpewlogwy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jianghu66.top/gtugdakwyl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.fzhhl.top/gttopluqry.html

================================================================================
来源：http://hz.kuanghao11.cn/gtuxrrzfed.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhijiandao.cn/gtqtdlxcgi.html

================================================================================
来源：http://hz.yangfankeji.com/gtphfgaexq.html

[M01] 读取命令行参数
来源：http://hz.ivvv.top/gtbopzzuuo.html

Py:   sys.argv[1:]
来源：http://hz.zhengqikj.top/gtkuserluu.html

PHP:  $argv;  $argc;
来源：http://hz.xylfe.cn/gtoakqfltb.html

JS:   process.argv.slice(2)
来源：http://hz.sxryk.cn/gtvutcbomw.html

TS:   process.argv.slice(2)
来源：http://hz.sufxvd.cn/gtmsacgytl.html

Java: args 数组（main 方法参数）
来源：http://hz.shuidangran.top/gtdkfevxyt.html

Go:   os.Args[1:]
来源：http://hz.yangfankeji.com/gtiudomaua.html

Ruby: ARGV
来源：http://hz.wangshuangyany.cn/gtxadxxwix.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cqqwz.cn/gtocbhskih.html

[M02] 读取环境变量
来源：http://hz.guowangkeji.top/gtatcpfpeh.html

Py:   os.environ.get("HOME")
来源：http://hz.iojbl.cn/gttyqlquwd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jqgfzy.top/gtlyafpkqg.html

JS:   process.env.HOME
来源：http://hz.redwolf501.top/gtcmatarkw.html

TS:   process.env.HOME
来源：http://hz.jinghuilouyu.cn/gtlutatkuz.html

Java: System.getenv("HOME")
来源：http://hz.yangfankeji.com/gthjtphllc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhengqikj.top/gtebmjwurq.html

Ruby: ENV["HOME"]
来源：http://hz.svipenyu.cn/gtonuhwsjs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhongyouzk.top/gteuspcspx.html

[M03] 执行外部命令
来源：http://hz.hysaishi.cn/gtudoulpts.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhijiandao.cn/gtjcijydlt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.nanxinkj.top/gtnhhdaqfi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.pengpengdd.cyou/gtrkkywhst.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhijiandao.cn/gtkasimwkd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yj20258888.top/gthyjnfxmr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sxryk.cn/gtfypkoime.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hnxiangtu.top/gtnnivopkc.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jinghuilouyu.cn/gtqivjrfxh.html

[M04] 获取当前工作目录
来源：http://hz.sxryk.cn/gtewbvjvtp.html

Py:   os.getcwd()
来源：http://hz.chenjidiqi.icu/gtgpbxsjml.html

PHP:  getcwd();
来源：http://hz.xingfuxueyuan.xyz/gtuwcsmygk.html

JS:   process.cwd()
来源：http://hz.hnqzz.top/gtigkasmos.html

TS:   process.cwd()
来源：http://hz.ydzc1.top/gtotqywbmm.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zycfv.cn/gtimyvyjal.html

Go:   os.Getwd()
来源：http://hz.hammf.cn/gtvysqhktn.html

Ruby: Dir.pwd
来源：http://hz.chenzaomai.com/gtnzswvuzx.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yj20258.top/gttpazojkh.html

[M05] 设置退出码
来源：http://hz.hnqzz.top/gtcnljgrav.html

Py:   sys.exit(1)
来源：http://hz.hysaishi.cn/gtdqltppwz.html

PHP:  exit(1);
来源：http://hz.shzxlz.cn/gtuijhmoyg.html

JS:   process.exit(1)
来源：http://hz.tianlin.xyz/gthaalrfea.html

TS:   process.exit(1)
来源：http://hz.xuetiantiany.cn/gtutkirsjk.html

Java: System.exit(1)
来源：http://hz.9152youxi.cn/gtgmvcrsfs.html

Go:   os.Exit(1)
来源：http://hz.jinghuilouyu.cn/gtcfluxfdt.html

Ruby: exit 1
来源：http://hz.hongshengwenyu.top/gtopmirrxp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zycfv.cn/gtaqwnuxwd.html

[M06] 向标准错误输出
来源：http://hz.ydzc1.top/gtdwrqqtic.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hnqzz.top/gtbqlbnxme.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ydjk.org.cn/gtstjlsopp.html

JS:   console.error("err")
来源：http://hz.guannengcc.top/gtvxcrawdi.html

TS:   console.error("err")
来源：http://hz.guowangkeji.top/gtnepbmgys.html

Java: System.err.println("err")
来源：http://hz.aizwys.cn/gttttoxeiv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jinqigufen.top/gtmrnkonct.html

Ruby: warn "err"
来源：http://hz.dianchejie.cn/gtnezikfye.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ehwqpu.com/gtaiqwzvpm.html

[M07] 判断是否为主入口
来源：http://hz.yuanzhike.top/gtoehwkapb.html

Py:   if __name__ == "__main__":
来源：http://hz.zycfv.cn/gtzlnernnh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhongyouzk.top/gtwddaapom.html

JS:   require.main === module
来源：http://hz.sysykeji.top/gtjcdxdxwg.html

TS:   require.main === module
来源：http://hz.hongshengwenyu.top/gtmooiiyvx.html

Java: public static void main(String[] args)
来源：http://hz.yj202588.top/gtaugxotvg.html

Go:   func main()
来源：http://hz.sweek.top/gtflxxtjny.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yonumen.top/gtoxapkaxh.html

C#:   static void Main(string[] args)
来源：http://hz.feifeiyinyue.top/gtijncotyo.html

[M08] 获取系统与运行时信息
来源：http://hz.jianghu66.top/gtlgdttdbs.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cqqwz.cn/gtjhrykjlm.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hammf.cn/gtgtkvbknp.html

JS:   process.platform;  process.version
来源：http://hz.daria6918.cn/gtpvbiqbtg.html

TS:   process.platform;  process.version
来源：http://hz.wangshuangyany.cn/gtehndjxtw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.aibaodan.cn/gtqonbbhsm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhengqikj.top/gtjiuwrbjm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.havefunace.top/gtgqgukwuj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cdnleiting.top/gtphwrhpal.html

================================================================================
来源：http://hz.sufxvd.cn/gttujsmjjz.html

N. 数据结构与算法
来源：http://hz.sysykeji.top/gtnfoqytps.html

================================================================================
来源：http://hz.wangdashe.top/gtvjkjonpz.html


<!-- 参考信息 -->