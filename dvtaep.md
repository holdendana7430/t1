代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://hz.quarkkingdee.top/gtsjsdurtz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhengqikj.top/gtljuhbgce.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.aizwys.cn/gtkbzakgsi.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.haohaochexian.top/gtskhzqobb.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.c1oappe.top/gtcbayoopk.html

[J08] 提取年月日与星期
来源：http://hz.0kj1m.cn/gthmnxewmf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.wangdashe.top/gtzogvuzeo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhengqikj.top/gtjhcyiznd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhixingplan.top/gtusybnfab.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yanxiufei.cn/gtalqrsxaw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yj20258.top/gtgemwykqv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xylfe.cn/gtcdlreugc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gaohongyu789.top/gtmplsjbof.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.nanxinkj.top/gtwnywvzvi.html

[J09] 时区处理
来源：http://hz.jyoumei.cn/gtibiostpm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.wangshuangyany.cn/gtvduigziq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.mhx1999.top/gtxuretpbs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sysykeji.top/gtrtvzneeh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.birdmap.top/gtayqqwaam.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinyuanbaomall.cn/gtgqgtcqbw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yueranfly.top/gtddvoluxn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jqgfzy.top/gtjofzuuit.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ppjwa.cn/gtajjxtfub.html

[J10] 取今天 / 本月第一天
来源：http://hz.sxryk.cn/gthwgzlrki.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ywan-chungtsiang.top/gtrkvnzupo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.daxiang520.top/gtdfnlavcu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xylfe.cn/gtbnyucabr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.fzhhl.top/gtqwhfofod.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xuanzx.com/gttvlhpaco.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinghuilouyu.cn/gtqdpgsntm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhaomingkeji.xyz/gtfrgdkqha.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhijiandao.cn/gtvmwfjqeg.html

================================================================================
来源：http://hz.xuanzx.com/gtixsgtubq.html

K. JSON 与序列化
来源：http://hz.hongshengwenyu.top/gtqhscwxkn.html

================================================================================
来源：http://hz.9152youxi.cn/gtnnnkdetp.html

[K01] 对象转 JSON 字符串
来源：http://hz.guannengcc.top/gttfdmweai.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yangfankeji.com/gtzopotpms.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.aibaodan.cn/gtvfbrwtcx.html

JS:   JSON.stringify(obj)
来源：http://hz.ydzc1.top/gtdicyccog.html

TS:   JSON.stringify(obj)
来源：http://hz.kuanghao11.cn/gtaddrhydq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.andypj.xyz/gtyjbwvqfd.html

Go:   json.Marshal(obj)
来源：http://hz.sxryk.cn/gtbuixxswt.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.guannengcc.top/gtyzuswzhc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.guannengcc.top/gtissjfryj.html

[K02] JSON 字符串转对象
来源：http://hz.sysykeji.top/gteeqgecnq.html

Py:   json.loads(s)
来源：http://hz.vqdsnc.cn/gtwmrwcliy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gotoacloud.top/gtxwfkcocz.html

JS:   JSON.parse(s)
来源：http://hz.haohaochexian.top/gtykyxogby.html

TS:   JSON.parse(s)
来源：http://hz.cashguo.top/gtptrukgzy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gotoacloud.top/gtcgqkohbk.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cucudq.cn/gttdgmuogh.html

Ruby: JSON.parse(s)
来源：http://hz.52xcode.cn/gtgnqswayp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sweek.top/gthdbpdszb.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.kuanghao11.cn/gteiicvcjl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cdnleiting.top/gtkhhrgkcs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhixingplan.top/gtgttbzals.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.tian-w.cn/gtgavhpaoe.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sxryk.cn/gtqqnaktwu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.havefunace.top/gtqopjczwg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jqgfzy.top/gtuwkfklpu.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xuetiantiany.cn/gtwwqayfoc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.birdmap.top/gtqmolwzye.html

[K04] 读取 JSON 文件
来源：http://hz.vqdsnc.cn/gtiferyduq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinqigfzy.top/gtasjqweuj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yangfankeji.com/gtskucyums.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tian-w.cn/gtuaqvafdw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yanxiufei.cn/gtrzjqgrzk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sxryk.cn/gtahlesmwd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yonumen.top/gtxhafcoud.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gaohongyu789.top/gtbjcyimww.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cqqwz.cn/gtntupgivw.html

[K05] 深拷贝对象
来源：http://hz.yj20258.top/gtumvhlkfd.html

Py:   copy.deepcopy(obj)
来源：http://hz.jqgufenzy.top/gtuhebqlov.html

PHP:  unserialize(serialize($obj));
来源：http://hz.nanxuanxn.top/gtxfdcliig.html

JS:   structuredClone(obj)
来源：http://hz.ehwqpu.com/gtbyxzpkbl.html

TS:   structuredClone(obj)
来源：http://hz.feifeiyinyue.top/gtyjyvxlvq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.andypj.xyz/gtatjfubkk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.fengsongda.top/gtdwivtefg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.c1oappe.top/gtgzucciaf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yj20258888.top/gtcagcyrpr.html

[K06] 解析 URL 查询串
来源：http://hz.cashguo.top/gtysguhfgg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.tianlin.xyz/gtsqlrumby.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jlsjyb.cn/gtkgcgmqab.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenjidiqi.icu/gtvuupqjvc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jyoumei.cn/gtutgynnaf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinqigufen.top/gtnxvvwaar.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.haohaochexian.top/gtulqkjehc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shzxlz.cn/gtyomxrdnm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinghuilouyu.cn/gtoeaclhls.html

[K07] 进制转换
来源：http://hz.xuetiantiany.cn/gttpkcyasu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hongshengwenyu.top/gtbianqvji.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj20258.top/gtpvcrgjat.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hongshengwenyu.top/gtgkguqtzu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.dashuyun.cn/gtlbvgmscd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.chenzaomai.com/gtamawjxjv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.tianlin.xyz/gtdrhhxzhq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xuanzx.com/gtqxnmjgrx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.snrcjt.cn/gtytjgdwyp.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.iojbl.cn/gthsboygrb.html

Py:   pickle.dumps(obj)
来源：http://hz.316326.xyz/gtkcvjmplu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhaomingkeji.xyz/gtthhmvfxc.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.feifeiyinyue.top/gtxkdazmvc.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.mhx1999.top/gtyqdirbxh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.316326.xyz/gtqrgsuaps.html

Go:   encoding/gob
来源：http://hz.cdnleiting.top/gtzocupppl.html

Ruby: Marshal.dump(obj)
来源：http://hz.xylfe.cn/gtqjkpyztl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ydzc1.top/gtscblkqaq.html

================================================================================
来源：http://hz.zycfv.cn/gtbkxjfqvm.html

L. 网络请求
来源：http://hz.vqdsnc.cn/gtnolqrupb.html

================================================================================
来源：http://hz.ivvv.top/gtynkyzgyq.html

[L01] 发送 GET 请求
来源：http://hz.jlsjyb.cn/gtrlgdtpay.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ywan-chungtsiang.top/gtwrxqhbiq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hongshengwenyu.top/gtcgthhgjf.html

JS:   await fetch(url)
来源：http://hz.yj20258888.top/gtwajsoqva.html

TS:   await fetch(url)
来源：http://hz.yueranfly.top/gtkgwvcbgq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ivvv.top/gtsbjqxgzw.html

Go:   resp, err := http.Get(url)
来源：http://hz.ybcxt.top/gtisijmfct.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cheryme.top/gtmkxzhtuv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.chenzaomai.com/gtvjstpqjr.html

[L02] 发送 POST JSON
来源：http://hz.kuanghao11.cn/gtcwbdrfwp.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhijiandao.cn/gtbehjrdol.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sysykeji.top/gtooclogwl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yvedp.cn/gtryiuhosd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhijiandao.cn/gthcykfnpt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.chenzaomai.com/gtxdkgwcip.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xylfe.cn/gtjedqkcrg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhiwuduotai.top/gtangftubh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.tianlin.xyz/gtqpkmleqi.html

[L03] 设置自定义请求头
来源：http://hz.gzhubu.top/gtsevmmlgj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ivvv.top/gtnougkarx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhaomingkeji.xyz/gtwgzfminr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tianlin.xyz/gtdfwcmdli.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuetiantiany.cn/gtbzavhhlj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yanxiufei.cn/gtbjwykvzm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hywenlv.cn/gtmsjhkito.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sufxvd.cn/gtbnbjnmck.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.dashuyun.cn/gtyfcqzefl.html

[L04] 设置超时
来源：http://hz.pycfn.com/gtlgeuzarb.html

Py:   requests.get(url, timeout=5)
来源：http://hz.chenlongwang.top/gtzpgynltv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cqqwz.cn/gtxwotrkkt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.meibo888.top/gtxwpwvqsg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.pycfn.com/gttquwzoar.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhaomingkeji.xyz/gtvpwfkgbf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.daria6918.cn/gtkeqzvpjl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhongyouzk.top/gtltqlddrm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.snrcjt.cn/gtdxndpcum.html

[L05] 上传文件（multipart）
来源：http://hz.ydjk.org.cn/gtqtuejfmi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.svipenyu.cn/gtzyaveerm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hysaishi.cn/gtacnoxllx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.c1oappe.top/gtljvwxjgg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.havefunace.top/gtqqsqltxk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gogol.net.cn/gtrahguaxb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zycfv.cn/gtqlokjdln.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shzxlz.cn/gtnsiogvkc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.feifeiyinyue.top/gtntdgoagv.html

[L06] 解析响应为 JSON
来源：http://hz.hammf.cn/gtkkfpwgzl.html

Py:   resp.json()
来源：http://hz.ehwqpu.com/gtddkgteku.html

PHP:  json_decode($body, true);
来源：http://hz.c1oappe.top/gtawqmbujw.html

JS:   await resp.json()
来源：http://hz.quarkkingdee.top/gtvwditsmd.html

TS:   await resp.json()
来源：http://hz.tianlin.xyz/gtomdmvhqk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ybcxt.top/gtnemhhnkn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.tianlin.xyz/gtnxlsksli.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yanxiufei.cn/gtuqlnymge.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ydzc1.top/gtqpshylka.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhoulong.xyz/gtdhagtebe.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.pycfn.com/gtmrhmepci.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhoulong.xyz/gtmtsurftq.html

JS:   resp.ok;  resp.status
来源：http://hz.vqdsnc.cn/gtcrnjjson.html

TS:   resp.ok;  resp.status
来源：http://hz.cheryme.top/gtqxprgrkk.html

Java: resp.statusCode()
来源：http://hz.daxiang520.top/gtzpnifnno.html

Go:   resp.StatusCode
来源：http://hz.birdmap.top/gtxqhiujrr.html

Ruby: resp.code.to_i
来源：http://hz.xingfuxueyuan.xyz/gtatdjuucw.html

C#:   (int)resp.StatusCode
来源：http://hz.yuanzhike.top/gtnmnlupnp.html

[L08] 并发请求多个地址
来源：http://hz.ehwqpu.com/gtdmakyqwp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.aibaodan.cn/gtsuujatlk.html

PHP:  curl_multi_init() 系列
来源：http://hz.yangfankeji.com/gtyzihlmuu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yongpay.top/gtucficeft.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenzaomai.com/gtzudzyaxk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhaomingkeji.xyz/gtwlpqfhcx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.meibo888.top/gteiveconp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.chenzaomai.com/gtqwbhegat.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.9152youxi.cn/gtusfuvyle.html

================================================================================
来源：http://hz.gaohongyu789.top/gtieeyecvs.html

M. 命令行 / 进程 / 环境
来源：http://hz.jlsjyb.cn/gtrndtwmfa.html

================================================================================
来源：http://hz.ydjk.org.cn/gtdpditkzs.html

[M01] 读取命令行参数
来源：http://hz.svipenyu.cn/gtjoleokvo.html

Py:   sys.argv[1:]
来源：http://hz.fzhhl.top/gtpajzdduy.html

PHP:  $argv;  $argc;
来源：http://hz.0kj1m.cn/gtpoouiqpr.html

JS:   process.argv.slice(2)
来源：http://hz.9152youxi.cn/gtikomyccr.html

TS:   process.argv.slice(2)
来源：http://hz.sysykeji.top/gtbokftdsq.html

Java: args 数组（main 方法参数）
来源：http://hz.pycfn.com/gthegngsgl.html

Go:   os.Args[1:]
来源：http://hz.zdqjudy.top/gtddtkgxym.html

Ruby: ARGV
来源：http://hz.kuanghao11.cn/gtlxsaplqm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sweek.top/gttwwnvpkl.html

[M02] 读取环境变量
来源：http://hz.quarkkingdee.top/gtluuahmoq.html

Py:   os.environ.get("HOME")
来源：http://hz.shzxlz.cn/gtzvanzrbl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.havefunace.top/gtuqmjiijd.html

JS:   process.env.HOME
来源：http://hz.hongshengwenyu.top/gttfpqjjkf.html

TS:   process.env.HOME
来源：http://hz.tianlin.xyz/gtvaoecaia.html

Java: System.getenv("HOME")
来源：http://hz.hysaishi.cn/gtrtqqcpgb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.316326.xyz/gtwvqhobtp.html

Ruby: ENV["HOME"]
来源：http://hz.shangyingyoupin.top/gtkvwnanhw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ehwqpu.com/gtvdjuetuh.html

[M03] 执行外部命令
来源：http://hz.zdqjudy.top/gtkxlfymdf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jinyuanbaomall.cn/gtjyijudqq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.smart0.xyz/gtlubcrpce.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hammf.cn/gtucxtivgv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shzxlz.cn/gtjghkilcf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hysaishi.cn/gtwqrkfabt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.guannengcc.top/gtpsaqgymm.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jinyuanbaomall.cn/gtqiqrjmbj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shanyushiyangkeji.top/gtstlmpzls.html

[M04] 获取当前工作目录
来源：http://hz.yangfankeji.com/gtagxcpnvp.html

Py:   os.getcwd()
来源：http://hz.shzxlz.cn/gtiyloghhr.html

PHP:  getcwd();
来源：http://hz.kuanghao11.cn/gtfszfirwb.html

JS:   process.cwd()
来源：http://hz.xylfe.cn/gtjqzjukld.html

TS:   process.cwd()
来源：http://hz.zhoulong.xyz/gtavljhtow.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xingfuxueyuan.xyz/gtsyhhxqkq.html

Go:   os.Getwd()
来源：http://hz.yj20258888.top/gtjfordhjx.html

Ruby: Dir.pwd
来源：http://hz.zhongyouzk.top/gtcqbpaimu.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shuidangran.top/gtgsjwskdd.html

[M05] 设置退出码
来源：http://hz.hnxiangtu.top/gtrchjiimu.html

Py:   sys.exit(1)
来源：http://hz.ydzc1.top/gtyrrfrdul.html

PHP:  exit(1);
来源：http://hz.zhoulong.xyz/gtflzqmjgc.html

JS:   process.exit(1)
来源：http://hz.snrcjt.cn/gtgcgknzym.html

TS:   process.exit(1)
来源：http://hz.ppjwa.cn/gtdstapzkz.html

Java: System.exit(1)
来源：http://hz.ydjk.org.cn/gtwffpddyi.html

Go:   os.Exit(1)
来源：http://hz.jqgfzy.top/gtcgjscgjs.html

Ruby: exit 1
来源：http://hz.0kj1m.cn/gtksyjiyvn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hammf.cn/gtqxmzmunu.html

[M06] 向标准错误输出
来源：http://hz.jinqigufen.top/gticsrpcvk.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gaohongyu789.top/gtdwpdtmgs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hywenlv.cn/gtfajzjrbt.html

JS:   console.error("err")
来源：http://hz.zhijiandao.cn/gtqtejxkrm.html

TS:   console.error("err")
来源：http://hz.redwolf501.top/gtzylhmisq.html

Java: System.err.println("err")
来源：http://hz.c1oappe.top/gtnebddvjc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhaomingkeji.xyz/gtfexwziiw.html

Ruby: warn "err"
来源：http://hz.yonumen.top/gtaymztinn.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.redwolf501.top/gtguvslzko.html

[M07] 判断是否为主入口
来源：http://hz.nwbrower.top/gtstyfpqoj.html

Py:   if __name__ == "__main__":
来源：http://hz.jlsjyb.cn/gtflaltieu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.fengsongda.top/gteopzyfcv.html

JS:   require.main === module
来源：http://hz.bjfxy.top/gtvwrskizf.html

TS:   require.main === module
来源：http://hz.iojbl.cn/gtbfxvyxeg.html

Java: public static void main(String[] args)
来源：http://hz.fzhhl.top/gtwlzohyuu.html

Go:   func main()
来源：http://hz.hongshengwenyu.top/gtsvxqlwcz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.c1oappe.top/gtkvzigbri.html

C#:   static void Main(string[] args)
来源：http://hz.havefunace.top/gtzfwvheyh.html

[M08] 获取系统与运行时信息
来源：http://hz.gzhubu.top/gtkguyejwr.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhixingplan.top/gtcnwtwsbh.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhaomingkeji.xyz/gtzafspwtr.html

JS:   process.platform;  process.version
来源：http://hz.yonumen.top/gtkbqlnlpr.html

TS:   process.platform;  process.version
来源：http://hz.nwbrower.top/gtrfzvaqgr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.iojbl.cn/gtlfgmvkfr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jqgfzy.top/gtxntzlcqh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yangfankeji.com/gthouoibfq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.316326.xyz/gtzohissys.html

================================================================================
来源：http://hz.c1oappe.top/gteiubdxcd.html

N. 数据结构与算法
来源：http://hz.0kj1m.cn/gtbwkzbvif.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtnwrovgpb.html

[N01] 二分查找（有序数组）
来源：http://hz.daria6918.cn/gtdmsigqzs.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hnxiangtu.top/gtgdcutvak.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.dianchejie.cn/gtyxsxofwv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.vqdsnc.cn/gtnrcfgxnf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhiwuduotai.top/gtqqpnplbx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.smart0.xyz/gtfckfkntm.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hfpthk.cn/gtnmfonnds.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jqgfzy.top/gtftvweefe.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.wangdashe.top/gteufogbsd.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yuxming.cn/gtboxlxufi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenlongwang.top/gtspshlecg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.pengpengdd.cyou/gtgavmkqhs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sufxvd.cn/gtknbwyucp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.wangshuangyany.cn/gtqqhljxym.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhaomingkeji.xyz/gtkcgjfhsa.html

Go:   slices.Sort(arr)
来源：http://hz.nanxuanxn.top/gtntzhkujd.html

Ruby: arr.sort
来源：http://hz.jlsjyb.cn/gtwjaltelz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cashguo.top/gttwyqfloz.html

[N03] 快速排序（分治示例）
来源：http://hz.iojbl.cn/gtokpelgir.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.tanke756.top/gtxyxwmawv.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xinyue.icu/gtakraawrp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangshuangyany.cn/gtgtwylbdo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigfzy.top/gthvyukbnf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shanyushiyangkeji.top/gtcjpkjsoc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xinyue.icu/gtiekuvxew.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.9152youxi.cn/gtkvcdrzok.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zdqjudy.top/gtftdpknxk.html

[N04] 斐波那契数列
来源：http://hz.yuanzhike.top/gtwshcnaxn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shanyushiyangkeji.top/gtfodkuvez.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.fengsongda.top/gtmfkzoxzq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ivvv.top/gtnmpjigim.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.kuanghao11.cn/gtidzajrig.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shzxlz.cn/gtpmxfdrmj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yuxming.cn/gtjlyqyvju.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinghuilouyu.cn/gtoyuhixwu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sysykeji.top/gthcdexhwh.html

[N05] 最大公约数
来源：http://hz.xinyue.icu/gtvzgorcka.html

Py:   math.gcd(a, b)
来源：http://hz.9152youxi.cn/gtsbphxrew.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yuxming.cn/gtscwcoizj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.smart0.xyz/gtnmjsjawn.html


<!-- 参考信息 -->