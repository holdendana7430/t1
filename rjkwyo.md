代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://hz.pycfn.com/gtxygfqdvy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xylfe.cn/gtrdqeuzvo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.mhx1999.top/gtdvcnfcyg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gtpiutdtbz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtunktklpr.html

[J08] 提取年月日与星期
来源：http://hz.yj20258888.top/gtcayoropf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hywenlv.cn/gtqcbtxznd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.chenlongwang.top/gtnckylmip.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhongyouzk.top/gtxmewswih.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.meibo888.top/gttzkaswau.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.daria6918.cn/gtplmrnbqm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.snrcjt.cn/gtorggytqn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sweek.top/gtmwecuypl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hysaishi.cn/gtnsjelypn.html

[J09] 时区处理
来源：http://hz.vqdsnc.cn/gtteeqfmbx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.havefunace.top/gtpfgyzblq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hnxiangtu.top/gtwzveubyj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xylfe.cn/gtxxuhmwqb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhaomingkeji.xyz/gtejhmprpu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nanxinkj.top/gtvyqlaqvi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jqgufenzy.top/gtuukodgfn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.sxryk.cn/gtnnsytfse.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xziqi.cn/gtermixpqj.html

[J10] 取今天 / 本月第一天
来源：http://hz.gaohongyu789.top/gtqszciidt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xinyue.icu/gtxyafgmas.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jyoumei.cn/gtfyndymxl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.mhx1999.top/gtdvrbuwpo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cdnleiting.top/gtzhkydliv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yongpay.top/gtuofcjytx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gotoacloud.top/gtewlzemcl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xylfe.cn/gtgqsmuxts.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shangyingyoupin.top/gtdzdskzhe.html

================================================================================
来源：http://hz.jyoumei.cn/gtenqsshdw.html

K. JSON 与序列化
来源：http://hz.snrcjt.cn/gtpjtdujic.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtxlxwjmfp.html

[K01] 对象转 JSON 字符串
来源：http://hz.chenzaomai.com/gticcdloji.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yongpay.top/gthpgofwzh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xylfe.cn/gtixtnxfqr.html

JS:   JSON.stringify(obj)
来源：http://hz.jqgufenzy.top/gtxbkcdizg.html

TS:   JSON.stringify(obj)
来源：http://hz.kuanghao11.cn/gtqelxuveu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.sxryk.cn/gtxzixplff.html

Go:   json.Marshal(obj)
来源：http://hz.yj202588.top/gtbbrcswvj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.316326.xyz/gtviuqgwby.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jyoumei.cn/gtlieyobag.html

[K02] JSON 字符串转对象
来源：http://hz.gotoacloud.top/gtyavcjsto.html

Py:   json.loads(s)
来源：http://hz.mhx1999.top/gtftwfoxkn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gaohongyu789.top/gtujkinlxy.html

JS:   JSON.parse(s)
来源：http://hz.jinghuilouyu.cn/gtoduknwyd.html

TS:   JSON.parse(s)
来源：http://hz.ybcxt.top/gtibqfiloe.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yj20258888.top/gtgirnhpir.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.mhx1999.top/gtptpxsvfb.html

Ruby: JSON.parse(s)
来源：http://hz.hammf.cn/gtqhnrhyjo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.c1oappe.top/gtmkclipzl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.daxiang520.top/gtfpbkkxkx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yj202588.top/gtqcemmexz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.meibo888.top/gtglzozuld.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.aizwys.cn/gtenlsfdpg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.tianlin.xyz/gtzmwooydo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.guowangkeji.top/gtaksbncuu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hammf.cn/gtkbdujjcw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.dashuyun.cn/gtpbfsrefg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yongpay.top/gtoleixpnz.html

[K04] 读取 JSON 文件
来源：http://hz.gzhubu.top/gtmisnqfrt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xylfe.cn/gtfqjyextt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.svipenyu.cn/gtlhsfnpgd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhoulong.xyz/gtjfxqnljc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xylfe.cn/gtzagqxxvc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.smart0.xyz/gtbboqzltj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.gogol.net.cn/gtjajbrvog.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.chenjidiqi.icu/gtvmpqcaxl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hongshengwenyu.top/gtxfqgwoff.html

[K05] 深拷贝对象
来源：http://hz.xziqi.cn/gtosrgiqoo.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinqigfzy.top/gthgogimwh.html

PHP:  unserialize(serialize($obj));
来源：http://hz.havefunace.top/gtwmghwrwm.html

JS:   structuredClone(obj)
来源：http://hz.tianlin.xyz/gtclsnzblp.html

TS:   structuredClone(obj)
来源：http://hz.tianlin.xyz/gtgeeqomey.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xylfe.cn/gtuhosuowe.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xziqi.cn/gtxcisxtrw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ywan-chungtsiang.top/gtmeyommdt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhengqikj.top/gtcxbghgyd.html

[K06] 解析 URL 查询串
来源：http://hz.shzxlz.cn/gteaopaqjb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhixingplan.top/gtmcytapys.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhixingplan.top/gtzqrwbjog.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ivvv.top/gtjfxoctlg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shzxlz.cn/gtngpjgtcz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ywan-chungtsiang.top/gtcvmtmoqs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cashguo.top/gtsjqjyqos.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.tian-w.cn/gtapcblanw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhongyouzk.top/gtuvirldfn.html

[K07] 进制转换
来源：http://hz.yueranfly.top/gtoplumxzq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.sufxvd.cn/gttqnonxzj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hnqzz.top/gtvhgwwrep.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.cdnleiting.top/gtisdlzxrt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtxshcvtfy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tianlin.xyz/gthojadvzk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.0kj1m.cn/gtoqgdioci.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinqigfzy.top/gtjmopjnxx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj20258.top/gtcajeyypo.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.52xcode.cn/gtfetbeisz.html

Py:   pickle.dumps(obj)
来源：http://hz.yueranfly.top/gtgpqzztnf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cqqwz.cn/gtthonbgsz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xuanzx.com/gtrjmeesrq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.sysykeji.top/gtpbbvqdia.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hysaishi.cn/gtgyohvffb.html

Go:   encoding/gob
来源：http://hz.gaohongyu789.top/gtumvflhfh.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhaomingkeji.xyz/gtaiyaaemf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.kuanghao11.cn/gtwrpolefg.html

================================================================================
来源：http://hz.meibo888.top/gtqwtryqcx.html

L. 网络请求
来源：http://hz.dashuyun.cn/gtzsbscxvw.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtbulrtlqe.html

[L01] 发送 GET 请求
来源：http://hz.jqgfzy.top/gtphnobvpj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhongyouzk.top/gtaznuudxx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.wangdashe.top/gtgdzwksmp.html

JS:   await fetch(url)
来源：http://hz.iojbl.cn/gtjferhdvl.html

TS:   await fetch(url)
来源：http://hz.birdmap.top/gtfqfjjbxd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hywenlv.cn/gtkfxtxmlk.html

Go:   resp, err := http.Get(url)
来源：http://hz.hfpthk.cn/gtnwnzjquk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.pengpengdd.cyou/gtpsmcqqif.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shuidangran.top/gtbliyxcmd.html

[L02] 发送 POST JSON
来源：http://hz.chenjidiqi.icu/gtpkzydzbd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xingfuxueyuan.xyz/gtyisnhvzp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xinyue.icu/gtvbsoyveh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhaomingkeji.xyz/gtvllydtyr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.iojbl.cn/gtdpuwbvlt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yangfankeji.com/gtlyqicjkf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hnqzz.top/gthrjsjyht.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jyoumei.cn/gtyippwoic.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.tianlin.xyz/gtebjbgvwj.html

[L03] 设置自定义请求头
来源：http://hz.zhengqikj.top/gtlyfdwhrx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jyoumei.cn/gtadmmwlni.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ywan-chungtsiang.top/gtjxkdyxgh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuxming.cn/gtmmfpibkv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinqigufen.top/gtmzyogkpt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shanyushiyangkeji.top/gtxqpygqub.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhiwuduotai.top/gtnxucrfew.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yuxming.cn/gtwawovxub.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hnqzz.top/gthznbpszq.html

[L04] 设置超时
来源：http://hz.yongpay.top/gtsuqqgdun.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yuanzhike.top/gtakmjwqej.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.52xcode.cn/gtymsvqjjv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tanke756.top/gtofcuhecb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhiwuduotai.top/gtwypkdcrp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhoulong.xyz/gtamxidtyc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinghuilouyu.cn/gtslrkgxtj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jqgfzy.top/gtjgdzcbis.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yueranfly.top/gtwfoupkeh.html

[L05] 上传文件（multipart）
来源：http://hz.svipenyu.cn/gtmjetwbhl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.daxiang520.top/gtxjdbadad.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xylfe.cn/gtzrbmszko.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.sufxvd.cn/gtehvafczj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhiwuduotai.top/gtnzrbyqab.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xuetiantiany.cn/gtehvgbrcu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.daxiang520.top/gtxnwuoanz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ivvv.top/gtljbltsxf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cucudq.cn/gtrorkupqk.html

[L06] 解析响应为 JSON
来源：http://hz.hnxiangtu.top/gtiadhneav.html

Py:   resp.json()
来源：http://hz.c1oappe.top/gtgphtxsuh.html

PHP:  json_decode($body, true);
来源：http://hz.redwolf501.top/gtrmszmwbf.html

JS:   await resp.json()
来源：http://hz.wangshuangyany.cn/gtqilazywd.html

TS:   await resp.json()
来源：http://hz.sxryk.cn/gtoyoxmqka.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yanxiufei.cn/gtajeykmlo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yongpay.top/gtqtpatccr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.52xcode.cn/gthhscdcgp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ywan-chungtsiang.top/gtqyyudpng.html

[L07] 处理 HTTP 状态码
来源：http://hz.daria6918.cn/gtdwztsqpb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yj20258888.top/gtuizlmgnf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.feifeiyinyue.top/gtvinolxif.html

JS:   resp.ok;  resp.status
来源：http://hz.andypj.xyz/gtdkylyxyn.html

TS:   resp.ok;  resp.status
来源：http://hz.yj202588.top/gtrkgmtxww.html

Java: resp.statusCode()
来源：http://hz.ehwqpu.com/gtsugwnzbe.html

Go:   resp.StatusCode
来源：http://hz.sysykeji.top/gtmwndehab.html

Ruby: resp.code.to_i
来源：http://hz.gzhubu.top/gtunwqygfj.html

C#:   (int)resp.StatusCode
来源：http://hz.xylfe.cn/gttohfkbhc.html

[L08] 并发请求多个地址
来源：http://hz.jinqigufen.top/gtoyakvual.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yonumen.top/gtnhmlxesq.html

PHP:  curl_multi_init() 系列
来源：http://hz.gogol.net.cn/gtohqgnnvw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhijiandao.cn/gtggqrqdbp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cqqwz.cn/gtgotwvufe.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.0kj1m.cn/gtyrlgjhcd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ivvv.top/gtdrnfimlk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.fengsongda.top/gtxacjpgyr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhijiandao.cn/gtqbbnynxa.html

================================================================================
来源：http://hz.gaohongyu789.top/gtaiyrgsiq.html

M. 命令行 / 进程 / 环境
来源：http://hz.pycfn.com/gtaagdblgh.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtwiytjkib.html

[M01] 读取命令行参数
来源：http://hz.yueranfly.top/gtifmyojjw.html

Py:   sys.argv[1:]
来源：http://hz.xziqi.cn/gtivkbgemv.html

PHP:  $argv;  $argc;
来源：http://hz.zhengqikj.top/gtywgpwsmb.html

JS:   process.argv.slice(2)
来源：http://hz.hysaishi.cn/gtzsivtxmq.html

TS:   process.argv.slice(2)
来源：http://hz.smart0.xyz/gtcfshfvbu.html

Java: args 数组（main 方法参数）
来源：http://hz.yanxiufei.cn/gtuxphnpwk.html

Go:   os.Args[1:]
来源：http://hz.vqdsnc.cn/gtkytbeksd.html

Ruby: ARGV
来源：http://hz.sysykeji.top/gttoktuxin.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cdnleiting.top/gtlhcnaldb.html

[M02] 读取环境变量
来源：http://hz.cucudq.cn/gtyazorujy.html

Py:   os.environ.get("HOME")
来源：http://hz.hnxiangtu.top/gtlcnarbxi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jyoumei.cn/gtnzytljto.html

JS:   process.env.HOME
来源：http://hz.shanyushiyangtech.top/gtyzislxzu.html

TS:   process.env.HOME
来源：http://hz.cucudq.cn/gtugxrijll.html

Java: System.getenv("HOME")
来源：http://hz.hywenlv.cn/gtavwushln.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gotoacloud.top/gtxyoplrbm.html

Ruby: ENV["HOME"]
来源：http://hz.pycfn.com/gtshvwwwnd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ydzc1.top/gteyzpmurc.html

[M03] 执行外部命令
来源：http://hz.ehwqpu.com/gtghdhyfxy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shuidangran.top/gtvpqitnyn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.birdmap.top/gtdvtwyqef.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ehwqpu.com/gtogjklskp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.aibaodan.cn/gtnrlslkkw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hywenlv.cn/gtkreovdjb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cashguo.top/gtwkfganhh.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.aizwys.cn/gtkmkuaukh.html

C#:   Process.Start("ls", "-l");
来源：http://hz.9152youxi.cn/gtdytkcrvz.html

[M04] 获取当前工作目录
来源：http://hz.nanxuanxn.top/gtthnbaoul.html

Py:   os.getcwd()
来源：http://hz.hammf.cn/gtzhqehgfo.html

PHP:  getcwd();
来源：http://hz.jianghu66.top/gtqdanublu.html

JS:   process.cwd()
来源：http://hz.yvedp.cn/gtolcintbm.html

TS:   process.cwd()
来源：http://hz.fengsongda.top/gtcgnexsmj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.cqqwz.cn/gtoeshclfz.html

Go:   os.Getwd()
来源：http://hz.bjfxy.top/gttdstfzkd.html

Ruby: Dir.pwd
来源：http://hz.andypj.xyz/gtfwdsubyw.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.vqdsnc.cn/gthytzrolw.html

[M05] 设置退出码
来源：http://hz.jianghu66.top/gtfncbhbxd.html

Py:   sys.exit(1)
来源：http://hz.havefunace.top/gtquwkrwrl.html

PHP:  exit(1);
来源：http://hz.jqgufenzy.top/gtiehwnsyd.html

JS:   process.exit(1)
来源：http://hz.nwbrower.top/gtscirnqhk.html

TS:   process.exit(1)
来源：http://hz.zhengqikj.top/gtuafyuhjm.html

Java: System.exit(1)
来源：http://hz.ydjk.org.cn/gtmbrwsxfs.html

Go:   os.Exit(1)
来源：http://hz.fzhhl.top/gtmdcihyxj.html

Ruby: exit 1
来源：http://hz.shuidangran.top/gtroikyilg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yueranfly.top/gtkerdfkub.html

[M06] 向标准错误输出
来源：http://hz.tianlin.xyz/gtxwdoiqss.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yanxiufei.cn/gttfjvqzhq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.sweek.top/gtrkdykxxi.html

JS:   console.error("err")
来源：http://hz.shanyushiyangkeji.top/gtivfhrxio.html

TS:   console.error("err")
来源：http://hz.hongshengwenyu.top/gtiwaprqgh.html

Java: System.err.println("err")
来源：http://hz.dashuyun.cn/gtftzvyybw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhoulong.xyz/gttlhdgdbq.html

Ruby: warn "err"
来源：http://hz.chenjidiqi.icu/gtplajrnea.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cashguo.top/gtbwoabxzk.html

[M07] 判断是否为主入口
来源：http://hz.yj202588.top/gtrjkfwokh.html

Py:   if __name__ == "__main__":
来源：http://hz.quarkkingdee.top/gtvfqqwqph.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.birdmap.top/gtmuxcvzvf.html

JS:   require.main === module
来源：http://hz.zycfv.cn/gtxrdwgqkx.html

TS:   require.main === module
来源：http://hz.ydjk.org.cn/gtifehzgua.html

Java: public static void main(String[] args)
来源：http://hz.ydzc1.top/gtosljzyen.html

Go:   func main()
来源：http://hz.zhijiandao.cn/gtraqxceeq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.dianchejie.cn/gtqliuukka.html

C#:   static void Main(string[] args)
来源：http://hz.c1oappe.top/gtfvgdchrn.html

[M08] 获取系统与运行时信息
来源：http://hz.aibaodan.cn/gtxfskkkju.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yanxiufei.cn/gtjyqzxpyn.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.bjfxy.top/gtsysmrrno.html

JS:   process.platform;  process.version
来源：http://hz.haohaochexian.top/gtrmrwbrvc.html

TS:   process.platform;  process.version
来源：http://hz.yanxiufei.cn/gtkectmgde.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xuanzx.com/gtzqkxyhqx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yongpay.top/gtuuyggwoc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hnxiangtu.top/gtaeuwwisf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xinyue.icu/gthtwbbmtw.html

================================================================================
来源：http://hz.jiagoushi.top/gtvcylhzvc.html

N. 数据结构与算法
来源：http://hz.chenzaomai.com/gtimpteokj.html

================================================================================
来源：http://hz.jqgufenzy.top/gtxnolgeft.html

[N01] 二分查找（有序数组）
来源：http://hz.shzxlz.cn/gtfaygztyt.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.wangshuangyany.cn/gtqfxdclwe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zdqjudy.top/gtocwbsuxb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fengsongda.top/gtneqnughf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jiagoushi.top/gtfvvmzwwn.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xuetiantiany.cn/gtvgfzntya.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hywenlv.cn/gtjxzatxqv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.cashguo.top/gtvrywguby.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shanyushiyangkeji.top/gtiggimdls.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cqqwz.cn/gthtijynej.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.pengpengdd.cyou/gtzafouinx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.gotoacloud.top/gtodbsegcj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cheryme.top/gtyyutqdne.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.snrcjt.cn/gttcbpjida.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.316326.xyz/gttfcqutzm.html

Go:   slices.Sort(arr)
来源：http://hz.chenlongwang.top/gtlzshswus.html

Ruby: arr.sort
来源：http://hz.yvedp.cn/gtscgmnocs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cucudq.cn/gtdfceulhn.html

[N03] 快速排序（分治示例）
来源：http://hz.yueranfly.top/gteodohlmz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yangfankeji.com/gtftnlwlua.html

PHP:  // 递归实现，或用 usort
来源：http://hz.guowangkeji.top/gtghbdfwfd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jiagoushi.top/gtjeudaftf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgufenzy.top/gtztiruzaj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yvedp.cn/gtflxdsavf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.nanxinkj.top/gtnfcprpen.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.dashuyun.cn/gtjboseuuj.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yuanzhike.top/gtxktjhhyp.html

[N04] 斐波那契数列
来源：http://hz.xingfuxueyuan.xyz/gttaarkmbu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hongshengwenyu.top/gtlsxjupdu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xylfe.cn/gtjieiorkp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigfzy.top/gtycraxzuk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shanyushiyangkeji.top/gtlbwaapkk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhaomingkeji.xyz/gthxustsbd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.daxiang520.top/gtibunpbco.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.shanyushiyangtech.top/gtlyagbrse.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.wangshuangyany.cn/gtyrtokxfn.html

[N05] 最大公约数
来源：http://hz.shzxlz.cn/gtraycnigc.html

Py:   math.gcd(a, b)
来源：http://hz.c1oappe.top/gtelhtfwel.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.bjfxy.top/gtauuxhxzn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnqzz.top/gtyhhqnxth.html


<!-- 参考信息 -->