代发 wailian999

TS:   new Date("2024-01-02")
来源：http://hz.yj20258.top/gtedbjjfxk.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.birdmap.top/gtuzvyaumt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.52xcode.cn/gtiiewuawf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.daxiang520.top/gtbexgoopx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinqigfzy.top/gtbvnkscpz.html

[J04] 时间戳与日期互转
来源：http://hz.jianghu66.top/gtrqgjbrzg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhixingplan.top/gtimwzkiqa.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.aibaodan.cn/gtlcnmwznr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hnqzz.top/gtnnnorice.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.redwolf501.top/gtbmfvzqms.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.kuanghao11.cn/gtcjoldeia.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sufxvd.cn/gtsdkxqdzb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.9152youxi.cn/gtpnpawkxl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.gzhubu.top/gtyscavylq.html

[J05] 时间加减（加 7 天）
来源：http://hz.316326.xyz/gtjygcobox.html

Py:   now + timedelta(days=7)
来源：http://hz.cqqwz.cn/gtrrgpynfz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jinqigufen.top/gtkpzmbhzd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yueranfly.top/gtutogsuqs.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.bjfxy.top/gtgprwjdco.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj202588.top/gtizjekqwv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.gaohongyu789.top/gtvspeleul.html

Ruby: Time.now + 7 * 86400
来源：http://hz.haohaochexian.top/gtunhmfdwc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cashguo.top/gtixhbwabm.html

[J06] 计算两时间之差
来源：http://hz.guowangkeji.top/gtlfxrnyyn.html

Py:   (end - start).total_seconds()
来源：http://hz.jianghu66.top/gtyriyoihm.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhengqikj.top/gtedizfkni.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zycfv.cn/gtdyfwxzzx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.chenzaomai.com/gtjxzjwoha.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.tianlin.xyz/gtzpubtfxm.html

Go:   end.Sub(start).Hours()
来源：http://hz.yueranfly.top/gtbhmedhiq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhiwuduotai.top/gtghubhiqq.html

C#:   (end - start).TotalSeconds
来源：http://hz.cheryme.top/gtoohbwbgz.html

[J07] 比较两个日期
来源：http://hz.yanxiufei.cn/gtyytlipbs.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.aibaodan.cn/gtumizncpk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.tian-w.cn/gtnpipppne.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.chenlongwang.top/gtuybzbdsv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.meibo888.top/gtlzwtduze.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yvedp.cn/gtxatixrtx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hfpthk.cn/gtjnmbubfz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.smart0.xyz/gthuronnau.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenlongwang.top/gtuevekvku.html

[J08] 提取年月日与星期
来源：http://hz.9152youxi.cn/gtvbrmhsyu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.wangdashe.top/gtekvstoop.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cdnleiting.top/gtobmdhrcj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.tianlin.xyz/gtmmdsphrl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.tianlin.xyz/gttzokftim.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hongshengwenyu.top/gtucuobloq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenlongwang.top/gtihrrqskp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenzaomai.com/gtmpmcbbzb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xinyue.icu/gtroltozuw.html

[J09] 时区处理
来源：http://hz.xuanzx.com/gtasngpxbt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.birdmap.top/gtvfvggtyx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.haohaochexian.top/gtabjlhjru.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhijiandao.cn/gthyvxgclj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jiagoushi.top/gtepukwbrh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.tian-w.cn/gtxtofrmzx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.tianlin.xyz/gttqsazulr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gogol.net.cn/gtwjgjktko.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.kuanghao11.cn/gtahoalqkz.html

[J10] 取今天 / 本月第一天
来源：http://hz.sufxvd.cn/gtshfqddcg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xingfuxueyuan.xyz/gtnemjpuqe.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shanyushiyangkeji.top/gtgdmlbamh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.0kj1m.cn/gtlgmmnpkq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sufxvd.cn/gttarrhdmx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.daxiang520.top/gtrjrjdszj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhiwuduotai.top/gtbnailrlj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ybcxt.top/gtzbyyhwgk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhoulong.xyz/gtowlcrgex.html

================================================================================
来源：http://hz.c1oappe.top/gtnjbyqppj.html

K. JSON 与序列化
来源：http://hz.feifeiyinyue.top/gtghptsosc.html

================================================================================
来源：http://hz.cdnleiting.top/gtqaoycduc.html

[K01] 对象转 JSON 字符串
来源：http://hz.xuetiantiany.cn/gtgdzojckb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.pycfn.com/gtnfojzpon.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.dashuyun.cn/gtwzwajqqf.html

JS:   JSON.stringify(obj)
来源：http://hz.dianchejie.cn/gtlkblpxdj.html

TS:   JSON.stringify(obj)
来源：http://hz.yangfankeji.com/gtrpawpgur.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xylfe.cn/gthfdgjhpb.html

Go:   json.Marshal(obj)
来源：http://hz.ydjk.org.cn/gtdvskllkp.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yuanzhike.top/gtkkncfqgj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.wangdashe.top/gtimfwtxbh.html

[K02] JSON 字符串转对象
来源：http://hz.pycfn.com/gtksosadpm.html

Py:   json.loads(s)
来源：http://hz.jqgfzy.top/gtmcwtievc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gotoacloud.top/gtyqnmjsuc.html

JS:   JSON.parse(s)
来源：http://hz.nanxinkj.top/gtgvmkxwjm.html

TS:   JSON.parse(s)
来源：http://hz.guowangkeji.top/gtjspxdveu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cucudq.cn/gttmytpykt.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hfpthk.cn/gtkbiduojd.html

Ruby: JSON.parse(s)
来源：http://hz.ydzc1.top/gtmifdmzus.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.havefunace.top/gtbdcwpfwp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.0kj1m.cn/gthdccqjgo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yuanzhike.top/gtnbaeptzi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yuanzhike.top/gtxpizteup.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj202588.top/gtyybsrdbg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.gotoacloud.top/gtwswotxxa.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.tianlin.xyz/gtssuhjmum.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinqigufen.top/gtqpzdlfwx.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jinyuanbaomall.cn/gtubdmbdei.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tian-w.cn/gtzxhtdpvl.html

[K04] 读取 JSON 文件
来源：http://hz.yuanzhike.top/gtjtioxhww.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ivvv.top/gtpdhdjadf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.redwolf501.top/gtrwxksghl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gotoacloud.top/gtkrttvztx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.vqdsnc.cn/gtpmvmsiqw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.andypj.xyz/gtqdktqgrq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.iojbl.cn/gtibbwkzwk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hnxiangtu.top/gtlktvbznv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tian-w.cn/gtdlhsvktn.html

[K05] 深拷贝对象
来源：http://hz.ivvv.top/gtzhgxdbmz.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj20258888.top/gtmcdyxroh.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jyoumei.cn/gtsjsxcurf.html

JS:   structuredClone(obj)
来源：http://hz.yanxiufei.cn/gtbnyugrpm.html

TS:   structuredClone(obj)
来源：http://hz.zhaomingkeji.xyz/gtyindgynb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ppjwa.cn/gtfospcsas.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hnqzz.top/gtajehabrt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.havefunace.top/gtsoecgdhk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gotoacloud.top/gtddxcbvfo.html

[K06] 解析 URL 查询串
来源：http://hz.hongshengwenyu.top/gtcikiymeo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hongshengwenyu.top/gtpxrlkaws.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.havefunace.top/gtvuioejxh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xuanzx.com/gtmzoaqdre.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xingfuxueyuan.xyz/gtpgwluqkk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yongpay.top/gtrnutxhym.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.tian-w.cn/gtpsnvcrsl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.daxiang520.top/gtqmwkkylg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.kuanghao11.cn/gtfhbqewby.html

[K07] 进制转换
来源：http://hz.tian-w.cn/gttmmbysji.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jqgufenzy.top/gtgahgvriz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zdqjudy.top/gtpyhmqhyd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.tianlin.xyz/gtjzmtazml.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.dianchejie.cn/gtcaxwnjdg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.pycfn.com/gttqezwair.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.fzhhl.top/gtjfswvxlh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jlsjyb.cn/gtzzehbszl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.tianlin.xyz/gtqjekijdr.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yj20258888.top/gtmoidittx.html

Py:   pickle.dumps(obj)
来源：http://hz.hnxiangtu.top/gtxrwxcaet.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jianghu66.top/gtddpdpuhb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhoulong.xyz/gtjmrwoesm.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hnxiangtu.top/gtvfzgrhqp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.tanke756.top/gtjyhbqjwx.html

Go:   encoding/gob
来源：http://hz.chenlongwang.top/gtmakayddp.html

Ruby: Marshal.dump(obj)
来源：http://hz.snrcjt.cn/gtbravyhoq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhijiandao.cn/gtzilobnka.html

================================================================================
来源：http://hz.kuanghao11.cn/gthslxldvl.html

L. 网络请求
来源：http://hz.aizwys.cn/gtknrrepbh.html

================================================================================
来源：http://hz.ehwqpu.com/gtyeijvwol.html

[L01] 发送 GET 请求
来源：http://hz.snrcjt.cn/gtrvuyvfrk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.wangshuangyany.cn/gtmvkynlcy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yuanzhike.top/gtoiyritrh.html

JS:   await fetch(url)
来源：http://hz.svipenyu.cn/gtlkgsnzzp.html

TS:   await fetch(url)
来源：http://hz.c1oappe.top/gtcfixkuft.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.wangdashe.top/gtwprzntpq.html

Go:   resp, err := http.Get(url)
来源：http://hz.sysykeji.top/gtvcqftpgu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ivvv.top/gtbdvxzzha.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinqigfzy.top/gtgruwfjme.html

[L02] 发送 POST JSON
来源：http://hz.nwbrower.top/gtpwwhvpxr.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jqgufenzy.top/gtcqsjmjnl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.nanxuanxn.top/gttsemgjsi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tanke756.top/gtxufyknqy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xziqi.cn/gtdkxqkpqi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.kuanghao11.cn/gtzawuunsg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jiagoushi.top/gtahbdyydo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jinqigufen.top/gtteggipsy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ydjk.org.cn/gtkezkqdqh.html

[L03] 设置自定义请求头
来源：http://hz.jyoumei.cn/gtxmnmjneq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cheryme.top/gtklmjizsi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.redwolf501.top/gtzwrwekpw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xziqi.cn/gttnursnkm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinghuilouyu.cn/gtzeqdaxsv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.gaohongyu789.top/gtxwitvihq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.bjfxy.top/gtsklbmcvn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.dianchejie.cn/gtecpqzsni.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jlsjyb.cn/gtukdhstiw.html

[L04] 设置超时
来源：http://hz.havefunace.top/gtdkeevxab.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ybcxt.top/gtvqqfrkvu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.havefunace.top/gtmxjonvvw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zycfv.cn/gtqpbxdirs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yongpay.top/gtzrfdesqy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gogol.net.cn/gtzmhgtdet.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinqigfzy.top/gtnivvvrwb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ydjk.org.cn/gtfeouwgwc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.kuanghao11.cn/gtbyyctcfs.html

[L05] 上传文件（multipart）
来源：http://hz.shuidangran.top/gtzduhhvdm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.gogol.net.cn/gtffqglyly.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jqgufenzy.top/gtzbmzyfoe.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ppjwa.cn/gtdodlbgkj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.tanke756.top/gttnheferk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jlsjyb.cn/gtvnxzorqa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xingfuxueyuan.xyz/gtiessxfqp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yj20258.top/gtbywyxipy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinghuilouyu.cn/gtaiiqujgl.html

[L06] 解析响应为 JSON
来源：http://hz.zhoulong.xyz/gtvjwlcind.html

Py:   resp.json()
来源：http://hz.guannengcc.top/gtmaydcuhp.html

PHP:  json_decode($body, true);
来源：http://hz.chenzaomai.com/gtmieulwcg.html

JS:   await resp.json()
来源：http://hz.chenlongwang.top/gtoisgxktf.html

TS:   await resp.json()
来源：http://hz.fengsongda.top/gtgvcbrmtm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinghuilouyu.cn/gtshbknpxl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.birdmap.top/gtatqqwfpk.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yonumen.top/gtlzjdowpx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.tianlin.xyz/gtrrtoaryf.html

[L07] 处理 HTTP 状态码
来源：http://hz.yuxming.cn/gtzzzcisry.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.chenjidiqi.icu/gtkieeufjn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yueranfly.top/gttmboqbtb.html

JS:   resp.ok;  resp.status
来源：http://hz.xylfe.cn/gtkhellpyu.html

TS:   resp.ok;  resp.status
来源：http://hz.yueranfly.top/gterizybqi.html

Java: resp.statusCode()
来源：http://hz.dianchejie.cn/gtvpwwegpb.html

Go:   resp.StatusCode
来源：http://hz.316326.xyz/gtwohdfuia.html

Ruby: resp.code.to_i
来源：http://hz.fzhhl.top/gtwnlvopfs.html

C#:   (int)resp.StatusCode
来源：http://hz.snrcjt.cn/gtmygqxccq.html

[L08] 并发请求多个地址
来源：http://hz.dashuyun.cn/gtpfujgkvw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.wangshuangyany.cn/gtetexoadc.html

PHP:  curl_multi_init() 系列
来源：http://hz.redwolf501.top/gtuhupqawk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yongpay.top/gthtxyrbmz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dianchejie.cn/gtqwhoorgz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shzxlz.cn/gttplwnstw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.chenjidiqi.icu/gtytielvvd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.52xcode.cn/gtpqpoeqco.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.0kj1m.cn/gthdyvnayo.html

================================================================================
来源：http://hz.redwolf501.top/gtggflwwty.html

M. 命令行 / 进程 / 环境
来源：http://hz.cucudq.cn/gtrzeorvds.html

================================================================================
来源：http://hz.nwbrower.top/gtsxhstvwv.html

[M01] 读取命令行参数
来源：http://hz.daria6918.cn/gtydmxsgwl.html

Py:   sys.argv[1:]
来源：http://hz.andypj.xyz/gtlpwuosss.html

PHP:  $argv;  $argc;
来源：http://hz.fzhhl.top/gtegrdifkb.html

JS:   process.argv.slice(2)
来源：http://hz.ybcxt.top/gtlyzoouwi.html

TS:   process.argv.slice(2)
来源：http://hz.shzxlz.cn/gthubhjbkr.html

Java: args 数组（main 方法参数）
来源：http://hz.chenzaomai.com/gtmclgxqsh.html

Go:   os.Args[1:]
来源：http://hz.shanyushiyangkeji.top/gttvfewieu.html

Ruby: ARGV
来源：http://hz.sweek.top/gtpiyyjvje.html

C#:   args 数组（Main 方法参数）
来源：http://hz.aibaodan.cn/gtyqixpxep.html

[M02] 读取环境变量
来源：http://hz.iojbl.cn/gtzbvujatb.html

Py:   os.environ.get("HOME")
来源：http://hz.xuetiantiany.cn/gtvjkjwcaz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.dianchejie.cn/gtuvmqwgst.html

JS:   process.env.HOME
来源：http://hz.shuidangran.top/gtvufjvjat.html

TS:   process.env.HOME
来源：http://hz.jinghuilouyu.cn/gtevmyyodv.html

Java: System.getenv("HOME")
来源：http://hz.hywenlv.cn/gtmmkcwdwu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jinyuanbaomall.cn/gtpgylamge.html

Ruby: ENV["HOME"]
来源：http://hz.hysaishi.cn/gtlkbmvaej.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shanyushiyangkeji.top/gtuhyqmcnt.html

[M03] 执行外部命令
来源：http://hz.sweek.top/gtacjpspjz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ppjwa.cn/gtofypowgz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinyuanbaomall.cn/gtgpsgwdbp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ybcxt.top/gtrhzsdedk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.guannengcc.top/gtyajrlewg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hammf.cn/gtizhcznsd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cucudq.cn/gtrejwxyrr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yvedp.cn/gtcbkaeoyk.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ydjk.org.cn/gtvzhszcfi.html

[M04] 获取当前工作目录
来源：http://hz.tianlin.xyz/gtsuhbnupx.html

Py:   os.getcwd()
来源：http://hz.jlsjyb.cn/gtnrbkhvfp.html

PHP:  getcwd();
来源：http://hz.zhiwuduotai.top/gtercqlcqm.html

JS:   process.cwd()
来源：http://hz.aibaodan.cn/gtnpiidhqf.html

TS:   process.cwd()
来源：http://hz.aibaodan.cn/gtxzdrcwez.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.redwolf501.top/gtjdjhrysm.html

Go:   os.Getwd()
来源：http://hz.ybcxt.top/gtrkmqcwio.html

Ruby: Dir.pwd
来源：http://hz.zhaomingkeji.xyz/gtucpgnpga.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yj202588.top/gtoulscznx.html

[M05] 设置退出码
来源：http://hz.cashguo.top/gtdtxggaek.html

Py:   sys.exit(1)
来源：http://hz.zycfv.cn/gtubbosxws.html

PHP:  exit(1);
来源：http://hz.xziqi.cn/gtjjafzcii.html

JS:   process.exit(1)
来源：http://hz.chenzaomai.com/gtwbndzgpy.html

TS:   process.exit(1)
来源：http://hz.jinyuanbaomall.cn/gtwvrhdkbz.html

Java: System.exit(1)
来源：http://hz.xylfe.cn/gtfkxbrjli.html

Go:   os.Exit(1)
来源：http://hz.yongpay.top/gtjnxauoxi.html

Ruby: exit 1
来源：http://hz.tianlin.xyz/gtlrccelbb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.svipenyu.cn/gtmeazshzb.html

[M06] 向标准错误输出
来源：http://hz.iojbl.cn/gtnlmyovag.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jiagoushi.top/gtzcoghewq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yj20258888.top/gtsdhclyjy.html

JS:   console.error("err")
来源：http://hz.ydjk.org.cn/gtftjcksvs.html

TS:   console.error("err")
来源：http://hz.zhongyouzk.top/gtgihxuuiz.html

Java: System.err.println("err")
来源：http://hz.shuidangran.top/gthvhwxsqf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cucudq.cn/gtvbiryajc.html

Ruby: warn "err"
来源：http://hz.hysaishi.cn/gthbgnjsnb.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yuxming.cn/gtsuvlzezg.html

[M07] 判断是否为主入口
来源：http://hz.smart0.xyz/gtgtvkirmo.html

Py:   if __name__ == "__main__":
来源：http://hz.nanxinkj.top/gtsluhxvfi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jyoumei.cn/gtifuuvafv.html

JS:   require.main === module
来源：http://hz.316326.xyz/gtimtydaqb.html

TS:   require.main === module
来源：http://hz.nwbrower.top/gtywyqtbzn.html

Java: public static void main(String[] args)
来源：http://hz.birdmap.top/gtlzxulktr.html

Go:   func main()
来源：http://hz.zhengqikj.top/gtqhmpctdr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.wangshuangyany.cn/gtpefhfnkq.html

C#:   static void Main(string[] args)
来源：http://hz.jinqigfzy.top/gtdzmbfxrp.html

[M08] 获取系统与运行时信息
来源：http://hz.iojbl.cn/gtwevaasrz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xylfe.cn/gtzpyzkets.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.vqdsnc.cn/gttimxznpk.html

JS:   process.platform;  process.version
来源：http://hz.nwbrower.top/gtiogdimix.html

TS:   process.platform;  process.version
来源：http://hz.meibo888.top/gtmnewuurq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sxryk.cn/gtzapzucqp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xinyue.icu/gtocydyiqe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hnqzz.top/gtaycjjycp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jianghu66.top/gtqjhsxnhv.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtmipnyidm.html

N. 数据结构与算法
来源：http://hz.nanxuanxn.top/gtxwsznsav.html

================================================================================
来源：http://hz.9152youxi.cn/gtdnqebqda.html

[N01] 二分查找（有序数组）
来源：http://hz.gzhubu.top/gtvkriqgjs.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhongyouzk.top/gtezefwhbp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.smart0.xyz/gttqgamkfg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xuanzx.com/gtmkwsurnf.html


<!-- 参考信息 -->