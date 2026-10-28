代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jinghuilouyu.cn/gtegcmcufx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gzhubu.top/gtgvekqukg.html

[J09] 时区处理
来源：http://hz.yuxming.cn/gtbiaxmdep.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.andypj.xyz/gtxeheoiqg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jinqigufen.top/gtbamceuwa.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuxming.cn/gtgqnkpszm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ydzc1.top/gtlizcvscn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinqigfzy.top/gtxmxneafw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.316326.xyz/gtzminfqsk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ywan-chungtsiang.top/gtaykvleke.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yuxming.cn/gtalawvois.html

[J10] 取今天 / 本月第一天
来源：http://hz.jqgfzy.top/gtqkoehswq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shangyingyoupin.top/gtsfzvimxu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xingfuxueyuan.xyz/gtmtvfnuub.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ydjk.org.cn/gtgkshxgfi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.kuanghao11.cn/gtfawynsqp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shanyushiyangkeji.top/gtrdasnauj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.smart0.xyz/gtsxzhfsja.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yj20258.top/gtgymefiqj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.aizwys.cn/gtjdefljvg.html

================================================================================
来源：http://hz.ehwqpu.com/gtrrhiseku.html

K. JSON 与序列化
来源：http://hz.mhx1999.top/gtbftemqmx.html

================================================================================
来源：http://hz.jqgfzy.top/gtwpsmbguq.html

[K01] 对象转 JSON 字符串
来源：http://hz.nwbrower.top/gtdpdzknsh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.gotoacloud.top/gtwqhbeagr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ppjwa.cn/gtqacyevwa.html

JS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangtech.top/gtjzyqvhnh.html

TS:   JSON.stringify(obj)
来源：http://hz.daria6918.cn/gtcjsltxyh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tanke756.top/gtsktdfrbo.html

Go:   json.Marshal(obj)
来源：http://hz.zhoulong.xyz/gtwkdhugxm.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zdqjudy.top/gtwryxjsqb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shuidangran.top/gtrajacqmz.html

[K02] JSON 字符串转对象
来源：http://hz.zhengqikj.top/gtwsdvwrim.html

Py:   json.loads(s)
来源：http://hz.feifeiyinyue.top/gtlnhvqfci.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yueranfly.top/gtpvromujf.html

JS:   JSON.parse(s)
来源：http://hz.andypj.xyz/gtftkthedi.html

TS:   JSON.parse(s)
来源：http://hz.zdqjudy.top/gthkqtrydi.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhengqikj.top/gtawcrlour.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shanyushiyangtech.top/gtrmhdoaef.html

Ruby: JSON.parse(s)
来源：http://hz.gzhubu.top/gtekvkoevk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gzhubu.top/gttxhuecsm.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.shanyushiyangtech.top/gtrynvvhvr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hongshengwenyu.top/gtofjbqqtp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigfzy.top/gtzjjfskkl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj202588.top/gtmvhxmdet.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.dashuyun.cn/gtkwkotdhw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.sysykeji.top/gtsreuomjx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zycfv.cn/gtlpoammob.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jyoumei.cn/gtzwcrexcu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hnqzz.top/gteylhyrss.html

[K04] 读取 JSON 文件
来源：http://hz.0kj1m.cn/gtzdwplykj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.fengsongda.top/gtkwwghpax.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.tian-w.cn/gtjqhmfrjg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangkeji.top/gtvrvyarix.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cqqwz.cn/gtaozajqiq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinqigufen.top/gtipoljayc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinqigfzy.top/gtvrlhwavc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yangfankeji.com/gtgssjtbla.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shanyushiyangtech.top/gteytngnbw.html

[K05] 深拷贝对象
来源：http://hz.dashuyun.cn/gtnsrsvktf.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhongyouzk.top/gtcjlhnjze.html

PHP:  unserialize(serialize($obj));
来源：http://hz.feifeiyinyue.top/gtzmlsxwrf.html

JS:   structuredClone(obj)
来源：http://hz.pengpengdd.cyou/gtyzijqqpz.html

TS:   structuredClone(obj)
来源：http://hz.jinyuanbaomall.cn/gtmhothuoa.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hongshengwenyu.top/gtcutowlyw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shanyushiyangkeji.top/gtkdyymwqv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hnxiangtu.top/gtvhawappd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gogol.net.cn/gtphkzfxrn.html

[K06] 解析 URL 查询串
来源：http://hz.zhijiandao.cn/gtqahloncp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yj20258888.top/gthheqforj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.tanke756.top/gtghiwtzub.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhoulong.xyz/gtwguysbem.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.haohaochexian.top/gtkdczbhqr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.c1oappe.top/gtilobfovl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.wangdashe.top/gtwdxpnilj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.0kj1m.cn/gtqrnjuqds.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.chenlongwang.top/gtmkycwovx.html

[K07] 进制转换
来源：http://hz.hysaishi.cn/gtqpelurvp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ydjk.org.cn/gtcsltsobe.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jinqigfzy.top/gtmawuwuka.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yj20258.top/gtdzsycfsl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.nanxuanxn.top/gtukmpcndx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xuanzx.com/gtauykxlfl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.cdnleiting.top/gtdceyaofn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ybcxt.top/gtusnzksga.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xylfe.cn/gtclqvpvlb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hnqzz.top/gtorwqrmjh.html

Py:   pickle.dumps(obj)
来源：http://hz.yuxming.cn/gtzrratmze.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shuidangran.top/gtwmqhddgz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jinyuanbaomall.cn/gtqioqlpvb.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.smart0.xyz/gtxaseuhpz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.52xcode.cn/gtftauyixq.html

Go:   encoding/gob
来源：http://hz.jianghu66.top/gtcilmmxtw.html

Ruby: Marshal.dump(obj)
来源：http://hz.bjfxy.top/gtexjwjuxz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ppjwa.cn/gtbemjodev.html

================================================================================
来源：http://hz.gotoacloud.top/gtrvhzknhi.html

L. 网络请求
来源：http://hz.jyoumei.cn/gtdgjikaow.html

================================================================================
来源：http://hz.sysykeji.top/gthegrwdou.html

[L01] 发送 GET 请求
来源：http://hz.jiagoushi.top/gtinmdzdyz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.nwbrower.top/gtqybrvkip.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sweek.top/gtqkppbbtc.html

JS:   await fetch(url)
来源：http://hz.jinqigufen.top/gtttwztmnp.html

TS:   await fetch(url)
来源：http://hz.yj20258888.top/gtyqxrfcwp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jianghu66.top/gtghrvxeip.html

Go:   resp, err := http.Get(url)
来源：http://hz.aibaodan.cn/gtnuktchzk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yj20258888.top/gttsyaieyw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.52xcode.cn/gtzluhndly.html

[L02] 发送 POST JSON
来源：http://hz.hongshengwenyu.top/gtgetjyhyk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.kuanghao11.cn/gtcapklerm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhoulong.xyz/gtvytepxtu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cqqwz.cn/gtjfpnxorq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenjidiqi.icu/gtpxhqpioc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sweek.top/gtixkajmoo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yonumen.top/gtuemeinoj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.haohaochexian.top/gtsjzonhuv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sysykeji.top/gtsqxufukq.html

[L03] 设置自定义请求头
来源：http://hz.sweek.top/gtwexbhgzd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ywan-chungtsiang.top/gtaqhsbxok.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.316326.xyz/gtfjckypsx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tian-w.cn/gtumtaepnh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jiagoushi.top/gtkkhbihak.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ehwqpu.com/gtwhxxqurk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jianghu66.top/gtgpjvaymo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.pycfn.com/gtvubgeklp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hnqzz.top/gtwqkjifgo.html

[L04] 设置超时
来源：http://hz.hywenlv.cn/gtbjazgtxl.html

Py:   requests.get(url, timeout=5)
来源：http://hz.nanxinkj.top/gtjnavdorx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhaomingkeji.xyz/gtejafzmuv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yvedp.cn/gtdxbqgggz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dashuyun.cn/gtjthfhfys.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.kuanghao11.cn/gtmsgrgxmr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jianghu66.top/gtbsxhzipc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ybcxt.top/gtmztepriu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jqgufenzy.top/gtcyasndqq.html

[L05] 上传文件（multipart）
来源：http://hz.yonumen.top/gtevlwxfeh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.birdmap.top/gtdzmjqocl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yanxiufei.cn/gtgkaoqyoi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangtech.top/gtfwjzfwmo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hongshengwenyu.top/gtyrnabndy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jinqigufen.top/gtkfecfjzv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.fengsongda.top/gtwojrumff.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yueranfly.top/gtztuycgqa.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nanxuanxn.top/gtpulxepnl.html

[L06] 解析响应为 JSON
来源：http://hz.zhongyouzk.top/gtmohqumyp.html

Py:   resp.json()
来源：http://hz.0kj1m.cn/gtwyijgino.html

PHP:  json_decode($body, true);
来源：http://hz.zycfv.cn/gtwnupbovm.html

JS:   await resp.json()
来源：http://hz.haohaochexian.top/gtpogjohyi.html

TS:   await resp.json()
来源：http://hz.0kj1m.cn/gthycnybgo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yvedp.cn/gtnqodrqju.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gaohongyu789.top/gtbukwejnl.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhoulong.xyz/gtkzaoqiqi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ehwqpu.com/gtdecgyzvu.html

[L07] 处理 HTTP 状态码
来源：http://hz.jyoumei.cn/gtikjthkhx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.vqdsnc.cn/gtxgksvgyq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.gzhubu.top/gtxtrbpniw.html

JS:   resp.ok;  resp.status
来源：http://hz.wangdashe.top/gtbvbazged.html

TS:   resp.ok;  resp.status
来源：http://hz.aibaodan.cn/gtqtuxgfvs.html

Java: resp.statusCode()
来源：http://hz.redwolf501.top/gttvcegmtt.html

Go:   resp.StatusCode
来源：http://hz.cucudq.cn/gtuphiuhhp.html

Ruby: resp.code.to_i
来源：http://hz.0kj1m.cn/gtstasqmqn.html

C#:   (int)resp.StatusCode
来源：http://hz.9152youxi.cn/gtkmvnjkyj.html

[L08] 并发请求多个地址
来源：http://hz.0kj1m.cn/gtxvmxdklb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinghuilouyu.cn/gtsdkjautf.html

PHP:  curl_multi_init() 系列
来源：http://hz.cqqwz.cn/gtqphjgvmw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hfpthk.cn/gtslijrcyi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgufenzy.top/gtzqihyqgx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yvedp.cn/gtpqgjlhnr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xuetiantiany.cn/gtewohpmgq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.sweek.top/gtvlyrfpkc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.pycfn.com/gtovrntxhb.html

================================================================================
来源：http://hz.dianchejie.cn/gtsvkmtwoj.html

M. 命令行 / 进程 / 环境
来源：http://hz.dianchejie.cn/gtcywjxkfr.html

================================================================================
来源：http://hz.tianlin.xyz/gtrnzxwxla.html

[M01] 读取命令行参数
来源：http://hz.9152youxi.cn/gtpnrzypkg.html

Py:   sys.argv[1:]
来源：http://hz.haohaochexian.top/gtmffzdgsj.html

PHP:  $argv;  $argc;
来源：http://hz.daxiang520.top/gtbipdhsne.html

JS:   process.argv.slice(2)
来源：http://hz.yonumen.top/gtcuabdmzh.html

TS:   process.argv.slice(2)
来源：http://hz.zhoulong.xyz/gtkbiagwld.html

Java: args 数组（main 方法参数）
来源：http://hz.zhijiandao.cn/gttfxrnzth.html

Go:   os.Args[1:]
来源：http://hz.nanxinkj.top/gtjfmivtao.html

Ruby: ARGV
来源：http://hz.hywenlv.cn/gtqygovgve.html

C#:   args 数组（Main 方法参数）
来源：http://hz.guannengcc.top/gtjupmqhfl.html

[M02] 读取环境变量
来源：http://hz.feifeiyinyue.top/gtjgxsddxd.html

Py:   os.environ.get("HOME")
来源：http://hz.zhongyouzk.top/gteuqxojqo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.0kj1m.cn/gtgwgxgrhj.html

JS:   process.env.HOME
来源：http://hz.shanyushiyangtech.top/gtshyexzuj.html

TS:   process.env.HOME
来源：http://hz.yj20258.top/gtsfrgnlwm.html

Java: System.getenv("HOME")
来源：http://hz.ybcxt.top/gtzarmdvpa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.iojbl.cn/gtuasxlohe.html

Ruby: ENV["HOME"]
来源：http://hz.shanyushiyangkeji.top/gtkpjuapwr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.smart0.xyz/gtyqbqzlhb.html

[M03] 执行外部命令
来源：http://hz.jinqigufen.top/gtzerhwdfn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jqgfzy.top/gtswdygtjr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.haohaochexian.top/gtibscplap.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.gzhubu.top/gtqqnckrcm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangdashe.top/gtanbimysd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhengqikj.top/gtvvtdezgo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cheryme.top/gtipwfmpgd.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jiagoushi.top/gttzfyakxq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jinghuilouyu.cn/gtbbvumgtm.html

[M04] 获取当前工作目录
来源：http://hz.shuidangran.top/gtbqozjoyj.html

Py:   os.getcwd()
来源：http://hz.yvedp.cn/gthdhibzgo.html

PHP:  getcwd();
来源：http://hz.pycfn.com/gtdebuvpwp.html

JS:   process.cwd()
来源：http://hz.9152youxi.cn/gtfjvjwoqu.html

TS:   process.cwd()
来源：http://hz.mhx1999.top/gtakxfgmhl.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.chenlongwang.top/gtxxaurwuh.html

Go:   os.Getwd()
来源：http://hz.jyoumei.cn/gtphordjyn.html

Ruby: Dir.pwd
来源：http://hz.dianchejie.cn/gtrqvwjnsx.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.0kj1m.cn/gtdotvirkc.html

[M05] 设置退出码
来源：http://hz.dashuyun.cn/gtknwqcgrj.html

Py:   sys.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtjviarrnj.html

PHP:  exit(1);
来源：http://hz.yonumen.top/gtdzbbxtia.html

JS:   process.exit(1)
来源：http://hz.jinyuanbaomall.cn/gtmomafkpt.html

TS:   process.exit(1)
来源：http://hz.chenzaomai.com/gtugrujqyk.html

Java: System.exit(1)
来源：http://hz.xuetiantiany.cn/gtuhknrjam.html

Go:   os.Exit(1)
来源：http://hz.yvedp.cn/gtegwcfjaz.html

Ruby: exit 1
来源：http://hz.cqqwz.cn/gtehztyqoo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.tanke756.top/gtfmhvltfc.html

[M06] 向标准错误输出
来源：http://hz.guannengcc.top/gthiljkggo.html

Py:   print("err", file=sys.stderr)
来源：http://hz.redwolf501.top/gtwwmnwozv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jianghu66.top/gthaakspzn.html

JS:   console.error("err")
来源：http://hz.0kj1m.cn/gtedpdmarx.html

TS:   console.error("err")
来源：http://hz.yvedp.cn/gtwboxrdbi.html

Java: System.err.println("err")
来源：http://hz.c1oappe.top/gtxmetjtew.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hywenlv.cn/gtfjnyfyzd.html

Ruby: warn "err"
来源：http://hz.zhixingplan.top/gttzfjlloe.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.bjfxy.top/gtsjxmmwhs.html

[M07] 判断是否为主入口
来源：http://hz.ehwqpu.com/gtzzsmfoka.html

Py:   if __name__ == "__main__":
来源：http://hz.zhoulong.xyz/gtmpffursr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.vqdsnc.cn/gtccxkzraa.html

JS:   require.main === module
来源：http://hz.ppjwa.cn/gtvabtuygk.html

TS:   require.main === module
来源：http://hz.havefunace.top/gtyvilrpuc.html

Java: public static void main(String[] args)
来源：http://hz.zdqjudy.top/gtnftycbcj.html

Go:   func main()
来源：http://hz.sysykeji.top/gteukoazzt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.vqdsnc.cn/gteennorku.html

C#:   static void Main(string[] args)
来源：http://hz.cucudq.cn/gttwtqvahn.html

[M08] 获取系统与运行时信息
来源：http://hz.hammf.cn/gtsnxmarsn.html

Py:   platform.system();  platform.python_version()
来源：http://hz.316326.xyz/gtyvohkyea.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.chenjidiqi.icu/gtcwadnbhn.html

JS:   process.platform;  process.version
来源：http://hz.cheryme.top/gtiqlcvzbq.html

TS:   process.platform;  process.version
来源：http://hz.zhixingplan.top/gtiuypczpm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jiagoushi.top/gtrawvwpqe.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.gogol.net.cn/gtymqapuqb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yangfankeji.com/gtpygakubv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.tian-w.cn/gtgaddxlpj.html

================================================================================
来源：http://hz.ehwqpu.com/gtbpnkejts.html

N. 数据结构与算法
来源：http://hz.wangshuangyany.cn/gtrcvifquy.html

================================================================================
来源：http://hz.yvedp.cn/gtbfebmkpi.html

[N01] 二分查找（有序数组）
来源：http://hz.shanyushiyangtech.top/gtwkfbiumq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jiagoushi.top/gtaqwihzsj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhijiandao.cn/gtvstrgscp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ywan-chungtsiang.top/gtrjeidury.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xinyue.icu/gtxfbswxlr.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.meibo888.top/gtnherdywx.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.gogol.net.cn/gtvgimouua.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ppjwa.cn/gtbbqzirgo.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hfpthk.cn/gtysmntmdu.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.shangyingyoupin.top/gtmgqmgtkh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.daria6918.cn/gtujvshqhs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yuxming.cn/gtpwgqpddj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aibaodan.cn/gtgktnwsqf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.iojbl.cn/gtjwwcwchv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.c1oappe.top/gtbnijvbvp.html

Go:   slices.Sort(arr)
来源：http://hz.yj202588.top/gttulussdk.html

Ruby: arr.sort
来源：http://hz.vqdsnc.cn/gthfmliujo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.aizwys.cn/gtuvsugahx.html

[N03] 快速排序（分治示例）
来源：http://hz.shangyingyoupin.top/gtypjnfwsn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shanyushiyangtech.top/gtzbasmvsy.html

PHP:  // 递归实现，或用 usort
来源：http://hz.chenlongwang.top/gtbdmfymbq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sweek.top/gtghpzeuze.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenlongwang.top/gtvkiiifby.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xuetiantiany.cn/gtwsjyceqw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.bjfxy.top/gtvfegtqdx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.0kj1m.cn/gtzefipqrm.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xinyue.icu/gtnqzedsaa.html

[N04] 斐波那契数列
来源：http://hz.sysykeji.top/gtdtvyzvwc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhengqikj.top/gtwnczokrl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhaomingkeji.xyz/gtamasexds.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenlongwang.top/gtthlaihio.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.quarkkingdee.top/gttpvyyayt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.chenzaomai.com/gtiocxfiwo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.52xcode.cn/gtlspfchka.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.andypj.xyz/gtlykerarl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.iojbl.cn/gtstbctsrn.html

[N05] 最大公约数
来源：http://hz.sxryk.cn/gtdwlnhyfl.html

Py:   math.gcd(a, b)
来源：http://hz.sweek.top/gttyiodgwo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinqigufen.top/gtidyxcfdn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jianghu66.top/gtggwbwqpx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jianghu66.top/gtsazytzuz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.vqdsnc.cn/gtsbvpjlma.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yj20258888.top/gtanposfwh.html

Ruby: a.gcd(b)
来源：http://hz.cashguo.top/gtstvokpwu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.snrcjt.cn/gtfkjhpenq.html

[N06] 判断回文字符串
来源：http://hz.tanke756.top/gtdfvxrvou.html

Py:   s == s[::-1]
来源：http://hz.dianchejie.cn/gtovvyuyxc.html

PHP:  $s === strrev($s);
来源：http://hz.daxiang520.top/gtazjffmay.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jyoumei.cn/gtvunbelkc.html

TS:   s === [...s].reverse().join("")
来源：http://hz.gaohongyu789.top/gthptfjsdd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.aizwys.cn/gticakjpwd.html

Go:   // 双指针从两端比较
来源：http://hz.nanxinkj.top/gtmjguppre.html


<!-- 参考信息 -->