代发 wailian999

TS:   new Date("2024-01-02")
来源：http://hz.tanke756.top/gtucgyiiht.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ydzc1.top/gtrxvijbjx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.c1oappe.top/gtjuqotpfv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.smart0.xyz/gtslmoucuw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jiagoushi.top/gtvtvvvsei.html

[J04] 时间戳与日期互转
来源：http://hz.yanxiufei.cn/gtcbxdrxft.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jyoumei.cn/gtzygvwhxz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sysykeji.top/gtiabllymm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.daria6918.cn/gtripawdho.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nanxinkj.top/gtwukojstu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hnqzz.top/gtklzvxgbx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nwbrower.top/gtpaabhtqc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.chenjidiqi.icu/gtimncygzq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.andypj.xyz/gtzjcjahvm.html

[J05] 时间加减（加 7 天）
来源：http://hz.ppjwa.cn/gtkwswqdyh.html

Py:   now + timedelta(days=7)
来源：http://hz.hnxiangtu.top/gtnwmggxhl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.chenjidiqi.icu/gtoxnoqrxh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.0kj1m.cn/gtmnruwkoi.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhijiandao.cn/gtkutzjshp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.52xcode.cn/gtjlytgxcc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.c1oappe.top/gtwiepzosi.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jiagoushi.top/gtuxkgifrp.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jianghu66.top/gtbhuwgedf.html

[J06] 计算两时间之差
来源：http://hz.wangshuangyany.cn/gtibmcvtla.html

Py:   (end - start).total_seconds()
来源：http://hz.zycfv.cn/gtpyrqcxuq.html

PHP:  $end->diff($start)->days;
来源：http://hz.tianlin.xyz/gtlhmjglhu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jianghu66.top/gtczchbraz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.dashuyun.cn/gtywmqthqe.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.sxryk.cn/gtlqqpljpt.html

Go:   end.Sub(start).Hours()
来源：http://hz.yangfankeji.com/gtmqcyiunu.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jqgufenzy.top/gtjvyyuarz.html

C#:   (end - start).TotalSeconds
来源：http://hz.sufxvd.cn/gtycquecsq.html

[J07] 比较两个日期
来源：http://hz.jinqigfzy.top/gtkhilriyq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhixingplan.top/gtdegpprrx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xylfe.cn/gtwsrijwuv.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.birdmap.top/gtqvgxucyv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xziqi.cn/gtzmyspmha.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hnxiangtu.top/gtujnrltzu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ivvv.top/gtjcltfbgx.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.52xcode.cn/gtrotcxeby.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yanxiufei.cn/gtgnssyqdf.html

[J08] 提取年月日与星期
来源：http://hz.nanxuanxn.top/gtiwzknnxi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.gogol.net.cn/gtwafoveth.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.gogol.net.cn/gthwtnbypy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hywenlv.cn/gtwcjmdavb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhijiandao.cn/gthsqghrkn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ydjk.org.cn/gtcjvyydlm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhongyouzk.top/gtikvaxzkw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yj20258888.top/gtcvfgbmiv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.pengpengdd.cyou/gtlogiahnd.html

[J09] 时区处理
来源：http://hz.jlsjyb.cn/gtgivalbwc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gaohongyu789.top/gtyhtepgps.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.smart0.xyz/gttotrpptl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cashguo.top/gtpfvcciya.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jianghu66.top/gthxhxrpfj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhijiandao.cn/gtbkmxfwrx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yongpay.top/gtygqvqava.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hfpthk.cn/gtuecxeblk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.mhx1999.top/gtryyxutoo.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhongyouzk.top/gtcvwtusxq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.wangshuangyany.cn/gtwjggwbub.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.snrcjt.cn/gtjirdicck.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.kuanghao11.cn/gtmusepljb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cdnleiting.top/gtqhmfefvx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yuxming.cn/gtvpxrfqeb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jyoumei.cn/gtalipvhhu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ybcxt.top/gtujriugmm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yangfankeji.com/gtxjdcghig.html

================================================================================
来源：http://hz.cucudq.cn/gtvowrnpjb.html

K. JSON 与序列化
来源：http://hz.kuanghao11.cn/gtwarmzegy.html

================================================================================
来源：http://hz.gogol.net.cn/gtgvijfbxn.html

[K01] 对象转 JSON 字符串
来源：http://hz.shangyingyoupin.top/gtqgqeysra.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hysaishi.cn/gtxotsjben.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yanxiufei.cn/gthogmacqh.html

JS:   JSON.stringify(obj)
来源：http://hz.gotoacloud.top/gtzogblsda.html

TS:   JSON.stringify(obj)
来源：http://hz.yuxming.cn/gtzttofkjx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.guowangkeji.top/gtupwyqben.html

Go:   json.Marshal(obj)
来源：http://hz.jqgufenzy.top/gtbkkqxthl.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.wangshuangyany.cn/gtikxqlqub.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.gaohongyu789.top/gtxgzmeyqd.html

[K02] JSON 字符串转对象
来源：http://hz.kuanghao11.cn/gthcdgbgni.html

Py:   json.loads(s)
来源：http://hz.feifeiyinyue.top/gtyiraeozr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yanxiufei.cn/gtpunaxnoj.html

JS:   JSON.parse(s)
来源：http://hz.cdnleiting.top/gtuuiyxadt.html

TS:   JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtdeivclwt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yj20258888.top/gtrrblknlr.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.mhx1999.top/gtjlidmxlc.html

Ruby: JSON.parse(s)
来源：http://hz.zhoulong.xyz/gtyiqzkelq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.smart0.xyz/gtxvlxsmhc.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ivvv.top/gtozlipzns.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xylfe.cn/gtjijypgyt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jianghu66.top/gtmlrloibg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.svipenyu.cn/gtnjdorovf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xylfe.cn/gtsbovfjir.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cashguo.top/gtpgksahhb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.meibo888.top/gtdegiyoue.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jinqigufen.top/gtjrspjpdt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.vqdsnc.cn/gtylsjwiyv.html

[K04] 读取 JSON 文件
来源：http://hz.ehwqpu.com/gtnemwexqm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ydzc1.top/gtqzfbvsft.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.316326.xyz/gtqagscyrc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.pycfn.com/gthcrccatg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhixingplan.top/gtdfddjwfx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jlsjyb.cn/gtymczgtyh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xziqi.cn/gtaffsyywp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ybcxt.top/gttoudexwm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.fzhhl.top/gtjjztwxnd.html

[K05] 深拷贝对象
来源：http://hz.jiagoushi.top/gtbwkjlolj.html

Py:   copy.deepcopy(obj)
来源：http://hz.mhx1999.top/gtfzsyotqa.html

PHP:  unserialize(serialize($obj));
来源：http://hz.tianlin.xyz/gtovnigsmo.html

JS:   structuredClone(obj)
来源：http://hz.tanke756.top/gtpmzviuek.html

TS:   structuredClone(obj)
来源：http://hz.hysaishi.cn/gthuaabaqc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.9152youxi.cn/gtmpqydfpv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hnqzz.top/gtydxkiuvs.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.tian-w.cn/gtdikfjifv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.mhx1999.top/gtmlqywrwy.html

[K06] 解析 URL 查询串
来源：http://hz.zhengqikj.top/gtmouwpkmy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hammf.cn/gtuyxmgpcr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ehwqpu.com/gtwhgrrnrt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhoulong.xyz/gtdebvvvbr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.daxiang520.top/gtywhctnwp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xuetiantiany.cn/gtmsaaeqjq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.aibaodan.cn/gtbsparqtv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ivvv.top/gtagwpawav.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shzxlz.cn/gtwhckvlex.html

[K07] 进制转换
来源：http://hz.sufxvd.cn/gtndcttfjz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.52xcode.cn/gtlkqvqqvl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.nanxinkj.top/gtcsorzkuk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ydjk.org.cn/gtksaahiwb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtxulrvxps.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shangyingyoupin.top/gtarauljhn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhaomingkeji.xyz/gtoglltcgn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.316326.xyz/gtjcfmmeaq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.cheryme.top/gtjgggdtwz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.svipenyu.cn/gtdcbzocpm.html

Py:   pickle.dumps(obj)
来源：http://hz.daria6918.cn/gtstbqsvjj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.52xcode.cn/gtgdckhpow.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cqqwz.cn/gttkxkzbjp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gogol.net.cn/gtgxufzviz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xylfe.cn/gtctnouqst.html

Go:   encoding/gob
来源：http://hz.snrcjt.cn/gtqbumnzvz.html

Ruby: Marshal.dump(obj)
来源：http://hz.shanyushiyangkeji.top/gttddatijc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhoulong.xyz/gtebsfyuwi.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtvhqcabcb.html

L. 网络请求
来源：http://hz.yonumen.top/gtskfihpjh.html

================================================================================
来源：http://hz.daxiang520.top/gtkcitmqvg.html

[L01] 发送 GET 请求
来源：http://hz.cqqwz.cn/gtnbzxqtda.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hnxiangtu.top/gtthqtzoue.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.bjfxy.top/gtkvbvdasa.html

JS:   await fetch(url)
来源：http://hz.jinyuanbaomall.cn/gthhbladcx.html

TS:   await fetch(url)
来源：http://hz.shangyingyoupin.top/gtqkkqshvp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yongpay.top/gtosykpwwx.html

Go:   resp, err := http.Get(url)
来源：http://hz.tianlin.xyz/gtjmumhklt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ywan-chungtsiang.top/gtyjfzgvcd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.dashuyun.cn/gtcpfeqrbx.html

[L02] 发送 POST JSON
来源：http://hz.jinghuilouyu.cn/gtpftliksi.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cucudq.cn/gttqhqyxoq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.wangdashe.top/gtnrpcbwki.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.iojbl.cn/gtaifuhbiq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ywan-chungtsiang.top/gtbigjarzb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hammf.cn/gtlehhcaws.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yueranfly.top/gtrpzhxpse.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.nanxuanxn.top/gtmkqtzacn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.meibo888.top/gtcudjsguz.html

[L03] 设置自定义请求头
来源：http://hz.snrcjt.cn/gtvmsijhqr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhiwuduotai.top/gtxunzrkmh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.bjfxy.top/gtubjhbplp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yvedp.cn/gtrzdzlwkc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.pengpengdd.cyou/gtqnvbcdkq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hfpthk.cn/gtlmbitcxz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shuidangran.top/gtmdztejhc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sysykeji.top/gtqeusllhy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.daxiang520.top/gtbyfpyuyv.html

[L04] 设置超时
来源：http://hz.xuetiantiany.cn/gtfxqoskqb.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xylfe.cn/gtzoqyxtur.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.shanyushiyangkeji.top/gtwhwszkmz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.feifeiyinyue.top/gtytcxgefz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gotoacloud.top/gtsezpnxsj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ydzc1.top/gtxclaywma.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.pengpengdd.cyou/gtchkbybwz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cqqwz.cn/gtgrjfcgnz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.dianchejie.cn/gtwebowzfb.html

[L05] 上传文件（multipart）
来源：http://hz.zhixingplan.top/gtpfylpksh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.svipenyu.cn/gtywzkpohv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yj20258.top/gtfvczfxap.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shzxlz.cn/gtbicufqwu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhengqikj.top/gthnqkxeqt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.daxiang520.top/gtimqivohn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ydzc1.top/gtbfaimfix.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cashguo.top/gtukzthdqd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.dianchejie.cn/gtkisezyca.html

[L06] 解析响应为 JSON
来源：http://hz.yuanzhike.top/gtmleiazdh.html

Py:   resp.json()
来源：http://hz.sysykeji.top/gtrixeodzg.html

PHP:  json_decode($body, true);
来源：http://hz.haohaochexian.top/gtuopeokzs.html

JS:   await resp.json()
来源：http://hz.xziqi.cn/gtivunosii.html

TS:   await resp.json()
来源：http://hz.zhijiandao.cn/gtglxhfrnm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.dashuyun.cn/gtruvwxhpj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jiagoushi.top/gtmbcxoxhq.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yuxming.cn/gtemoqcfnx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hywenlv.cn/gtjxqrgjxb.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinghuilouyu.cn/gtacqafxpq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shanyushiyangkeji.top/gtkwkhvsjc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.gotoacloud.top/gtdoypinkq.html

JS:   resp.ok;  resp.status
来源：http://hz.andypj.xyz/gtbdycswgo.html

TS:   resp.ok;  resp.status
来源：http://hz.xziqi.cn/gtgdtivehn.html

Java: resp.statusCode()
来源：http://hz.jinyuanbaomall.cn/gtmffuhqzq.html

Go:   resp.StatusCode
来源：http://hz.shangyingyoupin.top/gtyohmthzj.html

Ruby: resp.code.to_i
来源：http://hz.shzxlz.cn/gtqwjdjisy.html

C#:   (int)resp.StatusCode
来源：http://hz.jinqigfzy.top/gtpcnlbmpt.html

[L08] 并发请求多个地址
来源：http://hz.xuanzx.com/gtjmkijwms.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.shuidangran.top/gtmivrbikz.html

PHP:  curl_multi_init() 系列
来源：http://hz.guowangkeji.top/gtizavdlir.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.iojbl.cn/gtugvqjrxk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangkeji.top/gtjmbvjaku.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinyuanbaomall.cn/gttvgncsbp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zycfv.cn/gtuvkompwg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.nanxuanxn.top/gtzniuqtyt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.tian-w.cn/gtmfgmexax.html

================================================================================
来源：http://hz.fzhhl.top/gtrqvymyul.html

M. 命令行 / 进程 / 环境
来源：http://hz.xinyue.icu/gtftcikeqv.html

================================================================================
来源：http://hz.ivvv.top/gtobqbegvd.html

[M01] 读取命令行参数
来源：http://hz.wangshuangyany.cn/gtomtjndrv.html

Py:   sys.argv[1:]
来源：http://hz.shanyushiyangkeji.top/gtzchxstei.html

PHP:  $argv;  $argc;
来源：http://hz.andypj.xyz/gtwvaqmdbj.html

JS:   process.argv.slice(2)
来源：http://hz.xinyue.icu/gtcfkeonpn.html

TS:   process.argv.slice(2)
来源：http://hz.yvedp.cn/gtoojjwppi.html

Java: args 数组（main 方法参数）
来源：http://hz.yj20258888.top/gtxeqtsmtw.html

Go:   os.Args[1:]
来源：http://hz.52xcode.cn/gttjexunwr.html

Ruby: ARGV
来源：http://hz.pycfn.com/gtuflgnkoh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yueranfly.top/gtvzmuxmbq.html

[M02] 读取环境变量
来源：http://hz.svipenyu.cn/gtiuyontrk.html

Py:   os.environ.get("HOME")
来源：http://hz.guowangkeji.top/gtrjfueagz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.daria6918.cn/gtloebiaxq.html

JS:   process.env.HOME
来源：http://hz.sufxvd.cn/gtwgsncvpf.html

TS:   process.env.HOME
来源：http://hz.cdnleiting.top/gtfoqkvuzp.html

Java: System.getenv("HOME")
来源：http://hz.shzxlz.cn/gtrcacthmm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jianghu66.top/gtdbqrpkio.html

Ruby: ENV["HOME"]
来源：http://hz.bjfxy.top/gtpfeipxwh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.52xcode.cn/gtlbvmvbpi.html

[M03] 执行外部命令
来源：http://hz.yuanzhike.top/gtqplxcpen.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.fzhhl.top/gtngkksewx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhengqikj.top/gtmjjznhab.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.gotoacloud.top/gtralkjbif.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhengqikj.top/gtybtjybbu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.wangshuangyany.cn/gtrsnlzsdh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.0kj1m.cn/gtghqerwcw.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jqgufenzy.top/gttukdjfrg.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cdnleiting.top/gtsosviirz.html

[M04] 获取当前工作目录
来源：http://hz.yueranfly.top/gtrvckraxb.html

Py:   os.getcwd()
来源：http://hz.yj20258.top/gtdpscichu.html

PHP:  getcwd();
来源：http://hz.wangdashe.top/gtbrgszuuv.html

JS:   process.cwd()
来源：http://hz.tanke756.top/gtguwnahyn.html

TS:   process.cwd()
来源：http://hz.52xcode.cn/gtbykzgdhq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.pycfn.com/gtiqknowcj.html

Go:   os.Getwd()
来源：http://hz.jiagoushi.top/gtoqezjvtc.html

Ruby: Dir.pwd
来源：http://hz.xinyue.icu/gtxcmyetgb.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.chenjidiqi.icu/gtqwrtmmdk.html

[M05] 设置退出码
来源：http://hz.gotoacloud.top/gtobnraicf.html

Py:   sys.exit(1)
来源：http://hz.shanyushiyangkeji.top/gttkcjbzgt.html

PHP:  exit(1);
来源：http://hz.cqqwz.cn/gtxcuwrfhp.html

JS:   process.exit(1)
来源：http://hz.xinyue.icu/gtfgcqhibi.html

TS:   process.exit(1)
来源：http://hz.0kj1m.cn/gthdfolbqn.html

Java: System.exit(1)
来源：http://hz.aibaodan.cn/gtrqkzqtub.html

Go:   os.Exit(1)
来源：http://hz.bjfxy.top/gtgiuvlygd.html

Ruby: exit 1
来源：http://hz.zhengqikj.top/gtavxephmi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.guowangkeji.top/gtyfchpksl.html

[M06] 向标准错误输出
来源：http://hz.daria6918.cn/gtveubgkkm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.kuanghao11.cn/gtvjyuprhq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.pycfn.com/gtswnqchsg.html

JS:   console.error("err")
来源：http://hz.ybcxt.top/gtprshmsvq.html

TS:   console.error("err")
来源：http://hz.meibo888.top/gtnpkvimjr.html

Java: System.err.println("err")
来源：http://hz.gogol.net.cn/gtdorkrdon.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xuetiantiany.cn/gtwrfxqyvc.html

Ruby: warn "err"
来源：http://hz.ydzc1.top/gtzliwmvom.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ppjwa.cn/gtdubztjyv.html

[M07] 判断是否为主入口
来源：http://hz.dianchejie.cn/gttvdzspwf.html

Py:   if __name__ == "__main__":
来源：http://hz.zhongyouzk.top/gtusgjprmf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jinqigufen.top/gttvwkeyak.html

JS:   require.main === module
来源：http://hz.hywenlv.cn/gtuncdvvlt.html

TS:   require.main === module
来源：http://hz.dianchejie.cn/gtpejpvwov.html

Java: public static void main(String[] args)
来源：http://hz.svipenyu.cn/gtowebvkrg.html

Go:   func main()
来源：http://hz.yongpay.top/gtvjkdumeg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cheryme.top/gtwmnrpuoa.html

C#:   static void Main(string[] args)
来源：http://hz.hfpthk.cn/gtpacydcvz.html

[M08] 获取系统与运行时信息
来源：http://hz.redwolf501.top/gtohnbcamy.html

Py:   platform.system();  platform.python_version()
来源：http://hz.andypj.xyz/gtffznclio.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cdnleiting.top/gtubzguhdb.html

JS:   process.platform;  process.version
来源：http://hz.nanxuanxn.top/gttpzgizew.html

TS:   process.platform;  process.version
来源：http://hz.yj20258.top/gtfzqygfrj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.aizwys.cn/gtlcsdsspl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.smart0.xyz/gtkcvelesc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shuidangran.top/gtqrkzftta.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cashguo.top/gtyvgzrtfo.html

================================================================================
来源：http://hz.dashuyun.cn/gtklipflii.html

N. 数据结构与算法
来源：http://hz.ywan-chungtsiang.top/gtpgwvbhjb.html

================================================================================
来源：http://hz.ivvv.top/gtzqrqkafl.html

[N01] 二分查找（有序数组）
来源：http://hz.nanxuanxn.top/gtantbgizv.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yongpay.top/gtigrxkhok.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.haohaochexian.top/gtybxnhegn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jqgfzy.top/gttchwlgof.html


<!-- 参考信息 -->