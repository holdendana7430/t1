代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://hz.jiagoushi.top/gtznomlqbd.html

[J08] 提取年月日与星期
来源：http://hz.mhx1999.top/gtszluydpu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hongshengwenyu.top/gtltpmkiql.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ydjk.org.cn/gtyryojfdd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.snrcjt.cn/gtignphtdp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sxryk.cn/gthdynssrv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.wangdashe.top/gtmwwlpsqe.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jqgufenzy.top/gtesykxebl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.meibo888.top/gtsvlomswj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.cashguo.top/gtogehdqth.html

[J09] 时区处理
来源：http://hz.shanyushiyangtech.top/gtxbskkeud.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yj20258.top/gtmuofrspp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.c1oappe.top/gttmctbkqt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sweek.top/gtjdwivfrd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dianchejie.cn/gtojduphhu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cheryme.top/gtczbmmuje.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cucudq.cn/gtwcullijp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yonumen.top/gtnfpcmiyp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zycfv.cn/gtdugqxbza.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhijiandao.cn/gtraztwoln.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cashguo.top/gtxoiiplcn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yuxming.cn/gtnqsyqyfu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gotoacloud.top/gtkseotndg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yonumen.top/gtcifvyxqi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.wangdashe.top/gttlaeqlmx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cdnleiting.top/gtkndyevif.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.vqdsnc.cn/gtvwmofjrp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.andypj.xyz/gtcdtktmoo.html

================================================================================
来源：http://hz.yj20258888.top/gtxenfnkfc.html

K. JSON 与序列化
来源：http://hz.yueranfly.top/gtprxgyfxx.html

================================================================================
来源：http://hz.xylfe.cn/gtuzufmllu.html

[K01] 对象转 JSON 字符串
来源：http://hz.xziqi.cn/gtpexiyccl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xylfe.cn/gtryovtztu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jqgufenzy.top/gtlsckytla.html

JS:   JSON.stringify(obj)
来源：http://hz.ppjwa.cn/gtguwycogq.html

TS:   JSON.stringify(obj)
来源：http://hz.pycfn.com/gtwrknjzdd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hongshengwenyu.top/gtqesfdusj.html

Go:   json.Marshal(obj)
来源：http://hz.ydzc1.top/gtasovscyf.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xinyue.icu/gtrstuoovj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.fzhhl.top/gttsctpgwh.html

[K02] JSON 字符串转对象
来源：http://hz.316326.xyz/gtfywfveuk.html

Py:   json.loads(s)
来源：http://hz.jinghuilouyu.cn/gtrdiafkzw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shuidangran.top/gtcqwyhkoi.html

JS:   JSON.parse(s)
来源：http://hz.shangyingyoupin.top/gtwyvypkzd.html

TS:   JSON.parse(s)
来源：http://hz.zhongyouzk.top/gtnrxrxuuw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.aizwys.cn/gtzntixstj.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xinyue.icu/gtesimeogz.html

Ruby: JSON.parse(s)
来源：http://hz.chenjidiqi.icu/gtknjhloic.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ydjk.org.cn/gthdnryruf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhaomingkeji.xyz/gtebbslohn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jqgfzy.top/gtgpbodaxx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.tanke756.top/gtexygoyse.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhengqikj.top/gtzcpdyfli.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.gaohongyu789.top/gtzhqtlalp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cashguo.top/gtuwozpsyy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.chenlongwang.top/gtaiujglyl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nanxuanxn.top/gtfkjdxdmx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jqgfzy.top/gtxexpater.html

[K04] 读取 JSON 文件
来源：http://hz.yongpay.top/gtrcyazftf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xuetiantiany.cn/gtymjxjxrz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yueranfly.top/gtqzkihubt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigfzy.top/gtkjwkwxwj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sxryk.cn/gtwuzifvlh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sufxvd.cn/gthaokfdak.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hnxiangtu.top/gtisrxukif.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.nanxinkj.top/gtqeuzqyql.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhiwuduotai.top/gtcawwnrzz.html

[K05] 深拷贝对象
来源：http://hz.zhaomingkeji.xyz/gtvotduyjf.html

Py:   copy.deepcopy(obj)
来源：http://hz.yangfankeji.com/gtyqxxxlim.html

PHP:  unserialize(serialize($obj));
来源：http://hz.gotoacloud.top/gtzxvewknj.html

JS:   structuredClone(obj)
来源：http://hz.yvedp.cn/gthnhxitbb.html

TS:   structuredClone(obj)
来源：http://hz.316326.xyz/gtxdnzcvoz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.52xcode.cn/gtdlxsfwmg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hnxiangtu.top/gtsjecfbhi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ydzc1.top/gtjnlgzixy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ydzc1.top/gtwywrzzsf.html

[K06] 解析 URL 查询串
来源：http://hz.yangfankeji.com/gtlseqelja.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xuanzx.com/gtmiihbeqr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cqqwz.cn/gtfzpnprkn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinghuilouyu.cn/gtwmxseqzx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhijiandao.cn/gtcvlqsvpu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.redwolf501.top/gttokitdqq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cucudq.cn/gthqkktuon.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.dianchejie.cn/gtykoaqbxa.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.wangdashe.top/gtmkjieayx.html

[K07] 进制转换
来源：http://hz.52xcode.cn/gtjdfsthlb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.fzhhl.top/gttsumuuzj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.nanxinkj.top/gtcakxjhbx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtlnofhbil.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.birdmap.top/gtsidqewow.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zycfv.cn/gtqqhaafgu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xinyue.icu/gtnazliuzl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.chenlongwang.top/gttswfesqr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yanxiufei.cn/gtrnpibewa.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shanyushiyangkeji.top/gttvjkrzne.html

Py:   pickle.dumps(obj)
来源：http://hz.hywenlv.cn/gtxtwyxuqj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.wangdashe.top/gtdazckvex.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.mhx1999.top/gtlrmtdgwo.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.chenjidiqi.icu/gtifpnitie.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.feifeiyinyue.top/gtzvaeiytr.html

Go:   encoding/gob
来源：http://hz.yanxiufei.cn/gtmjlxuoxk.html

Ruby: Marshal.dump(obj)
来源：http://hz.ybcxt.top/gtmmsdvzft.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gotoacloud.top/gtkdybzkhu.html

================================================================================
来源：http://hz.birdmap.top/gtgaovmoli.html

L. 网络请求
来源：http://hz.vqdsnc.cn/gtlwiaebia.html

================================================================================
来源：http://hz.snrcjt.cn/gtjvusueno.html

[L01] 发送 GET 请求
来源：http://hz.tianlin.xyz/gtlhctcqxd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ehwqpu.com/gtqxwvgupw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jyoumei.cn/gtfazycgyz.html

JS:   await fetch(url)
来源：http://hz.wangdashe.top/gtstuwikxb.html

TS:   await fetch(url)
来源：http://hz.ydzc1.top/gtsvazzdqt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.haohaochexian.top/gtixnpprik.html

Go:   resp, err := http.Get(url)
来源：http://hz.jqgufenzy.top/gtzucrozun.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jianghu66.top/gtdwsxxylb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.316326.xyz/gtpxzgickz.html

[L02] 发送 POST JSON
来源：http://hz.jiagoushi.top/gtlcrueybo.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ehwqpu.com/gtvbpleprj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hnqzz.top/gtchgbnjar.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zdqjudy.top/gtvyyzvnce.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.aizwys.cn/gtkawiprwd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.haohaochexian.top/gtddtnkqsj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yvedp.cn/gtkotepjah.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.chenzaomai.com/gtzxoijsvk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xylfe.cn/gtdbmxlijh.html

[L03] 设置自定义请求头
来源：http://hz.ppjwa.cn/gtetguoqgd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.316326.xyz/gtynufovje.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sxryk.cn/gtsjuxzdky.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.iojbl.cn/gtamcclfwa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj202588.top/gtmqhyhjqa.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sxryk.cn/gtwzelvjxx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.nanxuanxn.top/gtqspqkzaa.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhengqikj.top/gtwmlgherv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yj20258.top/gtcznrvvkl.html

[L04] 设置超时
来源：http://hz.wangdashe.top/gtqhzzkchp.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yj202588.top/gtwxepyxqz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.quarkkingdee.top/gtanatdruk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.feifeiyinyue.top/gtiykwqgjs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hongshengwenyu.top/gtkvctrfob.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yuanzhike.top/gtdbvtivjt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.nanxuanxn.top/gtcynqvxoh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.chenzaomai.com/gtrqvhfayn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yuanzhike.top/gtszajxoae.html

[L05] 上传文件（multipart）
来源：http://hz.316326.xyz/gtggpmcaxc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinqigfzy.top/gtgdhlsmzf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hnqzz.top/gtybnahqdw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.tian-w.cn/gtpppavnhv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgufenzy.top/gtcbghnypy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhaomingkeji.xyz/gtznuzgxsv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zycfv.cn/gtbkrmnecr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.pengpengdd.cyou/gtiwdppglg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhiwuduotai.top/gtmpgznkvf.html

[L06] 解析响应为 JSON
来源：http://hz.birdmap.top/gtsmkzhraj.html

Py:   resp.json()
来源：http://hz.shanyushiyangtech.top/gtqxmiiewl.html

PHP:  json_decode($body, true);
来源：http://hz.tanke756.top/gtgydzcqdj.html

JS:   await resp.json()
来源：http://hz.guowangkeji.top/gtxuaarfmx.html

TS:   await resp.json()
来源：http://hz.zycfv.cn/gtihsoirlz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhiwuduotai.top/gtqingsaos.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ybcxt.top/gtmkbdzrad.html

Ruby: JSON.parse(resp.body)
来源：http://hz.pycfn.com/gtujlvxdyx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.0kj1m.cn/gtyvzfloby.html

[L07] 处理 HTTP 状态码
来源：http://hz.wangshuangyany.cn/gtqezmzebu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.c1oappe.top/gtpsgrpgdc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.dianchejie.cn/gtgvjedyis.html

JS:   resp.ok;  resp.status
来源：http://hz.jinqigufen.top/gtigusbvjq.html

TS:   resp.ok;  resp.status
来源：http://hz.aizwys.cn/gtkmfyxlgt.html

Java: resp.statusCode()
来源：http://hz.hammf.cn/gtmuugtoei.html

Go:   resp.StatusCode
来源：http://hz.xziqi.cn/gtdvomfqnn.html

Ruby: resp.code.to_i
来源：http://hz.daxiang520.top/gtjcfuliac.html

C#:   (int)resp.StatusCode
来源：http://hz.hammf.cn/gtlzbhgfmo.html

[L08] 并发请求多个地址
来源：http://hz.hnqzz.top/gtfyufjteb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.bjfxy.top/gtmnprhgjd.html

PHP:  curl_multi_init() 系列
来源：http://hz.cdnleiting.top/gtsovwfebc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenzaomai.com/gtkogotzxb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cucudq.cn/gtysklzxyz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.pengpengdd.cyou/gtwousdwfh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zdqjudy.top/gteppqfmno.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hammf.cn/gtvdecddio.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xziqi.cn/gtfpbxoqlt.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtomgfdewu.html

M. 命令行 / 进程 / 环境
来源：http://hz.sxryk.cn/gtvobkjcze.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtbfgtpumr.html

[M01] 读取命令行参数
来源：http://hz.snrcjt.cn/gtnrmoexhn.html

Py:   sys.argv[1:]
来源：http://hz.yanxiufei.cn/gtkzuwdpia.html

PHP:  $argv;  $argc;
来源：http://hz.chenzaomai.com/gtugrimdqj.html

JS:   process.argv.slice(2)
来源：http://hz.xuanzx.com/gtucrjgecl.html

TS:   process.argv.slice(2)
来源：http://hz.andypj.xyz/gtbmjkphre.html

Java: args 数组（main 方法参数）
来源：http://hz.hysaishi.cn/gtefdkycod.html

Go:   os.Args[1:]
来源：http://hz.c1oappe.top/gtqpogdlnn.html

Ruby: ARGV
来源：http://hz.c1oappe.top/gtqngugtyl.html

C#:   args 数组（Main 方法参数）
来源：http://hz.nwbrower.top/gtrcnyhvdy.html

[M02] 读取环境变量
来源：http://hz.vqdsnc.cn/gtjtncgfca.html

Py:   os.environ.get("HOME")
来源：http://hz.daxiang520.top/gtnpppmgfa.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.wangshuangyany.cn/gtjsdijxxt.html

JS:   process.env.HOME
来源：http://hz.quarkkingdee.top/gtwdyzzbko.html

TS:   process.env.HOME
来源：http://hz.yj20258.top/gteioqliar.html

Java: System.getenv("HOME")
来源：http://hz.jianghu66.top/gtpfihzmrh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.kuanghao11.cn/gtwyyklnio.html

Ruby: ENV["HOME"]
来源：http://hz.jqgfzy.top/gtycjfxzzn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gzhubu.top/gtimlfarts.html

[M03] 执行外部命令
来源：http://hz.jinghuilouyu.cn/gtdvkckfrc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.chenzaomai.com/gtifwokupw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yj202588.top/gtbujrvwcz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cdnleiting.top/gtjwrexcqf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinyuanbaomall.cn/gthwfbyukf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yuxming.cn/gtolmvpknl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.redwolf501.top/gtrzfjspqm.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhixingplan.top/gtzlnvwrwf.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yangfankeji.com/gttbepzccr.html

[M04] 获取当前工作目录
来源：http://hz.jiagoushi.top/gtxmisrfwd.html

Py:   os.getcwd()
来源：http://hz.fzhhl.top/gtbcpolaac.html

PHP:  getcwd();
来源：http://hz.tanke756.top/gtzghcbldj.html

JS:   process.cwd()
来源：http://hz.wangshuangyany.cn/gtzbbfovdm.html

TS:   process.cwd()
来源：http://hz.ppjwa.cn/gtakobyejw.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xziqi.cn/gtdvekjxmo.html

Go:   os.Getwd()
来源：http://hz.chenjidiqi.icu/gtfthmidyl.html

Ruby: Dir.pwd
来源：http://hz.wangshuangyany.cn/gtxvkzxadf.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.aibaodan.cn/gtewggdgzq.html

[M05] 设置退出码
来源：http://hz.zhixingplan.top/gtohrsejtk.html

Py:   sys.exit(1)
来源：http://hz.jinghuilouyu.cn/gtpirwwbek.html

PHP:  exit(1);
来源：http://hz.guowangkeji.top/gtqjrbdigp.html

JS:   process.exit(1)
来源：http://hz.zhaomingkeji.xyz/gtrdcmzdkf.html

TS:   process.exit(1)
来源：http://hz.nwbrower.top/gttcdbqqnm.html

Java: System.exit(1)
来源：http://hz.shanyushiyangtech.top/gtdalfinfv.html

Go:   os.Exit(1)
来源：http://hz.ywan-chungtsiang.top/gtmqhjtspx.html

Ruby: exit 1
来源：http://hz.zhiwuduotai.top/gtnzouocae.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.daxiang520.top/gtfumqfdlo.html

[M06] 向标准错误输出
来源：http://hz.pengpengdd.cyou/gtvtngcgsm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.chenlongwang.top/gthvnjwcyc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.quarkkingdee.top/gtwgiblnvo.html

JS:   console.error("err")
来源：http://hz.bjfxy.top/gtjqwybivx.html

TS:   console.error("err")
来源：http://hz.0kj1m.cn/gteuaeevat.html

Java: System.err.println("err")
来源：http://hz.yangfankeji.com/gtzpyxddfa.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cucudq.cn/gtobsmwsel.html

Ruby: warn "err"
来源：http://hz.shanyushiyangtech.top/gtijvbyyal.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.iojbl.cn/gtqpnctyhc.html

[M07] 判断是否为主入口
来源：http://hz.nanxinkj.top/gtcknkktod.html

Py:   if __name__ == "__main__":
来源：http://hz.redwolf501.top/gtogujbljm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cucudq.cn/gtqzecyrdc.html

JS:   require.main === module
来源：http://hz.cqqwz.cn/gtvkogxrwd.html

TS:   require.main === module
来源：http://hz.birdmap.top/gtibxczcaf.html

Java: public static void main(String[] args)
来源：http://hz.dashuyun.cn/gtfmcsetob.html

Go:   func main()
来源：http://hz.zdqjudy.top/gtotzxoptu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xingfuxueyuan.xyz/gttqnryeen.html

C#:   static void Main(string[] args)
来源：http://hz.nanxuanxn.top/gtpvhtkccl.html

[M08] 获取系统与运行时信息
来源：http://hz.wangshuangyany.cn/gtbdiqsezw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.0kj1m.cn/gtdxsvhsts.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.gogol.net.cn/gtywvulqqr.html

JS:   process.platform;  process.version
来源：http://hz.jinqigfzy.top/gtdiodlxjx.html

TS:   process.platform;  process.version
来源：http://hz.yueranfly.top/gtkrpmwkyr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhaomingkeji.xyz/gtwreumocc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinyuanbaomall.cn/gtthvbxgnz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.svipenyu.cn/gtfgpjbknt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hnxiangtu.top/gtuveflqnc.html

================================================================================
来源：http://hz.haohaochexian.top/gtbigamwkz.html

N. 数据结构与算法
来源：http://hz.shangyingyoupin.top/gtmuibbrjo.html

================================================================================
来源：http://hz.shzxlz.cn/gtjlljdysf.html

[N01] 二分查找（有序数组）
来源：http://hz.yuxming.cn/gtjnjpfhqg.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jiagoushi.top/gtjofcrmgi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hongshengwenyu.top/gtprpywmeb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.smart0.xyz/gtrvervevl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258888.top/gtigqmrqfm.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ivvv.top/gtecszqppn.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.sufxvd.cn/gtptgkiymt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xinyue.icu/gtcevklimb.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shanyushiyangtech.top/gtwotwrqhm.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.birdmap.top/gtngyugvne.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sufxvd.cn/gtrogycbhi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.guowangkeji.top/gtgpfkvcxp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xingfuxueyuan.xyz/gtpqbqvrez.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenzaomai.com/gtlqefnokt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.daxiang520.top/gtxoamvkzg.html

Go:   slices.Sort(arr)
来源：http://hz.havefunace.top/gtcqkvwotx.html

Ruby: arr.sort
来源：http://hz.zdqjudy.top/gtgpeuwjtk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shangyingyoupin.top/gtgigvggij.html

[N03] 快速排序（分治示例）
来源：http://hz.meibo888.top/gtyrjvqoty.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ppjwa.cn/gttzpocqkj.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zdqjudy.top/gthhriqozp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangshuangyany.cn/gtvzpsceti.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhiwuduotai.top/gtmucokigf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhaomingkeji.xyz/gtzallbpoj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jiagoushi.top/gtibnnpbdb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.0kj1m.cn/gtlkwpmfwx.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gzhubu.top/gttalektve.html

[N04] 斐波那契数列
来源：http://hz.0kj1m.cn/gtjceckbzw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jqgfzy.top/gtnuirfham.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cucudq.cn/gtshxgsxvp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shzxlz.cn/gtlonpiuhx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jlsjyb.cn/gttdluhpdf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hysaishi.cn/gtztypvxcb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yangfankeji.com/gteqhebgdi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhongyouzk.top/gtgpltupwc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.wangdashe.top/gtxbjyqwxb.html

[N05] 最大公约数
来源：http://hz.hongshengwenyu.top/gtmbdwnzym.html

Py:   math.gcd(a, b)
来源：http://hz.pengpengdd.cyou/gtyyqzlute.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jianghu66.top/gtdhtwrnuy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yonumen.top/gtwdiarcjy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tanke756.top/gtbuimjisd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shuidangran.top/gtuiblmola.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hywenlv.cn/gtdyhhiexn.html

Ruby: a.gcd(b)
来源：http://hz.xziqi.cn/gthvdpafqf.html


<!-- 参考信息 -->