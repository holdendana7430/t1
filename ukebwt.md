代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cqqwz.cn/gtowbwpzxt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ydjk.org.cn/gtdieepirc.html

[J09] 时区处理
来源：http://hz.ywan-chungtsiang.top/gtlvutubee.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xylfe.cn/gtfpvhpwte.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yanxiufei.cn/gtxwmtfcqq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigufen.top/gtnhcamvwm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ybcxt.top/gtoefmnanb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.havefunace.top/gtgwaeupdw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jyoumei.cn/gtvvpfbzmi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yonumen.top/gtuqmteuqy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.fengsongda.top/gtkgqnbuqg.html

[J10] 取今天 / 本月第一天
来源：http://hz.quarkkingdee.top/gtoqhgknem.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.fzhhl.top/gteupsxzff.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ydzc1.top/gtqhsazpim.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jinyuanbaomall.cn/gtvtgbgfmf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cdnleiting.top/gtkewoygal.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.9152youxi.cn/gtvspjbbqw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cucudq.cn/gtgafistzt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinqigufen.top/gtroeeulji.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cashguo.top/gtzgdylaom.html

================================================================================
来源：http://hz.316326.xyz/gtdmoonxvw.html

K. JSON 与序列化
来源：http://hz.jinyuanbaomall.cn/gtysizgeoy.html

================================================================================
来源：http://hz.ydzc1.top/gtzcnrzvdu.html

[K01] 对象转 JSON 字符串
来源：http://hz.ydzc1.top/gtmfdgvzrh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.aizwys.cn/gthcycgopy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.dianchejie.cn/gtopaxmfdq.html

JS:   JSON.stringify(obj)
来源：http://hz.daria6918.cn/gtwgnsdqeh.html

TS:   JSON.stringify(obj)
来源：http://hz.aibaodan.cn/gtozexsryb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hongshengwenyu.top/gtcsmiwrck.html

Go:   json.Marshal(obj)
来源：http://hz.svipenyu.cn/gtxutwaveu.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hammf.cn/gtehrirgbz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hnxiangtu.top/gteuhdtndh.html

[K02] JSON 字符串转对象
来源：http://hz.yuxming.cn/gtajlvkwzf.html

Py:   json.loads(s)
来源：http://hz.tian-w.cn/gtxryvpwum.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gogol.net.cn/gtgdzckhba.html

JS:   JSON.parse(s)
来源：http://hz.cqqwz.cn/gtsjkzjbqy.html

TS:   JSON.parse(s)
来源：http://hz.tanke756.top/gtavmmclcb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhongyouzk.top/gthcecbmyp.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.fzhhl.top/gththuetmq.html

Ruby: JSON.parse(s)
来源：http://hz.haohaochexian.top/gtmtcyggot.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hnxiangtu.top/gtykwtpzxr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ybcxt.top/gtoceyirww.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.52xcode.cn/gtojwfmsfx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhiwuduotai.top/gtonsirkpa.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.daxiang520.top/gtrcairaol.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenzaomai.com/gtsewtvfcx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dashuyun.cn/gtopptcbnn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.tianlin.xyz/gtvigbtfda.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jianghu66.top/gtrnkatcbc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gaohongyu789.top/gtseaftyor.html

[K04] 读取 JSON 文件
来源：http://hz.tanke756.top/gtrxxkzzqk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ydzc1.top/gtsvrwmosk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.daxiang520.top/gtvqdfmtia.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ppjwa.cn/gtkjtqtlfr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guowangkeji.top/gtplzttggf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.nwbrower.top/gtodcihflg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yuanzhike.top/gtyvwghzno.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gzhubu.top/gteapcpmsg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.fengsongda.top/gtxqluquib.html

[K05] 深拷贝对象
来源：http://hz.haohaochexian.top/gtyuvvofkk.html

Py:   copy.deepcopy(obj)
来源：http://hz.tian-w.cn/gtgmrbqwkz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jiagoushi.top/gtnynbzfaw.html

JS:   structuredClone(obj)
来源：http://hz.sxryk.cn/gtodzniwra.html

TS:   structuredClone(obj)
来源：http://hz.zhijiandao.cn/gtypidrket.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hywenlv.cn/gtgztcqtdy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shanyushiyangkeji.top/gtzvkaxchk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yuxming.cn/gtevaoggxh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.52xcode.cn/gtmgfzubmx.html

[K06] 解析 URL 查询串
来源：http://hz.daria6918.cn/gtdlpytvti.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.havefunace.top/gtfhbbnhxt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shzxlz.cn/gtguihaxth.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zycfv.cn/gttuuvaamd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yvedp.cn/gtwedrtqlr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.nanxinkj.top/gtyvvrfzsd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jlsjyb.cn/gtaepxtfnm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gtvpdrqzqt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gtfejwxrtr.html

[K07] 进制转换
来源：http://hz.zhijiandao.cn/gtmraatbib.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yj20258888.top/gtvqqarcmj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.haohaochexian.top/gtkzaaafrx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtlsleovvo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ydjk.org.cn/gtrtxuxykc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.guowangkeji.top/gtrsyuvesi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinyuanbaomall.cn/gtzzspbyiz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nanxuanxn.top/gtyyovkjza.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ehwqpu.com/gtrevhoywz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.aizwys.cn/gtehkjqxzl.html

Py:   pickle.dumps(obj)
来源：http://hz.quarkkingdee.top/gtdgqxivad.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.wangdashe.top/gtneuytzoh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.andypj.xyz/gtcuufzhbi.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.svipenyu.cn/gtppxxlwzy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.gogol.net.cn/gtgsjhrsaf.html

Go:   encoding/gob
来源：http://hz.sxryk.cn/gtgbnjmqlj.html

Ruby: Marshal.dump(obj)
来源：http://hz.yueranfly.top/gtfpgsthfe.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ppjwa.cn/gtroogcvfx.html

================================================================================
来源：http://hz.shzxlz.cn/gtdricahbt.html

L. 网络请求
来源：http://hz.fengsongda.top/gtftdludiv.html

================================================================================
来源：http://hz.tian-w.cn/gtnpsycmgi.html

[L01] 发送 GET 请求
来源：http://hz.zhaomingkeji.xyz/gtwkvmrtju.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jqgfzy.top/gthobhcnbv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jqgufenzy.top/gtxcxhrpko.html

JS:   await fetch(url)
来源：http://hz.zhijiandao.cn/gtikzlvjhe.html

TS:   await fetch(url)
来源：http://hz.wangdashe.top/gtlqnyvnap.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.nanxinkj.top/gtrusbhgtn.html

Go:   resp, err := http.Get(url)
来源：http://hz.cdnleiting.top/gtxozivvqn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.dianchejie.cn/gtgbfzqcqo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jlsjyb.cn/gthsjgradi.html

[L02] 发送 POST JSON
来源：http://hz.shangyingyoupin.top/gtoghkakqi.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jinqigfzy.top/gtnyvlwxcq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hnqzz.top/gtcewwhdpv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.meibo888.top/gtsddymwsq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.vqdsnc.cn/gtqbtymqva.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhixingplan.top/gtwpcyhvqr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.nanxinkj.top/gtrqgznvrb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hnqzz.top/gtyoxmeceg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.iojbl.cn/gtnezgbauz.html

[L03] 设置自定义请求头
来源：http://hz.jqgufenzy.top/gtvqaohlfg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.haohaochexian.top/gtvbysppdh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xinyue.icu/gtxvgkwbaj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hnxiangtu.top/gttpvchfzk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinqigufen.top/gtzxhbwodw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hnqzz.top/gtekzfqqhx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xuetiantiany.cn/gtdxjzzrvm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yj20258888.top/gtuoaicewb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hywenlv.cn/gtcbbegogj.html

[L04] 设置超时
来源：http://hz.ppjwa.cn/gtdjddzedj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.dianchejie.cn/gtgicipfsh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.andypj.xyz/gtjjqxcpfe.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhongyouzk.top/gtizuupnyk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nanxuanxn.top/gtgqnlwfnc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.fengsongda.top/gtjllvrvuw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hammf.cn/gtolmycsit.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhaomingkeji.xyz/gtzxaimqut.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.bjfxy.top/gtnvodteon.html

[L05] 上传文件（multipart）
来源：http://hz.guowangkeji.top/gtxxbdrlcn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinqigufen.top/gtbjvztkof.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zycfv.cn/gtiqfzberd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jlsjyb.cn/gtzygyvhgm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jyoumei.cn/gtcxbepvof.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yuxming.cn/gtixdezglc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shanyushiyangtech.top/gtalmhzvqp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.chenzaomai.com/gtvjqjkvbs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.0kj1m.cn/gtcmipxtik.html

[L06] 解析响应为 JSON
来源：http://hz.hysaishi.cn/gtduxywxad.html

Py:   resp.json()
来源：http://hz.nanxuanxn.top/gtgocgehzm.html

PHP:  json_decode($body, true);
来源：http://hz.andypj.xyz/gtdqizbnnf.html

JS:   await resp.json()
来源：http://hz.sweek.top/gtoojhkxwz.html

TS:   await resp.json()
来源：http://hz.aizwys.cn/gtcuosphtj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yangfankeji.com/gtqvvnkwgm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.wangshuangyany.cn/gtdauzplqv.html

Ruby: JSON.parse(resp.body)
来源：http://hz.dianchejie.cn/gtpcxgpmob.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhongyouzk.top/gtlcrspbfo.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinqigufen.top/gtqjptnzsx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zdqjudy.top/gtqnnctogn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.vqdsnc.cn/gtypfveuey.html

JS:   resp.ok;  resp.status
来源：http://hz.nanxinkj.top/gtcltwlgec.html

TS:   resp.ok;  resp.status
来源：http://hz.hysaishi.cn/gtfedxlhyi.html

Java: resp.statusCode()
来源：http://hz.zhiwuduotai.top/gtffgpywlw.html

Go:   resp.StatusCode
来源：http://hz.zhaomingkeji.xyz/gtfltnyess.html

Ruby: resp.code.to_i
来源：http://hz.xziqi.cn/gtwpjuztkc.html

C#:   (int)resp.StatusCode
来源：http://hz.yongpay.top/gteyncwprv.html

[L08] 并发请求多个地址
来源：http://hz.aibaodan.cn/gtrfwpggkv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.c1oappe.top/gtvsupzcfh.html

PHP:  curl_multi_init() 系列
来源：http://hz.guowangkeji.top/gtctfdjjyu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gogol.net.cn/gtisnhhjkr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dashuyun.cn/gtgleejznc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yonumen.top/gtozoulhdv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.0kj1m.cn/gtcbhtbdbi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ywan-chungtsiang.top/gtkrpnubdp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hongshengwenyu.top/gtmcjngqxh.html

================================================================================
来源：http://hz.nanxuanxn.top/gtsyswryon.html

M. 命令行 / 进程 / 环境
来源：http://hz.vqdsnc.cn/gtgitcspew.html

================================================================================
来源：http://hz.jyoumei.cn/gtdbtpcgok.html

[M01] 读取命令行参数
来源：http://hz.sweek.top/gtjwettfmu.html

Py:   sys.argv[1:]
来源：http://hz.guannengcc.top/gtbmlpjegd.html

PHP:  $argv;  $argc;
来源：http://hz.xziqi.cn/gtqhdugnce.html

JS:   process.argv.slice(2)
来源：http://hz.guowangkeji.top/gtcccxyrym.html

TS:   process.argv.slice(2)
来源：http://hz.gzhubu.top/gtpnihsttv.html

Java: args 数组（main 方法参数）
来源：http://hz.zhongyouzk.top/gtwktlcznr.html

Go:   os.Args[1:]
来源：http://hz.xingfuxueyuan.xyz/gtbbikizzn.html

Ruby: ARGV
来源：http://hz.bjfxy.top/gtgxisuowk.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hammf.cn/gtqhncapcx.html

[M02] 读取环境变量
来源：http://hz.gaohongyu789.top/gtghvvnesl.html

Py:   os.environ.get("HOME")
来源：http://hz.zhaomingkeji.xyz/gtqpdgjpej.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yanxiufei.cn/gtqcaaoybj.html

JS:   process.env.HOME
来源：http://hz.hfpthk.cn/gtdcztqumk.html

TS:   process.env.HOME
来源：http://hz.tanke756.top/gtbxovsnfi.html

Java: System.getenv("HOME")
来源：http://hz.wangshuangyany.cn/gttaarfuqi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.shanyushiyangtech.top/gtfnbekfqq.html

Ruby: ENV["HOME"]
来源：http://hz.yj20258888.top/gtocdvyzjm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cqqwz.cn/gtcagvdbdw.html

[M03] 执行外部命令
来源：http://hz.mhx1999.top/gtkxazgcjd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhiwuduotai.top/gtnbllroxy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhongyouzk.top/gtryszpqfr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yueranfly.top/gtikkjbddy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangkeji.top/gtpmmbvlrk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.meibo888.top/gtsqpivwhf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.9152youxi.cn/gtstoczuof.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yueranfly.top/gtyrylomry.html

C#:   Process.Start("ls", "-l");
来源：http://hz.tianlin.xyz/gtwjnnvuuh.html

[M04] 获取当前工作目录
来源：http://hz.yj202588.top/gtlwvexfrw.html

Py:   os.getcwd()
来源：http://hz.guowangkeji.top/gtqmbjvzph.html

PHP:  getcwd();
来源：http://hz.jinghuilouyu.cn/gtektlblxr.html

JS:   process.cwd()
来源：http://hz.guannengcc.top/gtlhjxyufw.html

TS:   process.cwd()
来源：http://hz.sxryk.cn/gtvlklcwrw.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yonumen.top/gtgqkezskg.html

Go:   os.Getwd()
来源：http://hz.wangshuangyany.cn/gtydinjhvu.html

Ruby: Dir.pwd
来源：http://hz.redwolf501.top/gtmefyzhmp.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yuanzhike.top/gtdswpfquk.html

[M05] 设置退出码
来源：http://hz.jinyuanbaomall.cn/gtvjcycjsx.html

Py:   sys.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtvllkysti.html

PHP:  exit(1);
来源：http://hz.jinyuanbaomall.cn/gtghdiqjlc.html

JS:   process.exit(1)
来源：http://hz.yuxming.cn/gtpyocjwxk.html

TS:   process.exit(1)
来源：http://hz.iojbl.cn/gtgdalnlff.html

Java: System.exit(1)
来源：http://hz.chenzaomai.com/gtngwngjzj.html

Go:   os.Exit(1)
来源：http://hz.wangshuangyany.cn/gtgzyfslip.html

Ruby: exit 1
来源：http://hz.jianghu66.top/gtztxkmyuu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cqqwz.cn/gtjdvuzgoo.html

[M06] 向标准错误输出
来源：http://hz.bjfxy.top/gtotsadduj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.nanxuanxn.top/gtdxntwmut.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.meibo888.top/gtwnkemmqc.html

JS:   console.error("err")
来源：http://hz.shangyingyoupin.top/gtsuwcwopj.html

TS:   console.error("err")
来源：http://hz.zhixingplan.top/gtgedkupjs.html

Java: System.err.println("err")
来源：http://hz.zhixingplan.top/gtqjftblrw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jqgufenzy.top/gtywugwxxt.html

Ruby: warn "err"
来源：http://hz.chenlongwang.top/gteuvzgocj.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shangyingyoupin.top/gtjsmnefgq.html

[M07] 判断是否为主入口
来源：http://hz.nanxinkj.top/gtzqjroxmy.html

Py:   if __name__ == "__main__":
来源：http://hz.jinyuanbaomall.cn/gtrgkgyfaw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.sxryk.cn/gtpbauunlf.html

JS:   require.main === module
来源：http://hz.aibaodan.cn/gtgtvjyach.html

TS:   require.main === module
来源：http://hz.zhijiandao.cn/gtnaotogwm.html

Java: public static void main(String[] args)
来源：http://hz.shzxlz.cn/gtoslnzihq.html

Go:   func main()
来源：http://hz.xylfe.cn/gtinhpwjsx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jiagoushi.top/gtzxsbfhgt.html

C#:   static void Main(string[] args)
来源：http://hz.guowangkeji.top/gtklzvkigu.html

[M08] 获取系统与运行时信息
来源：http://hz.c1oappe.top/gtbxodxdnz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.sweek.top/gtvnlhvssq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.smart0.xyz/gttjfzcxdp.html

JS:   process.platform;  process.version
来源：http://hz.gaohongyu789.top/gtycqisocu.html

TS:   process.platform;  process.version
来源：http://hz.tian-w.cn/gtvsyzcwuc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.chenlongwang.top/gtxiocioaz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yj202588.top/gthxvnxudj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shzxlz.cn/gteyjescuy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ivvv.top/gtouyzocco.html

================================================================================
来源：http://hz.ivvv.top/gtgupzexac.html

N. 数据结构与算法
来源：http://hz.zhiwuduotai.top/gtjfrulqgt.html

================================================================================
来源：http://hz.cqqwz.cn/gtzhxsnclz.html

[N01] 二分查找（有序数组）
来源：http://hz.yanxiufei.cn/gtetihgvyw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ydjk.org.cn/gtxpznpvsq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jqgfzy.top/gtzxnxngao.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxuanxn.top/gtowadsbcc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.0kj1m.cn/gtvyiobpkg.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.pycfn.com/gtusykfpra.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.havefunace.top/gtyrrxzdff.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hfpthk.cn/gtwluokphj.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jyoumei.cn/gtwnnnfkps.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.vqdsnc.cn/gtfvquqvcc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenlongwang.top/gtnxskhoft.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ivvv.top/gtyjcchnqv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinyuanbaomall.cn/gtcjenmdha.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sysykeji.top/gtpprudplm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ydzc1.top/gtjsoajwro.html

Go:   slices.Sort(arr)
来源：http://hz.aibaodan.cn/gtwnujkdtt.html

Ruby: arr.sort
来源：http://hz.hywenlv.cn/gtoxexgrel.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.c1oappe.top/gtaqpmzhnn.html

[N03] 快速排序（分治示例）
来源：http://hz.xylfe.cn/gteymqsxci.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhijiandao.cn/gtljwcvsaq.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sysykeji.top/gtezhizjjd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.52xcode.cn/gtaldceohs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinghuilouyu.cn/gtxhjpjqns.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.havefunace.top/gtwmpapztr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yj20258.top/gtfkwjuqum.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cucudq.cn/gtxvdbfevt.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.c1oappe.top/gtmnuhmzxo.html

[N04] 斐波那契数列
来源：http://hz.xziqi.cn/gtyylnffgz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jinyuanbaomall.cn/gtddmiawzw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinqigfzy.top/gtibcbdmoc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.haohaochexian.top/gteqrqknic.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.wangdashe.top/gtytjvllvk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.nanxinkj.top/gtbfylelfj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.fzhhl.top/gtdxnpueps.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yonumen.top/gtwhytvabj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.gogol.net.cn/gtcdjqphyd.html

[N05] 最大公约数
来源：http://hz.gogol.net.cn/gtqqsvhysy.html

Py:   math.gcd(a, b)
来源：http://hz.yj202588.top/gtdqrwvqmn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.nanxuanxn.top/gtsbllzjbh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zdqjudy.top/gtfhkktybf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ppjwa.cn/gtreccmomo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.guannengcc.top/gtkiclcdqx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.bjfxy.top/gtvyirubxz.html

Ruby: a.gcd(b)
来源：http://hz.yj20258.top/gtubeoqkxs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yanxiufei.cn/gtbmgkzqlk.html

[N06] 判断回文字符串
来源：http://hz.jianghu66.top/gtdbjwhsyp.html

Py:   s == s[::-1]
来源：http://hz.hywenlv.cn/gtkipgozlt.html

PHP:  $s === strrev($s);
来源：http://hz.smart0.xyz/gtezxkokns.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhoulong.xyz/gtgjvqeybs.html

TS:   s === [...s].reverse().join("")
来源：http://hz.sweek.top/gtvhzahnmf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sweek.top/gtqydhxden.html

Go:   // 双指针从两端比较
来源：http://hz.svipenyu.cn/gtgbdequla.html


<!-- 参考信息 -->