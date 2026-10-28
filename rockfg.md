代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://hz.tian-w.cn/gtdrimgnus.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhaomingkeji.xyz/gtfkvjhnwt.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xziqi.cn/gtgiipjewi.html

C#:   (end - start).TotalSeconds
来源：http://hz.sufxvd.cn/gtrlgdahji.html

[J07] 比较两个日期
来源：http://hz.jianghu66.top/gtcvxrivgz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cucudq.cn/gtzoyoyotz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ybcxt.top/gtiqcktruk.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yonumen.top/gtbnbcscod.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shangyingyoupin.top/gtjgzrpydt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.fengsongda.top/gtdgrivudr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.smart0.xyz/gtdxwqaoeg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.havefunace.top/gttkopzxtc.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtvpaimsfi.html

[J08] 提取年月日与星期
来源：http://hz.guowangkeji.top/gtfwuoywkz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.meibo888.top/gtzjjavxdo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yangfankeji.com/gtopfxwsxh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.dashuyun.cn/gtkkyuxdhq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ppjwa.cn/gtwqjaeboj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xingfuxueyuan.xyz/gtmltlqxez.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cdnleiting.top/gtwhjrklmj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.dashuyun.cn/gtslotvkqe.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinyuanbaomall.cn/gtxoviiich.html

[J09] 时区处理
来源：http://hz.dashuyun.cn/gthecobxuu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gzhubu.top/gtcewdyhbn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ydjk.org.cn/gtvdrxvnvo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.fengsongda.top/gttualonmn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tanke756.top/gtvoqoekll.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.iojbl.cn/gtibowztpq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.iojbl.cn/gtyzwqwfdr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.nanxuanxn.top/gthrqeuuld.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.svipenyu.cn/gterwyjoyw.html

[J10] 取今天 / 本月第一天
来源：http://hz.dashuyun.cn/gtkwgxfaka.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sufxvd.cn/gtauwelftc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.dashuyun.cn/gtcnrdbtkd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.haohaochexian.top/gtqcobaavd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sysykeji.top/gtqmvmkzcd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.gotoacloud.top/gtsqvadwxh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.smart0.xyz/gtbjlmebul.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xylfe.cn/gtiplrbkdc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.0kj1m.cn/gthztsklot.html

================================================================================
来源：http://hz.jinqigfzy.top/gtqapcodfu.html

K. JSON 与序列化
来源：http://hz.dashuyun.cn/gtsempxpcm.html

================================================================================
来源：http://hz.yvedp.cn/gtqkyaqmvz.html

[K01] 对象转 JSON 字符串
来源：http://hz.c1oappe.top/gtovpcugav.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.0kj1m.cn/gtwjuwodgm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yonumen.top/gtpozxtoca.html

JS:   JSON.stringify(obj)
来源：http://hz.nanxuanxn.top/gtfiomqjhc.html

TS:   JSON.stringify(obj)
来源：http://hz.fengsongda.top/gtkmfibgob.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tianlin.xyz/gtsqiujyou.html

Go:   json.Marshal(obj)
来源：http://hz.redwolf501.top/gtutxxslhb.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhixingplan.top/gttupfwdbo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yangfankeji.com/gtyjoqjtjw.html

[K02] JSON 字符串转对象
来源：http://hz.yj20258.top/gtdanmrgmj.html

Py:   json.loads(s)
来源：http://hz.xuanzx.com/gtexorcicc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jinqigufen.top/gtgfsxycek.html

JS:   JSON.parse(s)
来源：http://hz.vqdsnc.cn/gtckgkbqzw.html

TS:   JSON.parse(s)
来源：http://hz.yongpay.top/gtqzpqbqws.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zycfv.cn/gtsptwfkib.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yuxming.cn/gtmfyxsaui.html

Ruby: JSON.parse(s)
来源：http://hz.ydzc1.top/gtkowyqcsc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yvedp.cn/gtiglupkmz.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sxryk.cn/gtmtmgwglv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xingfuxueyuan.xyz/gtskqxiiyq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ywan-chungtsiang.top/gtgckkvdvh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangkeji.top/gtrlktkokv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.52xcode.cn/gtsrogioqn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.redwolf501.top/gtzgkbncjx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cashguo.top/gtvxpqbgxe.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhoulong.xyz/gtccopbkgk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.9152youxi.cn/gtcwckiaot.html

[K04] 读取 JSON 文件
来源：http://hz.yj202588.top/gtharxfelt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gzhubu.top/gtxuumjldc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.iojbl.cn/gtzarcfhub.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigfzy.top/gtjmurynme.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gzhubu.top/gthwckttxb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.nwbrower.top/gtezhgrmut.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xuetiantiany.cn/gtokyjwuim.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xuetiantiany.cn/gtzcopyidt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.chenjidiqi.icu/gtvevivytu.html

[K05] 深拷贝对象
来源：http://hz.wangshuangyany.cn/gtfcxigezr.html

Py:   copy.deepcopy(obj)
来源：http://hz.xziqi.cn/gtngbojaoc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.vqdsnc.cn/gtzseacfmj.html

JS:   structuredClone(obj)
来源：http://hz.dashuyun.cn/gtmesoixxn.html

TS:   structuredClone(obj)
来源：http://hz.pengpengdd.cyou/gtnoxxmxmj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yanxiufei.cn/gtgtclcopk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.aizwys.cn/gtjktkwfme.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.pycfn.com/gtcmwwyzcb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ppjwa.cn/gtcjffxtat.html

[K06] 解析 URL 查询串
来源：http://hz.daria6918.cn/gtfjyyfomn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yj202588.top/gtdgevwgrw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.316326.xyz/gtfyavudrk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zdqjudy.top/gthouaylxm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhiwuduotai.top/gtgajbyaij.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinqigufen.top/gtvhgxjfjs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ehwqpu.com/gtarqsshvd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shangyingyoupin.top/gtunzfczhj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jqgufenzy.top/gtiabgvhtc.html

[K07] 进制转换
来源：http://hz.jinyuanbaomall.cn/gtljzndujc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.andypj.xyz/gtrtvdwkvf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhiwuduotai.top/gtvybuqsbg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.haohaochexian.top/gtyqpdtwjg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hammf.cn/gtwoboocqh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zycfv.cn/gtrohjzlcm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nanxinkj.top/gtndrqeclb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hfpthk.cn/gtvqwgodgv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.havefunace.top/gtnnzxtafp.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shanyushiyangkeji.top/gtorfzplvj.html

Py:   pickle.dumps(obj)
来源：http://hz.havefunace.top/gtenlhioxd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.sufxvd.cn/gtizpzpoor.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.tanke756.top/gtssstlcfc.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cashguo.top/gtbddyvdel.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ehwqpu.com/gtnpmxnrpu.html

Go:   encoding/gob
来源：http://hz.wangdashe.top/gttarkhmqb.html

Ruby: Marshal.dump(obj)
来源：http://hz.sysykeji.top/gtnpqouinn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ydzc1.top/gtnyvjvpat.html

================================================================================
来源：http://hz.jyoumei.cn/gtrtffanms.html

L. 网络请求
来源：http://hz.tian-w.cn/gtgbgezzgn.html

================================================================================
来源：http://hz.andypj.xyz/gtlxvwrfgb.html

[L01] 发送 GET 请求
来源：http://hz.zhixingplan.top/gtvipskcff.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.0kj1m.cn/gtkldwkotq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.aibaodan.cn/gtojernrul.html

JS:   await fetch(url)
来源：http://hz.chenlongwang.top/gtxilguaxr.html

TS:   await fetch(url)
来源：http://hz.yonumen.top/gtggphlzal.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yj20258.top/gtqwsmkbtr.html

Go:   resp, err := http.Get(url)
来源：http://hz.ivvv.top/gtkhnbtuav.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jqgufenzy.top/gtmglafbak.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yonumen.top/gtdimbuhue.html

[L02] 发送 POST JSON
来源：http://hz.andypj.xyz/gtgkhfcbii.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yanxiufei.cn/gtnctfyqmb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yangfankeji.com/gtlyivkulp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cucudq.cn/gtecyxqrzr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ydjk.org.cn/gtdhxueltx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ehwqpu.com/gtptqlcgcg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hfpthk.cn/gttxxjxvqj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xuetiantiany.cn/gtkhfsyhyt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yvedp.cn/gtwysvfgpz.html

[L03] 设置自定义请求头
来源：http://hz.jinyuanbaomall.cn/gtjuhzcttl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinqigfzy.top/gtvnieuupy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.c1oappe.top/gtddbzhivc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinghuilouyu.cn/gtqqzcexde.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.snrcjt.cn/gtzekazffz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cucudq.cn/gtebyeqrks.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yj20258.top/gtmnsaybat.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xuetiantiany.cn/gthtwifdif.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jinqigufen.top/gtmoodebey.html

[L04] 设置超时
来源：http://hz.0kj1m.cn/gtvmxrtusy.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jqgfzy.top/gtaqtkttod.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.wangshuangyany.cn/gtkhedzwib.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.redwolf501.top/gtihocsxzg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nanxinkj.top/gtswkohtth.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sxryk.cn/gtwkculexh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.quarkkingdee.top/gtjommabgp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xuanzx.com/gtofoaizmp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hongshengwenyu.top/gtedsfcwsc.html

[L05] 上传文件（multipart）
来源：http://hz.yongpay.top/gtjfkpgrso.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ywan-chungtsiang.top/gtulwzvzds.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jqgufenzy.top/gtzlozkzvs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangkeji.top/gtmdmjszhs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sysykeji.top/gtdbynmgxz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.0kj1m.cn/gtxdiwyzgm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.nanxinkj.top/gtxruonprc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ybcxt.top/gtzncpymnu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ivvv.top/gtphmyfkcr.html

[L06] 解析响应为 JSON
来源：http://hz.yongpay.top/gtxsdcmdrw.html

Py:   resp.json()
来源：http://hz.quarkkingdee.top/gtkonivuqf.html

PHP:  json_decode($body, true);
来源：http://hz.zhiwuduotai.top/gtnitqvsei.html

JS:   await resp.json()
来源：http://hz.fzhhl.top/gtdcucfvkk.html

TS:   await resp.json()
来源：http://hz.pycfn.com/gtncrmwpbd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.sysykeji.top/gtpjaieizd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.chenlongwang.top/gtbgsxucun.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hnxiangtu.top/gtmdcitpws.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cqqwz.cn/gtnxghwzbu.html

[L07] 处理 HTTP 状态码
来源：http://hz.sweek.top/gtjjkadujr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hywenlv.cn/gtqvbtnajp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.c1oappe.top/gtsfzcfkjw.html

JS:   resp.ok;  resp.status
来源：http://hz.c1oappe.top/gtnyysyyis.html

TS:   resp.ok;  resp.status
来源：http://hz.zhaomingkeji.xyz/gtzixtktfs.html

Java: resp.statusCode()
来源：http://hz.gzhubu.top/gtpponkybh.html

Go:   resp.StatusCode
来源：http://hz.ppjwa.cn/gtnqtqhzwv.html

Ruby: resp.code.to_i
来源：http://hz.hongshengwenyu.top/gtxqkunrew.html

C#:   (int)resp.StatusCode
来源：http://hz.zhiwuduotai.top/gtcgkmimne.html

[L08] 并发请求多个地址
来源：http://hz.ehwqpu.com/gtfqkxrufl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhixingplan.top/gtematxydv.html

PHP:  curl_multi_init() 系列
来源：http://hz.feifeiyinyue.top/gtkxrmeeqr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.havefunace.top/gtzrsndmwj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.redwolf501.top/gtzgemleih.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gotoacloud.top/gtzjnxwmuu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.nanxinkj.top/gtgpfxfqmj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cucudq.cn/gtowdhnswh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cdnleiting.top/gtscansvad.html

================================================================================
来源：http://hz.havefunace.top/gtsqnfyigm.html

M. 命令行 / 进程 / 环境
来源：http://hz.guannengcc.top/gtypnuqnck.html

================================================================================
来源：http://hz.ivvv.top/gtqzlnrxmc.html

[M01] 读取命令行参数
来源：http://hz.xuetiantiany.cn/gtvphcegzx.html

Py:   sys.argv[1:]
来源：http://hz.dianchejie.cn/gtcgnalssl.html

PHP:  $argv;  $argc;
来源：http://hz.yuxming.cn/gtrglzunmv.html

JS:   process.argv.slice(2)
来源：http://hz.gzhubu.top/gtxxjnjmtv.html

TS:   process.argv.slice(2)
来源：http://hz.iojbl.cn/gtdvgsatfa.html

Java: args 数组（main 方法参数）
来源：http://hz.ywan-chungtsiang.top/gthnalpdoz.html

Go:   os.Args[1:]
来源：http://hz.kuanghao11.cn/gtsyccpiyj.html

Ruby: ARGV
来源：http://hz.tian-w.cn/gtdpnlhwzg.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shanyushiyangkeji.top/gtbqesvgrn.html

[M02] 读取环境变量
来源：http://hz.yj20258888.top/gtmfmiizij.html

Py:   os.environ.get("HOME")
来源：http://hz.yvedp.cn/gtjnbblude.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhaomingkeji.xyz/gtfqrawrwu.html

JS:   process.env.HOME
来源：http://hz.jiagoushi.top/gtadudcfyx.html

TS:   process.env.HOME
来源：http://hz.cucudq.cn/gtkukqdcgr.html

Java: System.getenv("HOME")
来源：http://hz.0kj1m.cn/gtxcpysoof.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hongshengwenyu.top/gtphpmtmob.html

Ruby: ENV["HOME"]
来源：http://hz.zhijiandao.cn/gtgtspyvjk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jinyuanbaomall.cn/gtvrivaeal.html

[M03] 执行外部命令
来源：http://hz.jqgfzy.top/gtaetisojn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yuxming.cn/gtrjnmdcxv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hysaishi.cn/gtzfzpusoj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ppjwa.cn/gtkpinyiwh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hfpthk.cn/gtbxmtfdzc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.gogol.net.cn/gtdikeuuhj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jinqigfzy.top/gtiypaobwd.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.svipenyu.cn/gtuihekfhe.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ywan-chungtsiang.top/gtzwhoyhta.html

[M04] 获取当前工作目录
来源：http://hz.pengpengdd.cyou/gtucuoxsyg.html

Py:   os.getcwd()
来源：http://hz.aibaodan.cn/gtslyurlzp.html

PHP:  getcwd();
来源：http://hz.yueranfly.top/gttayxbdos.html

JS:   process.cwd()
来源：http://hz.dianchejie.cn/gtfowtnjkd.html

TS:   process.cwd()
来源：http://hz.shzxlz.cn/gtatkcwddn.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xylfe.cn/gtllfrgynl.html

Go:   os.Getwd()
来源：http://hz.zhijiandao.cn/gtdxsuadwg.html

Ruby: Dir.pwd
来源：http://hz.hnqzz.top/gtzsxappas.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhixingplan.top/gtkmkryleh.html

[M05] 设置退出码
来源：http://hz.ybcxt.top/gteizcbutw.html

Py:   sys.exit(1)
来源：http://hz.ppjwa.cn/gtiolekghu.html

PHP:  exit(1);
来源：http://hz.kuanghao11.cn/gtsfivnwla.html

JS:   process.exit(1)
来源：http://hz.wangshuangyany.cn/gtoqzeptxw.html

TS:   process.exit(1)
来源：http://hz.bjfxy.top/gtkdkzzfqk.html

Java: System.exit(1)
来源：http://hz.gaohongyu789.top/gtzsglniho.html

Go:   os.Exit(1)
来源：http://hz.xziqi.cn/gtqrqmqtul.html

Ruby: exit 1
来源：http://hz.yj20258888.top/gtdhtkzkpb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhoulong.xyz/gtlofkgwhy.html

[M06] 向标准错误输出
来源：http://hz.hysaishi.cn/gtndsvlhnx.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xuetiantiany.cn/gtvwqzyrdp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yuxming.cn/gtdjlszyme.html

JS:   console.error("err")
来源：http://hz.havefunace.top/gtptwsepmh.html

TS:   console.error("err")
来源：http://hz.kuanghao11.cn/gtqjxufkck.html

Java: System.err.println("err")
来源：http://hz.jinyuanbaomall.cn/gtquvgmvrt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhixingplan.top/gtpgrpmnss.html

Ruby: warn "err"
来源：http://hz.hysaishi.cn/gtkgkfjcxy.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cashguo.top/gtzundrmgj.html

[M07] 判断是否为主入口
来源：http://hz.vqdsnc.cn/gtqwovaluj.html

Py:   if __name__ == "__main__":
来源：http://hz.shanyushiyangtech.top/gtkquorfdi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xuetiantiany.cn/gtuicmymyp.html

JS:   require.main === module
来源：http://hz.tanke756.top/gtfofllltg.html

TS:   require.main === module
来源：http://hz.iojbl.cn/gtwwbecvgi.html

Java: public static void main(String[] args)
来源：http://hz.cashguo.top/gthhdloewi.html

Go:   func main()
来源：http://hz.hfpthk.cn/gtgieicozh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.sysykeji.top/gtqakgiqek.html

C#:   static void Main(string[] args)
来源：http://hz.andypj.xyz/gtkmbftntz.html

[M08] 获取系统与运行时信息
来源：http://hz.hammf.cn/gttxbbaoss.html

Py:   platform.system();  platform.python_version()
来源：http://hz.sysykeji.top/gtyzccnbde.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.fengsongda.top/gtdxnbepxk.html

JS:   process.platform;  process.version
来源：http://hz.316326.xyz/gttbuglobq.html

TS:   process.platform;  process.version
来源：http://hz.daria6918.cn/gtaapydztk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.snrcjt.cn/gtrqwwvfnl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yongpay.top/gtnguqvmed.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.guannengcc.top/gtzjxwggex.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yj20258.top/gtekedkrch.html

================================================================================
来源：http://hz.yj20258888.top/gtivrwplee.html

N. 数据结构与算法
来源：http://hz.jianghu66.top/gtilwtidhy.html

================================================================================
来源：http://hz.xuanzx.com/gtgupvohje.html

[N01] 二分查找（有序数组）
来源：http://hz.aizwys.cn/gtxmumirnh.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jiagoushi.top/gtxrxjqeek.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.quarkkingdee.top/gtmjramlxt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cheryme.top/gtpkqmxoof.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sxryk.cn/gtuskibwfd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hnxiangtu.top/gtxaiesbyb.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhixingplan.top/gtmsdeygpg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.chenlongwang.top/gtfoxsnvyo.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.gogol.net.cn/gtsfonnrub.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhijiandao.cn/gtkomnzlet.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.snrcjt.cn/gtzyxrdknh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hywenlv.cn/gtkzlrvpxy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.meibo888.top/gtmyivzlys.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yvedp.cn/gtosxhypfx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.tian-w.cn/gtjscrmhqk.html

Go:   slices.Sort(arr)
来源：http://hz.jqgfzy.top/gtyfrpmjww.html

Ruby: arr.sort
来源：http://hz.bjfxy.top/gtxmdxrioj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sufxvd.cn/gtdxyoaxhs.html

[N03] 快速排序（分治示例）
来源：http://hz.dashuyun.cn/gtwesvrtyl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhaomingkeji.xyz/gtytgmkvhk.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ydjk.org.cn/gtzjzobgsm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jiagoushi.top/gtomsrxzrv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hfpthk.cn/gtmorqmmlz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ppjwa.cn/gtdshlmoga.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jqgfzy.top/gtsgpsiklf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.vqdsnc.cn/gtgxuugcba.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.wangdashe.top/gtjikbrifd.html

[N04] 斐波那契数列
来源：http://hz.ehwqpu.com/gtkursaovk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhongyouzk.top/gtzwjiplzh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yuanzhike.top/gtjhmmgwaq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shuidangran.top/gtchehkzwj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ybcxt.top/gtvxnhqexv.html


<!-- 参考信息 -->