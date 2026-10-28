代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sweek.top/gtyjvvnfsz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sweek.top/gthxecjopm.html

[J09] 时区处理
来源：http://hz.yj20258888.top/gtdawwzpsy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shanyushiyangtech.top/gtpcnivbag.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.smart0.xyz/gtyzfgwily.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shuidangran.top/gtzspouirg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ywan-chungtsiang.top/gtmlkswkmj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinyuanbaomall.cn/gtobnwhbhe.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhijiandao.cn/gtjxscuywq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hnqzz.top/gtfupjrnwz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ehwqpu.com/gtoiljvejw.html

[J10] 取今天 / 本月第一天
来源：http://hz.daria6918.cn/gtrzqfoqwr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.wangdashe.top/gtxoznoiok.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jyoumei.cn/gthzhglgbo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xziqi.cn/gtcolhksau.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hnqzz.top/gtreadrtra.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yj202588.top/gticzwcneg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.vqdsnc.cn/gtwaeudcia.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.pengpengdd.cyou/gtgsbbueqc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhongyouzk.top/gtweonuiei.html

================================================================================
来源：http://hz.zhixingplan.top/gtvuetbvgx.html

K. JSON 与序列化
来源：http://hz.jinyuanbaomall.cn/gtzmyxhybm.html

================================================================================
来源：http://hz.jinqigfzy.top/gttelakxsn.html

[K01] 对象转 JSON 字符串
来源：http://hz.0kj1m.cn/gtxtwqcsgp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.chenlongwang.top/gtaayhzqjd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ydzc1.top/gtyxrrbzib.html

JS:   JSON.stringify(obj)
来源：http://hz.guannengcc.top/gtiwahsidd.html

TS:   JSON.stringify(obj)
来源：http://hz.feifeiyinyue.top/gtqspxwmzj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.gotoacloud.top/gtofyzahwb.html

Go:   json.Marshal(obj)
来源：http://hz.fengsongda.top/gtqkghbnbg.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jianghu66.top/gtmualfhbl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xinyue.icu/gtpugyagzf.html

[K02] JSON 字符串转对象
来源：http://hz.guowangkeji.top/gtzaykyoxc.html

Py:   json.loads(s)
来源：http://hz.sweek.top/gtubnkuhxe.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhiwuduotai.top/gtmklborov.html

JS:   JSON.parse(s)
来源：http://hz.52xcode.cn/gtunpyaxtp.html

TS:   JSON.parse(s)
来源：http://hz.ppjwa.cn/gtbttrnaxt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.nanxuanxn.top/gtknmnzwpk.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.dianchejie.cn/gtugnqzohl.html

Ruby: JSON.parse(s)
来源：http://hz.cashguo.top/gtvywbjgui.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinqigfzy.top/gthhsdxvwl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hywenlv.cn/gtnrcxnhyx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.smart0.xyz/gtwtklifzt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yuanzhike.top/gtuxlsaiko.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhiwuduotai.top/gtzumcrbsk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yuanzhike.top/gtbhaesyyx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhaomingkeji.xyz/gtnxmeuojy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.nanxinkj.top/gtpphrptmt.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sxryk.cn/gthpwniwwx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.sxryk.cn/gtpeehfltu.html

[K04] 读取 JSON 文件
来源：http://hz.wangdashe.top/gtwuboczpr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.vqdsnc.cn/gtyndfqtyb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hongshengwenyu.top/gtemafrvwk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xingfuxueyuan.xyz/gtvctgvddg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dashuyun.cn/gtjkecsrmc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hysaishi.cn/gtzgibiwgs.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hnxiangtu.top/gtddqvfaia.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jiagoushi.top/gtwfkahnpx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ydjk.org.cn/gtqtntyljk.html

[K05] 深拷贝对象
来源：http://hz.gotoacloud.top/gtdkgfsdbi.html

Py:   copy.deepcopy(obj)
来源：http://hz.yuanzhike.top/gtfhwdnhfp.html

PHP:  unserialize(serialize($obj));
来源：http://hz.fzhhl.top/gtkeayyldi.html

JS:   structuredClone(obj)
来源：http://hz.feifeiyinyue.top/gtgonksfsn.html

TS:   structuredClone(obj)
来源：http://hz.sufxvd.cn/gteiulbnwq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.andypj.xyz/gtopuifdbe.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ppjwa.cn/gttpovigwo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.52xcode.cn/gthfoynven.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.nanxuanxn.top/gturvrowpi.html

[K06] 解析 URL 查询串
来源：http://hz.zhiwuduotai.top/gtgiszivqw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hywenlv.cn/gtpxiksxrz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shanyushiyangtech.top/gtttxskpgv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cucudq.cn/gtoimqbrbt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.52xcode.cn/gtjefneyuv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinqigufen.top/gtcltpdkhb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gaohongyu789.top/gtdxtkktpp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.smart0.xyz/gtzvdlcsty.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yvedp.cn/gttmqvjpcw.html

[K07] 进制转换
来源：http://hz.hywenlv.cn/gtgwvenghj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yj20258888.top/gttctzrmem.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.wangshuangyany.cn/gtbztiiwck.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.nwbrower.top/gtdhcvmfcs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yuxming.cn/gtiortjwvh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gtohybrioh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.andypj.xyz/gtakwdsoqe.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sxryk.cn/gtwgixvbnk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ehwqpu.com/gtnktgonfg.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xingfuxueyuan.xyz/gtsirszquz.html

Py:   pickle.dumps(obj)
来源：http://hz.sufxvd.cn/gtowsadzgv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.guannengcc.top/gtjmzqblum.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.guowangkeji.top/gtsqticvsi.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cheryme.top/gtbsdoagfm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.gaohongyu789.top/gtxiyfaeyo.html

Go:   encoding/gob
来源：http://hz.pycfn.com/gtvaqakfvz.html

Ruby: Marshal.dump(obj)
来源：http://hz.tanke756.top/gtqyexxhvy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sweek.top/gtlbcmviru.html

================================================================================
来源：http://hz.jqgfzy.top/gtckiqsovv.html

L. 网络请求
来源：http://hz.yvedp.cn/gtvytsxxvr.html

================================================================================
来源：http://hz.yvedp.cn/gtzrcmevnw.html

[L01] 发送 GET 请求
来源：http://hz.nanxuanxn.top/gtkkfkalrr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.52xcode.cn/gtgjyunbck.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.mhx1999.top/gtapnxpska.html

JS:   await fetch(url)
来源：http://hz.jqgufenzy.top/gtsrnpbkmw.html

TS:   await fetch(url)
来源：http://hz.c1oappe.top/gtqdqpuoff.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jianghu66.top/gtbuiyhccc.html

Go:   resp, err := http.Get(url)
来源：http://hz.yuanzhike.top/gtchirovwp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jqgufenzy.top/gtctehdpyd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xingfuxueyuan.xyz/gthzwrzdhr.html

[L02] 发送 POST JSON
来源：http://hz.xylfe.cn/gtjxshxcgy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zdqjudy.top/gtssolwvwb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xinyue.icu/gtgozzxgwt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pycfn.com/gthtnciknx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigufen.top/gtfbsgmttw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ywan-chungtsiang.top/gtpvevkkhq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.0kj1m.cn/gtrcscxssb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.andypj.xyz/gtkpxqlvrz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.c1oappe.top/gtajyjahxd.html

[L03] 设置自定义请求头
来源：http://hz.shanyushiyangtech.top/gtxasszims.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ydjk.org.cn/gtctgiuiim.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.9152youxi.cn/gtnqecadqg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jqgufenzy.top/gtxflnumud.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jiagoushi.top/gtzqmjuxtj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hnqzz.top/gttnooyvxd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.sxryk.cn/gtilmihehl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jianghu66.top/gtekxbcwww.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hywenlv.cn/gtcwkiazvl.html

[L04] 设置超时
来源：http://hz.pengpengdd.cyou/gtmcjquwer.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hammf.cn/gtitpxdtea.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.gotoacloud.top/gtqtvckcyc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shzxlz.cn/gtzxsdyxyr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhoulong.xyz/gtnfmzfrbx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.dashuyun.cn/gttiajcwyx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shangyingyoupin.top/gtkmtxzgvk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.mhx1999.top/gtchtbhyrm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hnqzz.top/gtjzxdfakj.html

[L05] 上传文件（multipart）
来源：http://hz.havefunace.top/gtbsobspeg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jqgfzy.top/gtiycdmwaj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yj20258888.top/gtfmmkpqcn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ybcxt.top/gtqbufkndg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.guowangkeji.top/gtvfggmldj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yj202588.top/gttvhoiuwu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.pycfn.com/gtspfgrnap.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yuxming.cn/gtkcznixju.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.tianlin.xyz/gtbvllyoes.html

[L06] 解析响应为 JSON
来源：http://hz.jiagoushi.top/gtcufdbrbs.html

Py:   resp.json()
来源：http://hz.wangshuangyany.cn/gtddnaxnoe.html

PHP:  json_decode($body, true);
来源：http://hz.smart0.xyz/gtkfmnrozi.html

JS:   await resp.json()
来源：http://hz.snrcjt.cn/gtuuzhujwo.html

TS:   await resp.json()
来源：http://hz.jiagoushi.top/gtsjxonobu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jlsjyb.cn/gtifzlbqnf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.chenzaomai.com/gtmqqrdgve.html

Ruby: JSON.parse(resp.body)
来源：http://hz.daxiang520.top/gtwdwscizh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shanyushiyangtech.top/gtzbetqnzz.html

[L07] 处理 HTTP 状态码
来源：http://hz.xuanzx.com/gthypeufem.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zdqjudy.top/gtpvosbbbi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.shuidangran.top/gtkkciyccv.html

JS:   resp.ok;  resp.status
来源：http://hz.zhoulong.xyz/gtpmhyzpnm.html

TS:   resp.ok;  resp.status
来源：http://hz.52xcode.cn/gtqgxkxaqz.html

Java: resp.statusCode()
来源：http://hz.zycfv.cn/gtkwktvfqg.html

Go:   resp.StatusCode
来源：http://hz.zhongyouzk.top/gtzzwyrqfh.html

Ruby: resp.code.to_i
来源：http://hz.jqgufenzy.top/gtlavhivpm.html

C#:   (int)resp.StatusCode
来源：http://hz.yvedp.cn/gtbkanirtf.html

[L08] 并发请求多个地址
来源：http://hz.yonumen.top/gtlkvkhehx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.shangyingyoupin.top/gtjvyrsgay.html

PHP:  curl_multi_init() 系列
来源：http://hz.zdqjudy.top/gtxbjxilqv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhaomingkeji.xyz/gtneucqgcs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.meibo888.top/gtxxywiawz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yj20258888.top/gtqsbetsmd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.bjfxy.top/gtzhkvmyai.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.dianchejie.cn/gtbviwommy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gaohongyu789.top/gtsptlxcqe.html

================================================================================
来源：http://hz.hnqzz.top/gtoeyxcoor.html

M. 命令行 / 进程 / 环境
来源：http://hz.gaohongyu789.top/gtzohagroq.html

================================================================================
来源：http://hz.zhoulong.xyz/gthrmxoxbn.html

[M01] 读取命令行参数
来源：http://hz.snrcjt.cn/gtrwmsfxlx.html

Py:   sys.argv[1:]
来源：http://hz.bjfxy.top/gtngsztaov.html

PHP:  $argv;  $argc;
来源：http://hz.aizwys.cn/gtffosxuaj.html

JS:   process.argv.slice(2)
来源：http://hz.xinyue.icu/gthamfrgei.html

TS:   process.argv.slice(2)
来源：http://hz.ydzc1.top/gtnlcozqdm.html

Java: args 数组（main 方法参数）
来源：http://hz.redwolf501.top/gtsjzywaha.html

Go:   os.Args[1:]
来源：http://hz.dianchejie.cn/gtgpddqdmv.html

Ruby: ARGV
来源：http://hz.feifeiyinyue.top/gtcitihbup.html

C#:   args 数组（Main 方法参数）
来源：http://hz.fzhhl.top/gtimtknynl.html

[M02] 读取环境变量
来源：http://hz.wangshuangyany.cn/gtmkszhmog.html

Py:   os.environ.get("HOME")
来源：http://hz.nwbrower.top/gtupyiuttp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sweek.top/gtxqpnidhc.html

JS:   process.env.HOME
来源：http://hz.daxiang520.top/gturqzzfvs.html

TS:   process.env.HOME
来源：http://hz.xylfe.cn/gtysbhcxrt.html

Java: System.getenv("HOME")
来源：http://hz.hammf.cn/gtdrermqst.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xylfe.cn/gtaolziqvn.html

Ruby: ENV["HOME"]
来源：http://hz.quarkkingdee.top/gtnrvzhhqt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jqgufenzy.top/gtqxypzaqd.html

[M03] 执行外部命令
来源：http://hz.cheryme.top/gtmwglmqwb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhongyouzk.top/gtrgctdbfl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yj20258888.top/gtqhaukbsy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sysykeji.top/gtvfdsqzdq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shangyingyoupin.top/gtnxllvfuj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.svipenyu.cn/gtqiiywgnq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.gogol.net.cn/gtzcqdpmpx.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shangyingyoupin.top/gtvrttxqdk.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xziqi.cn/gtsqwmqqab.html

[M04] 获取当前工作目录
来源：http://hz.redwolf501.top/gtdjspcvvv.html

Py:   os.getcwd()
来源：http://hz.guowangkeji.top/gtocnjxdkl.html

PHP:  getcwd();
来源：http://hz.jianghu66.top/gtazuubapt.html

JS:   process.cwd()
来源：http://hz.cdnleiting.top/gtrgqzejtx.html

TS:   process.cwd()
来源：http://hz.shanyushiyangtech.top/gthfilttek.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhixingplan.top/gtxqdhdjur.html

Go:   os.Getwd()
来源：http://hz.hnxiangtu.top/gtlmnlodlc.html

Ruby: Dir.pwd
来源：http://hz.yangfankeji.com/gtiagdxzov.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.9152youxi.cn/gtwheopzda.html

[M05] 设置退出码
来源：http://hz.yj202588.top/gtuccigmqu.html

Py:   sys.exit(1)
来源：http://hz.ydjk.org.cn/gtjjhgqniz.html

PHP:  exit(1);
来源：http://hz.chenlongwang.top/gtarccpnqu.html

JS:   process.exit(1)
来源：http://hz.yj20258.top/gtetoudqmk.html

TS:   process.exit(1)
来源：http://hz.kuanghao11.cn/gtfazweeiz.html

Java: System.exit(1)
来源：http://hz.hywenlv.cn/gtaavuzifa.html

Go:   os.Exit(1)
来源：http://hz.ehwqpu.com/gtrqxfmxgh.html

Ruby: exit 1
来源：http://hz.andypj.xyz/gtnhrmwlbf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cdnleiting.top/gtuvpkzeyj.html

[M06] 向标准错误输出
来源：http://hz.ydjk.org.cn/gtohvucpih.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jyoumei.cn/gtcgczouqw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.tian-w.cn/gtjwsbidjn.html

JS:   console.error("err")
来源：http://hz.zdqjudy.top/gtttktrjcc.html

TS:   console.error("err")
来源：http://hz.wangdashe.top/gtqcvnbktc.html

Java: System.err.println("err")
来源：http://hz.0kj1m.cn/gtsckjtlde.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.havefunace.top/gtaakpjtes.html

Ruby: warn "err"
来源：http://hz.sufxvd.cn/gtdfynjbmc.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.fzhhl.top/gtzdrcsgte.html

[M07] 判断是否为主入口
来源：http://hz.gogol.net.cn/gtxzorfljk.html

Py:   if __name__ == "__main__":
来源：http://hz.cashguo.top/gtexlojlzp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.birdmap.top/gtzjxbhqoc.html

JS:   require.main === module
来源：http://hz.wangshuangyany.cn/gtuhlhdulm.html

TS:   require.main === module
来源：http://hz.snrcjt.cn/gtwbrispyp.html

Java: public static void main(String[] args)
来源：http://hz.zhengqikj.top/gtfgcbuiye.html

Go:   func main()
来源：http://hz.cdnleiting.top/gtpwblxqvd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.meibo888.top/gtrkqxtsws.html

C#:   static void Main(string[] args)
来源：http://hz.wangdashe.top/gtsjjksprq.html

[M08] 获取系统与运行时信息
来源：http://hz.cdnleiting.top/gtvbhzztep.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ehwqpu.com/gtajzrmudo.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.tianlin.xyz/gtcvghuytp.html

JS:   process.platform;  process.version
来源：http://hz.cucudq.cn/gtfmpnznuk.html

TS:   process.platform;  process.version
来源：http://hz.jianghu66.top/gtsdilaywb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jiagoushi.top/gtjbzyejyc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhiwuduotai.top/gtmugewmyb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.tianlin.xyz/gtpudhvvyg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.redwolf501.top/gtqqdmntim.html

================================================================================
来源：http://hz.ppjwa.cn/gtrpdskoqu.html

N. 数据结构与算法
来源：http://hz.zhengqikj.top/gtojrwtfei.html

================================================================================
来源：http://hz.aizwys.cn/gtprgzptqy.html

[N01] 二分查找（有序数组）
来源：http://hz.ybcxt.top/gtotbwmtzu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtznbxgecm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shanyushiyangkeji.top/gtjupkzyia.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.havefunace.top/gtnajuloef.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sysykeji.top/gtvcyxtmoe.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yuxming.cn/gtzkdkjmzy.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.sysykeji.top/gtsvdyzqiv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.guowangkeji.top/gtglhxgiym.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhijiandao.cn/gtevcyodsi.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.guowangkeji.top/gtunpmcbio.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.bjfxy.top/gtzxfrqfar.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.havefunace.top/gtwhbmxxuv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ydzc1.top/gtrpatxkke.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gogol.net.cn/gtriaiclcx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jyoumei.cn/gtanabaafa.html

Go:   slices.Sort(arr)
来源：http://hz.cqqwz.cn/gtqxgocjrh.html

Ruby: arr.sort
来源：http://hz.xylfe.cn/gtmxqdcxux.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.pycfn.com/gtusvgzhmi.html

[N03] 快速排序（分治示例）
来源：http://hz.yonumen.top/gtglorvloj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xziqi.cn/gtmfpbiyit.html

PHP:  // 递归实现，或用 usort
来源：http://hz.bjfxy.top/gtbuzwwvxk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zdqjudy.top/gtgrlbofik.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gotoacloud.top/gtyzilvftf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xinyue.icu/gtyejdfzoj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jinyuanbaomall.cn/gtxfrbvffr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.havefunace.top/gtzqzutbat.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.aizwys.cn/gttrmykhlv.html

[N04] 斐波那契数列
来源：http://hz.gzhubu.top/gtuxzlmtes.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.daxiang520.top/gtmlhksuzo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hongshengwenyu.top/gtvzuaqauk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhoulong.xyz/gtggiuqpho.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xuetiantiany.cn/gtnkcbikjc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.chenzaomai.com/gtalbpnzbr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.nanxuanxn.top/gtnwsqhefz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.shanyushiyangkeji.top/gtcoivoyyr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhiwuduotai.top/gtbuklzxjk.html

[N05] 最大公约数
来源：http://hz.yuanzhike.top/gttocgjxov.html

Py:   math.gcd(a, b)
来源：http://hz.birdmap.top/gtgaljstza.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shangyingyoupin.top/gthyvpjxck.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aibaodan.cn/gteolnvoxy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xinyue.icu/gtcippufws.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.cqqwz.cn/gtyazyfyot.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shzxlz.cn/gtxemamoba.html

Ruby: a.gcd(b)
来源：http://hz.vqdsnc.cn/gtgoioqbmw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xingfuxueyuan.xyz/gtsdewfeyo.html

[N06] 判断回文字符串
来源：http://hz.dashuyun.cn/gtwhanoelx.html

Py:   s == s[::-1]
来源：http://hz.c1oappe.top/gtwbcdowxv.html

PHP:  $s === strrev($s);
来源：http://hz.aibaodan.cn/gthfrfglqq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.tian-w.cn/gtzrqguxgn.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shzxlz.cn/gtrutekizo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ehwqpu.com/gtxjgmwhyc.html

Go:   // 双指针从两端比较
来源：http://hz.pycfn.com/gtwnajzfwq.html


<!-- 参考信息 -->