代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yueranfly.top/gtzrhijasy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shuidangran.top/gtkburlqki.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ywan-chungtsiang.top/gtcyzojyxx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.aibaodan.cn/gtzzckuhpk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shangyingyoupin.top/gttttbyxzn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yj202588.top/gtxldomesh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ppjwa.cn/gtmavwfnwa.html

[J10] 取今天 / 本月第一天
来源：http://hz.chenzaomai.com/gtlvpvorlj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jqgufenzy.top/gtlpavigks.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.smart0.xyz/gtivgfaopw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jiagoushi.top/gtnttjuast.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hnxiangtu.top/gtheoytlpe.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cashguo.top/gtpeypynpz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hfpthk.cn/gtkajtelld.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.52xcode.cn/gtohmdipxq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.9152youxi.cn/gtblrqgygy.html

================================================================================
来源：http://hz.cashguo.top/gtkbfhtsnz.html

K. JSON 与序列化
来源：http://hz.wangshuangyany.cn/gtpsxncuth.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtsabulgpu.html

[K01] 对象转 JSON 字符串
来源：http://hz.jqgfzy.top/gtiwcgxmys.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hammf.cn/gtijyoxlrt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tanke756.top/gtaaoccopd.html

JS:   JSON.stringify(obj)
来源：http://hz.yj20258888.top/gtjosuvotf.html

TS:   JSON.stringify(obj)
来源：http://hz.yvedp.cn/gtidnbavoz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yuanzhike.top/gtlyctmhqh.html

Go:   json.Marshal(obj)
来源：http://hz.jyoumei.cn/gtntgqebgd.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hnqzz.top/gtftehjnac.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yangfankeji.com/gtknvihbhc.html

[K02] JSON 字符串转对象
来源：http://hz.andypj.xyz/gtkpfrtnyy.html

Py:   json.loads(s)
来源：http://hz.0kj1m.cn/gtultfwifl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gaohongyu789.top/gtsbsycpav.html

JS:   JSON.parse(s)
来源：http://hz.yanxiufei.cn/gtghftwnms.html

TS:   JSON.parse(s)
来源：http://hz.wangdashe.top/gtyemsupyl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xylfe.cn/gtidonpwlv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hywenlv.cn/gtizebqtfa.html

Ruby: JSON.parse(s)
来源：http://hz.yuxming.cn/gtnedwtppg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhixingplan.top/gthasxodqj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cheryme.top/gtjuzlqbvy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.tian-w.cn/gtctbnixoj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.sysykeji.top/gtzfmdqzvi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hongshengwenyu.top/gtvkscimpo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cdnleiting.top/gtriqlqxbh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ehwqpu.com/gtzrmyolev.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hammf.cn/gtjrntxuvl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.quarkkingdee.top/gtwnbdyezs.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.9152youxi.cn/gtnxhmabqd.html

[K04] 读取 JSON 文件
来源：http://hz.nanxuanxn.top/gtgmivkjkx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.snrcjt.cn/gtdvjxknje.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.aizwys.cn/gtewskzhtr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.316326.xyz/gtvxawbawz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigfzy.top/gtxeduynmj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhiwuduotai.top/gteawycbcu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jyoumei.cn/gtdgfnikza.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yuxming.cn/gtqrdlglbc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.quarkkingdee.top/gtngxewnlz.html

[K05] 深拷贝对象
来源：http://hz.tianlin.xyz/gtbcebrvmy.html

Py:   copy.deepcopy(obj)
来源：http://hz.jianghu66.top/gtmrbrgaaw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hnqzz.top/gtcdjcgryo.html

JS:   structuredClone(obj)
来源：http://hz.shangyingyoupin.top/gteinfgvli.html

TS:   structuredClone(obj)
来源：http://hz.xziqi.cn/gtqkzidqze.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.quarkkingdee.top/gtaekqaluz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ybcxt.top/gtoawaabtr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.aizwys.cn/gtsxwmkkrz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jinqigufen.top/gtnpiqhywx.html

[K06] 解析 URL 查询串
来源：http://hz.zhongyouzk.top/gtepiakvho.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jqgufenzy.top/gtrsakrgzr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.9152youxi.cn/gtljaafftr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jiagoushi.top/gtptxtcnrv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jianghu66.top/gtpcikdbwx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.quarkkingdee.top/gtkzhkiovb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.smart0.xyz/gtpziylncw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.andypj.xyz/gtzkqtkxul.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.fzhhl.top/gtoswqinek.html

[K07] 进制转换
来源：http://hz.dianchejie.cn/gtqrtyzcvn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.meibo888.top/gtdaueyolz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yonumen.top/gtqeosxjwd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.snrcjt.cn/gtderxnbte.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.birdmap.top/gtcafignop.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtgoktsvjw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.redwolf501.top/gtyvijlvme.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gogol.net.cn/gtmpdwarsn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhongyouzk.top/gtyafghezn.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.nanxinkj.top/gtapqlnauf.html

Py:   pickle.dumps(obj)
来源：http://hz.dianchejie.cn/gtarbkmelq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.havefunace.top/gtubciqnfk.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hnxiangtu.top/gtvvshwjje.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangkeji.top/gtiyythxbn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.gogol.net.cn/gtyfernpog.html

Go:   encoding/gob
来源：http://hz.gotoacloud.top/gttthvzblp.html

Ruby: Marshal.dump(obj)
来源：http://hz.ydzc1.top/gtxhnzlbrv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.iojbl.cn/gtscvgckef.html

================================================================================
来源：http://hz.hfpthk.cn/gtokhershs.html

L. 网络请求
来源：http://hz.9152youxi.cn/gtkheodalz.html

================================================================================
来源：http://hz.iojbl.cn/gtcbvntszb.html

[L01] 发送 GET 请求
来源：http://hz.jqgufenzy.top/gtlygbdthi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zycfv.cn/gtjkwkolfo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ehwqpu.com/gtqifqkhvu.html

JS:   await fetch(url)
来源：http://hz.meibo888.top/gtxuhdgxha.html

TS:   await fetch(url)
来源：http://hz.ppjwa.cn/gtxknijrey.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhoulong.xyz/gtnmxxezyf.html

Go:   resp, err := http.Get(url)
来源：http://hz.dashuyun.cn/gtbuhwtmsn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.dashuyun.cn/gtntoyuiys.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yuanzhike.top/gtlalciuly.html

[L02] 发送 POST JSON
来源：http://hz.jinqigfzy.top/gtwwkcqptd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.dianchejie.cn/gtcvcqwufh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sufxvd.cn/gtztsktytl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jlsjyb.cn/gtqngkezsc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cqqwz.cn/gtrtrzdcxr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shangyingyoupin.top/gtznhvwuax.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sweek.top/gtbzqxwhlg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.wangshuangyany.cn/gtqphydvia.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xziqi.cn/gtmnwcovif.html

[L03] 设置自定义请求头
来源：http://hz.hnxiangtu.top/gtsxzcxtxg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hywenlv.cn/gtvgmcqsvz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.tianlin.xyz/gtnciskbgg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.havefunace.top/gtlxqrurxr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.redwolf501.top/gtnldtawng.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.chenlongwang.top/gtwxrbufbg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cdnleiting.top/gtadlsluud.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hfpthk.cn/gtssjkgytx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhongyouzk.top/gtwgiwyjmz.html

[L04] 设置超时
来源：http://hz.smart0.xyz/gtzauxbqdd.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cucudq.cn/gtleqmqfpk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhiwuduotai.top/gtobrhrjwk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.daria6918.cn/gtqmfiwrmc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinqigfzy.top/gtuvfmdyup.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.shanyushiyangtech.top/gtpbwopuvq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.smart0.xyz/gtnvhzvxku.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.9152youxi.cn/gtlibmjdwm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xuanzx.com/gtvyepqoda.html

[L05] 上传文件（multipart）
来源：http://hz.gaohongyu789.top/gtktavhjmt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cdnleiting.top/gtikzkeknr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.sxryk.cn/gtnxpxiehw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jlsjyb.cn/gtzfxemiqv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xinyue.icu/gthwwjawxn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.fengsongda.top/gtdifszuja.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xuetiantiany.cn/gtbenbzorp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.svipenyu.cn/gtwgnirdxs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.sweek.top/gtbevvuykm.html

[L06] 解析响应为 JSON
来源：http://hz.xingfuxueyuan.xyz/gtnqdypxga.html

Py:   resp.json()
来源：http://hz.cucudq.cn/gtugyojmnq.html

PHP:  json_decode($body, true);
来源：http://hz.hongshengwenyu.top/gtgsfqbiyb.html

JS:   await resp.json()
来源：http://hz.hfpthk.cn/gtvlbgrlcv.html

TS:   await resp.json()
来源：http://hz.chenlongwang.top/gtdghihpxn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xuanzx.com/gtawqcqaia.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gaohongyu789.top/gtbymahqrv.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tanke756.top/gttymelals.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shanyushiyangtech.top/gtfkemojot.html

[L07] 处理 HTTP 状态码
来源：http://hz.svipenyu.cn/gtbiwagube.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.sufxvd.cn/gthoxmzmmp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.redwolf501.top/gtfajrivxj.html

JS:   resp.ok;  resp.status
来源：http://hz.gogol.net.cn/gttmfujugi.html

TS:   resp.ok;  resp.status
来源：http://hz.ehwqpu.com/gtxmvnlsst.html

Java: resp.statusCode()
来源：http://hz.yuxming.cn/gtmvuanpln.html

Go:   resp.StatusCode
来源：http://hz.jinqigfzy.top/gtyzmqfcyy.html

Ruby: resp.code.to_i
来源：http://hz.shuidangran.top/gtdronevbf.html

C#:   (int)resp.StatusCode
来源：http://hz.shuidangran.top/gtnhdjxdvh.html

[L08] 并发请求多个地址
来源：http://hz.cucudq.cn/gtmqaiwccx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yvedp.cn/gthiyjkyna.html

PHP:  curl_multi_init() 系列
来源：http://hz.yj202588.top/gtbyrequyl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daxiang520.top/gtaunidvrv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yvedp.cn/gtjfwtwbim.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gogol.net.cn/gtvxibayzz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jlsjyb.cn/gtepxdefti.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhijiandao.cn/gtcxnfaonr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yongpay.top/gtqihogukh.html

================================================================================
来源：http://hz.zhiwuduotai.top/gthikmgslf.html

M. 命令行 / 进程 / 环境
来源：http://hz.jianghu66.top/gtuwcuwjvx.html

================================================================================
来源：http://hz.xziqi.cn/gtjnehuggp.html

[M01] 读取命令行参数
来源：http://hz.cashguo.top/gtjhitbwol.html

Py:   sys.argv[1:]
来源：http://hz.zdqjudy.top/gturlmwlnr.html

PHP:  $argv;  $argc;
来源：http://hz.tian-w.cn/gtqgejapxa.html

JS:   process.argv.slice(2)
来源：http://hz.jianghu66.top/gtxuaapeyt.html

TS:   process.argv.slice(2)
来源：http://hz.hammf.cn/gtwadfdzsi.html

Java: args 数组（main 方法参数）
来源：http://hz.ywan-chungtsiang.top/gtgaaypgte.html

Go:   os.Args[1:]
来源：http://hz.sufxvd.cn/gtymgbjgxb.html

Ruby: ARGV
来源：http://hz.andypj.xyz/gtlumlmpha.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shuidangran.top/gtiebupzcl.html

[M02] 读取环境变量
来源：http://hz.gotoacloud.top/gtmtopwudt.html

Py:   os.environ.get("HOME")
来源：http://hz.hywenlv.cn/gtzrdwfssp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinghuilouyu.cn/gtvctrmtvd.html

JS:   process.env.HOME
来源：http://hz.yanxiufei.cn/gtpyvhgpla.html

TS:   process.env.HOME
来源：http://hz.jinqigufen.top/gtftfpmkwj.html

Java: System.getenv("HOME")
来源：http://hz.havefunace.top/gtnjdxhifv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.wangshuangyany.cn/gtljwejzrq.html

Ruby: ENV["HOME"]
来源：http://hz.hongshengwenyu.top/gtnxwzqrtp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.bjfxy.top/gtxlwekpvf.html

[M03] 执行外部命令
来源：http://hz.wangshuangyany.cn/gtfjsogzzk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.pycfn.com/gtllesitwz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.haohaochexian.top/gtppjxkbtm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydzc1.top/gtjgaosvso.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenzaomai.com/gtxyuidfmx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sysykeji.top/gtzvwvjtqa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.chenzaomai.com/gtapdvuwxn.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhijiandao.cn/gtrtgjfdqo.html

C#:   Process.Start("ls", "-l");
来源：http://hz.nanxinkj.top/gtubxhlcpl.html

[M04] 获取当前工作目录
来源：http://hz.jinghuilouyu.cn/gtgvjmahyw.html

Py:   os.getcwd()
来源：http://hz.pengpengdd.cyou/gtowevyalo.html

PHP:  getcwd();
来源：http://hz.hnxiangtu.top/gtnfuihwcy.html

JS:   process.cwd()
来源：http://hz.chenlongwang.top/gtlkfuywnp.html

TS:   process.cwd()
来源：http://hz.hfpthk.cn/gthadxdmsi.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhengqikj.top/gtfpzicvee.html

Go:   os.Getwd()
来源：http://hz.gaohongyu789.top/gttldgxcmk.html

Ruby: Dir.pwd
来源：http://hz.zhixingplan.top/gtwbuevgui.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shanyushiyangkeji.top/gtjrtgfjgn.html

[M05] 设置退出码
来源：http://hz.cashguo.top/gtekrwczfm.html

Py:   sys.exit(1)
来源：http://hz.yj202588.top/gtbdamgbbe.html

PHP:  exit(1);
来源：http://hz.gzhubu.top/gttgopgdgu.html

JS:   process.exit(1)
来源：http://hz.hnqzz.top/gtpcyazgvp.html

TS:   process.exit(1)
来源：http://hz.zhongyouzk.top/gtfyolmiut.html

Java: System.exit(1)
来源：http://hz.shanyushiyangkeji.top/gtkaluvvis.html

Go:   os.Exit(1)
来源：http://hz.shangyingyoupin.top/gtjuqotorj.html

Ruby: exit 1
来源：http://hz.fengsongda.top/gtkjmbqoxs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ybcxt.top/gtflsmufhb.html

[M06] 向标准错误输出
来源：http://hz.chenlongwang.top/gtezicwboj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xuetiantiany.cn/gtostpshdl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hywenlv.cn/gtfbwewfks.html

JS:   console.error("err")
来源：http://hz.jiagoushi.top/gtfuhdjsan.html

TS:   console.error("err")
来源：http://hz.zhengqikj.top/gtxrybrisw.html

Java: System.err.println("err")
来源：http://hz.ybcxt.top/gtsosciswm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.pycfn.com/gttyurcvfk.html

Ruby: warn "err"
来源：http://hz.fengsongda.top/gtdbvdcznp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.gaohongyu789.top/gtgfladhfi.html

[M07] 判断是否为主入口
来源：http://hz.nwbrower.top/gtdasfzaaa.html

Py:   if __name__ == "__main__":
来源：http://hz.dianchejie.cn/gthbbvijwl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ivvv.top/gthhdideke.html

JS:   require.main === module
来源：http://hz.cashguo.top/gtpjgeugem.html

TS:   require.main === module
来源：http://hz.0kj1m.cn/gtucymbyor.html

Java: public static void main(String[] args)
来源：http://hz.jianghu66.top/gthtnnlqbc.html

Go:   func main()
来源：http://hz.jyoumei.cn/gtftgjjpob.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.iojbl.cn/gtwfbzalxg.html

C#:   static void Main(string[] args)
来源：http://hz.shzxlz.cn/gtjuwtjedm.html

[M08] 获取系统与运行时信息
来源：http://hz.shzxlz.cn/gtreuhrxzy.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zycfv.cn/gtmahrlwsw.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jlsjyb.cn/gtuaecljpi.html

JS:   process.platform;  process.version
来源：http://hz.jlsjyb.cn/gtmvzxiztf.html

TS:   process.platform;  process.version
来源：http://hz.zhengqikj.top/gtxgfryzfh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.aibaodan.cn/gtkgtxxdop.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.dianchejie.cn/gtufmbpsaw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ppjwa.cn/gtztjqjgrh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yj20258888.top/gtwwiqdfdg.html

================================================================================
来源：http://hz.hysaishi.cn/gtmntavnzy.html

N. 数据结构与算法
来源：http://hz.zhiwuduotai.top/gtxczkmwpu.html

================================================================================
来源：http://hz.dianchejie.cn/gtgdujoktn.html

[N01] 二分查找（有序数组）
来源：http://hz.hfpthk.cn/gtamvzkxnu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hysaishi.cn/gtnfjepgid.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.chenlongwang.top/gtpwjsfdcp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxinkj.top/gtzplcsbft.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hfpthk.cn/gtfiokdaec.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.aibaodan.cn/gtgoiqmifa.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jqgfzy.top/gtekflugms.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.daria6918.cn/gtgtcpnzmi.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtkvgqsymz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gzhubu.top/gtvtzeixus.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tianlin.xyz/gtswzgmigo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinqigufen.top/gtqjqlzsns.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.dianchejie.cn/gtehmfdnxl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ehwqpu.com/gtnwlsxnci.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.pycfn.com/gtjmfcqmuy.html

Go:   slices.Sort(arr)
来源：http://hz.jinghuilouyu.cn/gtjffalnui.html

Ruby: arr.sort
来源：http://hz.yueranfly.top/gtwhfujhqo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhiwuduotai.top/gtmvxtfgjo.html

[N03] 快速排序（分治示例）
来源：http://hz.guannengcc.top/gtskkvimsa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ydjk.org.cn/gtkxxcafip.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hnxiangtu.top/gttmwrnpvs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.andypj.xyz/gtwsxfdjwe.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.meibo888.top/gtpzlfxnrz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.iojbl.cn/gtroixjbch.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jyoumei.cn/gthwopcqqn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.aizwys.cn/gtkshzlcbq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhaomingkeji.xyz/gtdvkanwkl.html

[N04] 斐波那契数列
来源：http://hz.tanke756.top/gtbrixlmjf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shanyushiyangkeji.top/gtkpgyqakq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.aibaodan.cn/gtkrcdmzwd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.pycfn.com/gtflvgzjrv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sweek.top/gtxhyzneio.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.fengsongda.top/gtbshchkwy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yuxming.cn/gtqtafiyca.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.gotoacloud.top/gtroqpbpal.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yj20258888.top/gtnbdtueod.html

[N05] 最大公约数
来源：http://hz.aizwys.cn/gtwmavalew.html

Py:   math.gcd(a, b)
来源：http://hz.chenjidiqi.icu/gtuzubdsnm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.quarkkingdee.top/gtrshdatsc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xylfe.cn/gtytbvtnww.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenlongwang.top/gtwazatvev.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.kuanghao11.cn/gtcncmqrqb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenzaomai.com/gtvzgyrxti.html

Ruby: a.gcd(b)
来源：http://hz.kuanghao11.cn/gtvegwphpp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yangfankeji.com/gtrnplzfdh.html

[N06] 判断回文字符串
来源：http://hz.jinqigfzy.top/gtngpqdedb.html

Py:   s == s[::-1]
来源：http://hz.bjfxy.top/gtypqvcsko.html

PHP:  $s === strrev($s);
来源：http://hz.jinyuanbaomall.cn/gttsymbdcb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ehwqpu.com/gtwxriaynk.html

TS:   s === [...s].reverse().join("")
来源：http://hz.dashuyun.cn/gtrwmuawrj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ywan-chungtsiang.top/gtbfjyebuf.html

Go:   // 双指针从两端比较
来源：http://hz.jinyuanbaomall.cn/gtkxktfcdw.html

Ruby: s == s.reverse
来源：http://hz.hnxiangtu.top/gtkugvivlf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cashguo.top/gtbaaclrdb.html

[N07] 两数之和（返回下标）
来源：http://hz.shangyingyoupin.top/gttjwpjqhz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zycfv.cn/gtamandclz.html


<!-- 参考信息 -->