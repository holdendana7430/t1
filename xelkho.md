代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.tianlin.xyz/gtlhzdsvjs.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gogol.net.cn/gtknmrlqdh.html

[J09] 时区处理
来源：http://hz.gotoacloud.top/gtxzeyhokv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zycfv.cn/gtglzhqmye.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.feifeiyinyue.top/gtqvrqllhs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenjidiqi.icu/gtfdogydny.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.meibo888.top/gtvmsezclj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gzhubu.top/gtbshbwrmv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.pengpengdd.cyou/gtrrhgseyf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinyuanbaomall.cn/gtdvleaihu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yongpay.top/gtzxqxbzey.html

[J10] 取今天 / 本月第一天
来源：http://hz.yj20258888.top/gtcohargqv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.snrcjt.cn/gtkplmhdpv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xingfuxueyuan.xyz/gtqtslemvr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.kuanghao11.cn/gtvcacgdhb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.daria6918.cn/gtgztovaqe.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.guowangkeji.top/gtdbmcbwhy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.tian-w.cn/gtzeiomzhq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.tanke756.top/gtzaxggyey.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.mhx1999.top/gttjrvbzcm.html

================================================================================
来源：http://hz.hfpthk.cn/gttjabztdx.html

K. JSON 与序列化
来源：http://hz.zhengqikj.top/gtdrumrkea.html

================================================================================
来源：http://hz.mhx1999.top/gthwalpuew.html

[K01] 对象转 JSON 字符串
来源：http://hz.yanxiufei.cn/gtxinwpkox.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ppjwa.cn/gturaduvmk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.chenzaomai.com/gtijdskqgy.html

JS:   JSON.stringify(obj)
来源：http://hz.cqqwz.cn/gttjyckytc.html

TS:   JSON.stringify(obj)
来源：http://hz.dianchejie.cn/gtuopgdorg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.dashuyun.cn/gtywcculhu.html

Go:   json.Marshal(obj)
来源：http://hz.sweek.top/gthteotxlq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.mhx1999.top/gtprwdcdmm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhiwuduotai.top/gthpzuzyoq.html

[K02] JSON 字符串转对象
来源：http://hz.hammf.cn/gtzgkgkopo.html

Py:   json.loads(s)
来源：http://hz.bjfxy.top/gtmpefxcsg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.smart0.xyz/gtgpwihmzk.html

JS:   JSON.parse(s)
来源：http://hz.chenjidiqi.icu/gtiftkbjcp.html

TS:   JSON.parse(s)
来源：http://hz.yongpay.top/gteijzucat.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shzxlz.cn/gtueugjdzh.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.wangshuangyany.cn/gtshkjwntp.html

Ruby: JSON.parse(s)
来源：http://hz.fengsongda.top/gtmzcuvqbs.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.snrcjt.cn/gtpynmqeqy.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xylfe.cn/gtjgdtrgru.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hnxiangtu.top/gtmckreaam.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.aizwys.cn/gtgwasoppp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ywan-chungtsiang.top/gtxvdocbrj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangtech.top/gtyhesymxw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zycfv.cn/gtxuucyprb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.aizwys.cn/gtwpttrgkv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.bjfxy.top/gtbdxsdcqf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinqigufen.top/gtjhltcaoy.html

[K04] 读取 JSON 文件
来源：http://hz.birdmap.top/gtvkluaqgm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jyoumei.cn/gtpezttqas.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hongshengwenyu.top/gtwkibwpiz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.316326.xyz/gtklnfuqah.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sysykeji.top/gtpujavyrf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shzxlz.cn/gtbnuvmszd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhoulong.xyz/gtqtnpnabz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhijiandao.cn/gtcnvacflt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hammf.cn/gtynyfvqti.html

[K05] 深拷贝对象
来源：http://hz.pycfn.com/gtitbmqnna.html

Py:   copy.deepcopy(obj)
来源：http://hz.feifeiyinyue.top/gtiqmqcifv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shanyushiyangkeji.top/gtejbauqlc.html

JS:   structuredClone(obj)
来源：http://hz.zhongyouzk.top/gtguuqbmwd.html

TS:   structuredClone(obj)
来源：http://hz.guowangkeji.top/gtuxslqokh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sxryk.cn/gtmzmauvbs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.birdmap.top/gtkdbkwugd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jinyuanbaomall.cn/gtflaqnvjy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xuanzx.com/gtrjnswdli.html

[K06] 解析 URL 查询串
来源：http://hz.havefunace.top/gttlkximof.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.iojbl.cn/gtolfwwbzc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.c1oappe.top/gtqzstuqrb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangkeji.top/gtdldaevof.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnqzz.top/gtrciubyue.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shangyingyoupin.top/gtwjwavwyd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhiwuduotai.top/gtaglenrfn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zdqjudy.top/gtyuvmpqfl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.snrcjt.cn/gtvqiltker.html

[K07] 进制转换
来源：http://hz.yangfankeji.com/gtbdnhvkkf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinqigfzy.top/gtjzdzlcbs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.bjfxy.top/gtfsotzvwo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gtlmeasagv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yj202588.top/gtpjhzjlbk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.aizwys.cn/gtibscwbxm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hfpthk.cn/gtaijxmxvd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zycfv.cn/gtktfenedd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhoulong.xyz/gtfbtzotsd.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.chenzaomai.com/gtlvzlmdgv.html

Py:   pickle.dumps(obj)
来源：http://hz.aizwys.cn/gtuyvkahdj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.svipenyu.cn/gtzfdfpfad.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.bjfxy.top/gtjshyblkl.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.fengsongda.top/gtpuavurbq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.wangshuangyany.cn/gtxmijukio.html

Go:   encoding/gob
来源：http://hz.jiagoushi.top/gtqbzzkzbn.html

Ruby: Marshal.dump(obj)
来源：http://hz.ppjwa.cn/gtgfcxfpzp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jqgfzy.top/gttrkrriza.html

================================================================================
来源：http://hz.pycfn.com/gtsbpryxfu.html

L. 网络请求
来源：http://hz.daxiang520.top/gtxswnmnlm.html

================================================================================
来源：http://hz.cucudq.cn/gthrcmvhtu.html

[L01] 发送 GET 请求
来源：http://hz.xingfuxueyuan.xyz/gtcpsgbkra.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.c1oappe.top/gtmpdegkri.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jinqigufen.top/gtqjxbwlsb.html

JS:   await fetch(url)
来源：http://hz.zdqjudy.top/gtigemwucn.html

TS:   await fetch(url)
来源：http://hz.ybcxt.top/gtvwvwevnr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yanxiufei.cn/gtjrfppwoc.html

Go:   resp, err := http.Get(url)
来源：http://hz.c1oappe.top/gtzdjdrwxp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.birdmap.top/gtuqhohyuw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.pycfn.com/gtzitfgjsj.html

[L02] 发送 POST JSON
来源：http://hz.shanyushiyangtech.top/gtengweais.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cashguo.top/gtzxtiqnlt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.iojbl.cn/gtvipmellb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shzxlz.cn/gtnwbggkqz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cqqwz.cn/gtzjacrkcb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gotoacloud.top/gtgnnvxdmq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yongpay.top/gtgmrmcchk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jqgufenzy.top/gtchmzaxca.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.meibo888.top/gtiapmtbqp.html

[L03] 设置自定义请求头
来源：http://hz.yonumen.top/gtovbexrbw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nanxinkj.top/gtptvzopbq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zdqjudy.top/gtrvxgsmhv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj20258.top/gthezrfrhb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhixingplan.top/gtnpjsgnty.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.haohaochexian.top/gtmwxwaouu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.guowangkeji.top/gtfxnysjcy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cheryme.top/gttpiautmy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.pycfn.com/gtyjverfbb.html

[L04] 设置超时
来源：http://hz.quarkkingdee.top/gtegkpyhof.html

Py:   requests.get(url, timeout=5)
来源：http://hz.aibaodan.cn/gtgyrwlyga.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.tianlin.xyz/gtiduviabj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yanxiufei.cn/gttcwiglfv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jlsjyb.cn/gtvhcnbzhy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.smart0.xyz/gtcwdajghb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jyoumei.cn/gthmyjhvtq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jqgfzy.top/gtlidaqzos.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jinqigfzy.top/gtggfvdjre.html

[L05] 上传文件（multipart）
来源：http://hz.andypj.xyz/gttucvqyiv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.svipenyu.cn/gtmbdeynks.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xingfuxueyuan.xyz/gtpwfrwald.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.tianlin.xyz/gtmndorztt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sxryk.cn/gtkkztngwm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yuxming.cn/gtodhofvap.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zdqjudy.top/gtolyimvpo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.chenzaomai.com/gtpuqmnbnt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yvedp.cn/gtgoqsrymj.html

[L06] 解析响应为 JSON
来源：http://hz.dianchejie.cn/gtwpmrvsmq.html

Py:   resp.json()
来源：http://hz.xuetiantiany.cn/gtctrimmjf.html

PHP:  json_decode($body, true);
来源：http://hz.yanxiufei.cn/gtjhptligs.html

JS:   await resp.json()
来源：http://hz.hnxiangtu.top/gthyeqaiin.html

TS:   await resp.json()
来源：http://hz.xuanzx.com/gtxjcjkjgg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.kuanghao11.cn/gtzfalhwnv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jlsjyb.cn/gtfdwzsyzx.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xingfuxueyuan.xyz/gtijinqbva.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.dashuyun.cn/gttxwpwvvr.html

[L07] 处理 HTTP 状态码
来源：http://hz.ivvv.top/gtlvsmkqip.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.svipenyu.cn/gtnpjgmdsb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ehwqpu.com/gtayujkcgm.html

JS:   resp.ok;  resp.status
来源：http://hz.chenlongwang.top/gtlxttpzby.html

TS:   resp.ok;  resp.status
来源：http://hz.shanyushiyangkeji.top/gtgamoosmd.html

Java: resp.statusCode()
来源：http://hz.zhengqikj.top/gtaxngudfp.html

Go:   resp.StatusCode
来源：http://hz.sweek.top/gtaspbwfzg.html

Ruby: resp.code.to_i
来源：http://hz.jqgufenzy.top/gtmosotfrs.html

C#:   (int)resp.StatusCode
来源：http://hz.xziqi.cn/gtovjtnsqi.html

[L08] 并发请求多个地址
来源：http://hz.fengsongda.top/gtnxmnjlsv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yueranfly.top/gtdjlqerqb.html

PHP:  curl_multi_init() 系列
来源：http://hz.hfpthk.cn/gtmwfwqntn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yvedp.cn/gtavzpwwtm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shuidangran.top/gtlnvsaidc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hysaishi.cn/gtvjixsqbo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.kuanghao11.cn/gtljirrepq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.sweek.top/gtqxlsxhtn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhongyouzk.top/gtriyrsowz.html

================================================================================
来源：http://hz.gzhubu.top/gtpicpcxas.html

M. 命令行 / 进程 / 环境
来源：http://hz.ydzc1.top/gtdwwqumpy.html

================================================================================
来源：http://hz.chenzaomai.com/gtncqptlia.html

[M01] 读取命令行参数
来源：http://hz.smart0.xyz/gtrufueqfd.html

Py:   sys.argv[1:]
来源：http://hz.hysaishi.cn/gtkczwymoi.html

PHP:  $argv;  $argc;
来源：http://hz.chenjidiqi.icu/gtjfroxwme.html

JS:   process.argv.slice(2)
来源：http://hz.andypj.xyz/gtudwqpvjt.html

TS:   process.argv.slice(2)
来源：http://hz.yvedp.cn/gtxgpfcbau.html

Java: args 数组（main 方法参数）
来源：http://hz.redwolf501.top/gtjtnlkqpw.html

Go:   os.Args[1:]
来源：http://hz.birdmap.top/gtwdvfldut.html

Ruby: ARGV
来源：http://hz.dashuyun.cn/gtrgzklzdg.html

C#:   args 数组（Main 方法参数）
来源：http://hz.nwbrower.top/gtejnyizmk.html

[M02] 读取环境变量
来源：http://hz.zdqjudy.top/gtifujyzan.html

Py:   os.environ.get("HOME")
来源：http://hz.cashguo.top/gtoymucukk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ppjwa.cn/gthxmskacf.html

JS:   process.env.HOME
来源：http://hz.daxiang520.top/gtwzfrlroj.html

TS:   process.env.HOME
来源：http://hz.xziqi.cn/gtxwwgytvy.html

Java: System.getenv("HOME")
来源：http://hz.hongshengwenyu.top/gtvfzgmkbn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jqgufenzy.top/gtpnjvrfgc.html

Ruby: ENV["HOME"]
来源：http://hz.shuidangran.top/gtrvaixlbx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.tanke756.top/gtacpfhrfv.html

[M03] 执行外部命令
来源：http://hz.jqgufenzy.top/gtaqhwuiud.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.fengsongda.top/gtkmnuaufp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.wangshuangyany.cn/gtebvdagad.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.52xcode.cn/gteuyulqld.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xuetiantiany.cn/gtufgtnzwh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.mhx1999.top/gtaybtcvkj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.andypj.xyz/gthhxauril.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jyoumei.cn/gtevduummi.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sweek.top/gtyyzkkmkk.html

[M04] 获取当前工作目录
来源：http://hz.gaohongyu789.top/gtrjxoqkya.html

Py:   os.getcwd()
来源：http://hz.cashguo.top/gtusabklgq.html

PHP:  getcwd();
来源：http://hz.nanxinkj.top/gtazkzodbr.html

JS:   process.cwd()
来源：http://hz.jianghu66.top/gtfhvqkwkl.html

TS:   process.cwd()
来源：http://hz.yonumen.top/gtfxjsjvrb.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.feifeiyinyue.top/gtjuqcbxng.html

Go:   os.Getwd()
来源：http://hz.havefunace.top/gtnnhdgdsr.html

Ruby: Dir.pwd
来源：http://hz.yongpay.top/gtajsqjebs.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.daxiang520.top/gtoatfdvjr.html

[M05] 设置退出码
来源：http://hz.hnqzz.top/gtshkbjvec.html

Py:   sys.exit(1)
来源：http://hz.0kj1m.cn/gtxxzwijmh.html

PHP:  exit(1);
来源：http://hz.hnxiangtu.top/gtwrhthsrc.html

JS:   process.exit(1)
来源：http://hz.guannengcc.top/gtlnyrclao.html

TS:   process.exit(1)
来源：http://hz.svipenyu.cn/gttsnleawz.html

Java: System.exit(1)
来源：http://hz.iojbl.cn/gtwbcteidl.html

Go:   os.Exit(1)
来源：http://hz.gzhubu.top/gtdyhpvlvz.html

Ruby: exit 1
来源：http://hz.aizwys.cn/gtoynmzbaj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sxryk.cn/gtxndzwiqo.html

[M06] 向标准错误输出
来源：http://hz.cheryme.top/gtiyxjvama.html

Py:   print("err", file=sys.stderr)
来源：http://hz.316326.xyz/gtswkmniuo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ywan-chungtsiang.top/gttsszfvjn.html

JS:   console.error("err")
来源：http://hz.gogol.net.cn/gtjgkkxvsr.html

TS:   console.error("err")
来源：http://hz.yanxiufei.cn/gtanpxnixv.html

Java: System.err.println("err")
来源：http://hz.hammf.cn/gtaqiiuqvp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.havefunace.top/gtyldffycu.html

Ruby: warn "err"
来源：http://hz.shangyingyoupin.top/gtkiclhwmi.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hfpthk.cn/gtpazbhhzz.html

[M07] 判断是否为主入口
来源：http://hz.daria6918.cn/gtveekwlah.html

Py:   if __name__ == "__main__":
来源：http://hz.jinyuanbaomall.cn/gtupgmajbf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yongpay.top/gtetoizrmc.html

JS:   require.main === module
来源：http://hz.jyoumei.cn/gtppoonfyy.html

TS:   require.main === module
来源：http://hz.shangyingyoupin.top/gttineuwid.html

Java: public static void main(String[] args)
来源：http://hz.cdnleiting.top/gtgzkqjfzb.html

Go:   func main()
来源：http://hz.ppjwa.cn/gtlgstvdgi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.havefunace.top/gtvvnvcxuu.html

C#:   static void Main(string[] args)
来源：http://hz.jiagoushi.top/gtwcqbmnqm.html

[M08] 获取系统与运行时信息
来源：http://hz.yvedp.cn/gtmnelcusi.html

Py:   platform.system();  platform.python_version()
来源：http://hz.aizwys.cn/gttkqmfofx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.wangdashe.top/gtjolhqtsm.html

JS:   process.platform;  process.version
来源：http://hz.sysykeji.top/gtzuvjlded.html

TS:   process.platform;  process.version
来源：http://hz.pengpengdd.cyou/gtylzlixrj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.pengpengdd.cyou/gtpotihksh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ivvv.top/gtsaeavdrr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jinyuanbaomall.cn/gtwixgyjhx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.tanke756.top/gtpnawrzar.html

================================================================================
来源：http://hz.tianlin.xyz/gtcsuzcwok.html

N. 数据结构与算法
来源：http://hz.feifeiyinyue.top/gtjtwjoexv.html

================================================================================
来源：http://hz.fzhhl.top/gtekjvvatw.html

[N01] 二分查找（有序数组）
来源：http://hz.ppjwa.cn/gtskgiopig.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gotoacloud.top/gtmvjvwlge.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.316326.xyz/gtpracuvra.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhongyouzk.top/gtqzwjfxjg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.birdmap.top/gtbxzlaerb.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.wangdashe.top/gtpjvsywfa.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xinyue.icu/gtyjogpxpj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jyoumei.cn/gtwfhupxmp.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.gaohongyu789.top/gtahaonimv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cqqwz.cn/gtouczarbp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydzc1.top/gtrkyzgswa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.nwbrower.top/gtniexodbo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.wangdashe.top/gtznpyevln.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hammf.cn/gtwdpcmsco.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.dianchejie.cn/gtiywjhqqy.html

Go:   slices.Sort(arr)
来源：http://hz.9152youxi.cn/gtmpdlexxk.html

Ruby: arr.sort
来源：http://hz.nanxinkj.top/gtohovpdad.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shanyushiyangtech.top/gtasazhwev.html

[N03] 快速排序（分治示例）
来源：http://hz.zhoulong.xyz/gtsxabubxf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xuanzx.com/gtjkkzhpgs.html

PHP:  // 递归实现，或用 usort
来源：http://hz.9152youxi.cn/gtjnkevfpv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.haohaochexian.top/gtbgoeqfex.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hammf.cn/gtccrbmezd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinqigufen.top/gtzueirmyz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.wangshuangyany.cn/gtwzycteof.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhiwuduotai.top/gtetkfgnkn.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gotoacloud.top/gtkjpqhdqz.html

[N04] 斐波那契数列
来源：http://hz.wangdashe.top/gtwvbjaddu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yongpay.top/gthqqsofyq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yueranfly.top/gtmnmzohpp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigfzy.top/gtqnzojdvp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gogol.net.cn/gtfvcbaqte.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.andypj.xyz/gtklroonfc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ybcxt.top/gtjaujjyyy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.shangyingyoupin.top/gthkbxsnjk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ybcxt.top/gtyhnzzthl.html

[N05] 最大公约数
来源：http://hz.ydzc1.top/gtmwrheahz.html

Py:   math.gcd(a, b)
来源：http://hz.wangdashe.top/gtuqgegckk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.gotoacloud.top/gtplofvwzl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.havefunace.top/gtvkbhdxdr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xinyue.icu/gtxrnddxox.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.wangshuangyany.cn/gtaieodjci.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.c1oappe.top/gtsuldwmey.html

Ruby: a.gcd(b)
来源：http://hz.hywenlv.cn/gthdgjamzd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.mhx1999.top/gtnssdpofc.html

[N06] 判断回文字符串
来源：http://hz.yonumen.top/gthvqlekui.html

Py:   s == s[::-1]
来源：http://hz.xingfuxueyuan.xyz/gtknwozbgc.html

PHP:  $s === strrev($s);
来源：http://hz.kuanghao11.cn/gtzdhrxjox.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhiwuduotai.top/gtsautuvgd.html

TS:   s === [...s].reverse().join("")
来源：http://hz.haohaochexian.top/gtsmkmvjkc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.feifeiyinyue.top/gtwknhdpsl.html

Go:   // 双指针从两端比较
来源：http://hz.guowangkeji.top/gtfkcjistj.html


<!-- 参考信息 -->