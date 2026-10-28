代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhongyouzk.top/gtkodqmkhd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shangyingyoupin.top/gtdyumouxz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hywenlv.cn/gtvwkotwjt.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yongpay.top/gtnqrzetqx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.mhx1999.top/gtzugsexst.html

[J08] 提取年月日与星期
来源：http://hz.daria6918.cn/gtfqcopxui.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.nanxinkj.top/gtitylhuxq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xinyue.icu/gtdptjojns.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.tian-w.cn/gtrawyxlvw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sysykeji.top/gtcawktdgf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.daria6918.cn/gtmvsuybde.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.tian-w.cn/gtajdqvqas.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cdnleiting.top/gtfsqscgfy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sufxvd.cn/gtgxpgiioz.html

[J09] 时区处理
来源：http://hz.zdqjudy.top/gtvorbdwcf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.bjfxy.top/gtmimntubf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ivvv.top/gtwqhdlxra.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.feifeiyinyue.top/gtixixjrwn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ppjwa.cn/gtdsmncieh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.wangdashe.top/gtclosrmnf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yanxiufei.cn/gtadoguymj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhengqikj.top/gttvvdahey.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.9152youxi.cn/gtflfyhqwk.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinyuanbaomall.cn/gtvcbdkwqy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yuanzhike.top/gtxtkulial.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xylfe.cn/gtqijaazcm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xinyue.icu/gtqkpbsary.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cqqwz.cn/gtztfxtzig.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.9152youxi.cn/gtxtdftptv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yj202588.top/gtlhoapjhh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xinyue.icu/gtvihpfqoq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhixingplan.top/gtwsahuxrb.html

================================================================================
来源：http://hz.cdnleiting.top/gttumihixe.html

K. JSON 与序列化
来源：http://hz.hnxiangtu.top/gtnrltmlof.html

================================================================================
来源：http://hz.ppjwa.cn/gtoohbczyt.html

[K01] 对象转 JSON 字符串
来源：http://hz.svipenyu.cn/gtimgtxiqt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.havefunace.top/gtkxbddiix.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.haohaochexian.top/gturhvxxqr.html

JS:   JSON.stringify(obj)
来源：http://hz.jiagoushi.top/gtwntjdqdv.html

TS:   JSON.stringify(obj)
来源：http://hz.sysykeji.top/gtukypkjhb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yangfankeji.com/gtjpitqpwo.html

Go:   json.Marshal(obj)
来源：http://hz.c1oappe.top/gtopsrvkwq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.316326.xyz/gtbhgigioy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.gotoacloud.top/gtmladwskn.html

[K02] JSON 字符串转对象
来源：http://hz.yj20258.top/gtnbvnocfj.html

Py:   json.loads(s)
来源：http://hz.haohaochexian.top/gttzjiduyv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cucudq.cn/gtwvdidegr.html

JS:   JSON.parse(s)
来源：http://hz.sxryk.cn/gtivxvjzwy.html

TS:   JSON.parse(s)
来源：http://hz.316326.xyz/gtzbudwfaj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zdqjudy.top/gtgayptvre.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.tian-w.cn/gtjxppspwa.html

Ruby: JSON.parse(s)
来源：http://hz.9152youxi.cn/gtbqmcugwz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.tianlin.xyz/gtptibakwv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yueranfly.top/gttwveusfn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shanyushiyangkeji.top/gtonydvdqx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xuetiantiany.cn/gtntxntlpd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shuidangran.top/gtrrinrrqa.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yongpay.top/gtyboaxzwy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yonumen.top/gtndtlznlw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.daria6918.cn/gtaaobadze.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ywan-chungtsiang.top/gtjyfyuosz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.haohaochexian.top/gtostwywhu.html

[K04] 读取 JSON 文件
来源：http://hz.pengpengdd.cyou/gtaswwbbwk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ydjk.org.cn/gtxglxucwq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.c1oappe.top/gtwrsjjjlt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnxiangtu.top/gtqrjmlmsm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhijiandao.cn/gtckroegxj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.redwolf501.top/gtomciltoe.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xylfe.cn/gtpspqtgod.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.chenjidiqi.icu/gteoeohimz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.wangdashe.top/gtvxdbngex.html

[K05] 深拷贝对象
来源：http://hz.zhixingplan.top/gtasevzzxc.html

Py:   copy.deepcopy(obj)
来源：http://hz.yvedp.cn/gtcxiwtiqn.html

PHP:  unserialize(serialize($obj));
来源：http://hz.52xcode.cn/gtctpijvxg.html

JS:   structuredClone(obj)
来源：http://hz.jiagoushi.top/gtlwabhgcx.html

TS:   structuredClone(obj)
来源：http://hz.yj202588.top/gtrmuatbbg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.52xcode.cn/gtbzzhklhx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.0kj1m.cn/gttuponjdh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.redwolf501.top/gtfivmhtam.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.c1oappe.top/gtazisvsuc.html

[K06] 解析 URL 查询串
来源：http://hz.cashguo.top/gtekelvwjl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yueranfly.top/gtikdbxhem.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yj20258888.top/gtxkqcgfki.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.smart0.xyz/gtskuugshj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenzaomai.com/gthxdzjsqk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hysaishi.cn/gtpnuaypbk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jyoumei.cn/gtfmhtzkxv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.mhx1999.top/gtrjwbcfkh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.iojbl.cn/gtcbltleem.html

[K07] 进制转换
来源：http://hz.gzhubu.top/gtuuhzsbec.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xziqi.cn/gtjmsznjue.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tanke756.top/gtwpegomjn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.cheryme.top/gtrbxqrqwj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jyoumei.cn/gtuekbmktq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.haohaochexian.top/gtdvowlkuk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.gaohongyu789.top/gtjdkawlmk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.pycfn.com/gtzfkxhben.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinqigfzy.top/gtwdejlfrr.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ydjk.org.cn/gtforoocnf.html

Py:   pickle.dumps(obj)
来源：http://hz.hnxiangtu.top/gtalkrsssf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jqgfzy.top/gtutkjqdgj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.52xcode.cn/gtrchypcss.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.tanke756.top/gtevharxdo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.bjfxy.top/gtafcyjbbp.html

Go:   encoding/gob
来源：http://hz.yueranfly.top/gtrqmhdcnn.html

Ruby: Marshal.dump(obj)
来源：http://hz.c1oappe.top/gtdfnizmbz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinyuanbaomall.cn/gtpobpyxjf.html

================================================================================
来源：http://hz.0kj1m.cn/gtblgtiohp.html

L. 网络请求
来源：http://hz.xziqi.cn/gtgngmovsa.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtpheuubpe.html

[L01] 发送 GET 请求
来源：http://hz.hongshengwenyu.top/gtmcnyqnqu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xuetiantiany.cn/gtohrssywb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sxryk.cn/gterhwwkas.html

JS:   await fetch(url)
来源：http://hz.yj20258.top/gtpyidgvhl.html

TS:   await fetch(url)
来源：http://hz.jyoumei.cn/gtuedeimvz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.andypj.xyz/gtsxfxidhm.html

Go:   resp, err := http.Get(url)
来源：http://hz.dashuyun.cn/gtskgasxgt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.bjfxy.top/gtwreprbyj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.iojbl.cn/gtqjhutumk.html

[L02] 发送 POST JSON
来源：http://hz.gzhubu.top/gtxcggwbrg.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hysaishi.cn/gtbojijwpz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.haohaochexian.top/gtscmhbmqn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dashuyun.cn/gtdlzohsow.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zdqjudy.top/gtpkunwkzz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhijiandao.cn/gtgmctfmeh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cheryme.top/gtneipzqwy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.fzhhl.top/gtdzezwzgd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinqigfzy.top/gtrgwdikhl.html

[L03] 设置自定义请求头
来源：http://hz.cqqwz.cn/gtqjimvgly.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.sweek.top/gtekitjmdp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yuanzhike.top/gttmewfdce.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj202588.top/gtwfsmpzxk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ivvv.top/gtqqrhpzrg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sxryk.cn/gtxouidxlu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.gzhubu.top/gtlpuuakrn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.vqdsnc.cn/gtxibthiaa.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhengqikj.top/gtiutokjkx.html

[L04] 设置超时
来源：http://hz.aibaodan.cn/gtsvxbsvec.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ivvv.top/gtbvvmzuyd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.redwolf501.top/gtnegppmzj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jlsjyb.cn/gtobpnpusd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fzhhl.top/gtrraneayr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xuetiantiany.cn/gtmuzqtuuw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hnxiangtu.top/gtdepnnxdh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.daria6918.cn/gttxdlvqrl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.daria6918.cn/gtpbjdklej.html

[L05] 上传文件（multipart）
来源：http://hz.wangshuangyany.cn/gthqcqqsqq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xziqi.cn/gtwdufumba.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hnqzz.top/gtxjnpgszo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shangyingyoupin.top/gtatwnztch.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yuxming.cn/gtzbncoyzr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xuanzx.com/gtrcipppnm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.haohaochexian.top/gtyvwtgwvi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ivvv.top/gtmjpykhby.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.havefunace.top/gtgqgugxaj.html

[L06] 解析响应为 JSON
来源：http://hz.xingfuxueyuan.xyz/gtkfefrhuk.html

Py:   resp.json()
来源：http://hz.xziqi.cn/gtcjfnpfay.html

PHP:  json_decode($body, true);
来源：http://hz.gaohongyu789.top/gtdypoghpg.html

JS:   await resp.json()
来源：http://hz.yangfankeji.com/gtsehycbfy.html

TS:   await resp.json()
来源：http://hz.yonumen.top/gtytaexshv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinqigufen.top/gtvgmvytyg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sxryk.cn/gtcojjwxpg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jinghuilouyu.cn/gttmzzccym.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jinghuilouyu.cn/gtxwqdvtaf.html

[L07] 处理 HTTP 状态码
来源：http://hz.daxiang520.top/gtuymagnbh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhijiandao.cn/gtrsfvslrg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.tanke756.top/gtmbbggopj.html

JS:   resp.ok;  resp.status
来源：http://hz.guowangkeji.top/gtaixpisds.html

TS:   resp.ok;  resp.status
来源：http://hz.chenlongwang.top/gtoaevxjke.html

Java: resp.statusCode()
来源：http://hz.jinghuilouyu.cn/gttsqsjmiq.html

Go:   resp.StatusCode
来源：http://hz.ybcxt.top/gtnjaavhha.html

Ruby: resp.code.to_i
来源：http://hz.hnxiangtu.top/gtpdttjwlo.html

C#:   (int)resp.StatusCode
来源：http://hz.feifeiyinyue.top/gtccrtljaf.html

[L08] 并发请求多个地址
来源：http://hz.hfpthk.cn/gtewjpeofj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.pengpengdd.cyou/gtxjqthfjn.html

PHP:  curl_multi_init() 系列
来源：http://hz.guannengcc.top/gtpkjnmuem.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hywenlv.cn/gtsvpshlwn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zdqjudy.top/gtlbyxqhaq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.daria6918.cn/gtcpphjdpg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cqqwz.cn/gtrgqvnkvr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hnxiangtu.top/gthrolcaxr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ydjk.org.cn/gtzpigwpta.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtqgawnmfp.html

M. 命令行 / 进程 / 环境
来源：http://hz.c1oappe.top/gtnabagbbb.html

================================================================================
来源：http://hz.pycfn.com/gtxxgdjqbb.html

[M01] 读取命令行参数
来源：http://hz.iojbl.cn/gtrazzjnnj.html

Py:   sys.argv[1:]
来源：http://hz.guannengcc.top/gtipkahjdh.html

PHP:  $argv;  $argc;
来源：http://hz.zycfv.cn/gtmgzcoqvq.html

JS:   process.argv.slice(2)
来源：http://hz.shangyingyoupin.top/gtqnpblcrd.html

TS:   process.argv.slice(2)
来源：http://hz.aibaodan.cn/gtcxzedoen.html

Java: args 数组（main 方法参数）
来源：http://hz.ppjwa.cn/gtkokwfvdd.html

Go:   os.Args[1:]
来源：http://hz.cucudq.cn/gtzneblkbu.html

Ruby: ARGV
来源：http://hz.zhongyouzk.top/gtpgybljrn.html

C#:   args 数组（Main 方法参数）
来源：http://hz.dashuyun.cn/gtsrmomrig.html

[M02] 读取环境变量
来源：http://hz.haohaochexian.top/gtsbwfbmwb.html

Py:   os.environ.get("HOME")
来源：http://hz.52xcode.cn/gtxmcnearf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yj20258888.top/gtdpdsergp.html

JS:   process.env.HOME
来源：http://hz.fengsongda.top/gtjbdowkxx.html

TS:   process.env.HOME
来源：http://hz.hnxiangtu.top/gtnysmspfi.html

Java: System.getenv("HOME")
来源：http://hz.pycfn.com/gtnwbothxe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xuanzx.com/gtezcultef.html

Ruby: ENV["HOME"]
来源：http://hz.wangdashe.top/gtfcqwtrib.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhaomingkeji.xyz/gtqugepwht.html

[M03] 执行外部命令
来源：http://hz.yangfankeji.com/gtkrdwqdxy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.pycfn.com/gtknictool.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.aibaodan.cn/gtvqirzlwo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shzxlz.cn/gtzbhqzpic.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.svipenyu.cn/gtqipeiadb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.nwbrower.top/gtvxijndoy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.kuanghao11.cn/gtjrtlwsup.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhongyouzk.top/gteaywefdp.html

C#:   Process.Start("ls", "-l");
来源：http://hz.fengsongda.top/gtovkriujf.html

[M04] 获取当前工作目录
来源：http://hz.sweek.top/gtkpuwszvt.html

Py:   os.getcwd()
来源：http://hz.cucudq.cn/gtmgwsirle.html

PHP:  getcwd();
来源：http://hz.tianlin.xyz/gtoqbudozp.html

JS:   process.cwd()
来源：http://hz.zhaomingkeji.xyz/gtvpepdrmm.html

TS:   process.cwd()
来源：http://hz.redwolf501.top/gtwycckkto.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jiagoushi.top/gttplmvazs.html

Go:   os.Getwd()
来源：http://hz.iojbl.cn/gteqqniuqj.html

Ruby: Dir.pwd
来源：http://hz.9152youxi.cn/gtknrqlbtu.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.aizwys.cn/gtoydxyfnb.html

[M05] 设置退出码
来源：http://hz.wangshuangyany.cn/gtcvvweewh.html

Py:   sys.exit(1)
来源：http://hz.shzxlz.cn/gtaawuwysr.html

PHP:  exit(1);
来源：http://hz.jianghu66.top/gtrozbxhoq.html

JS:   process.exit(1)
来源：http://hz.sxryk.cn/gtyozglkvs.html

TS:   process.exit(1)
来源：http://hz.quarkkingdee.top/gtdbmbleze.html

Java: System.exit(1)
来源：http://hz.shanyushiyangtech.top/gtyndifcpk.html

Go:   os.Exit(1)
来源：http://hz.yangfankeji.com/gtaposgqtp.html

Ruby: exit 1
来源：http://hz.daxiang520.top/gtoyyhosoj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nanxinkj.top/gtazjcbbfm.html

[M06] 向标准错误输出
来源：http://hz.ydzc1.top/gtuiqmzpjk.html

Py:   print("err", file=sys.stderr)
来源：http://hz.svipenyu.cn/gtbcsdjpjy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhiwuduotai.top/gtimcetfxe.html

JS:   console.error("err")
来源：http://hz.shuidangran.top/gteiwzafpa.html

TS:   console.error("err")
来源：http://hz.jqgfzy.top/gtltbadyyg.html

Java: System.err.println("err")
来源：http://hz.aizwys.cn/gtviolczbg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.feifeiyinyue.top/gtkwlytfjw.html

Ruby: warn "err"
来源：http://hz.shanyushiyangkeji.top/gttnbhpqbz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shangyingyoupin.top/gtqhbobqgw.html

[M07] 判断是否为主入口
来源：http://hz.yuxming.cn/gtcvbcnknw.html

Py:   if __name__ == "__main__":
来源：http://hz.shanyushiyangkeji.top/gtoyktkjsf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.svipenyu.cn/gtxvpprjcj.html

JS:   require.main === module
来源：http://hz.yvedp.cn/gtavivxavd.html

TS:   require.main === module
来源：http://hz.birdmap.top/gtiiebhxwa.html

Java: public static void main(String[] args)
来源：http://hz.jianghu66.top/gtgeqpomxq.html

Go:   func main()
来源：http://hz.0kj1m.cn/gtbddsavgu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.gaohongyu789.top/gtrcgggeui.html

C#:   static void Main(string[] args)
来源：http://hz.sweek.top/gttzyrtxif.html

[M08] 获取系统与运行时信息
来源：http://hz.jqgfzy.top/gthqnmurrf.html

Py:   platform.system();  platform.python_version()
来源：http://hz.0kj1m.cn/gtfillnptc.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.smart0.xyz/gtchbmlkrm.html

JS:   process.platform;  process.version
来源：http://hz.xingfuxueyuan.xyz/gtscunmmlu.html

TS:   process.platform;  process.version
来源：http://hz.cucudq.cn/gteypkeqqy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.nanxinkj.top/gtpzoyomxm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinyuanbaomall.cn/gtzdbuduke.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jqgfzy.top/gtlokgggwq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.dianchejie.cn/gtaeutbsxk.html

================================================================================
来源：http://hz.zhijiandao.cn/gtqgtugcqf.html

N. 数据结构与算法
来源：http://hz.fengsongda.top/gtpmxvfxug.html

================================================================================
来源：http://hz.ppjwa.cn/gtdwfytlvh.html

[N01] 二分查找（有序数组）
来源：http://hz.aibaodan.cn/gtitxhybib.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sysykeji.top/gtttqhgdkl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yuxming.cn/gtwqxhckhw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cheryme.top/gtwnezpfvk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jqgfzy.top/gtrlqmvqsc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.sweek.top/gtsqhsyudo.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cqqwz.cn/gtkjemqhly.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhiwuduotai.top/gtwpauncir.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.meibo888.top/gtzcbssaiz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hfpthk.cn/gtqjvxybpe.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sufxvd.cn/gtvviudree.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.havefunace.top/gtzlqvhnln.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hysaishi.cn/gtxgnkpaox.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.smart0.xyz/gtpeewmzoy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.svipenyu.cn/gtswzjboej.html

Go:   slices.Sort(arr)
来源：http://hz.xinyue.icu/gtmovicyxr.html

Ruby: arr.sort
来源：http://hz.yj20258.top/gtvwkwfkxr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hongshengwenyu.top/gtpqvxvcvy.html

[N03] 快速排序（分治示例）
来源：http://hz.jyoumei.cn/gtrcdtuhba.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jqgufenzy.top/gtjohwhrmf.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhixingplan.top/gtnimshndz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.vqdsnc.cn/gtzltpgdiy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.52xcode.cn/gtjvjbwnjp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.pengpengdd.cyou/gtawzgehiy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.gotoacloud.top/gtkygauxvl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.fzhhl.top/gtdjigtdpd.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shanyushiyangkeji.top/gtbhfpjrlx.html

[N04] 斐波那契数列
来源：http://hz.sweek.top/gtwnbxasyp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jianghu66.top/gtqdzwknna.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.wangdashe.top/gtuuxsrtbz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.mhx1999.top/gtiebcuqup.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ehwqpu.com/gttulruqgg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cashguo.top/gtoarxsplb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.9152youxi.cn/gtffxhpdsb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.vqdsnc.cn/gtacptfkvq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.guowangkeji.top/gtlxytokwu.html

[N05] 最大公约数
来源：http://hz.nwbrower.top/gtkpjdozvl.html

Py:   math.gcd(a, b)
来源：http://hz.kuanghao11.cn/gtxijpgaoq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xuanzx.com/gtbpimwijw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yvedp.cn/gtonzholib.html


<!-- 参考信息 -->