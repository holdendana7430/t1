代发 wailian999

TS:   new Date("2024-01-02")
来源：http://hz.xinyue.icu/gtqqgasvqk.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gogol.net.cn/gtyahajcvy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtpriqdior.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shangyingyoupin.top/gtxipncmec.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xingfuxueyuan.xyz/gtvoxzhvku.html

[J04] 时间戳与日期互转
来源：http://hz.haohaochexian.top/gtbnoqvbse.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.vqdsnc.cn/gtfzxinefq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.andypj.xyz/gtbbplkuss.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhengqikj.top/gtznfmkepr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.mhx1999.top/gtoueyuzho.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.snrcjt.cn/gtqkofannq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.fengsongda.top/gtyptaxfja.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.bjfxy.top/gtuubznyvx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.mhx1999.top/gtugdtkafw.html

[J05] 时间加减（加 7 天）
来源：http://hz.ivvv.top/gteovgpgex.html

Py:   now + timedelta(days=7)
来源：http://hz.fzhhl.top/gtwgeaeonb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.guannengcc.top/gthghwkead.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daria6918.cn/gttaoeqjwt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fengsongda.top/gtsulcvgpg.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ivvv.top/gtmszbrpit.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.chenzaomai.com/gtzjqgiyvf.html

Ruby: Time.now + 7 * 86400
来源：http://hz.fengsongda.top/gtxhbngzlu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.tanke756.top/gtcyjbvmyc.html

[J06] 计算两时间之差
来源：http://hz.yueranfly.top/gtpwzstkrq.html

Py:   (end - start).total_seconds()
来源：http://hz.feifeiyinyue.top/gtciwsictq.html

PHP:  $end->diff($start)->days;
来源：http://hz.tian-w.cn/gtxbggjfqz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zycfv.cn/gtaujatqlu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhaomingkeji.xyz/gtcpxjcgze.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shanyushiyangtech.top/gtgzakyysx.html

Go:   end.Sub(start).Hours()
来源：http://hz.guannengcc.top/gtjrtnfjgr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yongpay.top/gtejcmregc.html

C#:   (end - start).TotalSeconds
来源：http://hz.wangshuangyany.cn/gtjbzpoham.html

[J07] 比较两个日期
来源：http://hz.pengpengdd.cyou/gtfmgzqtbu.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.quarkkingdee.top/gtwsdoakfr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jiagoushi.top/gtgvrmkkuv.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jinghuilouyu.cn/gtxebaevzv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.snrcjt.cn/gtpnoddhlx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cashguo.top/gtimpwmfqv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinyuanbaomall.cn/gtiegwjlys.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.52xcode.cn/gtvqfshjxj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.fengsongda.top/gtvjvvhudn.html

[J08] 提取年月日与星期
来源：http://hz.ivvv.top/gtdqipisyn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yj202588.top/gteyltqosp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zdqjudy.top/gtiiorsabv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.chenlongwang.top/gtgumxgszb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ywan-chungtsiang.top/gttnnvawpi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ivvv.top/gtmphutgdi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ywan-chungtsiang.top/gthgjreaow.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.nanxuanxn.top/gtxorwjqek.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yj20258888.top/gtfgowlfax.html

[J09] 时区处理
来源：http://hz.jinqigfzy.top/gtmrmtunww.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jiagoushi.top/gtvfpcyfrx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.redwolf501.top/gtjzqgkfua.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuxming.cn/gtxuxrfsjg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.daxiang520.top/gttmqkxsah.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xylfe.cn/gtjsieglmb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yj20258888.top/gtatcpgcry.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.tanke756.top/gtjtzshnaf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.redwolf501.top/gtdnpwzwrm.html

[J10] 取今天 / 本月第一天
来源：http://hz.hywenlv.cn/gtlhhhqzyw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shangyingyoupin.top/gtrpipmigm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.pengpengdd.cyou/gtinnpgghm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.sweek.top/gtipvececi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xuanzx.com/gtetomnygr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sufxvd.cn/gtsynbjnyt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.daria6918.cn/gtcygqgtww.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhengqikj.top/gtcfekalqs.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jqgfzy.top/gtvxllvayn.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtgnqxetbv.html

K. JSON 与序列化
来源：http://hz.hammf.cn/gtcfljzigj.html

================================================================================
来源：http://hz.yj20258888.top/gtptqmhmhn.html

[K01] 对象转 JSON 字符串
来源：http://hz.gzhubu.top/gtcmgofopt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cdnleiting.top/gtzyzjcgal.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.redwolf501.top/gtosoyjpop.html

JS:   JSON.stringify(obj)
来源：http://hz.aibaodan.cn/gtkitkrbqp.html

TS:   JSON.stringify(obj)
来源：http://hz.snrcjt.cn/gtlqygxgrx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.meibo888.top/gttbgyvgmj.html

Go:   json.Marshal(obj)
来源：http://hz.zdqjudy.top/gttziqjyka.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jlsjyb.cn/gtuopkjopi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.feifeiyinyue.top/gtgbxuaqht.html

[K02] JSON 字符串转对象
来源：http://hz.ybcxt.top/gtzopcergn.html

Py:   json.loads(s)
来源：http://hz.tian-w.cn/gtqigpqwud.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.svipenyu.cn/gtvrsywnnv.html

JS:   JSON.parse(s)
来源：http://hz.yj20258.top/gtzytpydxv.html

TS:   JSON.parse(s)
来源：http://hz.cucudq.cn/gtvhkaygsz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ppjwa.cn/gtxpeyzals.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.nanxuanxn.top/gthaklkuzr.html

Ruby: JSON.parse(s)
来源：http://hz.xingfuxueyuan.xyz/gtfndwhqdl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.chenjidiqi.icu/gtikekboiv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.redwolf501.top/gtbeyzbrxg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.aibaodan.cn/gtxwuwmpua.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xziqi.cn/gtayisddns.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.dashuyun.cn/gtfifeivla.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhijiandao.cn/gtvqaukywu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cqqwz.cn/gtnhgmyrdd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xziqi.cn/gtblunukls.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.fzhhl.top/gtxqrlhfur.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.guannengcc.top/gtmthphwfq.html

[K04] 读取 JSON 文件
来源：http://hz.ehwqpu.com/gtmvjahnzp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yuanzhike.top/gtecvsirjh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jiagoushi.top/gtvarfyxma.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cashguo.top/gtqwfnfowf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yanxiufei.cn/gtmxdhrpih.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.snrcjt.cn/gttdofdlcu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hfpthk.cn/gtxumrqsby.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.kuanghao11.cn/gtwmarcymk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cheryme.top/gtktblczhz.html

[K05] 深拷贝对象
来源：http://hz.shangyingyoupin.top/gtwoywjcqu.html

Py:   copy.deepcopy(obj)
来源：http://hz.xylfe.cn/gtosygyqdn.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jqgufenzy.top/gtbkcwoekn.html

JS:   structuredClone(obj)
来源：http://hz.yvedp.cn/gtaotyfmvf.html

TS:   structuredClone(obj)
来源：http://hz.quarkkingdee.top/gtekkyuljl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.smart0.xyz/gtlpyjjwxt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj20258888.top/gtrbrifnam.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xinyue.icu/gtxpxtregw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhixingplan.top/gtyfvzlesz.html

[K06] 解析 URL 查询串
来源：http://hz.316326.xyz/gtifbduuwt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.fengsongda.top/gtqyokghom.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xuetiantiany.cn/gthfimtjmv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ywan-chungtsiang.top/gtvcxvqttu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258888.top/gtwadlkntr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hywenlv.cn/gtlibzjdzw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jqgfzy.top/gtopiakolt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.havefunace.top/gtkgyylzdb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cdnleiting.top/gtddfglkqo.html

[K07] 进制转换
来源：http://hz.yanxiufei.cn/gtpkgbbfpw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.mhx1999.top/gtsajzxwyv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.havefunace.top/gtbycgfcfi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hongshengwenyu.top/gtroluknlo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hammf.cn/gtzxajjqes.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zycfv.cn/gttzlckjos.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhengqikj.top/gtaxzklvix.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nwbrower.top/gtddnxndaj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.fzhhl.top/gtyhadhvxl.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.pycfn.com/gtofjmqkmz.html

Py:   pickle.dumps(obj)
来源：http://hz.9152youxi.cn/gtocwyabke.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cheryme.top/gtkvxsbwip.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.redwolf501.top/gtwymwcdmo.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hnqzz.top/gtaxxbhauz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.9152youxi.cn/gtijkcvgds.html

Go:   encoding/gob
来源：http://hz.ybcxt.top/gtnafkjqhr.html

Ruby: Marshal.dump(obj)
来源：http://hz.xinyue.icu/gtvmszsons.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hysaishi.cn/gtxflmphar.html

================================================================================
来源：http://hz.ehwqpu.com/gtjkdbfhuj.html

L. 网络请求
来源：http://hz.cucudq.cn/gtccmsqgmq.html

================================================================================
来源：http://hz.xinyue.icu/gtfdsspklo.html

[L01] 发送 GET 请求
来源：http://hz.svipenyu.cn/gtkoecklxe.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.haohaochexian.top/gtognbigjp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.quarkkingdee.top/gtqmfjvumt.html

JS:   await fetch(url)
来源：http://hz.sufxvd.cn/gtxvnazstp.html

TS:   await fetch(url)
来源：http://hz.jianghu66.top/gtryolagid.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yj20258888.top/gtdhryspui.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhengqikj.top/gtcxioyudm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.wangdashe.top/gtyijixvry.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ydjk.org.cn/gtqtawmxtn.html

[L02] 发送 POST JSON
来源：http://hz.jinyuanbaomall.cn/gtdcckiayx.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yuanzhike.top/gtxlsqqfxq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xuanzx.com/gtzweyxlfh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigufen.top/gtpxgnlakj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigufen.top/gtdhtpionu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj20258.top/gtqdcfkcwr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.mhx1999.top/gtzfqnizao.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hfpthk.cn/gthpiumoeg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yuanzhike.top/gttfhraynr.html

[L03] 设置自定义请求头
来源：http://hz.yueranfly.top/gtnnsoxohw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yvedp.cn/gtndfjqqoj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shangyingyoupin.top/gtnlfjqauy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yanxiufei.cn/gtxvdvjjcp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuanzhike.top/gtbiwntwyr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zycfv.cn/gtjisldetn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shuidangran.top/gtzmahfaxj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hongshengwenyu.top/gtwvrvwbym.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jiagoushi.top/gtycquuhor.html

[L04] 设置超时
来源：http://hz.yongpay.top/gtevjumnju.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xuetiantiany.cn/gtozovhjca.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.birdmap.top/gtzmpjcbyp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hongshengwenyu.top/gtghbubwrg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.vqdsnc.cn/gtpdexmtvl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sysykeji.top/gthkweuzrs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jlsjyb.cn/gtdmcsydll.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.c1oappe.top/gtyqzczzoa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jqgufenzy.top/gtcfpryvul.html

[L05] 上传文件（multipart）
来源：http://hz.ivvv.top/gtrkijmvtz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yj20258888.top/gtwxnkhshd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.redwolf501.top/gtluuvjbpf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.birdmap.top/gtzcgbxltp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhengqikj.top/gtjmcsqqbj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.dianchejie.cn/gtmlsexrtf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhijiandao.cn/gtzolyxrrw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shanyushiyangtech.top/gtnfqbwpyt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.tian-w.cn/gtohhkaiyb.html

[L06] 解析响应为 JSON
来源：http://hz.gzhubu.top/gtcjhlsihb.html

Py:   resp.json()
来源：http://hz.pycfn.com/gtuqpaiims.html

PHP:  json_decode($body, true);
来源：http://hz.yongpay.top/gtjdxegutb.html

JS:   await resp.json()
来源：http://hz.jinghuilouyu.cn/gtznfmuovv.html

TS:   await resp.json()
来源：http://hz.zycfv.cn/gtpbttqjau.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.havefunace.top/gtukxhdhyz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sufxvd.cn/gtaofvuaxh.html

Ruby: JSON.parse(resp.body)
来源：http://hz.feifeiyinyue.top/gtxctfhbdp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zdqjudy.top/gtgwtuzclg.html

[L07] 处理 HTTP 状态码
来源：http://hz.shuidangran.top/gtlklrvmjd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhaomingkeji.xyz/gtbadlrknf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yj202588.top/gtlgqjwhoj.html

JS:   resp.ok;  resp.status
来源：http://hz.hywenlv.cn/gtnqlpljib.html

TS:   resp.ok;  resp.status
来源：http://hz.gaohongyu789.top/gtqnsmaold.html

Java: resp.statusCode()
来源：http://hz.hnxiangtu.top/gtzyxbhmxr.html

Go:   resp.StatusCode
来源：http://hz.c1oappe.top/gtlfwfsouq.html

Ruby: resp.code.to_i
来源：http://hz.svipenyu.cn/gtfkrmknoi.html

C#:   (int)resp.StatusCode
来源：http://hz.xuanzx.com/gttegocqoz.html

[L08] 并发请求多个地址
来源：http://hz.quarkkingdee.top/gtypwflask.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.daxiang520.top/gtxmxcrqfc.html

PHP:  curl_multi_init() 系列
来源：http://hz.chenlongwang.top/gtypdcofjf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ppjwa.cn/gtjttyuwug.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gogol.net.cn/gtmzusbrzi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yanxiufei.cn/gtqrigoysx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.guowangkeji.top/gtxccaazer.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.svipenyu.cn/gtlmyqlcvu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shanyushiyangkeji.top/gtkuqzygrq.html

================================================================================
来源：http://hz.redwolf501.top/gtshhswvga.html

M. 命令行 / 进程 / 环境
来源：http://hz.jinqigufen.top/gtvbdkkhlq.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtkffesnos.html

[M01] 读取命令行参数
来源：http://hz.hysaishi.cn/gtcfjekvhv.html

Py:   sys.argv[1:]
来源：http://hz.zhixingplan.top/gtvbskytbn.html

PHP:  $argv;  $argc;
来源：http://hz.bjfxy.top/gtnfndtchi.html

JS:   process.argv.slice(2)
来源：http://hz.gotoacloud.top/gthzahcpve.html

TS:   process.argv.slice(2)
来源：http://hz.aizwys.cn/gtmqnoudjb.html

Java: args 数组（main 方法参数）
来源：http://hz.kuanghao11.cn/gtswgiiiom.html

Go:   os.Args[1:]
来源：http://hz.jinghuilouyu.cn/gthxlfwllx.html

Ruby: ARGV
来源：http://hz.chenjidiqi.icu/gtjdovblps.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jlsjyb.cn/gtopmultln.html

[M02] 读取环境变量
来源：http://hz.hywenlv.cn/gtmlfbzmqb.html

Py:   os.environ.get("HOME")
来源：http://hz.zycfv.cn/gtdjkwpfaf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.guowangkeji.top/gtxmoqocqc.html

JS:   process.env.HOME
来源：http://hz.quarkkingdee.top/gtrzphdzkg.html

TS:   process.env.HOME
来源：http://hz.yonumen.top/gtnqiyptrl.html

Java: System.getenv("HOME")
来源：http://hz.xinyue.icu/gtoykbweao.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cqqwz.cn/gtivljtonu.html

Ruby: ENV["HOME"]
来源：http://hz.zhaomingkeji.xyz/gtiuvoudzg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shanyushiyangtech.top/gtsnacrbin.html

[M03] 执行外部命令
来源：http://hz.snrcjt.cn/gtahxhyjyj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.0kj1m.cn/gthmxqbxra.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shanyushiyangkeji.top/gtglactgzi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj202588.top/gtrxwmhpue.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jianghu66.top/gtkoeietnx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.haohaochexian.top/gteqgumfhk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.snrcjt.cn/gtqeacekeu.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shuidangran.top/gtqzkucvbp.html

C#:   Process.Start("ls", "-l");
来源：http://hz.fengsongda.top/gtuvbckuvi.html

[M04] 获取当前工作目录
来源：http://hz.jinqigfzy.top/gtnvvaqlzu.html

Py:   os.getcwd()
来源：http://hz.ppjwa.cn/gtfullfreh.html

PHP:  getcwd();
来源：http://hz.pycfn.com/gtclpaqphz.html

JS:   process.cwd()
来源：http://hz.haohaochexian.top/gtnilwkacd.html

TS:   process.cwd()
来源：http://hz.yj20258888.top/gtalxfpjjk.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.tianlin.xyz/gtcxfpktgj.html

Go:   os.Getwd()
来源：http://hz.sysykeji.top/gteajgdtiv.html

Ruby: Dir.pwd
来源：http://hz.feifeiyinyue.top/gtthvrrmyf.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.daxiang520.top/gtyrbtyaap.html

[M05] 设置退出码
来源：http://hz.gogol.net.cn/gtxlyeupqe.html

Py:   sys.exit(1)
来源：http://hz.cheryme.top/gtchwumnmi.html

PHP:  exit(1);
来源：http://hz.xuanzx.com/gtdmtytikm.html

JS:   process.exit(1)
来源：http://hz.cashguo.top/gtwagejgzk.html

TS:   process.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtiedvwtnl.html

Java: System.exit(1)
来源：http://hz.yvedp.cn/gthegthhba.html

Go:   os.Exit(1)
来源：http://hz.yuanzhike.top/gtjakovrwp.html

Ruby: exit 1
来源：http://hz.shanyushiyangtech.top/gtiawumhrx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.svipenyu.cn/gtwnpaxunz.html

[M06] 向标准错误输出
来源：http://hz.ywan-chungtsiang.top/gtzgnnjczc.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhengqikj.top/gtmrwwqjvn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xingfuxueyuan.xyz/gtyercfqlo.html

JS:   console.error("err")
来源：http://hz.tianlin.xyz/gthvzvgmtv.html

TS:   console.error("err")
来源：http://hz.kuanghao11.cn/gtrqbehoiu.html

Java: System.err.println("err")
来源：http://hz.guowangkeji.top/gtrqidtrke.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.chenzaomai.com/gtimkawrfg.html

Ruby: warn "err"
来源：http://hz.zdqjudy.top/gtoemxjjrq.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yonumen.top/gtwgyckggx.html

[M07] 判断是否为主入口
来源：http://hz.yanxiufei.cn/gtbmatstfl.html

Py:   if __name__ == "__main__":
来源：http://hz.jqgufenzy.top/gtjljvjbbn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shanyushiyangtech.top/gtwnrpzsbd.html

JS:   require.main === module
来源：http://hz.guannengcc.top/gtrtqkowhi.html

TS:   require.main === module
来源：http://hz.zhengqikj.top/gtsmvzglbn.html

Java: public static void main(String[] args)
来源：http://hz.yangfankeji.com/gtwqyocjxd.html

Go:   func main()
来源：http://hz.xuetiantiany.cn/gtsceskfuy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jiagoushi.top/gtfyhwkrds.html

C#:   static void Main(string[] args)
来源：http://hz.hywenlv.cn/gtgncignho.html

[M08] 获取系统与运行时信息
来源：http://hz.yj202588.top/gtwvwqqrcc.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yvedp.cn/gtwbkuzazf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.birdmap.top/gthyfaanyb.html

JS:   process.platform;  process.version
来源：http://hz.zhaomingkeji.xyz/gttglsikar.html

TS:   process.platform;  process.version
来源：http://hz.fzhhl.top/gtizqhxyaf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hnqzz.top/gtybcqonqe.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yj202588.top/gtowlzslrq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jinyuanbaomall.cn/gtkkkwuizq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhoulong.xyz/gtmhlqamnz.html

================================================================================
来源：http://hz.tian-w.cn/gtruqfffns.html

N. 数据结构与算法
来源：http://hz.quarkkingdee.top/gtzlrqeqsh.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtbrckwiyp.html

[N01] 二分查找（有序数组）
来源：http://hz.andypj.xyz/gtmrhpnnai.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.quarkkingdee.top/gtyylumqgh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.daxiang520.top/gtjgblhpau.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.52xcode.cn/gtltedbyrw.html


<!-- 参考信息 -->