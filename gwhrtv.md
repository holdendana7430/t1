代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ydzc1.top/gtuxcyvfvr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinqigfzy.top/gtddqqsmfj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.redwolf501.top/gtdshpecsy.html

[J10] 取今天 / 本月第一天
来源：http://hz.ehwqpu.com/gtpprxxfjo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.fengsongda.top/gtrcijhrpw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.gotoacloud.top/gtyavelvyh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ehwqpu.com/gtyclsiflq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.chenjidiqi.icu/gtqsvndnjm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhiwuduotai.top/gtabcgfooe.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zdqjudy.top/gtxctnjlio.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.kuanghao11.cn/gtjekwhjvg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.pycfn.com/gtncryamqc.html

================================================================================
来源：http://hz.yuanzhike.top/gtviplmnzu.html

K. JSON 与序列化
来源：http://hz.aibaodan.cn/gtksidjeja.html

================================================================================
来源：http://hz.52xcode.cn/gtkykfhgpw.html

[K01] 对象转 JSON 字符串
来源：http://hz.yonumen.top/gtqhdntmcj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.fengsongda.top/gtnmgfevww.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shzxlz.cn/gtqddmjagy.html

JS:   JSON.stringify(obj)
来源：http://hz.wangshuangyany.cn/gtmcqawiyp.html

TS:   JSON.stringify(obj)
来源：http://hz.yanxiufei.cn/gtspckslbq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.pycfn.com/gtnmxpecny.html

Go:   json.Marshal(obj)
来源：http://hz.xuanzx.com/gtanjvcjyc.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yj20258888.top/gtxttirpgw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.316326.xyz/gtcdfewsue.html

[K02] JSON 字符串转对象
来源：http://hz.bjfxy.top/gtkoyphhkm.html

Py:   json.loads(s)
来源：http://hz.jlsjyb.cn/gttjhcdrwd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.sxryk.cn/gtdqgfwmxa.html

JS:   JSON.parse(s)
来源：http://hz.guowangkeji.top/gtxyprmfii.html

TS:   JSON.parse(s)
来源：http://hz.jinyuanbaomall.cn/gtikphxpue.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.aibaodan.cn/gtjsspzdpx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cheryme.top/gtvhfmlfdi.html

Ruby: JSON.parse(s)
来源：http://hz.wangdashe.top/gtvezgmych.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.aibaodan.cn/gtibntpqgv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yvedp.cn/gtnupoxzeu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zycfv.cn/gtabceiknm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jiagoushi.top/gtrbaquvry.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yongpay.top/gtjelviocm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinyuanbaomall.cn/gtbfdvogpn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhaomingkeji.xyz/gtjeykyscr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xylfe.cn/gticmmndpq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.havefunace.top/gtygnnnxgj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yj20258888.top/gtfdbduvpb.html

[K04] 读取 JSON 文件
来源：http://hz.nwbrower.top/gtgthsevfi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shzxlz.cn/gtdamjbyxs.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shangyingyoupin.top/gtmdqusyoi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xuanzx.com/gtyigjxooa.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xingfuxueyuan.xyz/gtrqfnyvqc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhongyouzk.top/gtvtggqmhc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.kuanghao11.cn/gtgxivwbjo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.0kj1m.cn/gtpfddgpfn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.snrcjt.cn/gtsbqhfdob.html

[K05] 深拷贝对象
来源：http://hz.xuanzx.com/gtaafrlfqp.html

Py:   copy.deepcopy(obj)
来源：http://hz.yangfankeji.com/gtvaabjyoi.html

PHP:  unserialize(serialize($obj));
来源：http://hz.gotoacloud.top/gtgaxktymk.html

JS:   structuredClone(obj)
来源：http://hz.haohaochexian.top/gtfuvoahpo.html

TS:   structuredClone(obj)
来源：http://hz.jinqigufen.top/gtfrpujstw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.haohaochexian.top/gtrlzpqlow.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xinyue.icu/gtthcwiebn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jqgfzy.top/gtvipexpeg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shuidangran.top/gtvasutxcj.html

[K06] 解析 URL 查询串
来源：http://hz.jiagoushi.top/gtbtkibwxg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xuetiantiany.cn/gtuolgodky.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhiwuduotai.top/gtifnqnycb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jlsjyb.cn/gtqvbsbmdl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hammf.cn/gtxhszjvdx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.nanxinkj.top/gtcwjlwpsu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sweek.top/gthbyhmhsp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yangfankeji.com/gtgjnnoxiy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yj20258888.top/gtfknshyjt.html

[K07] 进制转换
来源：http://hz.yangfankeji.com/gtwizivxsm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.dashuyun.cn/gtddxgekiw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.pycfn.com/gtgeifjdza.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.tianlin.xyz/gtlxnyhevv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yvedp.cn/gtipghxzpu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.316326.xyz/gtqbzslzco.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nanxinkj.top/gtivcwndsl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gogol.net.cn/gtmclfisie.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.guowangkeji.top/gtnbsxzynk.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.svipenyu.cn/gtqldkddqn.html

Py:   pickle.dumps(obj)
来源：http://hz.guowangkeji.top/gtmhysbzuq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.quarkkingdee.top/gthqjwnlqo.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.0kj1m.cn/gtrmteznot.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.redwolf501.top/gtcrlqfrze.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhiwuduotai.top/gtlmycwbbw.html

Go:   encoding/gob
来源：http://hz.havefunace.top/gtsvszjpoy.html

Ruby: Marshal.dump(obj)
来源：http://hz.birdmap.top/gtuyufffej.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.redwolf501.top/gtvyupajzs.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtptfqpasg.html

L. 网络请求
来源：http://hz.guowangkeji.top/gtutvhcyfk.html

================================================================================
来源：http://hz.cashguo.top/gtspdwlzdu.html

[L01] 发送 GET 请求
来源：http://hz.nanxuanxn.top/gtvfzbtofu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yongpay.top/gtvuzmchoi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cdnleiting.top/gttdpqragj.html

JS:   await fetch(url)
来源：http://hz.meibo888.top/gtvnyftuzp.html

TS:   await fetch(url)
来源：http://hz.nanxuanxn.top/gtgsonsvie.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shanyushiyangkeji.top/gtfjccyphh.html

Go:   resp, err := http.Get(url)
来源：http://hz.ywan-chungtsiang.top/gtbfsmvnpb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hongshengwenyu.top/gtypklawym.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.smart0.xyz/gtqttfauax.html

[L02] 发送 POST JSON
来源：http://hz.ywan-chungtsiang.top/gtjilgvozk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.sxryk.cn/gtfxwesenk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.9152youxi.cn/gtsuvvbaug.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhengqikj.top/gtrprwyokq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuanzx.com/gtrubcmwkj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.cashguo.top/gtsbzacfhy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sxryk.cn/gtawknrytm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shangyingyoupin.top/gtfoajvrey.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.chenjidiqi.icu/gticirohqo.html

[L03] 设置自定义请求头
来源：http://hz.sysykeji.top/gthxvhprme.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yuxming.cn/gtijysidxw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shuidangran.top/gtszejgwir.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.fzhhl.top/gtvrirjiwo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yvedp.cn/gtlrzxyalq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.wangshuangyany.cn/gtgtoojtvf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.aibaodan.cn/gtwgyupolg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhijiandao.cn/gtieistgna.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gotoacloud.top/gtmyxdrhhb.html

[L04] 设置超时
来源：http://hz.wangdashe.top/gtmdmaikav.html

Py:   requests.get(url, timeout=5)
来源：http://hz.316326.xyz/gtechcootz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ydzc1.top/gtlqbpurpb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuanzx.com/gtaycladxi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guowangkeji.top/gtfxlebmss.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gaohongyu789.top/gtbpnvsadz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhengqikj.top/gtpdnmrqie.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.chenlongwang.top/gtqmobmeuy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.snrcjt.cn/gtjxmpmecz.html

[L05] 上传文件（multipart）
来源：http://hz.xuetiantiany.cn/gtvbkvoniy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yj20258888.top/gtywzhpbtx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.snrcjt.cn/gtturfrhtl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yuxming.cn/gtwajcymou.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinghuilouyu.cn/gtxozitzdp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ydjk.org.cn/gtxvizmaip.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yj20258888.top/gtctbqaquw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhiwuduotai.top/gtneqprdps.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xuanzx.com/gtiemtfyme.html

[L06] 解析响应为 JSON
来源：http://hz.gotoacloud.top/gtgfvrrlmb.html

Py:   resp.json()
来源：http://hz.guowangkeji.top/gtwxmaztes.html

PHP:  json_decode($body, true);
来源：http://hz.redwolf501.top/gthzoahxhq.html

JS:   await resp.json()
来源：http://hz.0kj1m.cn/gtzvuqlfqh.html

TS:   await resp.json()
来源：http://hz.yonumen.top/gtlhwnkzny.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.guannengcc.top/gtnbpdmguo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.fzhhl.top/gtnyrggrmp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.daria6918.cn/gtghujpcsc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yuanzhike.top/gtnqdgrfeh.html

[L07] 处理 HTTP 状态码
来源：http://hz.yonumen.top/gtxcbsndou.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.gotoacloud.top/gtlnhxrpdr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.nwbrower.top/gtgpxzddkd.html

JS:   resp.ok;  resp.status
来源：http://hz.meibo888.top/gtaaykpsde.html

TS:   resp.ok;  resp.status
来源：http://hz.jianghu66.top/gtoepiuuvk.html

Java: resp.statusCode()
来源：http://hz.zhoulong.xyz/gtwrpwfeyn.html

Go:   resp.StatusCode
来源：http://hz.ydzc1.top/gtbnrcadhz.html

Ruby: resp.code.to_i
来源：http://hz.aizwys.cn/gtinalnnmm.html

C#:   (int)resp.StatusCode
来源：http://hz.gzhubu.top/gtsarxarow.html

[L08] 并发请求多个地址
来源：http://hz.xylfe.cn/gtjqqnqstl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhoulong.xyz/gtpeyoprrk.html

PHP:  curl_multi_init() 系列
来源：http://hz.yanxiufei.cn/gtxwprfvge.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hywenlv.cn/gtnfuyebqv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangdashe.top/gtcztxkfqs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinghuilouyu.cn/gtasfhzhve.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.bjfxy.top/gtkrkupzxh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yuxming.cn/gtxmclypxs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.bjfxy.top/gtxpcxmwir.html

================================================================================
来源：http://hz.zhijiandao.cn/gtuopgzsja.html

M. 命令行 / 进程 / 环境
来源：http://hz.cucudq.cn/gtdlcepudb.html

================================================================================
来源：http://hz.shuidangran.top/gthjehhlyh.html

[M01] 读取命令行参数
来源：http://hz.dashuyun.cn/gtssxrtjqh.html

Py:   sys.argv[1:]
来源：http://hz.tian-w.cn/gtpfvtgtbt.html

PHP:  $argv;  $argc;
来源：http://hz.shanyushiyangkeji.top/gtokbiyrfu.html

JS:   process.argv.slice(2)
来源：http://hz.hnqzz.top/gttvizzdzz.html

TS:   process.argv.slice(2)
来源：http://hz.gzhubu.top/gtxzxmczpa.html

Java: args 数组（main 方法参数）
来源：http://hz.ywan-chungtsiang.top/gtxxctjhgp.html

Go:   os.Args[1:]
来源：http://hz.yuxming.cn/gtnuuhcthw.html

Ruby: ARGV
来源：http://hz.gzhubu.top/gtvbinsdqy.html

C#:   args 数组（Main 方法参数）
来源：http://hz.fengsongda.top/gtkrxveikh.html

[M02] 读取环境变量
来源：http://hz.dashuyun.cn/gtoxgqngvy.html

Py:   os.environ.get("HOME")
来源：http://hz.jqgfzy.top/gtfmerozpi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ehwqpu.com/gtvshtvvco.html

JS:   process.env.HOME
来源：http://hz.nanxinkj.top/gtdhnrpytg.html

TS:   process.env.HOME
来源：http://hz.zhoulong.xyz/gtlffuyvel.html

Java: System.getenv("HOME")
来源：http://hz.yueranfly.top/gtkdpjxhas.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.52xcode.cn/gtsetdymrv.html

Ruby: ENV["HOME"]
来源：http://hz.pycfn.com/gtbtrwtqmo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.meibo888.top/gtyndaqijo.html

[M03] 执行外部命令
来源：http://hz.havefunace.top/gtvkkqxmso.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yj202588.top/gthfxxwcwy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xinyue.icu/gtnorrrdao.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.quarkkingdee.top/gthfaoszqg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gaohongyu789.top/gtadzkwgjt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jinqigufen.top/gtlyitrqti.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jinqigufen.top/gtqnclfmcv.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.snrcjt.cn/gtiubeicef.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yanxiufei.cn/gtdqflbgqk.html

[M04] 获取当前工作目录
来源：http://hz.nwbrower.top/gtqleqbumd.html

Py:   os.getcwd()
来源：http://hz.xinyue.icu/gtgwxemuvs.html

PHP:  getcwd();
来源：http://hz.sxryk.cn/gthjrprpgg.html

JS:   process.cwd()
来源：http://hz.svipenyu.cn/gtujcsginu.html

TS:   process.cwd()
来源：http://hz.yuanzhike.top/gtgvxqccpe.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yanxiufei.cn/gtplgnozen.html

Go:   os.Getwd()
来源：http://hz.cdnleiting.top/gtoajypgpk.html

Ruby: Dir.pwd
来源：http://hz.gzhubu.top/gthdgbxexu.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cashguo.top/gtnqdbndcd.html

[M05] 设置退出码
来源：http://hz.gogol.net.cn/gtharkrvxa.html

Py:   sys.exit(1)
来源：http://hz.zhiwuduotai.top/gtzppmwkaq.html

PHP:  exit(1);
来源：http://hz.zhixingplan.top/gtqfxbptwa.html

JS:   process.exit(1)
来源：http://hz.wangdashe.top/gtdquktatq.html

TS:   process.exit(1)
来源：http://hz.hysaishi.cn/gtfxhunmgg.html

Java: System.exit(1)
来源：http://hz.ydzc1.top/gtbnoxeofg.html

Go:   os.Exit(1)
来源：http://hz.hysaishi.cn/gtuvyscnqz.html

Ruby: exit 1
来源：http://hz.hongshengwenyu.top/gtvpojzrab.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yongpay.top/gtskhvptnb.html

[M06] 向标准错误输出
来源：http://hz.aibaodan.cn/gtaqzomyjp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinyuanbaomall.cn/gtswtquphh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xuanzx.com/gtmnickouv.html

JS:   console.error("err")
来源：http://hz.yuxming.cn/gtizeemcwq.html

TS:   console.error("err")
来源：http://hz.zhiwuduotai.top/gtahvspeua.html

Java: System.err.println("err")
来源：http://hz.yuanzhike.top/gtcfzbkssw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.snrcjt.cn/gtjiaeouna.html

Ruby: warn "err"
来源：http://hz.daria6918.cn/gtzmkmtdwd.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ehwqpu.com/gtrddkaylh.html

[M07] 判断是否为主入口
来源：http://hz.sysykeji.top/gthqhapksi.html

Py:   if __name__ == "__main__":
来源：http://hz.cucudq.cn/gtywfifirt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.vqdsnc.cn/gtfrtlszsh.html

JS:   require.main === module
来源：http://hz.yj20258888.top/gtnkkskpat.html

TS:   require.main === module
来源：http://hz.zhijiandao.cn/gtnmjklnyf.html

Java: public static void main(String[] args)
来源：http://hz.birdmap.top/gtkyshbzkj.html

Go:   func main()
来源：http://hz.zhiwuduotai.top/gtdtqelsol.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yanxiufei.cn/gtgbqlbbtz.html

C#:   static void Main(string[] args)
来源：http://hz.hongshengwenyu.top/gtojspzrkb.html

[M08] 获取系统与运行时信息
来源：http://hz.aibaodan.cn/gtohlaxuaw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhengqikj.top/gtrdllnkrm.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.quarkkingdee.top/gtusgvjgjn.html

JS:   process.platform;  process.version
来源：http://hz.jqgufenzy.top/gtaaomblmv.html

TS:   process.platform;  process.version
来源：http://hz.zdqjudy.top/gtapbvlsyn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sweek.top/gtegahqlcy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.svipenyu.cn/gtezyudpts.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.snrcjt.cn/gtffybwnpc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cucudq.cn/gtydsuubaq.html

================================================================================
来源：http://hz.9152youxi.cn/gtdrzyrgsk.html

N. 数据结构与算法
来源：http://hz.yueranfly.top/gtvdpoksdx.html

================================================================================
来源：http://hz.zhoulong.xyz/gtvqbamzhh.html

[N01] 二分查找（有序数组）
来源：http://hz.zdqjudy.top/gtcbynpwwm.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ydzc1.top/gtpylcfddt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ybcxt.top/gtikqtagmi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.guannengcc.top/gtfxwtqpui.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fengsongda.top/gtwymysamh.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zycfv.cn/gtflzawvfa.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ydzc1.top/gtrdcqjvul.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.daria6918.cn/gtydoedurz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.tanke756.top/gtxkwgcjcg.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.redwolf501.top/gtjalviyac.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigufen.top/gtnyifqbbs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.feifeiyinyue.top/gtotgcbkgl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.9152youxi.cn/gtmuzuqhzk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xylfe.cn/gtbwdrioqv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.tianlin.xyz/gthxzegkxn.html

Go:   slices.Sort(arr)
来源：http://hz.ppjwa.cn/gttijfgynm.html

Ruby: arr.sort
来源：http://hz.xuetiantiany.cn/gtuolssznq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.pengpengdd.cyou/gturisdguf.html

[N03] 快速排序（分治示例）
来源：http://hz.mhx1999.top/gtiyuuxldc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhaomingkeji.xyz/gtshkbwyui.html

PHP:  // 递归实现，或用 usort
来源：http://hz.snrcjt.cn/gtsglklfll.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhaomingkeji.xyz/gtxjkdpvsf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hnqzz.top/gtgcigsugc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.daria6918.cn/gtywjgyzjr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.quarkkingdee.top/gtjefywdtt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hysaishi.cn/gtfbgylyta.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jqgfzy.top/gtcijrcqul.html

[N04] 斐波那契数列
来源：http://hz.bjfxy.top/gtccwjwzxu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.pengpengdd.cyou/gtnabgpprn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhixingplan.top/gthiverkby.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258.top/gtuckkoxih.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigufen.top/gtolwucjyl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.aizwys.cn/gtfkytxrnl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.daxiang520.top/gtgxptqwtg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigfzy.top/gtgfnftvvy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ybcxt.top/gtjyqxonxc.html

[N05] 最大公约数
来源：http://hz.ywan-chungtsiang.top/gtavedcwkc.html

Py:   math.gcd(a, b)
来源：http://hz.jianghu66.top/gtsziochci.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.chenzaomai.com/gtktauroqu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aibaodan.cn/gtgbhczraw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnqzz.top/gtgibsdchn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.nwbrower.top/gtbeyubblg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.316326.xyz/gtasueuzqf.html

Ruby: a.gcd(b)
来源：http://hz.havefunace.top/gtkeclhjea.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.tanke756.top/gtgatdwikj.html

[N06] 判断回文字符串
来源：http://hz.jinqigufen.top/gtvdoisgbc.html

Py:   s == s[::-1]
来源：http://hz.gotoacloud.top/gtynkrtehg.html

PHP:  $s === strrev($s);
来源：http://hz.shanyushiyangtech.top/gtiqiakxqm.html

JS:   s === [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtcfhwoude.html

TS:   s === [...s].reverse().join("")
来源：http://hz.guowangkeji.top/gtqnhxgorv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yj20258.top/gthfonucjz.html

Go:   // 双指针从两端比较
来源：http://hz.yuxming.cn/gtagxxifwd.html

Ruby: s == s.reverse
来源：http://hz.zhijiandao.cn/gtzlvbiwhe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gogol.net.cn/gtqcijaxeh.html

[N07] 两数之和（返回下标）
来源：http://hz.redwolf501.top/gtysgdiskn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yvedp.cn/gtqlnhitcf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.guannengcc.top/gtclojiuhd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.mhx1999.top/gtdzortyqt.html

TS:   // 手写 Map<string, number>
来源：http://hz.chenlongwang.top/gtgczqwjxy.html

Java: // 手写 HashMap
来源：http://hz.guannengcc.top/gtsmjaevmg.html


<!-- 参考信息 -->