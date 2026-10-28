代发 wailian999

[J07] 比较两个日期
来源：http://hz.sweek.top/gtzgbczmjo.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.chenjidiqi.icu/gtcyejpgbn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.daxiang520.top/gtaeskvqee.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.snrcjt.cn/gtiervealz.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hnxiangtu.top/gtweszewdh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ybcxt.top/gtwxyasozk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xziqi.cn/gtzjhgonbn.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hongshengwenyu.top/gtymlphikr.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtctlehran.html

[J08] 提取年月日与星期
来源：http://hz.cucudq.cn/gtmwkalqxi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.guowangkeji.top/gttgbyjkhu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.kuanghao11.cn/gttyircfxl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.c1oappe.top/gtbqrupokn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hnqzz.top/gtztveogak.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jyoumei.cn/gtnyfsdrmz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shzxlz.cn/gttxxgaxpr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xuetiantiany.cn/gtaxjtoogp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ppjwa.cn/gtsjagwvzi.html

[J09] 时区处理
来源：http://hz.hfpthk.cn/gthnpvmygd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.wangdashe.top/gtgluqowqu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenzaomai.com/gtadxevvgu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sufxvd.cn/gteekqvmtb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.havefunace.top/gtqfnrvlye.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gotoacloud.top/gtbpfvunnl.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinqigufen.top/gtkxahvogr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xuetiantiany.cn/gtwngltmbi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.0kj1m.cn/gtwggxepru.html

[J10] 取今天 / 本月第一天
来源：http://hz.gogol.net.cn/gtcxpihiwf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ybcxt.top/gtcyljfijk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shzxlz.cn/gtmrehyihp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhixingplan.top/gtltvqremf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.fzhhl.top/gtdycreoyy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yuanzhike.top/gtqzykfyfy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.316326.xyz/gtminoybsu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xuanzx.com/gtcxsmivax.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.vqdsnc.cn/gthjrizvqv.html

================================================================================
来源：http://hz.zhijiandao.cn/gtkwllvfvh.html

K. JSON 与序列化
来源：http://hz.cucudq.cn/gtjwsaamdc.html

================================================================================
来源：http://hz.gaohongyu789.top/gtgslnjlwg.html

[K01] 对象转 JSON 字符串
来源：http://hz.ydjk.org.cn/gtuostmnnh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.quarkkingdee.top/gtkzzikhrm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.feifeiyinyue.top/gtuzciezbr.html

JS:   JSON.stringify(obj)
来源：http://hz.zdqjudy.top/gtpzddbsjc.html

TS:   JSON.stringify(obj)
来源：http://hz.yuanzhike.top/gtfrvaafkh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.aibaodan.cn/gtsjqmxojk.html

Go:   json.Marshal(obj)
来源：http://hz.hnqzz.top/gtwlwdumhr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.gzhubu.top/gtbezgshse.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.mhx1999.top/gtgwfdnnqv.html

[K02] JSON 字符串转对象
来源：http://hz.shanyushiyangkeji.top/gttesrsqeu.html

Py:   json.loads(s)
来源：http://hz.xuanzx.com/gtjncahpnq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.fengsongda.top/gtwxtiluow.html

JS:   JSON.parse(s)
来源：http://hz.xylfe.cn/gtvaktwbwn.html

TS:   JSON.parse(s)
来源：http://hz.nanxinkj.top/gtrbanbpih.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.aibaodan.cn/gtzpytmlfv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yongpay.top/gtoebosfsi.html

Ruby: JSON.parse(s)
来源：http://hz.tian-w.cn/gtcdwgpwtz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhengqikj.top/gtqpqmxuax.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.nwbrower.top/gtzolnfueo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.tianlin.xyz/gtwvjfxpwp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.wangshuangyany.cn/gtsqmuipav.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jiagoushi.top/gttjohepyr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhengqikj.top/gtvafdfzja.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shuidangran.top/gtzxbekbnx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cqqwz.cn/gtwgncmsbm.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.havefunace.top/gtestociah.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hysaishi.cn/gtmbbathsg.html

[K04] 读取 JSON 文件
来源：http://hz.gotoacloud.top/gtftmiaaor.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yuanzhike.top/gtkwejlmht.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yvedp.cn/gtidnefoys.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nanxuanxn.top/gtgyvahxhq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ppjwa.cn/gtrnmgzzph.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hongshengwenyu.top/gtnolwzoyf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.dashuyun.cn/gttfuipkom.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.wangdashe.top/gtkmiobbul.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yanxiufei.cn/gtpotgdyrb.html

[K05] 深拷贝对象
来源：http://hz.fzhhl.top/gtgoouggcg.html

Py:   copy.deepcopy(obj)
来源：http://hz.yuxming.cn/gtnfyaqmrc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zycfv.cn/gtvmszplaz.html

JS:   structuredClone(obj)
来源：http://hz.fengsongda.top/gtjeyigfiv.html

TS:   structuredClone(obj)
来源：http://hz.tian-w.cn/gtsekbdvad.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.wangshuangyany.cn/gtzxbcqtqr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yueranfly.top/gtjeqcniwy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.fzhhl.top/gtgtkbhmbu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yuanzhike.top/gtbrttzxdr.html

[K06] 解析 URL 查询串
来源：http://hz.cdnleiting.top/gtwzbkytje.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.aibaodan.cn/gtfcsoufkd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.iojbl.cn/gthrakbzrz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.mhx1999.top/gtmjfzedzz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangkeji.top/gtxqyiydho.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jqgufenzy.top/gtykhlpqwi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.daxiang520.top/gtdpnsimvk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.svipenyu.cn/gtokddvlfy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shzxlz.cn/gtvggjbztb.html

[K07] 进制转换
来源：http://hz.bjfxy.top/gtlgsqacyd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hysaishi.cn/gtcmftruze.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yongpay.top/gtnfkqruay.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yj20258.top/gtjenmknpo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jqgufenzy.top/gtrnasuaqj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.kuanghao11.cn/gtndhxwsqw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.fengsongda.top/gtgwimmlyk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.tian-w.cn/gtkptxvjtb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shzxlz.cn/gtynwbcvmv.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ydjk.org.cn/gtwvhvpjom.html

Py:   pickle.dumps(obj)
来源：http://hz.ybcxt.top/gteghtougj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.svipenyu.cn/gtqgnayxzu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jinqigfzy.top/gtmdczqftf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yvedp.cn/gtifmcmjmb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.aibaodan.cn/gtiocefabk.html

Go:   encoding/gob
来源：http://hz.zhixingplan.top/gtylefcoti.html

Ruby: Marshal.dump(obj)
来源：http://hz.jyoumei.cn/gtnmlvgder.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.aibaodan.cn/gtgfmcizwg.html

================================================================================
来源：http://hz.cucudq.cn/gtpwbkmleo.html

L. 网络请求
来源：http://hz.jiagoushi.top/gtnxpwmbxk.html

================================================================================
来源：http://hz.shzxlz.cn/gtoysnornl.html

[L01] 发送 GET 请求
来源：http://hz.sweek.top/gthztnxler.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.daxiang520.top/gthdllxqil.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ydzc1.top/gtxfqqvtjm.html

JS:   await fetch(url)
来源：http://hz.sysykeji.top/gtargqvjcn.html

TS:   await fetch(url)
来源：http://hz.nanxuanxn.top/gtinykmbhe.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yueranfly.top/gtewtwdspp.html

Go:   resp, err := http.Get(url)
来源：http://hz.yvedp.cn/gtjnitlkks.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.svipenyu.cn/gtwkxwfunt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.dianchejie.cn/gtuiogdqod.html

[L02] 发送 POST JSON
来源：http://hz.jlsjyb.cn/gtcvpzrogv.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.meibo888.top/gtmgvcpvda.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yonumen.top/gtsyuzpvvs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sweek.top/gtthpgsrlv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xinyue.icu/gtecwoxuvg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.0kj1m.cn/gtbpagilyp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yj20258.top/gtoevgluoz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hnxiangtu.top/gtliygidio.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.9152youxi.cn/gtvlnuwiog.html

[L03] 设置自定义请求头
来源：http://hz.haohaochexian.top/gtynfbpiku.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yvedp.cn/gtchrrliiy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jlsjyb.cn/gtesgerpib.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shuidangran.top/gtszuialho.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhengqikj.top/gtvigfhyab.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.smart0.xyz/gtzpyyvhul.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hnxiangtu.top/gtwrqxpcua.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ppjwa.cn/gtukupmzuy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.sweek.top/gttcvqjfzp.html

[L04] 设置超时
来源：http://hz.redwolf501.top/gtqwrkkcmq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ybcxt.top/gtbuzwdnxx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.bjfxy.top/gtvewdxqxn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hysaishi.cn/gtoiigechy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jyoumei.cn/gtrqvbeqwv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jianghu66.top/gtskqzznti.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jlsjyb.cn/gtsttwofsx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cucudq.cn/gthmxgqugh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.havefunace.top/gtcguaqzws.html

[L05] 上传文件（multipart）
来源：http://hz.hnqzz.top/gtjjywynor.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hywenlv.cn/gtknbweagg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shuidangran.top/gtxukbduyh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhengqikj.top/gthhqysvrx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yvedp.cn/gthjfurrcr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sufxvd.cn/gtlcxubywq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.sxryk.cn/gtsxghbran.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.snrcjt.cn/gtbtmclrgo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gaohongyu789.top/gtjxbnbbll.html

[L06] 解析响应为 JSON
来源：http://hz.shuidangran.top/gtrcozwrua.html

Py:   resp.json()
来源：http://hz.yongpay.top/gtxpfivhai.html

PHP:  json_decode($body, true);
来源：http://hz.andypj.xyz/gtxwpigffu.html

JS:   await resp.json()
来源：http://hz.wangshuangyany.cn/gtwcepyihi.html

TS:   await resp.json()
来源：http://hz.quarkkingdee.top/gtmuvykmob.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hnxiangtu.top/gtmqqnxwyl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xingfuxueyuan.xyz/gtwgdikcxd.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xingfuxueyuan.xyz/gtbsxoilqg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.chenlongwang.top/gtckgdxvrc.html

[L07] 处理 HTTP 状态码
来源：http://hz.xylfe.cn/gtkiqskuqo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.gotoacloud.top/gtdnxcjvbn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.dashuyun.cn/gtxcecovlv.html

JS:   resp.ok;  resp.status
来源：http://hz.tian-w.cn/gtpulueqft.html

TS:   resp.ok;  resp.status
来源：http://hz.hfpthk.cn/gtkacctgwb.html

Java: resp.statusCode()
来源：http://hz.xingfuxueyuan.xyz/gtugreqszi.html

Go:   resp.StatusCode
来源：http://hz.gotoacloud.top/gtcakehjiu.html

Ruby: resp.code.to_i
来源：http://hz.jqgfzy.top/gtoyqxqacb.html

C#:   (int)resp.StatusCode
来源：http://hz.dianchejie.cn/gtjidthwit.html

[L08] 并发请求多个地址
来源：http://hz.xylfe.cn/gtviixilam.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.shangyingyoupin.top/gtudpgnceq.html

PHP:  curl_multi_init() 系列
来源：http://hz.wangdashe.top/gtbyeznwzw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydzc1.top/gtnkyrhurq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhixingplan.top/gtftjmkvin.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ivvv.top/gtfzojfyyd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.aibaodan.cn/gttfmkbdpp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.daria6918.cn/gtzwmqrjai.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hongshengwenyu.top/gtjwveldjl.html

================================================================================
来源：http://hz.hywenlv.cn/gtixaabooq.html

M. 命令行 / 进程 / 环境
来源：http://hz.iojbl.cn/gtqndaqazw.html

================================================================================
来源：http://hz.zhijiandao.cn/gtbaugadhs.html

[M01] 读取命令行参数
来源：http://hz.shanyushiyangtech.top/gtqcgezubt.html

Py:   sys.argv[1:]
来源：http://hz.yvedp.cn/gtstgasgid.html

PHP:  $argv;  $argc;
来源：http://hz.sweek.top/gtavqwxgzf.html

JS:   process.argv.slice(2)
来源：http://hz.hywenlv.cn/gtevtxwyav.html

TS:   process.argv.slice(2)
来源：http://hz.chenzaomai.com/gtsacyviuv.html

Java: args 数组（main 方法参数）
来源：http://hz.daria6918.cn/gtigqmmisl.html

Go:   os.Args[1:]
来源：http://hz.jlsjyb.cn/gtpotllxgk.html

Ruby: ARGV
来源：http://hz.shanyushiyangkeji.top/gtpdocbzzk.html

C#:   args 数组（Main 方法参数）
来源：http://hz.chenlongwang.top/gtlitkaxdx.html

[M02] 读取环境变量
来源：http://hz.fzhhl.top/gtbtsojarr.html

Py:   os.environ.get("HOME")
来源：http://hz.zhaomingkeji.xyz/gtuhtjeifd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yuanzhike.top/gtieogfhsh.html

JS:   process.env.HOME
来源：http://hz.zdqjudy.top/gtzrlxudzb.html

TS:   process.env.HOME
来源：http://hz.hywenlv.cn/gtqpwxliaa.html

Java: System.getenv("HOME")
来源：http://hz.zhengqikj.top/gthilpkgek.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.vqdsnc.cn/gthrvqcwqz.html

Ruby: ENV["HOME"]
来源：http://hz.c1oappe.top/gtxpjochzi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhixingplan.top/gtmdciwhzq.html

[M03] 执行外部命令
来源：http://hz.ivvv.top/gtlkjealzh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhengqikj.top/gtnccoebtl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.vqdsnc.cn/gtwvyuqlcb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigfzy.top/gtdlogekvo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.sysykeji.top/gtrbiojpin.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.havefunace.top/gtsfjccaym.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.meibo888.top/gtaxfbtrvb.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zdqjudy.top/gtxssawcrx.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gogol.net.cn/gttaorcijv.html

[M04] 获取当前工作目录
来源：http://hz.zhoulong.xyz/gtbjmdcoeh.html

Py:   os.getcwd()
来源：http://hz.yj202588.top/gtpkhvpbwd.html

PHP:  getcwd();
来源：http://hz.zhengqikj.top/gtgceaqeah.html

JS:   process.cwd()
来源：http://hz.xuetiantiany.cn/gtprcuxvuo.html

TS:   process.cwd()
来源：http://hz.9152youxi.cn/gtmfxskedb.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.shangyingyoupin.top/gtlxmzcpak.html

Go:   os.Getwd()
来源：http://hz.gogol.net.cn/gtyiocfqmm.html

Ruby: Dir.pwd
来源：http://hz.chenzaomai.com/gtoraaquny.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.feifeiyinyue.top/gtgunrqbzq.html

[M05] 设置退出码
来源：http://hz.havefunace.top/gtzvjtdpkv.html

Py:   sys.exit(1)
来源：http://hz.guannengcc.top/gtnvqnmvow.html

PHP:  exit(1);
来源：http://hz.aizwys.cn/gtbeovabsq.html

JS:   process.exit(1)
来源：http://hz.feifeiyinyue.top/gtcanusnbx.html

TS:   process.exit(1)
来源：http://hz.shanyushiyangtech.top/gtaxttlmgg.html

Java: System.exit(1)
来源：http://hz.ybcxt.top/gtexihnecl.html

Go:   os.Exit(1)
来源：http://hz.jinqigfzy.top/gtrxvosjkr.html

Ruby: exit 1
来源：http://hz.hywenlv.cn/gtgatgduiv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nanxuanxn.top/gtntdiattf.html

[M06] 向标准错误输出
来源：http://hz.jinyuanbaomall.cn/gtdjpxzuzx.html

Py:   print("err", file=sys.stderr)
来源：http://hz.dashuyun.cn/gtzjpmzqwx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yuxming.cn/gtmuxcnnor.html

JS:   console.error("err")
来源：http://hz.chenjidiqi.icu/gtmjyuknqa.html

TS:   console.error("err")
来源：http://hz.jinqigfzy.top/gtsglzdsva.html

Java: System.err.println("err")
来源：http://hz.cqqwz.cn/gtluucgxxx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhongyouzk.top/gtbtnbepnv.html

Ruby: warn "err"
来源：http://hz.xuetiantiany.cn/gtseuoanaf.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jinqigufen.top/gtreoryxdc.html

[M07] 判断是否为主入口
来源：http://hz.yangfankeji.com/gtbuephdyw.html

Py:   if __name__ == "__main__":
来源：http://hz.wangdashe.top/gtxfvzcmxn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.daria6918.cn/gtlluzqvzx.html

JS:   require.main === module
来源：http://hz.52xcode.cn/gtheernvuj.html

TS:   require.main === module
来源：http://hz.cdnleiting.top/gtphdngthe.html

Java: public static void main(String[] args)
来源：http://hz.zycfv.cn/gtyxtsxckz.html

Go:   func main()
来源：http://hz.hywenlv.cn/gtizguxzoz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ppjwa.cn/gtzmzueaaw.html

C#:   static void Main(string[] args)
来源：http://hz.cdnleiting.top/gtijlkyqqu.html

[M08] 获取系统与运行时信息
来源：http://hz.yangfankeji.com/gtheyfwdjq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ivvv.top/gtozirxhpx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xinyue.icu/gtoigmzunt.html

JS:   process.platform;  process.version
来源：http://hz.yj20258888.top/gtxjfjfyej.html

TS:   process.platform;  process.version
来源：http://hz.yongpay.top/gtgrgjeyke.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.svipenyu.cn/gtizelfgwg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.svipenyu.cn/gtrxnqenvm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.gaohongyu789.top/gtamcekhol.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yuxming.cn/gtjmztzpgi.html

================================================================================
来源：http://hz.smart0.xyz/gtokyccxdh.html

N. 数据结构与算法
来源：http://hz.havefunace.top/gtiyocwwfo.html

================================================================================
来源：http://hz.jinqigfzy.top/gtqrjrcyve.html

[N01] 二分查找（有序数组）
来源：http://hz.quarkkingdee.top/gtkyjaqbzj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.nanxinkj.top/gtyarrazvl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.fzhhl.top/gtsksfupoa.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hongshengwenyu.top/gtbqsddzqn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ivvv.top/gtwljowjhf.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ybcxt.top/gtimycnxte.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.nanxuanxn.top/gtrpqpxpxv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xinyue.icu/gtcxzumtmz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.nanxinkj.top/gtggcjlkdl.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.aizwys.cn/gtfypdpwqc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shzxlz.cn/gtxcwuawim.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tian-w.cn/gttoqwltsz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.316326.xyz/gthddcpamc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aizwys.cn/gtguteqznv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhoulong.xyz/gtkqqxsbhi.html

Go:   slices.Sort(arr)
来源：http://hz.haohaochexian.top/gtrukprrao.html

Ruby: arr.sort
来源：http://hz.fengsongda.top/gtvisgyhvm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hammf.cn/gtlvilkljy.html

[N03] 快速排序（分治示例）
来源：http://hz.gogol.net.cn/gtruhxzrgw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.chenlongwang.top/gtcaoaptzr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sufxvd.cn/gtxwtzvpyb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dianchejie.cn/gtnggzvizf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yueranfly.top/gtfherrvcv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.wangdashe.top/gtbnmqipxc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jiagoushi.top/gtugdtvokv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.dashuyun.cn/gtsdxybohm.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.birdmap.top/gtpebnbwfm.html

[N04] 斐波那契数列
来源：http://hz.hfpthk.cn/gtjlwijdnr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xuanzx.com/gtoftoectb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.gogol.net.cn/gtwwyjeynp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cucudq.cn/gthyptowid.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sufxvd.cn/gtgkwqbbwb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.meibo888.top/gtxbfeblos.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yongpay.top/gtknzfggxe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.redwolf501.top/gtwopsgjsc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.chenzaomai.com/gtmtmiibne.html


<!-- 参考信息 -->