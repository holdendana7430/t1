代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinghuilouyu.cn/gteebkupiu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.pycfn.com/gtbippvqgm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yonumen.top/gtgvmcvrhq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.svipenyu.cn/gtxltobinc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.aibaodan.cn/gtrxazjafm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sufxvd.cn/gtvopqhnsl.html

[J09] 时区处理
来源：http://hz.jqgufenzy.top/gtiikulspi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shuidangran.top/gtxpbllttc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xingfuxueyuan.xyz/gtaocweqcl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.andypj.xyz/gtasbwlxhr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.andypj.xyz/gthxzjjqoz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yangfankeji.com/gtkhhogjgs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.nwbrower.top/gtxabomxmq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gogol.net.cn/gtrdagvczy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinqigufen.top/gtcgychejb.html

[J10] 取今天 / 本月第一天
来源：http://hz.redwolf501.top/gtzcrnjfme.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.chenzaomai.com/gtytcgdbfk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jyoumei.cn/gtnyceveoj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.vqdsnc.cn/gtjopszkge.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.bjfxy.top/gtprjozfve.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.guannengcc.top/gtsbsjxawk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xylfe.cn/gtrqprciqp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cdnleiting.top/gtgfhnrxta.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shangyingyoupin.top/gtzztdqwky.html

================================================================================
来源：http://hz.zhijiandao.cn/gtqkumbiax.html

K. JSON 与序列化
来源：http://hz.sxryk.cn/gtcsntqjxy.html

================================================================================
来源：http://hz.ydzc1.top/gtevoyznaz.html

[K01] 对象转 JSON 字符串
来源：http://hz.hongshengwenyu.top/gtlklyvpej.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.quarkkingdee.top/gthxraxlbr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.guannengcc.top/gtronqifbd.html

JS:   JSON.stringify(obj)
来源：http://hz.yvedp.cn/gtujqvzpvk.html

TS:   JSON.stringify(obj)
来源：http://hz.svipenyu.cn/gtgsenuzly.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.daria6918.cn/gtebucnknc.html

Go:   json.Marshal(obj)
来源：http://hz.yvedp.cn/gtlygzpntd.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.c1oappe.top/gtfksfemlt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.gotoacloud.top/gthrftmzai.html

[K02] JSON 字符串转对象
来源：http://hz.snrcjt.cn/gtbgtuiiob.html

Py:   json.loads(s)
来源：http://hz.chenjidiqi.icu/gtxcoysixe.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yonumen.top/gtpxrtzxtm.html

JS:   JSON.parse(s)
来源：http://hz.snrcjt.cn/gtqrulprnw.html

TS:   JSON.parse(s)
来源：http://hz.zdqjudy.top/gtwbsabazz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.feifeiyinyue.top/gtvsfursdo.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hywenlv.cn/gtzpfwldee.html

Ruby: JSON.parse(s)
来源：http://hz.birdmap.top/gtupfbiykp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yongpay.top/gtxgbpknbl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jyoumei.cn/gtdscrneei.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shangyingyoupin.top/gtoeiikgch.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhongyouzk.top/gthhonaojd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.tian-w.cn/gtavhvbswv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.birdmap.top/gtmofufkfu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cheryme.top/gteagtudbv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cheryme.top/gtnzogvbdr.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jinqigfzy.top/gtcmwaobqv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.sufxvd.cn/gtxswkexvl.html

[K04] 读取 JSON 文件
来源：http://hz.zhiwuduotai.top/gtzkemkail.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shuidangran.top/gtrbekqpas.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhoulong.xyz/gtpscpifmt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinghuilouyu.cn/gtbrtqxzwh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhongyouzk.top/gtmjgjhtab.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xziqi.cn/gtlesdjwob.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhiwuduotai.top/gttoxlzaka.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.birdmap.top/gtogroifct.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hysaishi.cn/gtjwtukvui.html

[K05] 深拷贝对象
来源：http://hz.316326.xyz/gtlnpgotmj.html

Py:   copy.deepcopy(obj)
来源：http://hz.sweek.top/gtarnkiyaw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yangfankeji.com/gtnupjsbft.html

JS:   structuredClone(obj)
来源：http://hz.xuanzx.com/gtmcdyclrs.html

TS:   structuredClone(obj)
来源：http://hz.meibo888.top/gtihwidzrs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jyoumei.cn/gtksfklkgu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hongshengwenyu.top/gteapohaqr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cqqwz.cn/gtwtnyflck.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hammf.cn/gtwevntmap.html

[K06] 解析 URL 查询串
来源：http://hz.shuidangran.top/gtxyawcafz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shangyingyoupin.top/gteiufvwig.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.chenjidiqi.icu/gtvgzcbflz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.andypj.xyz/gtajtbjlvx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hywenlv.cn/gtrypkomuh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.guowangkeji.top/gtyasuzqfb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhiwuduotai.top/gtispetdvw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.havefunace.top/gtnlbjysvb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.tanke756.top/gtexahapzi.html

[K07] 进制转换
来源：http://hz.hywenlv.cn/gthvpxrklw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gtljyppbqn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hnqzz.top/gtepzmdnrh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.chenzaomai.com/gtthafiozf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gaohongyu789.top/gttltgjrwb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhixingplan.top/gtqrlnejsz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hywenlv.cn/gtefxicahq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ybcxt.top/gtnupzqstb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hysaishi.cn/gtmiwgqwmt.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.chenzaomai.com/gtmskydlew.html

Py:   pickle.dumps(obj)
来源：http://hz.tian-w.cn/gtzhrnkhmo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yueranfly.top/gtgxgfclbr.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangtech.top/gttxjmsclx.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ehwqpu.com/gtrymsbdyt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.316326.xyz/gtxqlgrpmi.html

Go:   encoding/gob
来源：http://hz.sweek.top/gtjimdbzex.html

Ruby: Marshal.dump(obj)
来源：http://hz.hongshengwenyu.top/gtviaimhht.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yj20258.top/gtmxcojsav.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtbpuwnihq.html

L. 网络请求
来源：http://hz.bjfxy.top/gtujhbwfpm.html

================================================================================
来源：http://hz.svipenyu.cn/gtmebvjnda.html

[L01] 发送 GET 请求
来源：http://hz.bjfxy.top/gtvopeioyo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hnxiangtu.top/gtlzcatcqg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cheryme.top/gteyjqqrjs.html

JS:   await fetch(url)
来源：http://hz.vqdsnc.cn/gtfjqymesi.html

TS:   await fetch(url)
来源：http://hz.chenzaomai.com/gtocncglmg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.svipenyu.cn/gtlykljkka.html

Go:   resp, err := http.Get(url)
来源：http://hz.fzhhl.top/gtfsitjzhf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cdnleiting.top/gtwfzxgkaq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhiwuduotai.top/gtrtwsmktl.html

[L02] 发送 POST JSON
来源：http://hz.yj202588.top/gtilwehppe.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.316326.xyz/gtgdawummr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.nanxuanxn.top/gtmqmzhuok.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuanzx.com/gthpnoperb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cqqwz.cn/gtxdeldzqy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shanyushiyangtech.top/gtvpzhqzsw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.daxiang520.top/gtdvvedjqy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.nanxinkj.top/gtzvzadgai.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yj20258888.top/gtzfhppgyr.html

[L03] 设置自定义请求头
来源：http://hz.cheryme.top/gtohqfnlzk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.sufxvd.cn/gtudfbipyh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jinqigfzy.top/gtbgkgaebm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.feifeiyinyue.top/gttluatlcn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj20258.top/gtzydldfod.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.havefunace.top/gtksfrzldq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zycfv.cn/gtfapfpsso.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shuidangran.top/gtkjcdtjvv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.sufxvd.cn/gtsuuxiasd.html

[L04] 设置超时
来源：http://hz.ydzc1.top/gtsmenpbud.html

Py:   requests.get(url, timeout=5)
来源：http://hz.birdmap.top/gtqjiakkeq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ybcxt.top/gtsjdhstoh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.316326.xyz/gtpymitsjl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dianchejie.cn/gtzedbmqms.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.fengsongda.top/gtfgsjvaqk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xuanzx.com/gtiepqsdru.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xingfuxueyuan.xyz/gtxvmvjojh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xuetiantiany.cn/gtfheenrvu.html

[L05] 上传文件（multipart）
来源：http://hz.jinqigufen.top/gtidepbncb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yvedp.cn/gticmzkija.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jinqigufen.top/gthvbqgfzp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhixingplan.top/gtfxtvddtt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xziqi.cn/gtrdjxfbux.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xinyue.icu/gtnkwwhycu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.fengsongda.top/gtkbwzbuwr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yj20258888.top/gtnzgnlzww.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.dianchejie.cn/gtmdtwwnpj.html

[L06] 解析响应为 JSON
来源：http://hz.tanke756.top/gtphzbnqos.html

Py:   resp.json()
来源：http://hz.316326.xyz/gttvquldxt.html

PHP:  json_decode($body, true);
来源：http://hz.tian-w.cn/gtujqstnbk.html

JS:   await resp.json()
来源：http://hz.yvedp.cn/gtgfmfadww.html

TS:   await resp.json()
来源：http://hz.gzhubu.top/gtdreioqay.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.52xcode.cn/gtgplpklkd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.c1oappe.top/gtywfxzlcc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.svipenyu.cn/gtlwrhyruy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.chenlongwang.top/gtdcyciqnr.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhiwuduotai.top/gtphioeipj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yonumen.top/gtcjpcjmzz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sxryk.cn/gtnieywfmx.html

JS:   resp.ok;  resp.status
来源：http://hz.jiagoushi.top/gtqlgiozty.html

TS:   resp.ok;  resp.status
来源：http://hz.zhiwuduotai.top/gtytglocjl.html

Java: resp.statusCode()
来源：http://hz.ehwqpu.com/gtegyqmvgp.html

Go:   resp.StatusCode
来源：http://hz.smart0.xyz/gtxdoymbyq.html

Ruby: resp.code.to_i
来源：http://hz.yongpay.top/gtgskakgfq.html

C#:   (int)resp.StatusCode
来源：http://hz.nanxinkj.top/gtxtlptzux.html

[L08] 并发请求多个地址
来源：http://hz.hywenlv.cn/gtmecsffkc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xziqi.cn/gtvdnwmhwj.html

PHP:  curl_multi_init() 系列
来源：http://hz.mhx1999.top/gteqcdsncl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jiagoushi.top/gtuslhewhk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangtech.top/gtnohqnmin.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shangyingyoupin.top/gtpppdhuzv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yj20258.top/gtcydemwvi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cashguo.top/gtactrxnag.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.meibo888.top/gtpzrbjybg.html

================================================================================
来源：http://hz.snrcjt.cn/gtqmllvmyb.html

M. 命令行 / 进程 / 环境
来源：http://hz.gogol.net.cn/gtktgujbsv.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtikomsewu.html

[M01] 读取命令行参数
来源：http://hz.gotoacloud.top/gthlkzbowk.html

Py:   sys.argv[1:]
来源：http://hz.wangdashe.top/gtsxspyquj.html

PHP:  $argv;  $argc;
来源：http://hz.meibo888.top/gttlhsxekj.html

JS:   process.argv.slice(2)
来源：http://hz.fzhhl.top/gtixkspfsp.html

TS:   process.argv.slice(2)
来源：http://hz.xuetiantiany.cn/gtqgpqstoh.html

Java: args 数组（main 方法参数）
来源：http://hz.birdmap.top/gthbfxkhyh.html

Go:   os.Args[1:]
来源：http://hz.mhx1999.top/gttgvvfcfe.html

Ruby: ARGV
来源：http://hz.c1oappe.top/gtzxhrjyqc.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhixingplan.top/gtortscisl.html

[M02] 读取环境变量
来源：http://hz.haohaochexian.top/gtuvdkuotm.html

Py:   os.environ.get("HOME")
来源：http://hz.fengsongda.top/gtfttobljh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhixingplan.top/gtrvxxhmsz.html

JS:   process.env.HOME
来源：http://hz.cdnleiting.top/gtgdakfxub.html

TS:   process.env.HOME
来源：http://hz.zycfv.cn/gtntfvahpj.html

Java: System.getenv("HOME")
来源：http://hz.gaohongyu789.top/gtmqelhcpt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yangfankeji.com/gtfmenedlt.html

Ruby: ENV["HOME"]
来源：http://hz.yvedp.cn/gtqpgicvhs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jlsjyb.cn/gtkiozmgeo.html

[M03] 执行外部命令
来源：http://hz.shzxlz.cn/gtklongbsi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shanyushiyangkeji.top/gtlaynkqdg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hnqzz.top/gtkqbiplgu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydjk.org.cn/gtkfqyzlcq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydzc1.top/gtllhogmme.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xuetiantiany.cn/gthnadnwhr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.daria6918.cn/gtbfhcfbgg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.nwbrower.top/gtycbzceyl.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hammf.cn/gtqtkgmisb.html

[M04] 获取当前工作目录
来源：http://hz.chenlongwang.top/gtcjngirik.html

Py:   os.getcwd()
来源：http://hz.jinghuilouyu.cn/gtyfkoidfw.html

PHP:  getcwd();
来源：http://hz.zhijiandao.cn/gtkhyiessu.html

JS:   process.cwd()
来源：http://hz.pycfn.com/gtsqyjtahq.html

TS:   process.cwd()
来源：http://hz.iojbl.cn/gtdsocpfhd.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hfpthk.cn/gtvlknzgpy.html

Go:   os.Getwd()
来源：http://hz.xziqi.cn/gtnzarukqv.html

Ruby: Dir.pwd
来源：http://hz.jiagoushi.top/gteusvinus.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hnxiangtu.top/gtvsahcttj.html

[M05] 设置退出码
来源：http://hz.aizwys.cn/gtkqfiktwf.html

Py:   sys.exit(1)
来源：http://hz.snrcjt.cn/gtjckrqtou.html

PHP:  exit(1);
来源：http://hz.jiagoushi.top/gtwujfugkr.html

JS:   process.exit(1)
来源：http://hz.kuanghao11.cn/gtwnnwqkyb.html

TS:   process.exit(1)
来源：http://hz.havefunace.top/gtzschpots.html

Java: System.exit(1)
来源：http://hz.hnxiangtu.top/gtjsqfddtq.html

Go:   os.Exit(1)
来源：http://hz.dianchejie.cn/gthpswyqtd.html

Ruby: exit 1
来源：http://hz.vqdsnc.cn/gttctqyhsj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.svipenyu.cn/gtfqwskefu.html

[M06] 向标准错误输出
来源：http://hz.dianchejie.cn/gtnbeifvkn.html

Py:   print("err", file=sys.stderr)
来源：http://hz.havefunace.top/gtcovlbhqo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hammf.cn/gtnvtoifnv.html

JS:   console.error("err")
来源：http://hz.nanxuanxn.top/gtetsvbuhi.html

TS:   console.error("err")
来源：http://hz.shzxlz.cn/gtthtxuofh.html

Java: System.err.println("err")
来源：http://hz.zhengqikj.top/gtlaxcfmdn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hfpthk.cn/gtuvupuobb.html

Ruby: warn "err"
来源：http://hz.cashguo.top/gtwznhsxqs.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhoulong.xyz/gtvbgtqtop.html

[M07] 判断是否为主入口
来源：http://hz.yongpay.top/gtrngsyodh.html

Py:   if __name__ == "__main__":
来源：http://hz.xuetiantiany.cn/gtqjllvhao.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.guannengcc.top/gtbxlfnddd.html

JS:   require.main === module
来源：http://hz.hammf.cn/gtlfuzyboa.html

TS:   require.main === module
来源：http://hz.smart0.xyz/gttmwkfhkv.html

Java: public static void main(String[] args)
来源：http://hz.yuxming.cn/gtipogiulv.html

Go:   func main()
来源：http://hz.shanyushiyangkeji.top/gtmvsifjmf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jlsjyb.cn/gtqszsskzk.html

C#:   static void Main(string[] args)
来源：http://hz.fzhhl.top/gtyhganurm.html

[M08] 获取系统与运行时信息
来源：http://hz.havefunace.top/gtalaxzmhj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinghuilouyu.cn/gtwygiaptr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yongpay.top/gtjpvpbkot.html

JS:   process.platform;  process.version
来源：http://hz.zhoulong.xyz/gtbotbdsub.html

TS:   process.platform;  process.version
来源：http://hz.cashguo.top/gtitdwtdvh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shanyushiyangkeji.top/gtnrvnylzz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.aizwys.cn/gttflfgrrh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jqgufenzy.top/gtnlpeketa.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xingfuxueyuan.xyz/gtrpfnesvr.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtqdnffsdt.html

N. 数据结构与算法
来源：http://hz.tianlin.xyz/gtrqzpclnd.html

================================================================================
来源：http://hz.yueranfly.top/gtvjgwztcl.html

[N01] 二分查找（有序数组）
来源：http://hz.zycfv.cn/gtfztdimte.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.fengsongda.top/gteqqaijgj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.c1oappe.top/gtekxklrhc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangshuangyany.cn/gtcdbihgld.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xinyue.icu/gtsarqwtjd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.chenjidiqi.icu/gtycxfkhmg.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xziqi.cn/gtqqniuqrb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yonumen.top/gtzjcflehl.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.tanke756.top/gtlgluqvme.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.316326.xyz/gtybkevxqo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hongshengwenyu.top/gtxkykchgf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tianlin.xyz/gtlcvncxoz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenjidiqi.icu/gtrxsgyzxy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.dashuyun.cn/gtrewcjuak.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yj20258888.top/gtjwepmzfk.html

Go:   slices.Sort(arr)
来源：http://hz.zdqjudy.top/gtyslkmypx.html

Ruby: arr.sort
来源：http://hz.zhengqikj.top/gtbqcqptcr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.feifeiyinyue.top/gtgrdxnhbo.html

[N03] 快速排序（分治示例）
来源：http://hz.meibo888.top/gtegwpltyq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhaomingkeji.xyz/gtfzthhmoo.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tanke756.top/gtjvrljmnk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinyuanbaomall.cn/gtevldxfcu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ppjwa.cn/gteoeybjdg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.chenjidiqi.icu/gtajquqdvq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cqqwz.cn/gtgrskrnls.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ybcxt.top/gttzagdrpu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.smart0.xyz/gtfszsovgz.html

[N04] 斐波那契数列
来源：http://hz.zdqjudy.top/gtdwphtadg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.guowangkeji.top/gtjvhlnwqp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yuanzhike.top/gtovblfcge.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.52xcode.cn/gtanruyobr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigufen.top/gtczqnkccf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.tanke756.top/gtassqxayb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.haohaochexian.top/gtuspiebve.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.vqdsnc.cn/gtzrvvzoxb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.tian-w.cn/gtdsnsrbzx.html

[N05] 最大公约数
来源：http://hz.feifeiyinyue.top/gtoesejkag.html

Py:   math.gcd(a, b)
来源：http://hz.zhaomingkeji.xyz/gtfuxqnymv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yj202588.top/gtmqdhraem.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jianghu66.top/gtkwwfsbwy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yueranfly.top/gtisllxpeh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.nwbrower.top/gtnhmdzpvo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ppjwa.cn/gthfegplxl.html

Ruby: a.gcd(b)
来源：http://hz.wangdashe.top/gtycxsbrre.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.iojbl.cn/gtjcryldxc.html

[N06] 判断回文字符串
来源：http://hz.0kj1m.cn/gtszmnvlfu.html

Py:   s == s[::-1]
来源：http://hz.jyoumei.cn/gtdvykzebi.html

PHP:  $s === strrev($s);
来源：http://hz.shanyushiyangtech.top/gtljscoaon.html


<!-- 参考信息 -->