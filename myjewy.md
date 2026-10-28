代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.quarkkingdee.top/gtfbuexrko.html

[J04] 时间戳与日期互转
来源：http://hz.zhaomingkeji.xyz/gthbaeluty.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhongyouzk.top/gtexvkpoli.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.guowangkeji.top/gtmyhlyjjh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhiwuduotai.top/gtciomqpjk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shuidangran.top/gtizpxuvri.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shuidangran.top/gttxrynlmc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.gzhubu.top/gttzxxmfud.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.chenjidiqi.icu/gtasvbyhkg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yangfankeji.com/gttwjzmzwv.html

[J05] 时间加减（加 7 天）
来源：http://hz.hongshengwenyu.top/gtpyqwxzlr.html

Py:   now + timedelta(days=7)
来源：http://hz.hnxiangtu.top/gtdhlxhhgd.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.gotoacloud.top/gtfnlpcyvy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sufxvd.cn/gtsfquftfu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daria6918.cn/gtuageqbsr.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jiagoushi.top/gtfigtkxtq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.pengpengdd.cyou/gtkcnyhwlx.html

Ruby: Time.now + 7 * 86400
来源：http://hz.havefunace.top/gtfunlsjqa.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sweek.top/gtbtsdxdjv.html

[J06] 计算两时间之差
来源：http://hz.jinghuilouyu.cn/gtdtpijwyv.html

Py:   (end - start).total_seconds()
来源：http://hz.nanxinkj.top/gtivcikrnn.html

PHP:  $end->diff($start)->days;
来源：http://hz.aibaodan.cn/gtgheaphtr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yvedp.cn/gtuvkzqqnv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.haohaochexian.top/gtsvvsikgj.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zycfv.cn/gtozlinukq.html

Go:   end.Sub(start).Hours()
来源：http://hz.dashuyun.cn/gtipapnorh.html

Ruby: end - start                 # 返回秒数
来源：http://hz.kuanghao11.cn/gtvywzmkjd.html

C#:   (end - start).TotalSeconds
来源：http://hz.xuetiantiany.cn/gtnunglhgu.html

[J07] 比较两个日期
来源：http://hz.mhx1999.top/gtxhztwhvq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cqqwz.cn/gtwwuwbrfu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cdnleiting.top/gtvfsvmomp.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.9152youxi.cn/gtupppymsv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zdqjudy.top/gtpaejclre.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.andypj.xyz/gtddcxocql.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zycfv.cn/gticvphske.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sweek.top/gtofjzzmns.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtvcazskwx.html

[J08] 提取年月日与星期
来源：http://hz.snrcjt.cn/gtcekrczjc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ybcxt.top/gtzblrwmxj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jqgufenzy.top/gtkuzmtcap.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.gaohongyu789.top/gtolckkgbb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhijiandao.cn/gthvgtujod.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zdqjudy.top/gttynbfthh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.sysykeji.top/gtoglyedjs.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.pengpengdd.cyou/gtyiqggfqy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zycfv.cn/gtcawisqoh.html

[J09] 时区处理
来源：http://hz.havefunace.top/gtjmmvziuz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.aizwys.cn/gtwkzuwrwb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xuanzx.com/gtbwvbtsjq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tian-w.cn/gtffaiewvn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.svipenyu.cn/gtdnnxvpro.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cheryme.top/gtdfrcndcp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sysykeji.top/gtxgleuulz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cdnleiting.top/gtorxahcpa.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.bjfxy.top/gtnhxlvcte.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhaomingkeji.xyz/gtsyoqjftj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj202588.top/gtlkpgcrcc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhijiandao.cn/gtjbhvebnx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yonumen.top/gtzqlqnmin.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yj202588.top/gtaqghbaep.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhaomingkeji.xyz/gtnhseewsq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.pengpengdd.cyou/gtgjhycjqc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xingfuxueyuan.xyz/gtdjwfvezw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.tianlin.xyz/gtuoerxrfu.html

================================================================================
来源：http://hz.yangfankeji.com/gtgoptvywy.html

K. JSON 与序列化
来源：http://hz.xylfe.cn/gtfyvwzamc.html

================================================================================
来源：http://hz.daxiang520.top/gtfvwccyfi.html

[K01] 对象转 JSON 字符串
来源：http://hz.ehwqpu.com/gtetdytgkr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yangfankeji.com/gtqbiwplqq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.dianchejie.cn/gtrazstfqr.html

JS:   JSON.stringify(obj)
来源：http://hz.chenjidiqi.icu/gtpjejhnfa.html

TS:   JSON.stringify(obj)
来源：http://hz.guowangkeji.top/gtzywwuqyj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ywan-chungtsiang.top/gtakozzyyh.html

Go:   json.Marshal(obj)
来源：http://hz.gzhubu.top/gtejhlivhg.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ydjk.org.cn/gtrzbxuada.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xuetiantiany.cn/gtpkyycaaw.html

[K02] JSON 字符串转对象
来源：http://hz.hnxiangtu.top/gtwrrattzs.html

Py:   json.loads(s)
来源：http://hz.dashuyun.cn/gtligoobha.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.wangdashe.top/gtadtpgpii.html

JS:   JSON.parse(s)
来源：http://hz.zhongyouzk.top/gtyvzcsvwv.html

TS:   JSON.parse(s)
来源：http://hz.feifeiyinyue.top/gtavdjtcpo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shanyushiyangkeji.top/gtzgvpigzs.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.nanxinkj.top/gtjeaarhwu.html

Ruby: JSON.parse(s)
来源：http://hz.ydjk.org.cn/gtvfcmvnyq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xingfuxueyuan.xyz/gtrvknbfwx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yueranfly.top/gtrjtifgzm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.wangshuangyany.cn/gtjejebika.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigfzy.top/gtkkqypsbl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yuxming.cn/gtiexqhxvo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.haohaochexian.top/gtfstlgtwl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.gogol.net.cn/gtliryunzc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shuidangran.top/gtmsgzmstp.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gzhubu.top/gtsixxuwwu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.wangshuangyany.cn/gtxwixvpvj.html

[K04] 读取 JSON 文件
来源：http://hz.daria6918.cn/gtbxvuywbk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shzxlz.cn/gtlbqrusca.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sxryk.cn/gtrmhefqiu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yuxming.cn/gtaupnxezy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nanxinkj.top/gtmtwcyhmh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.wangdashe.top/gtjsurzpyb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenlongwang.top/gtzxaxzqee.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gzhubu.top/gtfiermprj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cashguo.top/gtjqyoarxy.html

[K05] 深拷贝对象
来源：http://hz.zhaomingkeji.xyz/gtmlochyrf.html

Py:   copy.deepcopy(obj)
来源：http://hz.guannengcc.top/gtawicticf.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ivvv.top/gtwrwezeej.html

JS:   structuredClone(obj)
来源：http://hz.zhijiandao.cn/gtazoddgew.html

TS:   structuredClone(obj)
来源：http://hz.zhijiandao.cn/gttocupwac.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.tianlin.xyz/gtfjggfmsu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jyoumei.cn/gtitclwgvx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.mhx1999.top/gtlkqommxm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hywenlv.cn/gtwdtqgpsh.html

[K06] 解析 URL 查询串
来源：http://hz.nanxinkj.top/gtqhtyysew.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xziqi.cn/gtgbmbqesf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xuanzx.com/gtyhpudcrk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xziqi.cn/gtmtirwpes.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cashguo.top/gtfneobany.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.guannengcc.top/gthlwamgsu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cashguo.top/gtxmidnmhj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ywan-chungtsiang.top/gtbcfxgwss.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yangfankeji.com/gtmhpjvhuz.html

[K07] 进制转换
来源：http://hz.shangyingyoupin.top/gtqrfrsqvy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.andypj.xyz/gtnmehihxt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jinqigufen.top/gtixxxuiuv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xziqi.cn/gtkxjrzyhm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yuanzhike.top/gtpridpooa.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.havefunace.top/gteugtmrjb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.gotoacloud.top/gtpavzuoqk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.fengsongda.top/gtetkxqjrf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jianghu66.top/gtpwlfymkf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jqgfzy.top/gtjwuoineu.html

Py:   pickle.dumps(obj)
来源：http://hz.birdmap.top/gtosydrxck.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ppjwa.cn/gtfnupzjqq.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hnqzz.top/gtknhqayff.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.iojbl.cn/gthlnjlikg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jinqigfzy.top/gtrvvmgspe.html

Go:   encoding/gob
来源：http://hz.kuanghao11.cn/gtxlzslucx.html

Ruby: Marshal.dump(obj)
来源：http://hz.redwolf501.top/gttnpopqoj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.9152youxi.cn/gtudsugjrp.html

================================================================================
来源：http://hz.bjfxy.top/gtonkqobib.html

L. 网络请求
来源：http://hz.yuxming.cn/gtzpxthenn.html

================================================================================
来源：http://hz.ivvv.top/gtfytbheqh.html

[L01] 发送 GET 请求
来源：http://hz.jinqigfzy.top/gtzayesziu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.guowangkeji.top/gtpeimbwcn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jinghuilouyu.cn/gtzoljsbae.html

JS:   await fetch(url)
来源：http://hz.fzhhl.top/gtzqzuxwww.html

TS:   await fetch(url)
来源：http://hz.birdmap.top/gtdzrdgank.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yangfankeji.com/gtgjlsywtp.html

Go:   resp, err := http.Get(url)
来源：http://hz.jinyuanbaomall.cn/gtryqzmxqi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cashguo.top/gtcicvfrqg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.dianchejie.cn/gtqksudpcr.html

[L02] 发送 POST JSON
来源：http://hz.ppjwa.cn/gtxoksdamm.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.snrcjt.cn/gtqbvokqqv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ppjwa.cn/gtwnpsrxyv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hysaishi.cn/gtjzltsypd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xinyue.icu/gtsgjcpcmi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jqgufenzy.top/gtkazmqbvr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sysykeji.top/gtcubftqlm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yanxiufei.cn/gtyocypipd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.havefunace.top/gtjhycuqrx.html

[L03] 设置自定义请求头
来源：http://hz.redwolf501.top/gtxtvmwdvh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.iojbl.cn/gtbsksvcdb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.chenjidiqi.icu/gtjntwstpc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxinkj.top/gtprknfhzu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuanzx.com/gtnrhvdghs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jqgufenzy.top/gtimbilqnl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.andypj.xyz/gtjsthplee.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.gogol.net.cn/gtblswxfqz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jyoumei.cn/gtzcyixpyd.html

[L04] 设置超时
来源：http://hz.ywan-chungtsiang.top/gtpxmudylm.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ydjk.org.cn/gtbjiuyefr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.birdmap.top/gtaoyutkca.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.bjfxy.top/gtnrbjkhvp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cheryme.top/gtifvjxkqt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gaohongyu789.top/gtvwygejzi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.c1oappe.top/gtuyimubzi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xziqi.cn/gtnoqrievf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ydzc1.top/gtuwwsiajo.html

[L05] 上传文件（multipart）
来源：http://hz.hammf.cn/gtsaotyleo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yonumen.top/gtrzwtajuw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jiagoushi.top/gtwkgldmtz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.316326.xyz/gtxnbjdxgn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgufenzy.top/gthlthojoq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shanyushiyangkeji.top/gtytcfexip.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.svipenyu.cn/gtbomurlll.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yj20258.top/gtxzwndopf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.vqdsnc.cn/gtjfokhsbd.html

[L06] 解析响应为 JSON
来源：http://hz.tian-w.cn/gtmgjszjcq.html

Py:   resp.json()
来源：http://hz.jqgufenzy.top/gtsptsxxsh.html

PHP:  json_decode($body, true);
来源：http://hz.hnxiangtu.top/gtyivyfvgq.html

JS:   await resp.json()
来源：http://hz.guannengcc.top/gtralplhyk.html

TS:   await resp.json()
来源：http://hz.feifeiyinyue.top/gtyrxpcoxn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yuanzhike.top/gtaarzawka.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jinyuanbaomall.cn/gtsdkxbras.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yongpay.top/gtqtrsevpm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhoulong.xyz/gtwismjtla.html

[L07] 处理 HTTP 状态码
来源：http://hz.ppjwa.cn/gthjciuzuv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jinqigfzy.top/gtfwikyihx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jqgfzy.top/gtnamagzmt.html

JS:   resp.ok;  resp.status
来源：http://hz.kuanghao11.cn/gtrimyufoq.html

TS:   resp.ok;  resp.status
来源：http://hz.zhaomingkeji.xyz/gtkryskoze.html

Java: resp.statusCode()
来源：http://hz.chenzaomai.com/gticshuedx.html

Go:   resp.StatusCode
来源：http://hz.jyoumei.cn/gtwbmatqkv.html

Ruby: resp.code.to_i
来源：http://hz.wangshuangyany.cn/gtxhahzyow.html

C#:   (int)resp.StatusCode
来源：http://hz.hywenlv.cn/gtktbbmekk.html

[L08] 并发请求多个地址
来源：http://hz.zhixingplan.top/gtbfcovalu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.havefunace.top/gtbafgmtrx.html

PHP:  curl_multi_init() 系列
来源：http://hz.xziqi.cn/gtixnrjfzn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.iojbl.cn/gthtadejtu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xingfuxueyuan.xyz/gtznzpkbcr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yuanzhike.top/gtldaibxca.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinyuanbaomall.cn/gtvmyvqctr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jianghu66.top/gtjcpvgkwf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xingfuxueyuan.xyz/gtrqqvpmek.html

================================================================================
来源：http://hz.jlsjyb.cn/gtijepouyp.html

M. 命令行 / 进程 / 环境
来源：http://hz.ehwqpu.com/gtykroxggw.html

================================================================================
来源：http://hz.jianghu66.top/gttkbmarzn.html

[M01] 读取命令行参数
来源：http://hz.iojbl.cn/gtlodvezpq.html

Py:   sys.argv[1:]
来源：http://hz.hnqzz.top/gtrcfpjdbz.html

PHP:  $argv;  $argc;
来源：http://hz.hysaishi.cn/gtfdluwhbq.html

JS:   process.argv.slice(2)
来源：http://hz.xuetiantiany.cn/gtpbmcsoap.html

TS:   process.argv.slice(2)
来源：http://hz.wangdashe.top/gtktmhhpqh.html

Java: args 数组（main 方法参数）
来源：http://hz.hywenlv.cn/gtsavxbrxw.html

Go:   os.Args[1:]
来源：http://hz.ppjwa.cn/gtddipbvkf.html

Ruby: ARGV
来源：http://hz.xuetiantiany.cn/gtajhpgzss.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jinqigfzy.top/gtqiqaejaa.html

[M02] 读取环境变量
来源：http://hz.xuanzx.com/gtuavwshws.html

Py:   os.environ.get("HOME")
来源：http://hz.redwolf501.top/gtkcwobemk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.smart0.xyz/gtsmznxvdt.html

JS:   process.env.HOME
来源：http://hz.ydzc1.top/gtfdbxkmce.html

TS:   process.env.HOME
来源：http://hz.xingfuxueyuan.xyz/gtolnibbni.html

Java: System.getenv("HOME")
来源：http://hz.0kj1m.cn/gtfiigkidc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sysykeji.top/gtsdrplewr.html

Ruby: ENV["HOME"]
来源：http://hz.tanke756.top/gtjdtatrxs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cqqwz.cn/gtdrcedvpq.html

[M03] 执行外部命令
来源：http://hz.wangdashe.top/gtlwfpzbmu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.tianlin.xyz/gtydilcuup.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yuxming.cn/gtlacdpiln.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigfzy.top/gtyqahneye.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cdnleiting.top/gtpriuzitd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.0kj1m.cn/gtqzelwjue.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.svipenyu.cn/gtdjxobstp.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.pycfn.com/gtykzafgro.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yanxiufei.cn/gtrrnagihm.html

[M04] 获取当前工作目录
来源：http://hz.yj202588.top/gtetxelykm.html

Py:   os.getcwd()
来源：http://hz.xylfe.cn/gtokhuxtix.html

PHP:  getcwd();
来源：http://hz.jinghuilouyu.cn/gtfpodyohk.html

JS:   process.cwd()
来源：http://hz.bjfxy.top/gtbxxabfrz.html

TS:   process.cwd()
来源：http://hz.52xcode.cn/gtzpzxfngg.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.dashuyun.cn/gtutyjtofl.html

Go:   os.Getwd()
来源：http://hz.sufxvd.cn/gtwqbaochd.html

Ruby: Dir.pwd
来源：http://hz.havefunace.top/gtiqhytvyp.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cheryme.top/gtdjriiolp.html

[M05] 设置退出码
来源：http://hz.jianghu66.top/gtkqrofahz.html

Py:   sys.exit(1)
来源：http://hz.xuanzx.com/gtqvzawvae.html

PHP:  exit(1);
来源：http://hz.dashuyun.cn/gtaegvhiqq.html

JS:   process.exit(1)
来源：http://hz.jinqigfzy.top/gtjondbzbt.html

TS:   process.exit(1)
来源：http://hz.hnxiangtu.top/gtesgkbiiq.html

Java: System.exit(1)
来源：http://hz.tian-w.cn/gtjcibauob.html

Go:   os.Exit(1)
来源：http://hz.daria6918.cn/gtsjmothkq.html

Ruby: exit 1
来源：http://hz.cashguo.top/gtqaknmyri.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yj20258.top/gtwsymbwee.html

[M06] 向标准错误输出
来源：http://hz.shanyushiyangkeji.top/gtvcmtjzoq.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhongyouzk.top/gthhxkwrca.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.quarkkingdee.top/gtzzqoskbr.html

JS:   console.error("err")
来源：http://hz.svipenyu.cn/gtzbbpgklw.html

TS:   console.error("err")
来源：http://hz.ivvv.top/gtxkycszhn.html

Java: System.err.println("err")
来源：http://hz.iojbl.cn/gtbaimnmdh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhengqikj.top/gteejevvcy.html

Ruby: warn "err"
来源：http://hz.gotoacloud.top/gtondodaom.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.pengpengdd.cyou/gtlykspkqh.html

[M07] 判断是否为主入口
来源：http://hz.cqqwz.cn/gtjomhrluw.html

Py:   if __name__ == "__main__":
来源：http://hz.bjfxy.top/gtqzfbpnsq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cqqwz.cn/gtnscprfap.html

JS:   require.main === module
来源：http://hz.gotoacloud.top/gtncbffnkh.html

TS:   require.main === module
来源：http://hz.9152youxi.cn/gtpbsndihi.html

Java: public static void main(String[] args)
来源：http://hz.hysaishi.cn/gtojcfinfb.html

Go:   func main()
来源：http://hz.fengsongda.top/gtngeggjvk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinqigfzy.top/gtkjwdmtdx.html

C#:   static void Main(string[] args)
来源：http://hz.sufxvd.cn/gtimdxctaz.html

[M08] 获取系统与运行时信息
来源：http://hz.fengsongda.top/gtoycfzvhq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhongyouzk.top/gtaaiiwbmq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ydzc1.top/gtqabcador.html

JS:   process.platform;  process.version
来源：http://hz.pycfn.com/gtrhjhrcfp.html

TS:   process.platform;  process.version
来源：http://hz.yj202588.top/gtyjzqqgec.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.iojbl.cn/gtwmdzpvqg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.gogol.net.cn/gtqiingzcn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.aibaodan.cn/gtyyveqwvt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yj20258888.top/gtgpsekhjb.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtfqthedtl.html

N. 数据结构与算法
来源：http://hz.shzxlz.cn/gtlkhjgmsk.html

================================================================================
来源：http://hz.yj202588.top/gtwmsvoqff.html

[N01] 二分查找（有序数组）
来源：http://hz.zdqjudy.top/gtljiiwzct.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.316326.xyz/gtpcbddfeo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shzxlz.cn/gtlalnrrko.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cucudq.cn/gtlwjzahfk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yongpay.top/gttbyfptvq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.kuanghao11.cn/gtxmplebou.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.52xcode.cn/gtiuplgcfk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.c1oappe.top/gtubmmxktj.html


<!-- 参考信息 -->