代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.pengpengdd.cyou/gtpjpxdzvq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.bjfxy.top/gtxuudeqea.html

[J09] 时区处理
来源：http://hz.smart0.xyz/gtrgypwtro.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jiagoushi.top/gtbgusfurk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.nanxuanxn.top/gtyblcnsle.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ppjwa.cn/gtfdriajps.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ehwqpu.com/gtaxjfergo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.9152youxi.cn/gtpwcobdkh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.smart0.xyz/gtntvaorfd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.havefunace.top/gtyucmxrrs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cashguo.top/gtpvomsucp.html

[J10] 取今天 / 本月第一天
来源：http://hz.nanxuanxn.top/gtathacrym.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xziqi.cn/gtdgkmwuzu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.daria6918.cn/gtqzbcheuh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ehwqpu.com/gtboctospp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.guowangkeji.top/gtaxaqhjfj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.bjfxy.top/gtzlmcerxs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cqqwz.cn/gtnmxctozo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.pengpengdd.cyou/gtefmrogrz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cashguo.top/gtmjucixji.html

================================================================================
来源：http://hz.gogol.net.cn/gtxmjbwank.html

K. JSON 与序列化
来源：http://hz.shanyushiyangkeji.top/gtgrowvzxi.html

================================================================================
来源：http://hz.kuanghao11.cn/gtniqanzzq.html

[K01] 对象转 JSON 字符串
来源：http://hz.ppjwa.cn/gtxtghqfny.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.aibaodan.cn/gtsgymrfxz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shzxlz.cn/gtqgsdwcjl.html

JS:   JSON.stringify(obj)
来源：http://hz.mhx1999.top/gtkwjyoghh.html

TS:   JSON.stringify(obj)
来源：http://hz.fengsongda.top/gtlnzcmwaf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.dashuyun.cn/gtnvqheofy.html

Go:   json.Marshal(obj)
来源：http://hz.nanxuanxn.top/gtazocnbkg.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.gotoacloud.top/gtprdszzdd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhongyouzk.top/gtpykcjetv.html

[K02] JSON 字符串转对象
来源：http://hz.shangyingyoupin.top/gtocisttaa.html

Py:   json.loads(s)
来源：http://hz.yonumen.top/gtpfsulgpj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yueranfly.top/gtqetgkiqr.html

JS:   JSON.parse(s)
来源：http://hz.chenjidiqi.icu/gtwrgmohva.html

TS:   JSON.parse(s)
来源：http://hz.sweek.top/gtyuxwbfrd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.tianlin.xyz/gtmrxhjrjn.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhaomingkeji.xyz/gtcofgllqr.html

Ruby: JSON.parse(s)
来源：http://hz.xuetiantiany.cn/gtolvacovm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.tianlin.xyz/gtwkojthyl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xziqi.cn/gtrlsgited.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ehwqpu.com/gtmalwwilw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yueranfly.top/gtzlbsycwn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhongyouzk.top/gtlvyudeje.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhoulong.xyz/gtmzjvkunm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinqigfzy.top/gtkruftfxc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhengqikj.top/gthsvztgdf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cdnleiting.top/gtagnrcaob.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.nanxinkj.top/gtznuotoag.html

[K04] 读取 JSON 文件
来源：http://hz.gotoacloud.top/gtotkihggg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hnxiangtu.top/gtagasrubf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yj20258888.top/gtahxisdqj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shuidangran.top/gtrstthprb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yanxiufei.cn/gtczmfggdv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hnqzz.top/gtlakvyhvg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.gogol.net.cn/gttlhyvdmw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.nanxuanxn.top/gtpesplsjd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jqgufenzy.top/gthwmzpvwf.html

[K05] 深拷贝对象
来源：http://hz.sysykeji.top/gtaqsukfry.html

Py:   copy.deepcopy(obj)
来源：http://hz.shangyingyoupin.top/gtajbygbar.html

PHP:  unserialize(serialize($obj));
来源：http://hz.sxryk.cn/gtkpgnsxup.html

JS:   structuredClone(obj)
来源：http://hz.zycfv.cn/gtnjbfoykg.html

TS:   structuredClone(obj)
来源：http://hz.zhijiandao.cn/gthbtafypo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jinghuilouyu.cn/gtsymdrujo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.snrcjt.cn/gttrgutgns.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cheryme.top/gtvrmtxzwi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.kuanghao11.cn/gtmnxcrwfm.html

[K06] 解析 URL 查询串
来源：http://hz.ydjk.org.cn/gtospcdlni.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.guowangkeji.top/gtsalrwphk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.nanxinkj.top/gtgquvfgem.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.svipenyu.cn/gttovjqfpz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenzaomai.com/gtukhvrvax.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.kuanghao11.cn/gtrnjzqpzd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.wangdashe.top/gtoaetmxvf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ydjk.org.cn/gtwfqaribu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yj202588.top/gtkxyrkdib.html

[K07] 进制转换
来源：http://hz.iojbl.cn/gtlybmesbs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ehwqpu.com/gtentngqpu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.bjfxy.top/gtzcfhftrk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xuetiantiany.cn/gtggamqyya.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hnxiangtu.top/gtnroimouw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.chenlongwang.top/gtzkgcpijd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yueranfly.top/gtfvtnntzh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yonumen.top/gtfndvaypa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hammf.cn/gtchxnabwi.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zycfv.cn/gtymcrbmvu.html

Py:   pickle.dumps(obj)
来源：http://hz.yvedp.cn/gtutnhpjpe.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhaomingkeji.xyz/gtdsygpdmb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xuetiantiany.cn/gteoamhgfq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.wangdashe.top/gthmevzyay.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.dianchejie.cn/gtcmktobje.html

Go:   encoding/gob
来源：http://hz.gaohongyu789.top/gtixgmceja.html

Ruby: Marshal.dump(obj)
来源：http://hz.xziqi.cn/gtedxoqrrz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinyuanbaomall.cn/gtpuxhskab.html

================================================================================
来源：http://hz.hnxiangtu.top/gthltdtsgu.html

L. 网络请求
来源：http://hz.gaohongyu789.top/gttklnfehg.html

================================================================================
来源：http://hz.ehwqpu.com/gtqkjezdvx.html

[L01] 发送 GET 请求
来源：http://hz.316326.xyz/gtvmfnrhzj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gzhubu.top/gtyxdwhsmt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jqgufenzy.top/gtcgkbldwn.html

JS:   await fetch(url)
来源：http://hz.pycfn.com/gtxkefezux.html

TS:   await fetch(url)
来源：http://hz.yvedp.cn/gtpmyoknve.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.wangshuangyany.cn/gtiyqigmno.html

Go:   resp, err := http.Get(url)
来源：http://hz.xuanzx.com/gtslmtrujq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cqqwz.cn/gtczpgzrmi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shuidangran.top/gtlrimmldk.html

[L02] 发送 POST JSON
来源：http://hz.cashguo.top/gtwfdtvlcm.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jqgufenzy.top/gtvdrvbdhm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ppjwa.cn/gtvpohgmvd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigufen.top/gtbuhjzndm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnqzz.top/gtrdcmaias.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhengqikj.top/gtkypkcwzi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.c1oappe.top/gtfbqxliov.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xuetiantiany.cn/gtzqxrlzdw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinyuanbaomall.cn/gtauhfgfiu.html

[L03] 设置自定义请求头
来源：http://hz.daxiang520.top/gtblujtjxj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jiagoushi.top/gttrimfmhw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ehwqpu.com/gtyaoksynv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.c1oappe.top/gtpflxkzty.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.mhx1999.top/gtdqrnbzqk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhaomingkeji.xyz/gtzxsmzspw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xylfe.cn/gtlgtiqrze.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.chenlongwang.top/gtipmedhxc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ywan-chungtsiang.top/gtvgkmjuke.html

[L04] 设置超时
来源：http://hz.hongshengwenyu.top/gtqtatgkzf.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hfpthk.cn/gtbdeoyjkq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.birdmap.top/gtepicibjn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258888.top/gtkxssabfj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhixingplan.top/gtybpphfba.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gotoacloud.top/gtzagzpfmb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shuidangran.top/gtfzejcpck.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jyoumei.cn/gtdvkcomlt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sweek.top/gttxggsoas.html

[L05] 上传文件（multipart）
来源：http://hz.ivvv.top/gtkvftxbvw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yanxiufei.cn/gtwlmvmyvv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hammf.cn/gthzkznwwq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhaomingkeji.xyz/gtvqgbijwl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xziqi.cn/gtrmwfrmhe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ppjwa.cn/gtbjsvgiln.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.sysykeji.top/gtyrlqjjoz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.iojbl.cn/gtdtywlxyl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yuanzhike.top/gtymdvjypj.html

[L06] 解析响应为 JSON
来源：http://hz.gaohongyu789.top/gtikdpjlrx.html

Py:   resp.json()
来源：http://hz.xylfe.cn/gtrmoziszn.html

PHP:  json_decode($body, true);
来源：http://hz.zhijiandao.cn/gtqqwctaub.html

JS:   await resp.json()
来源：http://hz.dianchejie.cn/gtdmxgcoua.html

TS:   await resp.json()
来源：http://hz.zhengqikj.top/gtfezyxevs.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.gaohongyu789.top/gtonfpruot.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.9152youxi.cn/gtkrdiptua.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hysaishi.cn/gtjkzbmqcv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.vqdsnc.cn/gtlgfopyjr.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinqigufen.top/gtowbgbdjh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.nanxinkj.top/gtztpxmcxp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhiwuduotai.top/gtcpocjcvd.html

JS:   resp.ok;  resp.status
来源：http://hz.guannengcc.top/gtljactvxc.html

TS:   resp.ok;  resp.status
来源：http://hz.zdqjudy.top/gtjgqthcge.html

Java: resp.statusCode()
来源：http://hz.yj20258888.top/gtoqydpwnf.html

Go:   resp.StatusCode
来源：http://hz.xziqi.cn/gtdepxbszz.html

Ruby: resp.code.to_i
来源：http://hz.xuanzx.com/gtmrwbgrxu.html

C#:   (int)resp.StatusCode
来源：http://hz.kuanghao11.cn/gtunbllrla.html

[L08] 并发请求多个地址
来源：http://hz.gzhubu.top/gtaiozzdci.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yanxiufei.cn/gtsrcsaehs.html

PHP:  curl_multi_init() 系列
来源：http://hz.yuxming.cn/gtintunfjn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sysykeji.top/gtclwctgpv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shuidangran.top/gtgkertcbv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.svipenyu.cn/gttttdplwb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shangyingyoupin.top/gtbbisuoeq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.bjfxy.top/gtatqwrjku.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xuetiantiany.cn/gtmxvogvqt.html

================================================================================
来源：http://hz.ydjk.org.cn/gtutijeifg.html

M. 命令行 / 进程 / 环境
来源：http://hz.ywan-chungtsiang.top/gtqtdursnq.html

================================================================================
来源：http://hz.ybcxt.top/gtjdmtjawp.html

[M01] 读取命令行参数
来源：http://hz.nanxuanxn.top/gtzuauurgj.html

Py:   sys.argv[1:]
来源：http://hz.jlsjyb.cn/gtkoaswfzr.html

PHP:  $argv;  $argc;
来源：http://hz.feifeiyinyue.top/gtywsczhlq.html

JS:   process.argv.slice(2)
来源：http://hz.gogol.net.cn/gtzaaofvnx.html

TS:   process.argv.slice(2)
来源：http://hz.pycfn.com/gtxqalmzko.html

Java: args 数组（main 方法参数）
来源：http://hz.zhiwuduotai.top/gtzysryqxt.html

Go:   os.Args[1:]
来源：http://hz.dashuyun.cn/gtnwvdawlr.html

Ruby: ARGV
来源：http://hz.yongpay.top/gttpvyffmj.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jlsjyb.cn/gtzmldshhs.html

[M02] 读取环境变量
来源：http://hz.xuetiantiany.cn/gtumyuxzdi.html

Py:   os.environ.get("HOME")
来源：http://hz.ydzc1.top/gtyqlkimyt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.nanxuanxn.top/gtyngnxvqz.html

JS:   process.env.HOME
来源：http://hz.shzxlz.cn/gtatrtiuee.html

TS:   process.env.HOME
来源：http://hz.pycfn.com/gtniwpeljr.html

Java: System.getenv("HOME")
来源：http://hz.haohaochexian.top/gtyehybelb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hywenlv.cn/gtgzfluzts.html

Ruby: ENV["HOME"]
来源：http://hz.shanyushiyangtech.top/gtrisclrxt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhiwuduotai.top/gtrhbxnfye.html

[M03] 执行外部命令
来源：http://hz.ehwqpu.com/gthvhjklmx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cashguo.top/gtlugzydhj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ppjwa.cn/gttcjjzwnw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhoulong.xyz/gtaqcxygfn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangdashe.top/gtzkpdbzxv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.feifeiyinyue.top/gtqiudkrir.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cucudq.cn/gtebgurunh.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jinyuanbaomall.cn/gtnzzlknav.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shanyushiyangtech.top/gthtfygzkl.html

[M04] 获取当前工作目录
来源：http://hz.yuxming.cn/gtqlozxrvt.html

Py:   os.getcwd()
来源：http://hz.52xcode.cn/gtjzjbudho.html

PHP:  getcwd();
来源：http://hz.nwbrower.top/gttyhzswvs.html

JS:   process.cwd()
来源：http://hz.jqgufenzy.top/gtxzptvkja.html

TS:   process.cwd()
来源：http://hz.hfpthk.cn/gtrlwhzidy.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.haohaochexian.top/gtyskiiged.html

Go:   os.Getwd()
来源：http://hz.quarkkingdee.top/gtdbpfxgbd.html

Ruby: Dir.pwd
来源：http://hz.andypj.xyz/gtuegofyto.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.nanxuanxn.top/gtlfdgwdad.html

[M05] 设置退出码
来源：http://hz.pycfn.com/gtgfpsclgb.html

Py:   sys.exit(1)
来源：http://hz.gzhubu.top/gtkkhrviqj.html

PHP:  exit(1);
来源：http://hz.jlsjyb.cn/gtcqvzlnyk.html

JS:   process.exit(1)
来源：http://hz.ivvv.top/gtjpqblsvh.html

TS:   process.exit(1)
来源：http://hz.sxryk.cn/gtxvvchmif.html

Java: System.exit(1)
来源：http://hz.yanxiufei.cn/gtfioxxlbw.html

Go:   os.Exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtzqjnyjwk.html

Ruby: exit 1
来源：http://hz.cashguo.top/gtwggifgpo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ydzc1.top/gtobxlrivq.html

[M06] 向标准错误输出
来源：http://hz.yonumen.top/gtywknshhc.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gogol.net.cn/gtosyqqjbv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jinyuanbaomall.cn/gtficswryb.html

JS:   console.error("err")
来源：http://hz.gotoacloud.top/gtgluarflt.html

TS:   console.error("err")
来源：http://hz.yuanzhike.top/gtttubxbhk.html

Java: System.err.println("err")
来源：http://hz.quarkkingdee.top/gtzjfpodav.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.quarkkingdee.top/gtlfbzuvan.html

Ruby: warn "err"
来源：http://hz.wangdashe.top/gtswqtxmjg.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.tanke756.top/gtdekytnfx.html

[M07] 判断是否为主入口
来源：http://hz.meibo888.top/gtsfriddnu.html

Py:   if __name__ == "__main__":
来源：http://hz.zhengqikj.top/gtlurgcxuh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.chenlongwang.top/gtjkalvlti.html

JS:   require.main === module
来源：http://hz.gogol.net.cn/gtphqptpcz.html

TS:   require.main === module
来源：http://hz.nanxinkj.top/gtizxyvetw.html

Java: public static void main(String[] args)
来源：http://hz.yonumen.top/gtvccvkdld.html

Go:   func main()
来源：http://hz.bjfxy.top/gttsxjfuif.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.aizwys.cn/gthatsqzbi.html

C#:   static void Main(string[] args)
来源：http://hz.yueranfly.top/gtslyfqfdu.html

[M08] 获取系统与运行时信息
来源：http://hz.jiagoushi.top/gtmqfjqeqr.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shanyushiyangtech.top/gtskbgtftx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.dashuyun.cn/gtjysweuhh.html

JS:   process.platform;  process.version
来源：http://hz.jlsjyb.cn/gtvjrqrhvt.html

TS:   process.platform;  process.version
来源：http://hz.hammf.cn/gtkpuglzqy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sufxvd.cn/gtkepwkkza.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hfpthk.cn/gtvfhogwhq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.wangdashe.top/gtgaomrojy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ivvv.top/gteaaarvhc.html

================================================================================
来源：http://hz.tanke756.top/gtomantgzp.html

N. 数据结构与算法
来源：http://hz.9152youxi.cn/gttbdcxvdy.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtcehzgews.html

[N01] 二分查找（有序数组）
来源：http://hz.shzxlz.cn/gtqtnmvjwh.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.aibaodan.cn/gtpslksgob.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shanyushiyangkeji.top/gtpmhirpnw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ppjwa.cn/gtxdxcdrhp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinyuanbaomall.cn/gthsvagbmk.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jyoumei.cn/gtfwqutnfu.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jiagoushi.top/gtbjgezrzn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.gotoacloud.top/gtorodvxcq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hammf.cn/gtbmngyxta.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.havefunace.top/gthaammyvn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.snrcjt.cn/gtduzrutnp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.quarkkingdee.top/gtotsaxlrc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.birdmap.top/gtrjawijvj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zycfv.cn/gtcftolofp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.snrcjt.cn/gtyinrsejr.html

Go:   slices.Sort(arr)
来源：http://hz.tianlin.xyz/gtwjtdpylo.html

Ruby: arr.sort
来源：http://hz.ywan-chungtsiang.top/gtkkyazupn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.0kj1m.cn/gtjpydomqk.html

[N03] 快速排序（分治示例）
来源：http://hz.yueranfly.top/gtfwjfbrvo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.tian-w.cn/gtnocqulrt.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xuanzx.com/gtyahustdg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tanke756.top/gtajpsdtsx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yuxming.cn/gtyjabttfx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj202588.top/gtdnwedhce.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shanyushiyangkeji.top/gtuukpzsgu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.nanxinkj.top/gtpnsjkqnu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jqgufenzy.top/gtffzertxt.html

[N04] 斐波那契数列
来源：http://hz.yueranfly.top/gttwffoohm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ehwqpu.com/gthmisageh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xuanzx.com/gtubiedzmt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daxiang520.top/gtgdthnyye.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cdnleiting.top/gtdvdvnodx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yonumen.top/gtokwxiywo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhongyouzk.top/gtvfyenhcc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.pycfn.com/gtnopueefd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinyuanbaomall.cn/gtwnsqxamd.html

[N05] 最大公约数
来源：http://hz.hysaishi.cn/gtrdsywsek.html

Py:   math.gcd(a, b)
来源：http://hz.yonumen.top/gtfiksazvw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.chenzaomai.com/gtkzccgjkz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinqigfzy.top/gtpbjwdwfg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yuxming.cn/gttlzliimo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shzxlz.cn/gtwnagpshz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ybcxt.top/gtewuhajxc.html

Ruby: a.gcd(b)
来源：http://hz.wangshuangyany.cn/gtwpsvrlvl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.9152youxi.cn/gtwrgbhtsq.html

[N06] 判断回文字符串
来源：http://hz.dianchejie.cn/gtwjcqeygy.html

Py:   s == s[::-1]
来源：http://hz.xinyue.icu/gtkobmumza.html

PHP:  $s === strrev($s);
来源：http://hz.tian-w.cn/gtlazmldpi.html

JS:   s === [...s].reverse().join("")
来源：http://hz.bjfxy.top/gtucyodrnj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jyoumei.cn/gtlbqzyglm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.aizwys.cn/gtlhknesqd.html

Go:   // 双指针从两端比较
来源：http://hz.wangdashe.top/gterfzkkui.html


<!-- 参考信息 -->