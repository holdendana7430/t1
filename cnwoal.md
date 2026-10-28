代发 wailian999

TS:   new Date("2024-01-02")
来源：http://hz.yueranfly.top/gtopgybbyn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gthdiyncwz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.andypj.xyz/gtovoauvkc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhengqikj.top/gtrsnafwhd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.bjfxy.top/gtobqtuqov.html

[J04] 时间戳与日期互转
来源：http://hz.shuidangran.top/gttirzwxvv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.fengsongda.top/gtbyjspuqo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cdnleiting.top/gtohrjxjtj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.snrcjt.cn/gtutdixxis.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jianghu66.top/gtfjjkezru.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shanyushiyangtech.top/gtiigkrucy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.cucudq.cn/gtnpysyejw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jqgufenzy.top/gtmycrqzsg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.guowangkeji.top/gtdjghfqxp.html

[J05] 时间加减（加 7 天）
来源：http://hz.cucudq.cn/gtrcreszvg.html

Py:   now + timedelta(days=7)
来源：http://hz.52xcode.cn/gtgpqhwchp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hnqzz.top/gtxoxxcnqk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xinyue.icu/gtbeuxrkkf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nanxuanxn.top/gtvsvwdjks.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.sysykeji.top/gttsqqxbof.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ppjwa.cn/gtfeisqlrx.html

Ruby: Time.now + 7 * 86400
来源：http://hz.9152youxi.cn/gtwrxgqxug.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.meibo888.top/gtsujmuzfd.html

[J06] 计算两时间之差
来源：http://hz.vqdsnc.cn/gtocqgluln.html

Py:   (end - start).total_seconds()
来源：http://hz.0kj1m.cn/gtvaqujcdw.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhengqikj.top/gtqdymrjqg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.tanke756.top/gtdxahhvam.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.chenlongwang.top/gtnzqyzqpc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yj202588.top/gtdzsfcjyk.html

Go:   end.Sub(start).Hours()
来源：http://hz.havefunace.top/gthrsezzpd.html

Ruby: end - start                 # 返回秒数
来源：http://hz.tian-w.cn/gtzygzrqhr.html

C#:   (end - start).TotalSeconds
来源：http://hz.smart0.xyz/gteyrwmryb.html

[J07] 比较两个日期
来源：http://hz.xuetiantiany.cn/gtsgshyjxk.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtyimsnfgk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zdqjudy.top/gtkshfmykd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gotoacloud.top/gtjxupeput.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sufxvd.cn/gtfunmslqi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhixingplan.top/gtiuslijzj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.tianlin.xyz/gtoovsashe.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yj20258.top/gtlnajbnfz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ybcxt.top/gtgaovzpva.html

[J08] 提取年月日与星期
来源：http://hz.jinghuilouyu.cn/gthxstdslc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.quarkkingdee.top/gtjqekiagh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hammf.cn/gtxohyhvpx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.bjfxy.top/gtaojgwgjt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jyoumei.cn/gtpgleznvi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jqgfzy.top/gtcxbtiuar.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.nwbrower.top/gtakursyzh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cheryme.top/gtbikiiddr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.cheryme.top/gtapijkkjd.html

[J09] 时区处理
来源：http://hz.ywan-chungtsiang.top/gtahgljhar.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cdnleiting.top/gtcnfpfste.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.daria6918.cn/gtxtzjcaqq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnxiangtu.top/gtldpwbgox.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.daxiang520.top/gthqveuime.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.meibo888.top/gtnzsedqqf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.quarkkingdee.top/gtivwiempo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zycfv.cn/gtktripxfk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jyoumei.cn/gtsrptjrtw.html

[J10] 取今天 / 本月第一天
来源：http://hz.hongshengwenyu.top/gtgrerdgjt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shangyingyoupin.top/gtfcyyrbzp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.chenjidiqi.icu/gtddibpvnd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.andypj.xyz/gteolxpypd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jyoumei.cn/gtardwicgh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhengqikj.top/gtpkgagjpf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.birdmap.top/gtjmvsbbdp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.guowangkeji.top/gttobohvpq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.nanxinkj.top/gtevmuhxss.html

================================================================================
来源：http://hz.yongpay.top/gtlgkydnqt.html

K. JSON 与序列化
来源：http://hz.zhongyouzk.top/gtihnzcbtr.html

================================================================================
来源：http://hz.jinqigufen.top/gtwqhsmibg.html

[K01] 对象转 JSON 字符串
来源：http://hz.xuetiantiany.cn/gtojflezmx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.quarkkingdee.top/gtxsardghq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxinkj.top/gtvqjifngw.html

JS:   JSON.stringify(obj)
来源：http://hz.xinyue.icu/gtycnieykg.html

TS:   JSON.stringify(obj)
来源：http://hz.yj20258888.top/gtcnohvshr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.smart0.xyz/gtkxyendow.html

Go:   json.Marshal(obj)
来源：http://hz.birdmap.top/gtudsmjtef.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhongyouzk.top/gtinwmwsjl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.pycfn.com/gtynobaadf.html

[K02] JSON 字符串转对象
来源：http://hz.wangdashe.top/gttdctlljg.html

Py:   json.loads(s)
来源：http://hz.ywan-chungtsiang.top/gtdlalyooz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jinqigufen.top/gtpppfnaqd.html

JS:   JSON.parse(s)
来源：http://hz.dianchejie.cn/gtniighwbs.html

TS:   JSON.parse(s)
来源：http://hz.chenjidiqi.icu/gtlarcbfyn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.tianlin.xyz/gtewncblwg.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.kuanghao11.cn/gtkcyhxmza.html

Ruby: JSON.parse(s)
来源：http://hz.zhijiandao.cn/gtaanqgieu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhengqikj.top/gtzyzjbvwy.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yangfankeji.com/gtisdwrwsp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jiagoushi.top/gtcrdtvpsy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gogol.net.cn/gtvggfdoea.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hysaishi.cn/gtezqxeytc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.nwbrower.top/gtyhkqxfjw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dashuyun.cn/gtmqdqzepf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.vqdsnc.cn/gtkesulfvd.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.feifeiyinyue.top/gtiukwvgke.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cheryme.top/gtafdnkumo.html

[K04] 读取 JSON 文件
来源：http://hz.shuidangran.top/gtbgsvwsns.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.svipenyu.cn/gtyxrxpfoi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yongpay.top/gtxfumlfls.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ydjk.org.cn/gtewrhvzmw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.birdmap.top/gttrofmyso.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.nanxuanxn.top/gtcxmfouti.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xziqi.cn/gtjdzrjvap.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yj20258.top/gtafnnnnew.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinyuanbaomall.cn/gttouazvti.html

[K05] 深拷贝对象
来源：http://hz.birdmap.top/gtnnqwbspw.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinqigufen.top/gtutxzegye.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yongpay.top/gtpzmxkosd.html

JS:   structuredClone(obj)
来源：http://hz.yj20258.top/gtygripizm.html

TS:   structuredClone(obj)
来源：http://hz.guannengcc.top/gtjlbbkbhh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cheryme.top/gtefjgnnoh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.cqqwz.cn/gtfastfnyi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.aizwys.cn/gtqsrgsocf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.vqdsnc.cn/gtbihojpzp.html

[K06] 解析 URL 查询串
来源：http://hz.zhoulong.xyz/gtyunidwjf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yonumen.top/gtcdeddfpq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.kuanghao11.cn/gtfxydjnfh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shuidangran.top/gtfsyfgvug.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gotoacloud.top/gtvieetjdr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.smart0.xyz/gtkyfqslkc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.redwolf501.top/gtbjcicayu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.kuanghao11.cn/gtvmfckzim.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.tanke756.top/gtoaoadsot.html

[K07] 进制转换
来源：http://hz.aizwys.cn/gtqbzeqgxg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.daria6918.cn/gtabhssvrc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.redwolf501.top/gtdtrnllrr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhoulong.xyz/gtijcqscht.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jiagoushi.top/gtxuivmdlz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.bjfxy.top/gtidupburp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.iojbl.cn/gtijuptoas.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yanxiufei.cn/gtzpuxuujy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.pycfn.com/gtsndwqpkm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shzxlz.cn/gtiikxgujb.html

Py:   pickle.dumps(obj)
来源：http://hz.yj20258.top/gtpolppamh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hfpthk.cn/gtlmmyrxir.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.tian-w.cn/gtjjhkmgri.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yj20258888.top/gtboevaifs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.quarkkingdee.top/gtevrwypsm.html

Go:   encoding/gob
来源：http://hz.yanxiufei.cn/gtegqfuszr.html

Ruby: Marshal.dump(obj)
来源：http://hz.snrcjt.cn/gtffltguyx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.aizwys.cn/gtpzveresi.html

================================================================================
来源：http://hz.yueranfly.top/gtopykbhnp.html

L. 网络请求
来源：http://hz.zhengqikj.top/gtadjzcmik.html

================================================================================
来源：http://hz.hnqzz.top/gtxidtgghf.html

[L01] 发送 GET 请求
来源：http://hz.sufxvd.cn/gtfdnurdas.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.andypj.xyz/gtsdtgilcj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sxryk.cn/gtvxgqusnd.html

JS:   await fetch(url)
来源：http://hz.yuxming.cn/gtqixrospw.html

TS:   await fetch(url)
来源：http://hz.wangshuangyany.cn/gtlugpyyta.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hysaishi.cn/gtespxsfrc.html

Go:   resp, err := http.Get(url)
来源：http://hz.jlsjyb.cn/gttxsygdoi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hongshengwenyu.top/gtvmihrhrx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xuetiantiany.cn/gtazwvwkzk.html

[L02] 发送 POST JSON
来源：http://hz.aibaodan.cn/gtisovnclb.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.wangdashe.top/gtjohuhaty.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yangfankeji.com/gtpqiadbkc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tanke756.top/gtjhdlimpp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jlsjyb.cn/gtozrezkck.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ehwqpu.com/gtneqepegs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jianghu66.top/gtnkisylyj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.smart0.xyz/gtkosklfks.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.meibo888.top/gtdysdwonj.html

[L03] 设置自定义请求头
来源：http://hz.yuxming.cn/gtstkgsyxh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hywenlv.cn/gtgrqyexyl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ybcxt.top/gtfpbxtdbr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jqgfzy.top/gtybbyenfe.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dianchejie.cn/gtygttnovn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jlsjyb.cn/gtgzdnwmiv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zdqjudy.top/gtrlihzlvr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.meibo888.top/gtzzkvyhfz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shanyushiyangkeji.top/gtqhxsrnmm.html

[L04] 设置超时
来源：http://hz.dashuyun.cn/gtdmoelwym.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hnqzz.top/gthiqbipul.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jlsjyb.cn/gtbsbcskng.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yongpay.top/gtvkadevdj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jlsjyb.cn/gtobnfoshu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hammf.cn/gteyhuxiti.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.c1oappe.top/gtzjjpsuxt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.sufxvd.cn/gtvtdhlijo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhongyouzk.top/gtbuntdaxl.html

[L05] 上传文件（multipart）
来源：http://hz.bjfxy.top/gtizczvoxt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cucudq.cn/gtklhckoic.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.fengsongda.top/gtovtgqmvq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yangfankeji.com/gtkicnbyyf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sweek.top/gtjhdlgiss.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.chenzaomai.com/gtidrqbmpw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.guowangkeji.top/gtipllzage.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sysykeji.top/gtqxkpsvmt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zycfv.cn/gtbresdoif.html

[L06] 解析响应为 JSON
来源：http://hz.gogol.net.cn/gtvwwbkqco.html

Py:   resp.json()
来源：http://hz.guowangkeji.top/gtrezkdtbo.html

PHP:  json_decode($body, true);
来源：http://hz.zhaomingkeji.xyz/gtsfbmfmkz.html

JS:   await resp.json()
来源：http://hz.zhengqikj.top/gtvodejayp.html

TS:   await resp.json()
来源：http://hz.gotoacloud.top/gtmojkozxa.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.guowangkeji.top/gtweyklthh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gzhubu.top/gtoijarhln.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sxryk.cn/gtpvlmtyfs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.sysykeji.top/gtdkdpvhtb.html

[L07] 处理 HTTP 状态码
来源：http://hz.hysaishi.cn/gtcjkrfcwi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yj20258888.top/gtcysaexil.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.smart0.xyz/gtxiagmrfp.html

JS:   resp.ok;  resp.status
来源：http://hz.c1oappe.top/gtmvpuhllx.html

TS:   resp.ok;  resp.status
来源：http://hz.sxryk.cn/gtbtrrgmxc.html

Java: resp.statusCode()
来源：http://hz.hysaishi.cn/gtmhpsvefh.html

Go:   resp.StatusCode
来源：http://hz.havefunace.top/gtusrrwlsb.html

Ruby: resp.code.to_i
来源：http://hz.xylfe.cn/gtvholkcif.html

C#:   (int)resp.StatusCode
来源：http://hz.hysaishi.cn/gtddkdghal.html

[L08] 并发请求多个地址
来源：http://hz.shanyushiyangtech.top/gtlorfqrjv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yangfankeji.com/gtklhpoljm.html

PHP:  curl_multi_init() 系列
来源：http://hz.chenlongwang.top/gtfusrztzx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangdashe.top/gteakdyeyt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ivvv.top/gtqopflxzo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.tianlin.xyz/gtleqydkve.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tian-w.cn/gtlgqkwycj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhijiandao.cn/gthgpnwvap.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.iojbl.cn/gtrhsztioo.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtcgjtysrq.html

M. 命令行 / 进程 / 环境
来源：http://hz.tanke756.top/gtouvrkhuj.html

================================================================================
来源：http://hz.yangfankeji.com/gtrwvwmgqe.html

[M01] 读取命令行参数
来源：http://hz.jqgufenzy.top/gttbsgwrhb.html

Py:   sys.argv[1:]
来源：http://hz.ywan-chungtsiang.top/gtdlevtnhu.html

PHP:  $argv;  $argc;
来源：http://hz.tianlin.xyz/gtqikkvftv.html

JS:   process.argv.slice(2)
来源：http://hz.guannengcc.top/gtdxpflgju.html

TS:   process.argv.slice(2)
来源：http://hz.havefunace.top/gtlptdcpat.html

Java: args 数组（main 方法参数）
来源：http://hz.jinqigufen.top/gtybizrnhg.html

Go:   os.Args[1:]
来源：http://hz.xuanzx.com/gtqsrobwlc.html

Ruby: ARGV
来源：http://hz.feifeiyinyue.top/gtwadmoohu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.nwbrower.top/gtcwnplpam.html

[M02] 读取环境变量
来源：http://hz.sweek.top/gttlauwxxe.html

Py:   os.environ.get("HOME")
来源：http://hz.hammf.cn/gtamgenlmf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.snrcjt.cn/gtuinazvyb.html

JS:   process.env.HOME
来源：http://hz.jinyuanbaomall.cn/gtelielxmx.html

TS:   process.env.HOME
来源：http://hz.fengsongda.top/gtmaoaskcj.html

Java: System.getenv("HOME")
来源：http://hz.nwbrower.top/gtnjqynlot.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jinqigfzy.top/gtzdwmjfwk.html

Ruby: ENV["HOME"]
来源：http://hz.shuidangran.top/gtnojgmfbr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jianghu66.top/gtpcyiypym.html

[M03] 执行外部命令
来源：http://hz.ehwqpu.com/gtwbonwfad.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hnxiangtu.top/gtzgcgzjiv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.vqdsnc.cn/gtuxusrkdv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sweek.top/gtppsxqpoh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.aibaodan.cn/gtpxkuaazx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jiagoushi.top/gtkahwdexi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yj20258.top/gtgmrukgbx.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhiwuduotai.top/gtrvxrumch.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhaomingkeji.xyz/gtxymchpxu.html

[M04] 获取当前工作目录
来源：http://hz.c1oappe.top/gtedbrydnz.html

Py:   os.getcwd()
来源：http://hz.redwolf501.top/gtnhsutygj.html

PHP:  getcwd();
来源：http://hz.hfpthk.cn/gtvpkidsxp.html

JS:   process.cwd()
来源：http://hz.ehwqpu.com/gtzozvpbvo.html

TS:   process.cwd()
来源：http://hz.ivvv.top/gttinrmsyt.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhaomingkeji.xyz/gtfmvljcpd.html

Go:   os.Getwd()
来源：http://hz.chenjidiqi.icu/gtmwikrgpu.html

Ruby: Dir.pwd
来源：http://hz.chenjidiqi.icu/gthchjvukt.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hysaishi.cn/gtelshygzw.html

[M05] 设置退出码
来源：http://hz.shanyushiyangtech.top/gtkniecnmh.html

Py:   sys.exit(1)
来源：http://hz.cdnleiting.top/gtuitzenmq.html

PHP:  exit(1);
来源：http://hz.feifeiyinyue.top/gtvzpqrqdh.html

JS:   process.exit(1)
来源：http://hz.havefunace.top/gtwawqwyzu.html

TS:   process.exit(1)
来源：http://hz.xuetiantiany.cn/gtmaeotwvr.html

Java: System.exit(1)
来源：http://hz.ydzc1.top/gtzvtlgvlf.html

Go:   os.Exit(1)
来源：http://hz.hongshengwenyu.top/gtjckktmxg.html

Ruby: exit 1
来源：http://hz.yj20258.top/gtgtxbjrue.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.redwolf501.top/gtzjeyasva.html

[M06] 向标准错误输出
来源：http://hz.chenjidiqi.icu/gtxudfngxo.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhixingplan.top/gtqzcmsruu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xingfuxueyuan.xyz/gtwzamawsh.html

JS:   console.error("err")
来源：http://hz.xziqi.cn/gtaarhdfqr.html

TS:   console.error("err")
来源：http://hz.hysaishi.cn/gtoahfmrpn.html

Java: System.err.println("err")
来源：http://hz.hywenlv.cn/gthygleils.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ydzc1.top/gtjsogmpzp.html

Ruby: warn "err"
来源：http://hz.sweek.top/gtstfrazek.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.birdmap.top/gtjbfnwyzk.html

[M07] 判断是否为主入口
来源：http://hz.iojbl.cn/gtodxrjvzh.html

Py:   if __name__ == "__main__":
来源：http://hz.smart0.xyz/gtjzntfyyo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yangfankeji.com/gtpgrlbgve.html

JS:   require.main === module
来源：http://hz.vqdsnc.cn/gtowaeasus.html

TS:   require.main === module
来源：http://hz.guowangkeji.top/gthogkqjdy.html

Java: public static void main(String[] args)
来源：http://hz.haohaochexian.top/gtkwpynqgu.html

Go:   func main()
来源：http://hz.ywan-chungtsiang.top/gtxznqjcil.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.bjfxy.top/gtryedpbke.html

C#:   static void Main(string[] args)
来源：http://hz.ehwqpu.com/gtwwcqrosu.html

[M08] 获取系统与运行时信息
来源：http://hz.snrcjt.cn/gtdgbnrahn.html

Py:   platform.system();  platform.python_version()
来源：http://hz.snrcjt.cn/gtdsquabbk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.sysykeji.top/gtmeeqeiwv.html

JS:   process.platform;  process.version
来源：http://hz.xuanzx.com/gtmuzrmhgy.html

TS:   process.platform;  process.version
来源：http://hz.hfpthk.cn/gtaaiuzyau.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.chenjidiqi.icu/gtvlexlrxg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hammf.cn/gtopuobnfi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.daxiang520.top/gtcxavznez.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xinyue.icu/gtsobplkmy.html

================================================================================
来源：http://hz.pycfn.com/gtatcrpxzq.html

N. 数据结构与算法
来源：http://hz.zycfv.cn/gtsrpgihvv.html

================================================================================
来源：http://hz.tianlin.xyz/gtzzqjjhfv.html

[N01] 二分查找（有序数组）
来源：http://hz.ivvv.top/gtcwbbzhqw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yongpay.top/gtzfwygrof.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jqgufenzy.top/gtkhiitqqt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinghuilouyu.cn/gtozpoyevk.html


<!-- 参考信息 -->