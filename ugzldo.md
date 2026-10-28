代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.wangshuangyany.cn/gtzzvilgbm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gaohongyu789.top/gtbdcrbllz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yangfankeji.com/gtgqmqfvne.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinyuanbaomall.cn/gtvvruqshz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jlsjyb.cn/gtnfpmakft.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xuanzx.com/gtpetienva.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yj20258.top/gtiuapmuyw.html

[J10] 取今天 / 本月第一天
来源：http://hz.9152youxi.cn/gtjmotovrv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hfpthk.cn/gtoajxfosm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.wangdashe.top/gtbrtkopgt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yongpay.top/gtkebqtzbg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yongpay.top/gtqaghuxyx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.smart0.xyz/gtrdftmejq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.fzhhl.top/gtcnpylbmu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhiwuduotai.top/gtllnrycuf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.mhx1999.top/gtabrkehwm.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtqgpgruzg.html

K. JSON 与序列化
来源：http://hz.nanxinkj.top/gtseiwjfab.html

================================================================================
来源：http://hz.hammf.cn/gtuucuvtms.html

[K01] 对象转 JSON 字符串
来源：http://hz.quarkkingdee.top/gthufckdwe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.dashuyun.cn/gtincffkfg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xinyue.icu/gtbojbpbcb.html

JS:   JSON.stringify(obj)
来源：http://hz.yuxming.cn/gtcetlkqqd.html

TS:   JSON.stringify(obj)
来源：http://hz.zhijiandao.cn/gtpydjcvbk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinghuilouyu.cn/gtwhbwoggv.html

Go:   json.Marshal(obj)
来源：http://hz.xziqi.cn/gtuomqvgzt.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.fzhhl.top/gtgflwipwn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yangfankeji.com/gtprlzfool.html

[K02] JSON 字符串转对象
来源：http://hz.birdmap.top/gtakumvuvo.html

Py:   json.loads(s)
来源：http://hz.yanxiufei.cn/gtpsgtucls.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.quarkkingdee.top/gtyvriybya.html

JS:   JSON.parse(s)
来源：http://hz.cqqwz.cn/gtwlfhztrj.html

TS:   JSON.parse(s)
来源：http://hz.xingfuxueyuan.xyz/gtimktugjm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hongshengwenyu.top/gtgqhfxilb.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.0kj1m.cn/gtnvplmuuz.html

Ruby: JSON.parse(s)
来源：http://hz.gotoacloud.top/gtmkpcaqfw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.snrcjt.cn/gtdrtczhid.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.tian-w.cn/gtnwdgzyic.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jyoumei.cn/gtvmlsyiui.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.daxiang520.top/gtkwctabeu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.guowangkeji.top/gtmqbiyyop.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.nwbrower.top/gtcaunkkmu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.tian-w.cn/gthdjlodti.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinyuanbaomall.cn/gtaorajiyb.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nanxuanxn.top/gtmmyeleuc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.shanyushiyangtech.top/gtvpcwpppd.html

[K04] 读取 JSON 文件
来源：http://hz.ivvv.top/gtflaqpqpr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jianghu66.top/gtxosqaxbg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ivvv.top/gtoaiitgsy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guowangkeji.top/gtylaepbtt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenzaomai.com/gtkfrygpks.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.fzhhl.top/gtrcglwnbz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.gaohongyu789.top/gtaamhyvtn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.birdmap.top/gtqxfxlgrv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yj20258.top/gtbivfqtui.html

[K05] 深拷贝对象
来源：http://hz.hammf.cn/gtewmdfidu.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj20258888.top/gtksscoipo.html

PHP:  unserialize(serialize($obj));
来源：http://hz.aibaodan.cn/gtjeijujcz.html

JS:   structuredClone(obj)
来源：http://hz.xylfe.cn/gtqbubvvik.html

TS:   structuredClone(obj)
来源：http://hz.haohaochexian.top/gtlzeoaqji.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yueranfly.top/gtkymblcdr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenzaomai.com/gtqucpypaj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gogol.net.cn/gtalryhieu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cashguo.top/gtjmncsjjj.html

[K06] 解析 URL 查询串
来源：http://hz.yueranfly.top/gtggqfmlmx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zdqjudy.top/gtlwphxdtq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hongshengwenyu.top/gtpiomkzve.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj202588.top/gthkvimhsb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.andypj.xyz/gtjkcwiynw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.mhx1999.top/gturbezdid.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ydzc1.top/gtrmcewuwf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yuxming.cn/gtrmxfyclq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cashguo.top/gtchefncgq.html

[K07] 进制转换
来源：http://hz.sxryk.cn/gtnbnrqqem.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gthfwuzcpi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jianghu66.top/gtooiydmqb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xuanzx.com/gtdstklzht.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shangyingyoupin.top/gtwnolodix.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hongshengwenyu.top/gtmyjoxswe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.fzhhl.top/gtphtikaku.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xuetiantiany.cn/gtwllsavqk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtrycysyjt.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yonumen.top/gtgwsmwrod.html

Py:   pickle.dumps(obj)
来源：http://hz.meibo888.top/gtnhufghqf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cdnleiting.top/gtgkzlpgrf.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yangfankeji.com/gtiswirkve.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.sxryk.cn/gtyrkrgbnk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.tianlin.xyz/gtkuaosjwv.html

Go:   encoding/gob
来源：http://hz.shzxlz.cn/gtwheatran.html

Ruby: Marshal.dump(obj)
来源：http://hz.yangfankeji.com/gtvjjulydv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jqgufenzy.top/gtvssfrfvu.html

================================================================================
来源：http://hz.yj20258888.top/gtiawklmbt.html

L. 网络请求
来源：http://hz.jqgfzy.top/gtufmkndum.html

================================================================================
来源：http://hz.c1oappe.top/gtwygnecxx.html

[L01] 发送 GET 请求
来源：http://hz.fengsongda.top/gtebhtfihn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yj20258888.top/gtfiindoqz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.gaohongyu789.top/gtitqtjcro.html

JS:   await fetch(url)
来源：http://hz.tian-w.cn/gtatgjgdjs.html

TS:   await fetch(url)
来源：http://hz.jlsjyb.cn/gtrquhcbkq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yangfankeji.com/gttogjmtwb.html

Go:   resp, err := http.Get(url)
来源：http://hz.wangshuangyany.cn/gtgzuxnkio.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jlsjyb.cn/gtjgxbjuut.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shanyushiyangtech.top/gtdpjlycet.html

[L02] 发送 POST JSON
来源：http://hz.iojbl.cn/gtqucynzcc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yuanzhike.top/gtjgxaxutj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.dianchejie.cn/gtgnltvndj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pycfn.com/gtirkhnicp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xinyue.icu/gttkporuft.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.chenzaomai.com/gtumlahoxm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sufxvd.cn/gtgctdoiqk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xinyue.icu/gtnmplzpui.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ydjk.org.cn/gtxpctushy.html

[L03] 设置自定义请求头
来源：http://hz.pycfn.com/gtdqelezup.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jlsjyb.cn/gttaoqrvhc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ywan-chungtsiang.top/gtsddnvgmp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinqigfzy.top/gthbescquq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.vqdsnc.cn/gtiovgoycs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jinqigufen.top/gtxqvkbqiu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yvedp.cn/gtbcjzlurg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhengqikj.top/gtbrykhrto.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.fengsongda.top/gtgdzhfjxa.html

[L04] 设置超时
来源：http://hz.zhijiandao.cn/gtjpuuuyuh.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yuxming.cn/gtweztenqf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ydjk.org.cn/gtejcbpzqn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuetiantiany.cn/gtzcggocud.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cashguo.top/gtgriwzojp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yj202588.top/gtleucrdvx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yuanzhike.top/gtixirlcrq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ybcxt.top/gtkqfzkajh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.gaohongyu789.top/gtpxqvbtxh.html

[L05] 上传文件（multipart）
来源：http://hz.yj202588.top/gtuwrbpfqt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.9152youxi.cn/gtarokkvtc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yvedp.cn/gthyorwekv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhongyouzk.top/gtmcnovpxy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hammf.cn/gtbkpsbtxb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhoulong.xyz/gtbejlxptp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yangfankeji.com/gtofmlwjod.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.redwolf501.top/gtgmowxgxn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhongyouzk.top/gtemvijdgo.html

[L06] 解析响应为 JSON
来源：http://hz.smart0.xyz/gtnplzptzy.html

Py:   resp.json()
来源：http://hz.smart0.xyz/gtajdkaprh.html

PHP:  json_decode($body, true);
来源：http://hz.snrcjt.cn/gthhrohaxy.html

JS:   await resp.json()
来源：http://hz.hongshengwenyu.top/gtzzwvztgh.html

TS:   await resp.json()
来源：http://hz.guannengcc.top/gtwvixhhdm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yongpay.top/gtlzzjyvte.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.fzhhl.top/gtchaqiylq.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yuanzhike.top/gtagaxzfpi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.9152youxi.cn/gtnuuvrmqi.html

[L07] 处理 HTTP 状态码
来源：http://hz.jlsjyb.cn/gtcjmgtokn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xingfuxueyuan.xyz/gtdhdwwsva.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jlsjyb.cn/gtwionnhbz.html

JS:   resp.ok;  resp.status
来源：http://hz.yuanzhike.top/gtcojmqvjr.html

TS:   resp.ok;  resp.status
来源：http://hz.feifeiyinyue.top/gtlmztlfir.html

Java: resp.statusCode()
来源：http://hz.cdnleiting.top/gtuqyvsmst.html

Go:   resp.StatusCode
来源：http://hz.zhaomingkeji.xyz/gthqzvcgqr.html

Ruby: resp.code.to_i
来源：http://hz.yanxiufei.cn/gtymoivcta.html

C#:   (int)resp.StatusCode
来源：http://hz.yangfankeji.com/gtjfslefqd.html

[L08] 并发请求多个地址
来源：http://hz.fengsongda.top/gtbfwevnbg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gotoacloud.top/gtylirtnuc.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhaomingkeji.xyz/gtnagvwhdf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yangfankeji.com/gthoxeboan.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.vqdsnc.cn/gtkrgvkzjj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.birdmap.top/gtjtkfzgth.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinqigfzy.top/gtqzfphkwv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.chenjidiqi.icu/gtkwfblzag.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.guannengcc.top/gthezhvuac.html

================================================================================
来源：http://hz.yongpay.top/gtrgozrzxj.html

M. 命令行 / 进程 / 环境
来源：http://hz.hfpthk.cn/gtxfxkvbvj.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtaplhsjsi.html

[M01] 读取命令行参数
来源：http://hz.xziqi.cn/gtftwhhrom.html

Py:   sys.argv[1:]
来源：http://hz.mhx1999.top/gtrtatsumi.html

PHP:  $argv;  $argc;
来源：http://hz.dianchejie.cn/gtmtkvezew.html

JS:   process.argv.slice(2)
来源：http://hz.zhijiandao.cn/gtitibvuoj.html

TS:   process.argv.slice(2)
来源：http://hz.fzhhl.top/gtvjejuxjj.html

Java: args 数组（main 方法参数）
来源：http://hz.jyoumei.cn/gtvkfenlpw.html

Go:   os.Args[1:]
来源：http://hz.zhiwuduotai.top/gthwmhvlkq.html

Ruby: ARGV
来源：http://hz.zhiwuduotai.top/gtkdlipdqb.html

C#:   args 数组（Main 方法参数）
来源：http://hz.fzhhl.top/gtiqlpqjyq.html

[M02] 读取环境变量
来源：http://hz.daxiang520.top/gtrjxqnalk.html

Py:   os.environ.get("HOME")
来源：http://hz.xinyue.icu/gtkmyazity.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinqigufen.top/gttdnwilmo.html

JS:   process.env.HOME
来源：http://hz.smart0.xyz/gtnmpccggt.html

TS:   process.env.HOME
来源：http://hz.vqdsnc.cn/gtdxnpggox.html

Java: System.getenv("HOME")
来源：http://hz.xinyue.icu/gtwailqcrp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.316326.xyz/gtehnqjrkn.html

Ruby: ENV["HOME"]
来源：http://hz.shanyushiyangtech.top/gtznvyehkm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhongyouzk.top/gttbjsgbaa.html

[M03] 执行外部命令
来源：http://hz.guowangkeji.top/gtbjbcnhtx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ydzc1.top/gtppsvzfdg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.wangshuangyany.cn/gtmhmdyrwc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj202588.top/gtwwaytfpl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangkeji.top/gtbfkhmnvl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.pycfn.com/gtlncvqdrp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.pengpengdd.cyou/gtdrqqtyvw.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhongyouzk.top/gtlzzqjmxi.html

C#:   Process.Start("ls", "-l");
来源：http://hz.guannengcc.top/gtkgomtrag.html

[M04] 获取当前工作目录
来源：http://hz.gogol.net.cn/gtdlzebghu.html

Py:   os.getcwd()
来源：http://hz.c1oappe.top/gthhpokkft.html

PHP:  getcwd();
来源：http://hz.shanyushiyangtech.top/gtmqjdxrpu.html

JS:   process.cwd()
来源：http://hz.zhengqikj.top/gtoxgbwxrx.html

TS:   process.cwd()
来源：http://hz.pycfn.com/gtactkynbj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.daria6918.cn/gtqvbzjafe.html

Go:   os.Getwd()
来源：http://hz.sweek.top/gtlrisfivj.html

Ruby: Dir.pwd
来源：http://hz.jianghu66.top/gtksdshazx.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hywenlv.cn/gtmiormrku.html

[M05] 设置退出码
来源：http://hz.nanxuanxn.top/gtphdqqxkm.html

Py:   sys.exit(1)
来源：http://hz.hongshengwenyu.top/gtxiffgugh.html

PHP:  exit(1);
来源：http://hz.xingfuxueyuan.xyz/gtxfftddbx.html

JS:   process.exit(1)
来源：http://hz.hnqzz.top/gtfcfnpqez.html

TS:   process.exit(1)
来源：http://hz.gogol.net.cn/gttmodvlvh.html

Java: System.exit(1)
来源：http://hz.guowangkeji.top/gtpxlpxoef.html

Go:   os.Exit(1)
来源：http://hz.cqqwz.cn/gtoxwuijck.html

Ruby: exit 1
来源：http://hz.cdnleiting.top/gtxmbjqzns.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.tanke756.top/gtbiakkovr.html

[M06] 向标准错误输出
来源：http://hz.kuanghao11.cn/gtqaffhqxk.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hysaishi.cn/gtadrsuzcc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xuetiantiany.cn/gtgtxpopjo.html

JS:   console.error("err")
来源：http://hz.quarkkingdee.top/gtyegbosye.html

TS:   console.error("err")
来源：http://hz.cashguo.top/gtkuvstqys.html

Java: System.err.println("err")
来源：http://hz.birdmap.top/gtppgvqokp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xylfe.cn/gtscddjdxo.html

Ruby: warn "err"
来源：http://hz.0kj1m.cn/gtrvrvcmyy.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shzxlz.cn/gtnnnsfbyj.html

[M07] 判断是否为主入口
来源：http://hz.sweek.top/gtglojlshj.html

Py:   if __name__ == "__main__":
来源：http://hz.chenlongwang.top/gtvnnalxrl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gogol.net.cn/gtspyocwkt.html

JS:   require.main === module
来源：http://hz.zdqjudy.top/gtygdmzbgi.html

TS:   require.main === module
来源：http://hz.jyoumei.cn/gtugynpirm.html

Java: public static void main(String[] args)
来源：http://hz.yuxming.cn/gtemykbaky.html

Go:   func main()
来源：http://hz.jlsjyb.cn/gtqfedmkyy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jqgufenzy.top/gtdyhxtruk.html

C#:   static void Main(string[] args)
来源：http://hz.316326.xyz/gtemjwiypv.html

[M08] 获取系统与运行时信息
来源：http://hz.ehwqpu.com/gtmdugubpi.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinqigfzy.top/gtqwvdzqgn.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.mhx1999.top/gtinextirb.html

JS:   process.platform;  process.version
来源：http://hz.jyoumei.cn/gtubkdotrs.html

TS:   process.platform;  process.version
来源：http://hz.tanke756.top/gtbarwukvp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.guowangkeji.top/gtplgcnmvs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xylfe.cn/gthfozlizs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hammf.cn/gtulwidkdk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.pengpengdd.cyou/gtawlsbpna.html

================================================================================
来源：http://hz.c1oappe.top/gteftmhahw.html

N. 数据结构与算法
来源：http://hz.svipenyu.cn/gtqgekwcpq.html

================================================================================
来源：http://hz.aizwys.cn/gtjhwiutwl.html

[N01] 二分查找（有序数组）
来源：http://hz.jinqigufen.top/gtncwdlvqg.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.wangdashe.top/gtmxlaejcj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhixingplan.top/gtqlpjeflm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aizwys.cn/gtqmvgjxyy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.mhx1999.top/gtscrqyrjq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.chenzaomai.com/gtohtrnted.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shuidangran.top/gthyxlqpgz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.guowangkeji.top/gtedskuwbq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jqgfzy.top/gtemiqiccb.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jianghu66.top/gtoaehtrxv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigufen.top/gtiojnvzwg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hnqzz.top/gthuntalpm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinyuanbaomall.cn/gtbpgtenjc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gzhubu.top/gtytvfhzui.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jqgufenzy.top/gtsjqoohov.html

Go:   slices.Sort(arr)
来源：http://hz.yangfankeji.com/gtpsepfwug.html

Ruby: arr.sort
来源：http://hz.hysaishi.cn/gtocqwaayq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.52xcode.cn/gtwpyxwwbj.html

[N03] 快速排序（分治示例）
来源：http://hz.sxryk.cn/gtesbbaznw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shanyushiyangtech.top/gtzivrjfwm.html

PHP:  // 递归实现，或用 usort
来源：http://hz.meibo888.top/gtwlmcfznr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.c1oappe.top/gtsjbactla.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jlsjyb.cn/gtfclrktjk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shuidangran.top/gtoqygchrq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.0kj1m.cn/gtpcaofihd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.tianlin.xyz/gtrttblgfp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hnqzz.top/gtxjsxdiwu.html

[N04] 斐波那契数列
来源：http://hz.sxryk.cn/gtxrafmzlh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.haohaochexian.top/gtbvvayhmr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhongyouzk.top/gtzsqrdqxg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhijiandao.cn/gtmjsemauw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258.top/gtgirvuxjs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yongpay.top/gtzaiuwnfl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinyuanbaomall.cn/gtiqdwxhjd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.birdmap.top/gtxlkmmnsf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zycfv.cn/gtduzpnifo.html

[N05] 最大公约数
来源：http://hz.jinghuilouyu.cn/gtuavqxwyd.html

Py:   math.gcd(a, b)
来源：http://hz.zhoulong.xyz/gtytpdxgpf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shzxlz.cn/gtxwptrfai.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.mhx1999.top/gtlzcezogm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xuetiantiany.cn/gtculumohz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.vqdsnc.cn/gtuwzkdaic.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zycfv.cn/gtfvzwsoba.html

Ruby: a.gcd(b)
来源：http://hz.chenzaomai.com/gtagfjmtiw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ppjwa.cn/gtzqtmatbl.html

[N06] 判断回文字符串
来源：http://hz.bjfxy.top/gtvfsvvgax.html

Py:   s == s[::-1]
来源：http://hz.hfpthk.cn/gtdeoirgjf.html

PHP:  $s === strrev($s);
来源：http://hz.zhongyouzk.top/gthxworeuk.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhoulong.xyz/gtnxslywai.html

TS:   s === [...s].reverse().join("")
来源：http://hz.chenjidiqi.icu/gtrtrwpail.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.smart0.xyz/gttxdicatj.html

Go:   // 双指针从两端比较
来源：http://hz.yueranfly.top/gtiwqcqwdf.html

Ruby: s == s.reverse
来源：http://hz.zhongyouzk.top/gtmkontpiv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hysaishi.cn/gtklertbhc.html

[N07] 两数之和（返回下标）
来源：http://hz.yueranfly.top/gtkuprbdss.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.tianlin.xyz/gtlwlghqzu.html


<!-- 参考信息 -->