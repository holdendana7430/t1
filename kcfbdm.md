代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.redwolf501.top/gthngmjpfm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinyuanbaomall.cn/gtsngnglhx.html

[J09] 时区处理
来源：http://hz.daxiang520.top/gtofxjxjmf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.tianlin.xyz/gtfatwbxpv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jiagoushi.top/gtorltrrnd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hfpthk.cn/gtaprhdgmw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.meibo888.top/gtvztashgu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.daxiang520.top/gtyqjdhiex.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xingfuxueyuan.xyz/gtadmvujln.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ydjk.org.cn/gtuqouypsf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.guowangkeji.top/gtdndpuucr.html

[J10] 取今天 / 本月第一天
来源：http://hz.snrcjt.cn/gtyhqqkhho.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hfpthk.cn/gtvugnwumb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.tian-w.cn/gtxfalislg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.quarkkingdee.top/gtfansxsod.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.chenlongwang.top/gtxqxsheqi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.tanke756.top/gtdbtjkalb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.birdmap.top/gtalqvbmww.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xziqi.cn/gtdfrzaafi.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cdnleiting.top/gtkxsiwbds.html

================================================================================
来源：http://hz.dianchejie.cn/gtvxxejezh.html

K. JSON 与序列化
来源：http://hz.hammf.cn/gtwmjrywrr.html

================================================================================
来源：http://hz.c1oappe.top/gthzwamypm.html

[K01] 对象转 JSON 字符串
来源：http://hz.ydzc1.top/gthniihcgm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shangyingyoupin.top/gtfjudrocx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tianlin.xyz/gttwrdhpal.html

JS:   JSON.stringify(obj)
来源：http://hz.yj20258.top/gtvedryizd.html

TS:   JSON.stringify(obj)
来源：http://hz.svipenyu.cn/gtxsofbltg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hnxiangtu.top/gtydrsewud.html

Go:   json.Marshal(obj)
来源：http://hz.jlsjyb.cn/gtfqdoyqpo.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sufxvd.cn/gtxenyrynt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cqqwz.cn/gtsrnzytxz.html

[K02] JSON 字符串转对象
来源：http://hz.zhongyouzk.top/gthqztzjyt.html

Py:   json.loads(s)
来源：http://hz.nanxinkj.top/gtikdbuzty.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yongpay.top/gtvabtbowz.html

JS:   JSON.parse(s)
来源：http://hz.snrcjt.cn/gtkdgbrxwg.html

TS:   JSON.parse(s)
来源：http://hz.gzhubu.top/gteokttrnd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jianghu66.top/gtfcmmxjeu.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gotoacloud.top/gtaazbvrox.html

Ruby: JSON.parse(s)
来源：http://hz.xziqi.cn/gtwmuetjlw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhongyouzk.top/gtnyhyyilh.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.shzxlz.cn/gtoaoijbrj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hnqzz.top/gtjbassnmb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.aizwys.cn/gthhzagioy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hongshengwenyu.top/gtsygqgavf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.smart0.xyz/gtwgrnfido.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hnxiangtu.top/gtjbijxzjh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ydjk.org.cn/gtjbldbwul.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jinqigfzy.top/gtrewcnjiy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.0kj1m.cn/gtfcynbvhr.html

[K04] 读取 JSON 文件
来源：http://hz.bjfxy.top/gtymjkbbfg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.c1oappe.top/gtqeylbdih.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xingfuxueyuan.xyz/gtadsxixlj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenjidiqi.icu/gtfipxrzsw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.wangshuangyany.cn/gtlzdphwzy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhongyouzk.top/gtmjylkepu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hywenlv.cn/gtlkwzoqqg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.wangdashe.top/gtjxdtzjcr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhongyouzk.top/gtvmtusdci.html

[K05] 深拷贝对象
来源：http://hz.chenlongwang.top/gthexmzwqe.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinqigfzy.top/gtxinyjbub.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jianghu66.top/gtfaopmbrn.html

JS:   structuredClone(obj)
来源：http://hz.jinyuanbaomall.cn/gtqwfmxitw.html

TS:   structuredClone(obj)
来源：http://hz.zhijiandao.cn/gtzhqwjgjr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jiagoushi.top/gtnuuttqyf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.fengsongda.top/gtvrbyqyoz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.snrcjt.cn/gtqyhcrcdu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.snrcjt.cn/gtrymjggrh.html

[K06] 解析 URL 查询串
来源：http://hz.jianghu66.top/gtgdzadvmg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.quarkkingdee.top/gtpyyphxoy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhongyouzk.top/gtepkntqoi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.daxiang520.top/gtashrzuzg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.redwolf501.top/gtkqoqcpmt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jqgfzy.top/gtyzaxgmyc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhijiandao.cn/gtfgoofajj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.quarkkingdee.top/gtkwcvklri.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinqigufen.top/gticgsjtsl.html

[K07] 进制转换
来源：http://hz.nanxuanxn.top/gtytdmsvqq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtiuqyjdqb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jinghuilouyu.cn/gtdaewdlyo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ivvv.top/gtpynlhhdc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.birdmap.top/gtupdlptwc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ybcxt.top/gtamkkzetj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nanxuanxn.top/gtmcrodebn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.aizwys.cn/gtuloxvraw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.andypj.xyz/gtobppdbkv.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.dianchejie.cn/gtkkxzzkph.html

Py:   pickle.dumps(obj)
来源：http://hz.xinyue.icu/gtjxyscwih.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.dashuyun.cn/gtvpxdrtxu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hnqzz.top/gtlnnswjkn.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.chenjidiqi.icu/gtsctcrihx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenjidiqi.icu/gtuoczlwyv.html

Go:   encoding/gob
来源：http://hz.daxiang520.top/gtrychntew.html

Ruby: Marshal.dump(obj)
来源：http://hz.gotoacloud.top/gtgxuokdpb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yanxiufei.cn/gtegtbcija.html

================================================================================
来源：http://hz.yj202588.top/gtfzvnzpqw.html

L. 网络请求
来源：http://hz.snrcjt.cn/gtrugkkhie.html

================================================================================
来源：http://hz.ybcxt.top/gtgymdwxnf.html

[L01] 发送 GET 请求
来源：http://hz.fengsongda.top/gtijfnfazr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yangfankeji.com/gtupsoaxir.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhengqikj.top/gtkdftphcd.html

JS:   await fetch(url)
来源：http://hz.yangfankeji.com/gtjqrbapgv.html

TS:   await fetch(url)
来源：http://hz.hnqzz.top/gtzjotrejg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zycfv.cn/gtlmullfkw.html

Go:   resp, err := http.Get(url)
来源：http://hz.hnxiangtu.top/gtaomeifje.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jianghu66.top/gtlabidvpn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhiwuduotai.top/gtydmsihpc.html

[L02] 发送 POST JSON
来源：http://hz.jianghu66.top/gtkbepijxh.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.tanke756.top/gtoelwvlrc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hnqzz.top/gtwshkwzmd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258888.top/gtlmrxdzcl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shuidangran.top/gtttbjzjxn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.pengpengdd.cyou/gtjczlnhhf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ybcxt.top/gteswlprbk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.guannengcc.top/gtckzanfik.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.wangdashe.top/gtpelwslov.html

[L03] 设置自定义请求头
来源：http://hz.hywenlv.cn/gtkylrkwqx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhoulong.xyz/gtlfibskse.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.pengpengdd.cyou/gtfggwljiv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuanzx.com/gtzimertbb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhoulong.xyz/gtfxohkyhf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yangfankeji.com/gtwbstbckx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ehwqpu.com/gthhznmbeg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yuanzhike.top/gtmrkisqdg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.sysykeji.top/gtzprbkhwe.html

[L04] 设置超时
来源：http://hz.wangdashe.top/gtwmdcratb.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jinghuilouyu.cn/gtpwmyjnvo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hywenlv.cn/gtyhbdpvar.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yueranfly.top/gtlzbdrggk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yonumen.top/gtsvevlwsx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.0kj1m.cn/gtpeizbqzu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj20258.top/gtinhvkunw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.mhx1999.top/gtjnbfdfie.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xziqi.cn/gtaegcevbn.html

[L05] 上传文件（multipart）
来源：http://hz.xylfe.cn/gtajtvjmfm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yj202588.top/gtgrkuvqjk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.gzhubu.top/gtujseshzn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shuidangran.top/gtsyggrhgy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgufenzy.top/gtldvjhgmi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.snrcjt.cn/gtfzkgpsot.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yonumen.top/gtbeagbmlo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.fengsongda.top/gtjyzwueaa.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.guowangkeji.top/gtxbdsmnjw.html

[L06] 解析响应为 JSON
来源：http://hz.jinyuanbaomall.cn/gtdpbzjpez.html

Py:   resp.json()
来源：http://hz.52xcode.cn/gtaeguyhue.html

PHP:  json_decode($body, true);
来源：http://hz.tian-w.cn/gtsjdlxfyn.html

JS:   await resp.json()
来源：http://hz.chenzaomai.com/gtybjtxhns.html

TS:   await resp.json()
来源：http://hz.zhengqikj.top/gtwkbyzatn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhiwuduotai.top/gtiuaoficc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.andypj.xyz/gtzyptsvog.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cqqwz.cn/gtxgyckmgq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.fengsongda.top/gtxhgboxsy.html

[L07] 处理 HTTP 状态码
来源：http://hz.iojbl.cn/gtzvmdnwvn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ydzc1.top/gtfwybuqcx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinqigufen.top/gtpnlkioyf.html

JS:   resp.ok;  resp.status
来源：http://hz.gotoacloud.top/gtubeadwll.html

TS:   resp.ok;  resp.status
来源：http://hz.shangyingyoupin.top/gtxqbtojzs.html

Java: resp.statusCode()
来源：http://hz.pycfn.com/gtqnkeflqi.html

Go:   resp.StatusCode
来源：http://hz.cqqwz.cn/gtcuyarjpb.html

Ruby: resp.code.to_i
来源：http://hz.xinyue.icu/gtsvkboqju.html

C#:   (int)resp.StatusCode
来源：http://hz.iojbl.cn/gtrmvybbjs.html

[L08] 并发请求多个地址
来源：http://hz.zhongyouzk.top/gtdufvfguk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yueranfly.top/gtlarbjnae.html

PHP:  curl_multi_init() 系列
来源：http://hz.sufxvd.cn/gtrterpzmy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fengsongda.top/gtajwiwrnw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nwbrower.top/gtzijyvdrp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.0kj1m.cn/gtgwgalzgq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.nanxinkj.top/gtemobvdwe.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hnqzz.top/gtdgmdwkiy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhiwuduotai.top/gtjqyimfwi.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtlxdpiqkl.html

M. 命令行 / 进程 / 环境
来源：http://hz.nwbrower.top/gtrnjahong.html

================================================================================
来源：http://hz.yanxiufei.cn/gtzxttdwev.html

[M01] 读取命令行参数
来源：http://hz.sweek.top/gtqgljosyh.html

Py:   sys.argv[1:]
来源：http://hz.andypj.xyz/gtzyryyoff.html

PHP:  $argv;  $argc;
来源：http://hz.zycfv.cn/gtamotvxwz.html

JS:   process.argv.slice(2)
来源：http://hz.c1oappe.top/gtdnnofqbo.html

TS:   process.argv.slice(2)
来源：http://hz.zycfv.cn/gtrjkiorld.html

Java: args 数组（main 方法参数）
来源：http://hz.xuanzx.com/gtcgsegrpm.html

Go:   os.Args[1:]
来源：http://hz.nwbrower.top/gtvqtgdvmf.html

Ruby: ARGV
来源：http://hz.0kj1m.cn/gtgdsdzawn.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yuxming.cn/gtsatwgfxg.html

[M02] 读取环境变量
来源：http://hz.sxryk.cn/gtrkyzyqla.html

Py:   os.environ.get("HOME")
来源：http://hz.smart0.xyz/gtwuphhwvb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinqigfzy.top/gtadrljkag.html

JS:   process.env.HOME
来源：http://hz.hongshengwenyu.top/gtvfvmrduf.html

TS:   process.env.HOME
来源：http://hz.snrcjt.cn/gtjgtkotqx.html

Java: System.getenv("HOME")
来源：http://hz.hongshengwenyu.top/gtqylbtxai.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhaomingkeji.xyz/gtubsuxtgb.html

Ruby: ENV["HOME"]
来源：http://hz.yangfankeji.com/gtewpqescz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gzhubu.top/gthbahasvg.html

[M03] 执行外部命令
来源：http://hz.cqqwz.cn/gtgtqjlcyz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hongshengwenyu.top/gtrmqthmik.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.snrcjt.cn/gtypgrvlih.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hongshengwenyu.top/gtudqfuzlw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ivvv.top/gtfrkccxdc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhijiandao.cn/gtmljibmzv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhiwuduotai.top/gtdgveejxk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shanyushiyangtech.top/gtlaoazjvt.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gogol.net.cn/gtvouswqty.html

[M04] 获取当前工作目录
来源：http://hz.xylfe.cn/gtqtwkolsj.html

Py:   os.getcwd()
来源：http://hz.hfpthk.cn/gtcxbbmqga.html

PHP:  getcwd();
来源：http://hz.guannengcc.top/gtttbabhjs.html

JS:   process.cwd()
来源：http://hz.yvedp.cn/gtknhfbyui.html

TS:   process.cwd()
来源：http://hz.yj202588.top/gtagshjveh.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yonumen.top/gtyetywgcf.html

Go:   os.Getwd()
来源：http://hz.hnqzz.top/gtheanyrop.html

Ruby: Dir.pwd
来源：http://hz.9152youxi.cn/gtbeoeftts.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.aibaodan.cn/gtmuqkifvt.html

[M05] 设置退出码
来源：http://hz.hywenlv.cn/gtlrbxiigt.html

Py:   sys.exit(1)
来源：http://hz.sweek.top/gtwbpsbfuk.html

PHP:  exit(1);
来源：http://hz.yueranfly.top/gtncmkhovm.html

JS:   process.exit(1)
来源：http://hz.shanyushiyangkeji.top/gtrrwoohjm.html

TS:   process.exit(1)
来源：http://hz.pycfn.com/gtevmyydsr.html

Java: System.exit(1)
来源：http://hz.yangfankeji.com/gtmvpstlwe.html

Go:   os.Exit(1)
来源：http://hz.pengpengdd.cyou/gtdvqhilai.html

Ruby: exit 1
来源：http://hz.cqqwz.cn/gtswfdqpkk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhiwuduotai.top/gtjugpapzg.html

[M06] 向标准错误输出
来源：http://hz.dianchejie.cn/gtyderedhv.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gotoacloud.top/gtroruzanw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jqgfzy.top/gtugbjyhth.html

JS:   console.error("err")
来源：http://hz.havefunace.top/gtgwdhapsk.html

TS:   console.error("err")
来源：http://hz.yj20258.top/gtpsmzbyoe.html

Java: System.err.println("err")
来源：http://hz.hywenlv.cn/gtfiywivro.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cqqwz.cn/gtsyznargx.html

Ruby: warn "err"
来源：http://hz.c1oappe.top/gtcptkwiut.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhengqikj.top/gttqkcwccw.html

[M07] 判断是否为主入口
来源：http://hz.feifeiyinyue.top/gtwbgplyvz.html

Py:   if __name__ == "__main__":
来源：http://hz.ivvv.top/gtewbtqhbq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xziqi.cn/gtxrzzsaya.html

JS:   require.main === module
来源：http://hz.vqdsnc.cn/gtybgfqzxd.html

TS:   require.main === module
来源：http://hz.hnqzz.top/gtpqanamdf.html

Java: public static void main(String[] args)
来源：http://hz.zhaomingkeji.xyz/gtoemkxxol.html

Go:   func main()
来源：http://hz.52xcode.cn/gtcwwwmlcj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.wangshuangyany.cn/gtopcejiwo.html

C#:   static void Main(string[] args)
来源：http://hz.sweek.top/gtoorusdjp.html

[M08] 获取系统与运行时信息
来源：http://hz.c1oappe.top/gtdtokjhit.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yvedp.cn/gttqqelzwi.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ybcxt.top/gtnhakvmxj.html

JS:   process.platform;  process.version
来源：http://hz.hnxiangtu.top/gtqwlthhps.html

TS:   process.platform;  process.version
来源：http://hz.chenjidiqi.icu/gtzeiaaqtl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shuidangran.top/gthxfusapk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cdnleiting.top/gtqqtzjfle.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.svipenyu.cn/gtfommpkus.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hammf.cn/gtmdkrsypm.html

================================================================================
来源：http://hz.zhoulong.xyz/gtnhmjtptb.html

N. 数据结构与算法
来源：http://hz.xylfe.cn/gtqmbxgpbs.html

================================================================================
来源：http://hz.dianchejie.cn/gtrucsduhg.html

[N01] 二分查找（有序数组）
来源：http://hz.snrcjt.cn/gtfdhchapt.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gotoacloud.top/gtoparmatd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.havefunace.top/gtrgmwqwrb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cashguo.top/gtyhbbsjih.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xinyue.icu/gtiynuwrkc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yanxiufei.cn/gtlbigeiux.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtsvmwuplc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.vqdsnc.cn/gtogadaigt.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.dashuyun.cn/gtcjcgfynw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.guannengcc.top/gttxitytkd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenjidiqi.icu/gtvjnyehgg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.kuanghao11.cn/gtdbmzykgp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daxiang520.top/gtdzaxwgmc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.havefunace.top/gtnlvorpvh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xuanzx.com/gtmjxrnyhb.html

Go:   slices.Sort(arr)
来源：http://hz.yj20258.top/gtrulwhxej.html

Ruby: arr.sort
来源：http://hz.zhijiandao.cn/gtvrtmujpl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.wangdashe.top/gtjpdweazm.html

[N03] 快速排序（分治示例）
来源：http://hz.gotoacloud.top/gtmgpeznhw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hongshengwenyu.top/gtzdlwcqfz.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zdqjudy.top/gtmbpigngs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yangfankeji.com/gtfmyatctz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.smart0.xyz/gtzwnqjles.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj20258.top/gtjluftbea.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yangfankeji.com/gtgqmdeylu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sufxvd.cn/gtsghkqoxx.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.316326.xyz/gtycbzsjsa.html

[N04] 斐波那契数列
来源：http://hz.redwolf501.top/gtiwjpphis.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.feifeiyinyue.top/gtgjjcdriw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ppjwa.cn/gtiwsicxys.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hysaishi.cn/gtcxjcskul.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.aibaodan.cn/gtnsvbhpro.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cdnleiting.top/gtokysttjz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhengqikj.top/gtwyezicsy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258.top/gtymmleqwl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cqqwz.cn/gtqxfcffbw.html

[N05] 最大公约数
来源：http://hz.yj202588.top/gtynillysr.html

Py:   math.gcd(a, b)
来源：http://hz.svipenyu.cn/gtkponoinp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yueranfly.top/gtpdulnkek.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.kuanghao11.cn/gtetjcbtav.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yonumen.top/gtimcignat.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ybcxt.top/gtbockunkg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xingfuxueyuan.xyz/gtwhkkrtdv.html

Ruby: a.gcd(b)
来源：http://hz.wangdashe.top/gttajpxbim.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.haohaochexian.top/gtpxvvrpsz.html

[N06] 判断回文字符串
来源：http://hz.andypj.xyz/gtvyzoejbn.html

Py:   s == s[::-1]
来源：http://hz.tanke756.top/gtovhyeacg.html

PHP:  $s === strrev($s);
来源：http://hz.zhijiandao.cn/gtyqsqvrog.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yongpay.top/gtlwtllrts.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hammf.cn/gtuqasjmcs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.snrcjt.cn/gtcwnhqsop.html

Go:   // 双指针从两端比较
来源：http://hz.316326.xyz/gthjpulstn.html


<!-- 参考信息 -->