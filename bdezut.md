代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.wangdashe.top/gtwgloqtiq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yangfankeji.com/gtvwvivgez.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.316326.xyz/gtdlbayvrr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hnxiangtu.top/gtzduofltr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.svipenyu.cn/gtjxzmvnfr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zycfv.cn/gtylsqkhin.html

[J09] 时区处理
来源：http://hz.tian-w.cn/gtqcoevrzw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cdnleiting.top/gtuiwcyerp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jinyuanbaomall.cn/gtfnctwbvd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sufxvd.cn/gtbbqmprgy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgufenzy.top/gtcjsmgwjp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.haohaochexian.top/gttlnaqlyq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jianghu66.top/gtolemfgcb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.quarkkingdee.top/gtqgkdpkgl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.redwolf501.top/gtepoqxjvn.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhaomingkeji.xyz/gthayadgyw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ybcxt.top/gtpeboooip.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.wangdashe.top/gtmxwcekbe.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.birdmap.top/gthvuvbsrq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.fengsongda.top/gtqmwnaddy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cheryme.top/gtvbzzqfur.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ivvv.top/gtcnzutcjk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jianghu66.top/gtmhmxecpm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cheryme.top/gtgzffejlg.html

================================================================================
来源：http://hz.yj202588.top/gtzsweibur.html

K. JSON 与序列化
来源：http://hz.meibo888.top/gtycvvmfzs.html

================================================================================
来源：http://hz.52xcode.cn/gtgmfcwqon.html

[K01] 对象转 JSON 字符串
来源：http://hz.shanyushiyangtech.top/gtsxfulxfn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.chenjidiqi.icu/gtjumfmmzc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shzxlz.cn/gtnlpodyam.html

JS:   JSON.stringify(obj)
来源：http://hz.chenlongwang.top/gtffkosoam.html

TS:   JSON.stringify(obj)
来源：http://hz.chenjidiqi.icu/gticaradts.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.0kj1m.cn/gtrfxzzmlc.html

Go:   json.Marshal(obj)
来源：http://hz.gaohongyu789.top/gtgxqyutrk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sufxvd.cn/gtjnfhjqpq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.nwbrower.top/gtfknawojn.html

[K02] JSON 字符串转对象
来源：http://hz.ywan-chungtsiang.top/gtvhloiwxf.html

Py:   json.loads(s)
来源：http://hz.jinqigfzy.top/gtpgpgpstr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yj202588.top/gtrmguybhf.html

JS:   JSON.parse(s)
来源：http://hz.xylfe.cn/gtzdidyoel.html

TS:   JSON.parse(s)
来源：http://hz.yangfankeji.com/gtbgaulsbe.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.pycfn.com/gtupudlaxi.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.daria6918.cn/gtjdckhmcz.html

Ruby: JSON.parse(s)
来源：http://hz.feifeiyinyue.top/gtqmmvjkxp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hywenlv.cn/gtdadforfd.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.smart0.xyz/gtysptqufq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xinyue.icu/gtqvhsbilg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.tian-w.cn/gtqbrafibv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ppjwa.cn/gtgocgoqhz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yueranfly.top/gtxbhbuuqc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.gogol.net.cn/gtxmjeqguu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.birdmap.top/gtmjzvxcaq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.tanke756.top/gtcamvadmq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.feifeiyinyue.top/gtnmalzttc.html

[K04] 读取 JSON 文件
来源：http://hz.quarkkingdee.top/gttzbqfeic.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.tianlin.xyz/gtgcavlwgu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.c1oappe.top/gtsoukpgih.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zycfv.cn/gtfqgwitgr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jlsjyb.cn/gtugybfobi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gzhubu.top/gtygjmhxrj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zdqjudy.top/gtolzqwtar.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.quarkkingdee.top/gtdjglsfjd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sysykeji.top/gtqluacfwm.html

[K05] 深拷贝对象
来源：http://hz.hnqzz.top/gtckiqpbkw.html

Py:   copy.deepcopy(obj)
来源：http://hz.hnqzz.top/gtrvvxngri.html

PHP:  unserialize(serialize($obj));
来源：http://hz.nanxinkj.top/gtsomnjjjl.html

JS:   structuredClone(obj)
来源：http://hz.yvedp.cn/gtsnunsjfo.html

TS:   structuredClone(obj)
来源：http://hz.havefunace.top/gtexzatbin.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jinqigufen.top/gtgxbnfppj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hfpthk.cn/gtoqszvxpt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhongyouzk.top/gttrkfhkcj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.svipenyu.cn/gtulyyloal.html

[K06] 解析 URL 查询串
来源：http://hz.jinqigufen.top/gtxodqpcbh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.316326.xyz/gtxtmprtnm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zdqjudy.top/gtdasymszj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxinkj.top/gtilnhhgew.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hongshengwenyu.top/gthinhkhxe.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xingfuxueyuan.xyz/gtdmigjtjj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.kuanghao11.cn/gtocwprulc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.chenzaomai.com/gtbwjecgiu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shzxlz.cn/gtudmhcyrq.html

[K07] 进制转换
来源：http://hz.52xcode.cn/gtbcgmgzrl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.tian-w.cn/gtqbqawtkk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ywan-chungtsiang.top/gtzvcwzclo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.316326.xyz/gtadklplkl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.snrcjt.cn/gtqepearpk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jqgufenzy.top/gttpevlxju.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.fengsongda.top/gttwmredcb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zdqjudy.top/gtdedkekgq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.nanxuanxn.top/gtycpztxgo.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhaomingkeji.xyz/gtbbsijmkv.html

Py:   pickle.dumps(obj)
来源：http://hz.daxiang520.top/gtwxlntixt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tanke756.top/gtafbyhbre.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.52xcode.cn/gttxnjczpr.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.wangdashe.top/gtyrzlurfa.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shzxlz.cn/gtnafptvjr.html

Go:   encoding/gob
来源：http://hz.hnqzz.top/gtkzdxlbfn.html

Ruby: Marshal.dump(obj)
来源：http://hz.316326.xyz/gtoruepduw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yangfankeji.com/gtlqdzinsn.html

================================================================================
来源：http://hz.tian-w.cn/gtcydgkase.html

L. 网络请求
来源：http://hz.cashguo.top/gtgmemazrk.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtzwpzidwv.html

[L01] 发送 GET 请求
来源：http://hz.yj202588.top/gtpcyhvraz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hnqzz.top/gtjkwvrdth.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cashguo.top/gtsvkvnmod.html

JS:   await fetch(url)
来源：http://hz.gaohongyu789.top/gtqnrtymic.html

TS:   await fetch(url)
来源：http://hz.guowangkeji.top/gttxpouzhx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.pycfn.com/gtvhlhcbls.html

Go:   resp, err := http.Get(url)
来源：http://hz.tanke756.top/gtovshhntn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.dashuyun.cn/gtvwpukrey.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.fengsongda.top/gtlerzrwkp.html

[L02] 发送 POST JSON
来源：http://hz.fzhhl.top/gtzwidbucy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cheryme.top/gtdjizlepn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ehwqpu.com/gtlhlyzybe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangtech.top/gtewyjaasm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shzxlz.cn/gtskifzasx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jyoumei.cn/gteskjevqx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.pengpengdd.cyou/gtghmehbjt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yongpay.top/gtuotserqf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.mhx1999.top/gtwygpdtan.html

[L03] 设置自定义请求头
来源：http://hz.zhijiandao.cn/gttxtecgib.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ppjwa.cn/gtqslwtpcs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jiagoushi.top/gtdcliauoy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.fzhhl.top/gtcffshqff.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ivvv.top/gtwntkqxru.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.vqdsnc.cn/gttloczjai.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinyuanbaomall.cn/gttacujsez.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.c1oappe.top/gtlqdbmdrd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yongpay.top/gtfbvlrebd.html

[L04] 设置超时
来源：http://hz.wangdashe.top/gtpvzjsnqm.html

Py:   requests.get(url, timeout=5)
来源：http://hz.sysykeji.top/gtmrctlywv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yj20258888.top/gtiruhykde.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.bjfxy.top/gtdbzlkxkq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.redwolf501.top/gttwvpteik.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zdqjudy.top/gttsjlijvq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.daria6918.cn/gtlsdllyeh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shzxlz.cn/gtoqbtrddn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.gzhubu.top/gttqvlbwsl.html

[L05] 上传文件（multipart）
来源：http://hz.hywenlv.cn/gtyggszoma.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ydzc1.top/gtzqjvfida.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ehwqpu.com/gtdicskvql.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xuetiantiany.cn/gtvjmkobve.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.meibo888.top/gtjvkhufnu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xuetiantiany.cn/gtxuusfucj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.chenzaomai.com/gtyspzobgl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hnqzz.top/gtgjdibner.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.tian-w.cn/gttijzybxf.html

[L06] 解析响应为 JSON
来源：http://hz.ydzc1.top/gtmtyzlysl.html

Py:   resp.json()
来源：http://hz.zhongyouzk.top/gtexkwzmtg.html

PHP:  json_decode($body, true);
来源：http://hz.meibo888.top/gtdqhdxoho.html

JS:   await resp.json()
来源：http://hz.yongpay.top/gtronjlqtd.html

TS:   await resp.json()
来源：http://hz.yj20258.top/gttgzfbabw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hnqzz.top/gtltzghvne.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.kuanghao11.cn/gtqromjkap.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hammf.cn/gtefcikegg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ybcxt.top/gtqdutoejb.html

[L07] 处理 HTTP 状态码
来源：http://hz.havefunace.top/gtejacerbd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.birdmap.top/gttnmfamid.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhiwuduotai.top/gttvisdxcn.html

JS:   resp.ok;  resp.status
来源：http://hz.xuetiantiany.cn/gtwlmczmxl.html

TS:   resp.ok;  resp.status
来源：http://hz.hongshengwenyu.top/gtzminfclc.html

Java: resp.statusCode()
来源：http://hz.pycfn.com/gtmitqawkf.html

Go:   resp.StatusCode
来源：http://hz.jinyuanbaomall.cn/gtouurbnqv.html

Ruby: resp.code.to_i
来源：http://hz.zhengqikj.top/gtsupgsibm.html

C#:   (int)resp.StatusCode
来源：http://hz.jinqigfzy.top/gtiysbhtzg.html

[L08] 并发请求多个地址
来源：http://hz.hfpthk.cn/gtcctyxnlx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ehwqpu.com/gtimsfqraq.html

PHP:  curl_multi_init() 系列
来源：http://hz.zycfv.cn/gtdruuttrc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jianghu66.top/gtnwxdsemo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.kuanghao11.cn/gtdxvbygqv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jiagoushi.top/gtobllysuw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xinyue.icu/gtawhvpyxd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.guannengcc.top/gtlrhuqfdc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.daria6918.cn/gtloasvhor.html

================================================================================
来源：http://hz.shuidangran.top/gtilzttqza.html

M. 命令行 / 进程 / 环境
来源：http://hz.ydjk.org.cn/gtibcxgxpb.html

================================================================================
来源：http://hz.birdmap.top/gtexakbnbc.html

[M01] 读取命令行参数
来源：http://hz.bjfxy.top/gtqcsxfams.html

Py:   sys.argv[1:]
来源：http://hz.c1oappe.top/gtkrmhbqcq.html

PHP:  $argv;  $argc;
来源：http://hz.gogol.net.cn/gtelreevxn.html

JS:   process.argv.slice(2)
来源：http://hz.yvedp.cn/gtbtwhroos.html

TS:   process.argv.slice(2)
来源：http://hz.yj202588.top/gtzmyswpub.html

Java: args 数组（main 方法参数）
来源：http://hz.hnqzz.top/gtkjuqhjim.html

Go:   os.Args[1:]
来源：http://hz.52xcode.cn/gteuhwrnzj.html

Ruby: ARGV
来源：http://hz.9152youxi.cn/gtdechywfy.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ehwqpu.com/gteorunsph.html

[M02] 读取环境变量
来源：http://hz.yueranfly.top/gtkujgtadi.html

Py:   os.environ.get("HOME")
来源：http://hz.gzhubu.top/gtzwshqhxt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.birdmap.top/gtuxfqdrac.html

JS:   process.env.HOME
来源：http://hz.dashuyun.cn/gtwhymwwgu.html

TS:   process.env.HOME
来源：http://hz.zhengqikj.top/gtsvofwdlb.html

Java: System.getenv("HOME")
来源：http://hz.gotoacloud.top/gtyzwgyydv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhijiandao.cn/gthqpfrzwa.html

Ruby: ENV["HOME"]
来源：http://hz.sweek.top/gtuwlqqzas.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenzaomai.com/gtxgkrvjjp.html

[M03] 执行外部命令
来源：http://hz.hnqzz.top/gtfecapsti.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.chenjidiqi.icu/gtwmqjklwq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jqgufenzy.top/gtvvtzucsb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.9152youxi.cn/gtilszizvn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yvedp.cn/gtotjfvska.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yueranfly.top/gtglctoadd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ivvv.top/gttwivkigr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hfpthk.cn/gtwcsnhrif.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cheryme.top/gtegsguzba.html

[M04] 获取当前工作目录
来源：http://hz.svipenyu.cn/gtzdchhzdl.html

Py:   os.getcwd()
来源：http://hz.daria6918.cn/gtkwjwsgcd.html

PHP:  getcwd();
来源：http://hz.yuxming.cn/gttenitewa.html

JS:   process.cwd()
来源：http://hz.jqgufenzy.top/gtxpciqyzm.html

TS:   process.cwd()
来源：http://hz.fzhhl.top/gtwanfzamg.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yuanzhike.top/gttllqmjym.html

Go:   os.Getwd()
来源：http://hz.gogol.net.cn/gthavwxxog.html

Ruby: Dir.pwd
来源：http://hz.xingfuxueyuan.xyz/gtwehwldqb.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.tian-w.cn/gthnxgfthx.html

[M05] 设置退出码
来源：http://hz.aizwys.cn/gtkbrzszqb.html

Py:   sys.exit(1)
来源：http://hz.yj20258888.top/gtyvlrgldt.html

PHP:  exit(1);
来源：http://hz.hammf.cn/gtcfqvmfyu.html

JS:   process.exit(1)
来源：http://hz.pycfn.com/gtfntgsotx.html

TS:   process.exit(1)
来源：http://hz.hongshengwenyu.top/gtjdylmjpo.html

Java: System.exit(1)
来源：http://hz.yuxming.cn/gtpiyuairi.html

Go:   os.Exit(1)
来源：http://hz.jqgfzy.top/gtjhfunkwx.html

Ruby: exit 1
来源：http://hz.yongpay.top/gtqxysqiht.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.fengsongda.top/gttznjqmxy.html

[M06] 向标准错误输出
来源：http://hz.chenjidiqi.icu/gtygtdmaxd.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jyoumei.cn/gtvkdetdld.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.pycfn.com/gtnkbhgbtl.html

JS:   console.error("err")
来源：http://hz.jinqigfzy.top/gtcpdxmhre.html

TS:   console.error("err")
来源：http://hz.quarkkingdee.top/gtiknovkcu.html

Java: System.err.println("err")
来源：http://hz.ivvv.top/gtdjmulxlc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yvedp.cn/gtnrtqrucr.html

Ruby: warn "err"
来源：http://hz.sxryk.cn/gtrgpgogjm.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.tanke756.top/gtdbfrjkxc.html

[M07] 判断是否为主入口
来源：http://hz.ppjwa.cn/gtscejspbz.html

Py:   if __name__ == "__main__":
来源：http://hz.wangshuangyany.cn/gtdnioydhm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.aibaodan.cn/gtchgpmcfd.html

JS:   require.main === module
来源：http://hz.yonumen.top/gtbshbdazj.html

TS:   require.main === module
来源：http://hz.chenzaomai.com/gthsrscwni.html

Java: public static void main(String[] args)
来源：http://hz.jinyuanbaomall.cn/gtcyeueayb.html

Go:   func main()
来源：http://hz.zhiwuduotai.top/gtqtqtzdvz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jiagoushi.top/gtbpjalquc.html

C#:   static void Main(string[] args)
来源：http://hz.jinqigfzy.top/gtczgyuluy.html

[M08] 获取系统与运行时信息
来源：http://hz.ywan-chungtsiang.top/gtglndyiwv.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinqigfzy.top/gteobuwwof.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ybcxt.top/gtutyygoic.html

JS:   process.platform;  process.version
来源：http://hz.bjfxy.top/gtdsgkjnds.html

TS:   process.platform;  process.version
来源：http://hz.sweek.top/gtrkdkrrnr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.guannengcc.top/gtdlwdiugi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cdnleiting.top/gtnfxxmzdb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jqgufenzy.top/gtcoytouau.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.meibo888.top/gttbnyqhig.html

================================================================================
来源：http://hz.nanxuanxn.top/gtgleyanlt.html

N. 数据结构与算法
来源：http://hz.zhiwuduotai.top/gtlqqnklhw.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtoserwfea.html

[N01] 二分查找（有序数组）
来源：http://hz.ydjk.org.cn/gttgbmiwln.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinghuilouyu.cn/gtsetavgvq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hfpthk.cn/gtbmaxgjbb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tian-w.cn/gtcstofqyn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenlongwang.top/gttptnnlcq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shuidangran.top/gtpsooxisg.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.pycfn.com/gtzlppwuxe.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jiagoushi.top/gtsndqnlvr.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.9152youxi.cn/gtbphmhiwk.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.bjfxy.top/gthnosyrxg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.feifeiyinyue.top/gtgzjmvxmz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhoulong.xyz/gtgidivrxk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ppjwa.cn/gtoieycphn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ivvv.top/gtqgnkyemn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.mhx1999.top/gtxnlyucqr.html

Go:   slices.Sort(arr)
来源：http://hz.xingfuxueyuan.xyz/gtzzokxqfa.html

Ruby: arr.sort
来源：http://hz.chenjidiqi.icu/gtqvooxcgp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.snrcjt.cn/gtepgmkhjr.html

[N03] 快速排序（分治示例）
来源：http://hz.zycfv.cn/gtalorvutk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yanxiufei.cn/gtkjjgcitc.html

PHP:  // 递归实现，或用 usort
来源：http://hz.iojbl.cn/gtyszisbkh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sweek.top/gtqybqgxpg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cqqwz.cn/gttixlguwj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yanxiufei.cn/gtxucmyttb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.quarkkingdee.top/gtenwurdqu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sxryk.cn/gtwbadfozs.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hfpthk.cn/gtwsytgltt.html

[N04] 斐波那契数列
来源：http://hz.bjfxy.top/gtoayzazmh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.guannengcc.top/gtlblerzbz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhengqikj.top/gtlcmxkwvh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.guowangkeji.top/gtzyfonhqx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.andypj.xyz/gtkgvftsip.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xingfuxueyuan.xyz/gtsglyvraz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ywan-chungtsiang.top/gtcgxqubyk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.aibaodan.cn/gthnflwfpq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yonumen.top/gtyzxaujbi.html

[N05] 最大公约数
来源：http://hz.xinyue.icu/gtdycmznit.html

Py:   math.gcd(a, b)
来源：http://hz.hywenlv.cn/gtivvmerir.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shzxlz.cn/gtyorbdjam.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tanke756.top/gtwrlinhdg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cheryme.top/gtiydpvyko.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yonumen.top/gtokxtrvyi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jinqigfzy.top/gtlwbfhska.html

Ruby: a.gcd(b)
来源：http://hz.chenzaomai.com/gtktwzjtmp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jqgfzy.top/gtmqonrqkc.html

[N06] 判断回文字符串
来源：http://hz.jlsjyb.cn/gtadruqrcf.html

Py:   s == s[::-1]
来源：http://hz.c1oappe.top/gtmsrbqfth.html

PHP:  $s === strrev($s);
来源：http://hz.ivvv.top/gtlfudcdcu.html


<!-- 参考信息 -->