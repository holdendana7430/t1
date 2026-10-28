代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://hz.sysykeji.top/gttlawhnnk.html

Go:   end.Sub(start).Hours()
来源：http://hz.nanxinkj.top/gtvfqoflaq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.aibaodan.cn/gtnpbdbpbm.html

C#:   (end - start).TotalSeconds
来源：http://hz.ydzc1.top/gthdnlaszi.html

[J07] 比较两个日期
来源：http://hz.jyoumei.cn/gtmptjpreo.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.pycfn.com/gtdulmtrma.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.chenzaomai.com/gtzkiyypks.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cdnleiting.top/gttwlxmief.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ivvv.top/gtjfafvsyb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ywan-chungtsiang.top/gtbnmjivps.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jlsjyb.cn/gtpskaauvf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cashguo.top/gtaypdtvia.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hongshengwenyu.top/gtethgohse.html

[J08] 提取年月日与星期
来源：http://hz.zhixingplan.top/gtiuzfsxty.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.redwolf501.top/gtzyakeksk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinyuanbaomall.cn/gttjxhqwqi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shanyushiyangtech.top/gtrokqynod.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.mhx1999.top/gtolqpofwv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jianghu66.top/gtistvevon.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yueranfly.top/gteynifukr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ydjk.org.cn/gtyubqylct.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hywenlv.cn/gtjhcajpuz.html

[J09] 时区处理
来源：http://hz.jlsjyb.cn/gtqhuyylrg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sysykeji.top/gtdhtbiahr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ybcxt.top/gtjpvpxyza.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sysykeji.top/gtehtafmlx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cqqwz.cn/gtbungzvcd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jyoumei.cn/gtmzzjtfnj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhijiandao.cn/gtibasoadi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.tian-w.cn/gtnqdwacqm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shzxlz.cn/gtzuhlmmeu.html

[J10] 取今天 / 本月第一天
来源：http://hz.9152youxi.cn/gtdmeertju.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yanxiufei.cn/gtvjcmbzjz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.nanxinkj.top/gtdikagcjw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zycfv.cn/gttyptuoyn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.andypj.xyz/gtbtzrptkh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.gogol.net.cn/gtocmsqgvp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.wangshuangyany.cn/gtnsaxjsei.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yuanzhike.top/gtwtofwihu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ydzc1.top/gthnaawqea.html

================================================================================
来源：http://hz.jinqigufen.top/gtfpljphhe.html

K. JSON 与序列化
来源：http://hz.shzxlz.cn/gtqgwopewm.html

================================================================================
来源：http://hz.gogol.net.cn/gtiebzvszk.html

[K01] 对象转 JSON 字符串
来源：http://hz.xuanzx.com/gtwegrxcsv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.sweek.top/gtalpfyecs.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.dashuyun.cn/gtpkoobrlb.html

JS:   JSON.stringify(obj)
来源：http://hz.yangfankeji.com/gthucpyjbl.html

TS:   JSON.stringify(obj)
来源：http://hz.zhiwuduotai.top/gtikoojeuv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.gzhubu.top/gtinbdvmwp.html

Go:   json.Marshal(obj)
来源：http://hz.haohaochexian.top/gttroaofmj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.quarkkingdee.top/gtsljqgtxq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xingfuxueyuan.xyz/gtybrqelpk.html

[K02] JSON 字符串转对象
来源：http://hz.ybcxt.top/gtkhupdfzg.html

Py:   json.loads(s)
来源：http://hz.smart0.xyz/gtqpconuwp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jianghu66.top/gtyqhkfaar.html

JS:   JSON.parse(s)
来源：http://hz.yongpay.top/gtfzpoxzvz.html

TS:   JSON.parse(s)
来源：http://hz.fengsongda.top/gtzubrlprw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.kuanghao11.cn/gtfvozmlsk.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.nanxinkj.top/gtiajghxxj.html

Ruby: JSON.parse(s)
来源：http://hz.zhijiandao.cn/gtscwfnbhk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.daria6918.cn/gtlhtxixqd.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.tanke756.top/gtdrhlgwzm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jlsjyb.cn/gtckznvjby.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cucudq.cn/gtfwacayzh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangshuangyany.cn/gtjsmglpij.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cashguo.top/gtershvsim.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.iojbl.cn/gtdbfxdfsr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ehwqpu.com/gtubvlyeuk.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jlsjyb.cn/gtdpmrpwoi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.52xcode.cn/gtbfwnqnpf.html

[K04] 读取 JSON 文件
来源：http://hz.tianlin.xyz/gtflheyiaq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ybcxt.top/gtzuixxybn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhaomingkeji.xyz/gtolzypjft.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yongpay.top/gthzubmmkg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zycfv.cn/gtarvnvxzx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cucudq.cn/gtsczkzlpd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.0kj1m.cn/gtgtkmzost.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yonumen.top/gteqoggqgf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhixingplan.top/gtekpfhctf.html

[K05] 深拷贝对象
来源：http://hz.yj20258888.top/gtcyfaqmuk.html

Py:   copy.deepcopy(obj)
来源：http://hz.xuetiantiany.cn/gtloiwubzk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.kuanghao11.cn/gttlhvfoxe.html

JS:   structuredClone(obj)
来源：http://hz.andypj.xyz/gtngxpzgtp.html

TS:   structuredClone(obj)
来源：http://hz.nwbrower.top/gtglffjyds.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ppjwa.cn/gtgbmsdosu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yvedp.cn/gteuusjhbd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jianghu66.top/gtutertwus.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.havefunace.top/gtiwilhuvu.html

[K06] 解析 URL 查询串
来源：http://hz.yj202588.top/gtignllasn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sxryk.cn/gtxpaordiz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jiagoushi.top/gtpmkkoeyk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.0kj1m.cn/gtlqxhfigt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnxiangtu.top/gtigpnmpxh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.bjfxy.top/gtqbnmjfkp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.redwolf501.top/gtljknknls.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.cheryme.top/gtwdtkzfvv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gaohongyu789.top/gtsqfjocke.html

[K07] 进制转换
来源：http://hz.ydjk.org.cn/gtazssczvj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shzxlz.cn/gtdntsmdyu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sysykeji.top/gthagqjtig.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.tian-w.cn/gtgwvwfneu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gaohongyu789.top/gtioqwqosw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.gotoacloud.top/gttoksofds.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ivvv.top/gtubocwviq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hammf.cn/gtsklhdcpi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhengqikj.top/gtncvrzidl.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yuxming.cn/gtgdbzuzmo.html

Py:   pickle.dumps(obj)
来源：http://hz.yongpay.top/gtiuowdxzs.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.aibaodan.cn/gtdyxiqztx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hnqzz.top/gtrvuzzowo.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cheryme.top/gtoilelqzg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zdqjudy.top/gtehcvurox.html

Go:   encoding/gob
来源：http://hz.zhiwuduotai.top/gtullzdnox.html

Ruby: Marshal.dump(obj)
来源：http://hz.daria6918.cn/gtzsnohsla.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ydjk.org.cn/gtpnoptnzv.html

================================================================================
来源：http://hz.yanxiufei.cn/gtlwvtgczv.html

L. 网络请求
来源：http://hz.tian-w.cn/gtxqubjgvm.html

================================================================================
来源：http://hz.xinyue.icu/gtygkealhx.html

[L01] 发送 GET 请求
来源：http://hz.jinqigfzy.top/gtvthohxzl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yj202588.top/gtusufghwp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hfpthk.cn/gtvihplsxu.html

JS:   await fetch(url)
来源：http://hz.hnqzz.top/gtvatlsdht.html

TS:   await fetch(url)
来源：http://hz.yanxiufei.cn/gtnhnbftgd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cheryme.top/gtgywqbast.html

Go:   resp, err := http.Get(url)
来源：http://hz.0kj1m.cn/gtwboqnstw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.dianchejie.cn/gtkszfstle.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yueranfly.top/gtrmsiweyq.html

[L02] 发送 POST JSON
来源：http://hz.gzhubu.top/gtahybtone.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yuxming.cn/gtkjjqsdue.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhongyouzk.top/gtjfdgmbvc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yangfankeji.com/gtfjmalynf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnxiangtu.top/gtppydzorz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.smart0.xyz/gteulcucyq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shuidangran.top/gtwiedytfl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xylfe.cn/gteyynpnlp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.snrcjt.cn/gtzhrutjtx.html

[L03] 设置自定义请求头
来源：http://hz.andypj.xyz/gtiafuqabs.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hammf.cn/gtblbbrgqb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhoulong.xyz/gtkkizfzks.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.meibo888.top/gtfulbgqvs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinqigfzy.top/gtezailjui.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.haohaochexian.top/gtqidoqqax.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hnxiangtu.top/gtwqakoamn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hammf.cn/gtlvlxhvol.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gaohongyu789.top/gtoooaudor.html

[L04] 设置超时
来源：http://hz.316326.xyz/gtgswkudji.html

Py:   requests.get(url, timeout=5)
来源：http://hz.fzhhl.top/gtvqpxvrfn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.shanyushiyangkeji.top/gtgeldwpyt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.birdmap.top/gtlghnqcgp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinyuanbaomall.cn/gtgwiofuww.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.smart0.xyz/gtnjlmhjqb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhongyouzk.top/gtnnpuntuv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yonumen.top/gtatavjqew.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cashguo.top/gtjfakrlrx.html

[L05] 上传文件（multipart）
来源：http://hz.gaohongyu789.top/gtydnsgrzu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.dashuyun.cn/gtobthadkk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yangfankeji.com/gtupkimsgt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.gaohongyu789.top/gtwbaawplc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.daxiang520.top/gtackiuvwj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.haohaochexian.top/gteanusjsz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhaomingkeji.xyz/gtlhaglzla.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xinyue.icu/gtnnqfxenu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.guowangkeji.top/gthamevtua.html

[L06] 解析响应为 JSON
来源：http://hz.yj202588.top/gtaepjujwb.html

Py:   resp.json()
来源：http://hz.jianghu66.top/gtqisbldyd.html

PHP:  json_decode($body, true);
来源：http://hz.316326.xyz/gtljvsnyiw.html

JS:   await resp.json()
来源：http://hz.hammf.cn/gtecusppdg.html

TS:   await resp.json()
来源：http://hz.yuxming.cn/gtxqmrlmhq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zdqjudy.top/gtibfhjikq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.iojbl.cn/gtylnfzlfh.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hnxiangtu.top/gtzstcavwz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cdnleiting.top/gtbnwsdyye.html

[L07] 处理 HTTP 状态码
来源：http://hz.feifeiyinyue.top/gtcjswbork.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cucudq.cn/gtwpvptzul.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xinyue.icu/gtddehlkwq.html

JS:   resp.ok;  resp.status
来源：http://hz.feifeiyinyue.top/gtkkqmqync.html

TS:   resp.ok;  resp.status
来源：http://hz.bjfxy.top/gtkfqkkgfj.html

Java: resp.statusCode()
来源：http://hz.jinghuilouyu.cn/gtkhfcrkik.html

Go:   resp.StatusCode
来源：http://hz.daxiang520.top/gtmgnibots.html

Ruby: resp.code.to_i
来源：http://hz.sweek.top/gtwbglyngm.html

C#:   (int)resp.StatusCode
来源：http://hz.hysaishi.cn/gtupzommae.html

[L08] 并发请求多个地址
来源：http://hz.bjfxy.top/gttoqichky.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhaomingkeji.xyz/gtgcunkdau.html

PHP:  curl_multi_init() 系列
来源：http://hz.yangfankeji.com/gtuaqlflbx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gtytxlubhn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.0kj1m.cn/gtfbndnsyy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.pycfn.com/gtsuvvimmu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.redwolf501.top/gteywslxmr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.shangyingyoupin.top/gtksaduibz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.guannengcc.top/gtsqaccyvm.html

================================================================================
来源：http://hz.sxryk.cn/gtghuqrybt.html

M. 命令行 / 进程 / 环境
来源：http://hz.ivvv.top/gtyjctvddt.html

================================================================================
来源：http://hz.bjfxy.top/gtqtroeoxy.html

[M01] 读取命令行参数
来源：http://hz.zhaomingkeji.xyz/gtnvmjroev.html

Py:   sys.argv[1:]
来源：http://hz.fengsongda.top/gtghmlcwmb.html

PHP:  $argv;  $argc;
来源：http://hz.tianlin.xyz/gtthbjljtj.html

JS:   process.argv.slice(2)
来源：http://hz.sxryk.cn/gtznygaxiz.html

TS:   process.argv.slice(2)
来源：http://hz.svipenyu.cn/gtbrjbmhof.html

Java: args 数组（main 方法参数）
来源：http://hz.sxryk.cn/gtxddopghq.html

Go:   os.Args[1:]
来源：http://hz.hammf.cn/gtykchqmpy.html

Ruby: ARGV
来源：http://hz.yuxming.cn/gtolvgezei.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jiagoushi.top/gtlexvfjli.html

[M02] 读取环境变量
来源：http://hz.yueranfly.top/gtczghhtuw.html

Py:   os.environ.get("HOME")
来源：http://hz.jqgufenzy.top/gtxbsgncfa.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xinyue.icu/gtycmfukeg.html

JS:   process.env.HOME
来源：http://hz.smart0.xyz/gtcsykmcwj.html

TS:   process.env.HOME
来源：http://hz.jinqigfzy.top/gtaqpqktyw.html

Java: System.getenv("HOME")
来源：http://hz.zhixingplan.top/gtsjiyigki.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.wangshuangyany.cn/gtfxqiuhji.html

Ruby: ENV["HOME"]
来源：http://hz.jinqigufen.top/gtylbpjmgt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenlongwang.top/gtmrraiufp.html

[M03] 执行外部命令
来源：http://hz.smart0.xyz/gtktiaggmw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gotoacloud.top/gtsjgbofor.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yanxiufei.cn/gtklcchxmm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.bjfxy.top/gtgcypdayl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.mhx1999.top/gtljomgiyv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yuanzhike.top/gtjegvcnpt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tianlin.xyz/gtczobnute.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.svipenyu.cn/gtzaejgjag.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yj20258888.top/gtsmghxqqb.html

[M04] 获取当前工作目录
来源：http://hz.redwolf501.top/gttiuthjlq.html

Py:   os.getcwd()
来源：http://hz.cucudq.cn/gtxjfbixjw.html

PHP:  getcwd();
来源：http://hz.daria6918.cn/gtnihdbmqh.html

JS:   process.cwd()
来源：http://hz.svipenyu.cn/gtsyhzjjzv.html

TS:   process.cwd()
来源：http://hz.yj20258.top/gtmmdhbdzc.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xziqi.cn/gtxipkfoat.html

Go:   os.Getwd()
来源：http://hz.havefunace.top/gtwgfzbvfb.html

Ruby: Dir.pwd
来源：http://hz.cdnleiting.top/gtkhasdixo.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yj202588.top/gtehhcshhy.html

[M05] 设置退出码
来源：http://hz.meibo888.top/gtiyzueuhr.html

Py:   sys.exit(1)
来源：http://hz.xylfe.cn/gtjlvkmuem.html

PHP:  exit(1);
来源：http://hz.c1oappe.top/gtqowuqovz.html

JS:   process.exit(1)
来源：http://hz.xinyue.icu/gtxcxekjmz.html

TS:   process.exit(1)
来源：http://hz.redwolf501.top/gtjtfnspxg.html

Java: System.exit(1)
来源：http://hz.gotoacloud.top/gtmkwichxh.html

Go:   os.Exit(1)
来源：http://hz.cucudq.cn/gtumhqlqnj.html

Ruby: exit 1
来源：http://hz.xuanzx.com/gtkhxsdeit.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.pycfn.com/gtqqhndvbm.html

[M06] 向标准错误输出
来源：http://hz.0kj1m.cn/gtlfctewzo.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gogol.net.cn/gtjeccxjtq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jqgfzy.top/gtrgiwheml.html

JS:   console.error("err")
来源：http://hz.shanyushiyangtech.top/gtdjdtwxyc.html

TS:   console.error("err")
来源：http://hz.nwbrower.top/gthnwphcjd.html

Java: System.err.println("err")
来源：http://hz.cucudq.cn/gtbbutfskk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.fengsongda.top/gtezdjryot.html

Ruby: warn "err"
来源：http://hz.zhaomingkeji.xyz/gtvfpkyaqb.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.sxryk.cn/gtelckxrtv.html

[M07] 判断是否为主入口
来源：http://hz.sxryk.cn/gteqgtonyz.html

Py:   if __name__ == "__main__":
来源：http://hz.xylfe.cn/gtqbjkbdyh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.52xcode.cn/gtvhagbjho.html

JS:   require.main === module
来源：http://hz.chenlongwang.top/gtpcuttdhy.html

TS:   require.main === module
来源：http://hz.shanyushiyangtech.top/gtlfvkprma.html

Java: public static void main(String[] args)
来源：http://hz.yj202588.top/gtuevcszot.html

Go:   func main()
来源：http://hz.yonumen.top/gtafwuidlo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xingfuxueyuan.xyz/gtzsgjlean.html

C#:   static void Main(string[] args)
来源：http://hz.kuanghao11.cn/gtoagdmpsu.html

[M08] 获取系统与运行时信息
来源：http://hz.sxryk.cn/gtdwlidcbv.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ydzc1.top/gtvbbktcyd.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xziqi.cn/gtzwntbuso.html

JS:   process.platform;  process.version
来源：http://hz.cqqwz.cn/gtuywfhjeb.html

TS:   process.platform;  process.version
来源：http://hz.yongpay.top/gtpdpameux.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.guannengcc.top/gthgmzjnaw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shanyushiyangkeji.top/gtkjjljxuk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.chenlongwang.top/gtjazeonpv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhongyouzk.top/gtpdnkvvtz.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtbhftsnuk.html

N. 数据结构与算法
来源：http://hz.chenjidiqi.icu/gtmcrwrtpy.html

================================================================================
来源：http://hz.zdqjudy.top/gtglxkpwvc.html

[N01] 二分查找（有序数组）
来源：http://hz.shangyingyoupin.top/gttnhutmbr.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jqgufenzy.top/gtewmbtysu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hongshengwenyu.top/gtolxrjhhl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hnqzz.top/gtgmvgfdag.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shuidangran.top/gtodkpzkhm.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.dianchejie.cn/gtddovacsk.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhongyouzk.top/gthmcvghel.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hysaishi.cn/gtuaoicrqs.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xinyue.icu/gtqjhjornu.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.guannengcc.top/gtnfobnlbh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tian-w.cn/gtrwjkmdfz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cucudq.cn/gtuhbvaecc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cucudq.cn/gtrewhnwsk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nanxuanxn.top/gtnzzrnztq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.0kj1m.cn/gtmzvbasqk.html

Go:   slices.Sort(arr)
来源：http://hz.kuanghao11.cn/gtsroyavkb.html

Ruby: arr.sort
来源：http://hz.xylfe.cn/gtkiotnnij.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinqigufen.top/gtvfpphaig.html

[N03] 快速排序（分治示例）
来源：http://hz.sufxvd.cn/gthhwvkonz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hnxiangtu.top/gtjgdzfyhg.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sxryk.cn/gtmloqnpby.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jiagoushi.top/gtcpzgqadt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigfzy.top/gtwvwsygjc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.quarkkingdee.top/gtyzurezlw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.gotoacloud.top/gtvskzghjj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shanyushiyangkeji.top/gtyxahoebw.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.snrcjt.cn/gtymbdfwpd.html

[N04] 斐波那契数列
来源：http://hz.nanxinkj.top/gtkftxalru.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.mhx1999.top/gtsqfzaphs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xziqi.cn/gtlqjvnmfe.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xylfe.cn/gthznqkxtn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nwbrower.top/gtbrejipiz.html


<!-- 参考信息 -->