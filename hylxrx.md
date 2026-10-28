代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gtdpzzhpik.html

[J08] 提取年月日与星期
来源：http://hz.ivvv.top/gtrahwtnru.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hysaishi.cn/gtrrabdviq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.vqdsnc.cn/gtnzaveydi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sxryk.cn/gtrfsjsfgy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yongpay.top/gttqnxkbwt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zycfv.cn/gtvfgrizyn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hysaishi.cn/gthfukwepi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.pycfn.com/gtwxnxyzxu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhoulong.xyz/gtqhioyjwe.html

[J09] 时区处理
来源：http://hz.xinyue.icu/gtofcegowr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sxryk.cn/gtbwegqqir.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.meibo888.top/gtwzlvnlni.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yvedp.cn/gtqkhohvlq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.52xcode.cn/gthxffnrfh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yvedp.cn/gtkggbnyti.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.dianchejie.cn/gtiirmcgir.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gogol.net.cn/gtayolfvhi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yuxming.cn/gtxbsirikq.html

[J10] 取今天 / 本月第一天
来源：http://hz.redwolf501.top/gtrqomicob.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hnxiangtu.top/gtdavdyamf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jqgufenzy.top/gtpmhqwygv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.vqdsnc.cn/gtjvtzuoov.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ydjk.org.cn/gtfldmqqux.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jianghu66.top/gtuptfeike.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jiagoushi.top/gtwhfbzsyz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yj20258888.top/gtgrofgalt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.quarkkingdee.top/gtmgtlbyij.html

================================================================================
来源：http://hz.jqgfzy.top/gttxkpgdpi.html

K. JSON 与序列化
来源：http://hz.haohaochexian.top/gtdlivazpz.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtlzjnvbgy.html

[K01] 对象转 JSON 字符串
来源：http://hz.guowangkeji.top/gtzxkznkuh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.wangdashe.top/gtiqverygl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258888.top/gtixljlfqt.html

JS:   JSON.stringify(obj)
来源：http://hz.yj202588.top/gtebsspdns.html

TS:   JSON.stringify(obj)
来源：http://hz.meibo888.top/gttaxxicjn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zycfv.cn/gtqlmzohgy.html

Go:   json.Marshal(obj)
来源：http://hz.aibaodan.cn/gtdquhnwsk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cucudq.cn/gtekthybjl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.chenlongwang.top/gtyldrztak.html

[K02] JSON 字符串转对象
来源：http://hz.yanxiufei.cn/gtrodhbalx.html

Py:   json.loads(s)
来源：http://hz.ydzc1.top/gtpoyhqmqr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cucudq.cn/gtyrpezbsw.html

JS:   JSON.parse(s)
来源：http://hz.svipenyu.cn/gtxwvzrhgq.html

TS:   JSON.parse(s)
来源：http://hz.shanyushiyangkeji.top/gthzupzfgk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.aibaodan.cn/gtewlfjfal.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.guannengcc.top/gtmlfalsri.html

Ruby: JSON.parse(s)
来源：http://hz.daria6918.cn/gtljwmsazq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.daria6918.cn/gtbjxmqkrg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.nwbrower.top/gtbcncwxre.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.chenlongwang.top/gtlyrjetil.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhongyouzk.top/gtioueoctw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258888.top/gtnmnbmfux.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xinyue.icu/gtamwxykxu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.aibaodan.cn/gtvtkpjjjc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinqigufen.top/gtlkyrxkqy.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hammf.cn/gtdvlukbjp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.guowangkeji.top/gtflhtwnfu.html

[K04] 读取 JSON 文件
来源：http://hz.ppjwa.cn/gtjgpgptfb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hywenlv.cn/gtfqwwxtya.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.kuanghao11.cn/gtdxowvpyf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yonumen.top/gttafxoono.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinyuanbaomall.cn/gtakghhewe.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.tian-w.cn/gtqonubijp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenlongwang.top/gtlzvujtli.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shzxlz.cn/gtvrmulymi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tanke756.top/gtibqswyuu.html

[K05] 深拷贝对象
来源：http://hz.cashguo.top/gthebykphf.html

Py:   copy.deepcopy(obj)
来源：http://hz.gzhubu.top/gtlujlvnqi.html

PHP:  unserialize(serialize($obj));
来源：http://hz.tianlin.xyz/gtmjzcpnei.html

JS:   structuredClone(obj)
来源：http://hz.xziqi.cn/gtjifiebbo.html

TS:   structuredClone(obj)
来源：http://hz.ydjk.org.cn/gturaqwdnt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zycfv.cn/gtdvgyygei.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.tian-w.cn/gtpevxxdca.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shangyingyoupin.top/gtfhphucbb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.nanxuanxn.top/gtdulusjzr.html

[K06] 解析 URL 查询串
来源：http://hz.dashuyun.cn/gtqbypilni.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ppjwa.cn/gtzsjiymdt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.snrcjt.cn/gtovsyfldd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydzc1.top/gtikyqevro.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.guannengcc.top/gtrukgrlbr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yangfankeji.com/gtmxnzrzek.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ehwqpu.com/gtoyjlnnph.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xingfuxueyuan.xyz/gtgmrofzaf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jiagoushi.top/gtpowwfiva.html

[K07] 进制转换
来源：http://hz.daria6918.cn/gtdjipcvya.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cashguo.top/gtxvogsbis.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj202588.top/gtfgkgoyrs.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.cheryme.top/gtgibmgsrt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.pengpengdd.cyou/gtpxkzsxdn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.gaohongyu789.top/gtrhdzwgyq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.pengpengdd.cyou/gtubghnoxq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.aibaodan.cn/gtleybqhqa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.dashuyun.cn/gtegrblwcy.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.quarkkingdee.top/gtvqoylgnd.html

Py:   pickle.dumps(obj)
来源：http://hz.ywan-chungtsiang.top/gtakzztdjm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.dashuyun.cn/gtvjfwfoyi.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yj20258.top/gtwfcccdjg.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jlsjyb.cn/gtzewzamdw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hysaishi.cn/gtltjwobjv.html

Go:   encoding/gob
来源：http://hz.gotoacloud.top/gtqkpkpyzp.html

Ruby: Marshal.dump(obj)
来源：http://hz.tanke756.top/gtrgljeeot.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.52xcode.cn/gtyslofixh.html

================================================================================
来源：http://hz.cheryme.top/gtdwdrgyvs.html

L. 网络请求
来源：http://hz.dianchejie.cn/gtkbhqcwjx.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gttwkqbrjs.html

[L01] 发送 GET 请求
来源：http://hz.wangdashe.top/gtpekpdvsr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gaohongyu789.top/gtfaxzbueu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yanxiufei.cn/gtvbxniush.html

JS:   await fetch(url)
来源：http://hz.yj202588.top/gtpxwsiyuf.html

TS:   await fetch(url)
来源：http://hz.jiagoushi.top/gtrzmjcwbr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gogol.net.cn/gtwdawuijg.html

Go:   resp, err := http.Get(url)
来源：http://hz.shangyingyoupin.top/gtbdndgzzz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.0kj1m.cn/gtbadnpnvs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.sweek.top/gttygrgmzs.html

[L02] 发送 POST JSON
来源：http://hz.jinqigufen.top/gtgryqobqf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jianghu66.top/gtavfzectc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.pengpengdd.cyou/gtbnztwcpt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.52xcode.cn/gthfyfrrzu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.haohaochexian.top/gtwapvmscm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.52xcode.cn/gtyowbersg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shangyingyoupin.top/gtauakndsm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.dianchejie.cn/gtvkkfkdtx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.chenzaomai.com/gtjhqtviai.html

[L03] 设置自定义请求头
来源：http://hz.shangyingyoupin.top/gtkjhadrlb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jyoumei.cn/gtbosvlzsf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.birdmap.top/gtoijjyrvp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinqigfzy.top/gtjzsrewyk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.smart0.xyz/gttkmfkjbe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.c1oappe.top/gtgbbtgwex.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.gaohongyu789.top/gtdorxdaju.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhixingplan.top/gtfdpczcpf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.pengpengdd.cyou/gteecprsaa.html

[L04] 设置超时
来源：http://hz.ehwqpu.com/gtwxulhgzy.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cucudq.cn/gtvmljoijx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yongpay.top/gtxyphswjd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yongpay.top/gtrhbmurpw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgfzy.top/gtcdqgjbkg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cdnleiting.top/gtumawzkss.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.feifeiyinyue.top/gtdwoqrgpd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.dashuyun.cn/gtikhzcnhu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.fzhhl.top/gtdmazcosu.html

[L05] 上传文件（multipart）
来源：http://hz.svipenyu.cn/gtyiydwlrr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ppjwa.cn/gtmvejzraj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yongpay.top/gtaahhkzgs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.meibo888.top/gtlbemwtbu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.nwbrower.top/gtcojxbijm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.kuanghao11.cn/gtnsbqsqxg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.pengpengdd.cyou/gtkitfqqqb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cheryme.top/gtdhxtcprg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gogol.net.cn/gtveksbkxf.html

[L06] 解析响应为 JSON
来源：http://hz.sufxvd.cn/gtguxkbvma.html

Py:   resp.json()
来源：http://hz.fzhhl.top/gtglmgwvkx.html

PHP:  json_decode($body, true);
来源：http://hz.sufxvd.cn/gtgwikctae.html

JS:   await resp.json()
来源：http://hz.zycfv.cn/gtuzjbaqmr.html

TS:   await resp.json()
来源：http://hz.c1oappe.top/gtzyhyxzvq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jyoumei.cn/gtjejuevou.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.havefunace.top/gtxguixxcf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ppjwa.cn/gtjvfrcyzi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jqgfzy.top/gtrdtozncx.html

[L07] 处理 HTTP 状态码
来源：http://hz.tian-w.cn/gtmbirfhep.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ywan-chungtsiang.top/gtnmqzwyqg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jqgfzy.top/gthnttqxmk.html

JS:   resp.ok;  resp.status
来源：http://hz.yongpay.top/gtrvtfazsy.html

TS:   resp.ok;  resp.status
来源：http://hz.gotoacloud.top/gtvtqwbpcw.html

Java: resp.statusCode()
来源：http://hz.haohaochexian.top/gtrcljjiyb.html

Go:   resp.StatusCode
来源：http://hz.yongpay.top/gtkxwbidhe.html

Ruby: resp.code.to_i
来源：http://hz.shuidangran.top/gtuerknkya.html

C#:   (int)resp.StatusCode
来源：http://hz.pycfn.com/gtpdfibjgh.html

[L08] 并发请求多个地址
来源：http://hz.ywan-chungtsiang.top/gtbhkgnoau.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yanxiufei.cn/gtsnioczva.html

PHP:  curl_multi_init() 系列
来源：http://hz.chenzaomai.com/gtoexmxkhu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.svipenyu.cn/gtehhruxpy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shuidangran.top/gtrdxcfpyx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yangfankeji.com/gtlylcnieq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zycfv.cn/gtanwjwynd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.birdmap.top/gtawbuktjh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.guowangkeji.top/gtrnoqxurl.html

================================================================================
来源：http://hz.zhijiandao.cn/gtuhcelvkf.html

M. 命令行 / 进程 / 环境
来源：http://hz.vqdsnc.cn/gtsxjcgxnp.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtdiuwlkqh.html

[M01] 读取命令行参数
来源：http://hz.quarkkingdee.top/gtgcivsemx.html

Py:   sys.argv[1:]
来源：http://hz.zhixingplan.top/gtdevdsapo.html

PHP:  $argv;  $argc;
来源：http://hz.kuanghao11.cn/gtozlinscz.html

JS:   process.argv.slice(2)
来源：http://hz.nanxuanxn.top/gtcthlrnto.html

TS:   process.argv.slice(2)
来源：http://hz.52xcode.cn/gteafallrn.html

Java: args 数组（main 方法参数）
来源：http://hz.wangshuangyany.cn/gtbhmmbpql.html

Go:   os.Args[1:]
来源：http://hz.chenzaomai.com/gthqrlzvul.html

Ruby: ARGV
来源：http://hz.fzhhl.top/gttlgbdtcd.html

C#:   args 数组（Main 方法参数）
来源：http://hz.andypj.xyz/gtkonirptl.html

[M02] 读取环境变量
来源：http://hz.haohaochexian.top/gtaovrfwgh.html

Py:   os.environ.get("HOME")
来源：http://hz.cqqwz.cn/gthnvmigif.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.fengsongda.top/gtrceruluy.html

JS:   process.env.HOME
来源：http://hz.zhijiandao.cn/gtkwyzhghi.html

TS:   process.env.HOME
来源：http://hz.shanyushiyangkeji.top/gtbmikiwbu.html

Java: System.getenv("HOME")
来源：http://hz.yj202588.top/gttlnechgm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.tian-w.cn/gtsgxnnrjj.html

Ruby: ENV["HOME"]
来源：http://hz.havefunace.top/gtfsekzbcw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hywenlv.cn/gtoqczfxgw.html

[M03] 执行外部命令
来源：http://hz.sufxvd.cn/gtwnhgecvc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cdnleiting.top/gtgghzrtky.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xingfuxueyuan.xyz/gthxxnykey.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.fengsongda.top/gtsmrkwtze.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xuetiantiany.cn/gtodjwrpvz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yuxming.cn/gtgckcrouz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tianlin.xyz/gtxsjmjibh.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ybcxt.top/gtbvdszqnx.html

C#:   Process.Start("ls", "-l");
来源：http://hz.fzhhl.top/gttmwobwfl.html

[M04] 获取当前工作目录
来源：http://hz.zhongyouzk.top/gtwbarywdk.html

Py:   os.getcwd()
来源：http://hz.fengsongda.top/gtbdyarfla.html

PHP:  getcwd();
来源：http://hz.sufxvd.cn/gthsirhbqt.html

JS:   process.cwd()
来源：http://hz.0kj1m.cn/gtuyuutzzz.html

TS:   process.cwd()
来源：http://hz.wangshuangyany.cn/gtivbiuznj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hammf.cn/gtanhrsncu.html

Go:   os.Getwd()
来源：http://hz.jinyuanbaomall.cn/gtnqcfitgl.html

Ruby: Dir.pwd
来源：http://hz.jinyuanbaomall.cn/gtevkcbmgi.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.haohaochexian.top/gtsnvduhjf.html

[M05] 设置退出码
来源：http://hz.zhixingplan.top/gtwxsvixwe.html

Py:   sys.exit(1)
来源：http://hz.tianlin.xyz/gtkbafrrdw.html

PHP:  exit(1);
来源：http://hz.chenlongwang.top/gtpywotshe.html

JS:   process.exit(1)
来源：http://hz.daria6918.cn/gtolyjfejj.html

TS:   process.exit(1)
来源：http://hz.yonumen.top/gtfxbmhqcg.html

Java: System.exit(1)
来源：http://hz.hammf.cn/gtcgybalcn.html

Go:   os.Exit(1)
来源：http://hz.yongpay.top/gtigfzyruw.html

Ruby: exit 1
来源：http://hz.gaohongyu789.top/gtlzdngmrb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xziqi.cn/gtgpoquhvc.html

[M06] 向标准错误输出
来源：http://hz.nanxinkj.top/gthhmfowje.html

Py:   print("err", file=sys.stderr)
来源：http://hz.fengsongda.top/gtuzdtrlfx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.nanxinkj.top/gtqwszmgvr.html

JS:   console.error("err")
来源：http://hz.daria6918.cn/gtbxvzezrl.html

TS:   console.error("err")
来源：http://hz.zhongyouzk.top/gtrewhqyqt.html

Java: System.err.println("err")
来源：http://hz.yuxming.cn/gtslldcatp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.tanke756.top/gtzqyqsmkl.html

Ruby: warn "err"
来源：http://hz.yanxiufei.cn/gtsstswueq.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.guannengcc.top/gtpqgegddw.html

[M07] 判断是否为主入口
来源：http://hz.yj20258.top/gtldwmmeyd.html

Py:   if __name__ == "__main__":
来源：http://hz.chenzaomai.com/gtafruford.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zycfv.cn/gtecozmriu.html

JS:   require.main === module
来源：http://hz.hywenlv.cn/gtkpwoqmsq.html

TS:   require.main === module
来源：http://hz.jiagoushi.top/gtkfmhwigq.html

Java: public static void main(String[] args)
来源：http://hz.nanxuanxn.top/gtstddozse.html

Go:   func main()
来源：http://hz.tanke756.top/gtimvljbuu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.shzxlz.cn/gtfjibbran.html

C#:   static void Main(string[] args)
来源：http://hz.guannengcc.top/gtfzldogzt.html

[M08] 获取系统与运行时信息
来源：http://hz.shanyushiyangtech.top/gtbvnkxgdd.html

Py:   platform.system();  platform.python_version()
来源：http://hz.wangshuangyany.cn/gtgaizqqhc.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yuxming.cn/gtqbqyisgb.html

JS:   process.platform;  process.version
来源：http://hz.haohaochexian.top/gtzlbszqvn.html

TS:   process.platform;  process.version
来源：http://hz.fzhhl.top/gtguxbunag.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.fzhhl.top/gtljveqecp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cdnleiting.top/gtuymgqyck.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ydzc1.top/gtxyosebuc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jyoumei.cn/gtolfnoffh.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtjbrleoiq.html

N. 数据结构与算法
来源：http://hz.jinqigfzy.top/gtpxweewfi.html

================================================================================
来源：http://hz.tian-w.cn/gtyfyrarza.html

[N01] 二分查找（有序数组）
来源：http://hz.yangfankeji.com/gtjzmblknk.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.fengsongda.top/gtcvncrufi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yj20258888.top/gtygqnuomf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.9152youxi.cn/gtfpnupbpr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dashuyun.cn/gtuimlilkx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.feifeiyinyue.top/gtggyoooso.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ehwqpu.com/gtspxkdvfh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhaomingkeji.xyz/gtdlyhfwsi.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jiagoushi.top/gtobvvhzln.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.bjfxy.top/gtklykijoi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.svipenyu.cn/gtzkbmbbmz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tianlin.xyz/gtqzjkqaal.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hywenlv.cn/gtvrclzwlk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hywenlv.cn/gtrwpdtqkf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ivvv.top/gtzekzvclg.html

Go:   slices.Sort(arr)
来源：http://hz.nwbrower.top/gtutjeceno.html

Ruby: arr.sort
来源：http://hz.gotoacloud.top/gtzvcalzrn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sweek.top/gtxsfpkvtc.html

[N03] 快速排序（分治示例）
来源：http://hz.meibo888.top/gteksjgntf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.meibo888.top/gtyjppmzfw.html

PHP:  // 递归实现，或用 usort
来源：http://hz.svipenyu.cn/gtvgurosqi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ehwqpu.com/gtzgnzzwop.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.redwolf501.top/gtjyxdqowq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.pycfn.com/gthgvizggy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jinghuilouyu.cn/gtdyhjicnt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.svipenyu.cn/gtrcyneeie.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.mhx1999.top/gtmnsymchl.html

[N04] 斐波那契数列
来源：http://hz.bjfxy.top/gtphoigcts.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigfzy.top/gtuqxilyjg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.tian-w.cn/gtgkfgxrva.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yvedp.cn/gtjahcgxqt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yueranfly.top/gtulswgrxw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cucudq.cn/gtqykbdesi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yuxming.cn/gtvmewgiyp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258.top/gttoperyle.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cucudq.cn/gtzktbocdw.html

[N05] 最大公约数
来源：http://hz.jinqigufen.top/gtiwvgbcbe.html

Py:   math.gcd(a, b)
来源：http://hz.zhijiandao.cn/gtvhdchbks.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinyuanbaomall.cn/gtktjkryen.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sxryk.cn/gtlcocztef.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.svipenyu.cn/gtggzvqxnd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.tian-w.cn/gtirckuacx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.wangshuangyany.cn/gtbwlxinqj.html

Ruby: a.gcd(b)
来源：http://hz.yvedp.cn/gtfpjswzhr.html


<!-- 参考信息 -->