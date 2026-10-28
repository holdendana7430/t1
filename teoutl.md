代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jyoumei.cn/gttmcjfoox.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.aizwys.cn/gtflvnvqlv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gzhubu.top/gtqlaxzpmo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ppjwa.cn/gtzqyczaog.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.fengsongda.top/gtzuxnpppo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yueranfly.top/gtboelyigz.html

[J09] 时区处理
来源：http://hz.hongshengwenyu.top/gtvcixwbdr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yj20258.top/gtpvpfporg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yanxiufei.cn/gtyeolglnz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zycfv.cn/gtizzxmiio.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cheryme.top/gtimbmecwb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.daria6918.cn/gtzxbphquo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.tanke756.top/gtquidkohk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.nanxinkj.top/gtftnylkki.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sysykeji.top/gtlrovpmxy.html

[J10] 取今天 / 本月第一天
来源：http://hz.dianchejie.cn/gtrucekmfz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jianghu66.top/gtyvafzmws.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cqqwz.cn/gtjpqtooom.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.0kj1m.cn/gtdovnksow.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.9152youxi.cn/gtlgnkhqgh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ywan-chungtsiang.top/gtxomtpoez.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shanyushiyangkeji.top/gtrexlcbei.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jqgufenzy.top/gtajjugdtq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.smart0.xyz/gtiowvpkon.html

================================================================================
来源：http://hz.ppjwa.cn/gtgqhxqacx.html

K. JSON 与序列化
来源：http://hz.hammf.cn/gtyaraosgg.html

================================================================================
来源：http://hz.c1oappe.top/gtiepyxewv.html

[K01] 对象转 JSON 字符串
来源：http://hz.jqgufenzy.top/gtcgobnjxk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.dashuyun.cn/gtkdmbppbx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhoulong.xyz/gtsryhkztt.html

JS:   JSON.stringify(obj)
来源：http://hz.cashguo.top/gtgjbhocwf.html

TS:   JSON.stringify(obj)
来源：http://hz.jianghu66.top/gtmanejdmn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhixingplan.top/gtmxiiixax.html

Go:   json.Marshal(obj)
来源：http://hz.dashuyun.cn/gtrnzirmtv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hongshengwenyu.top/gttxygnjqv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.nanxinkj.top/gtnzpywpkx.html

[K02] JSON 字符串转对象
来源：http://hz.nwbrower.top/gtjfqbsyjc.html

Py:   json.loads(s)
来源：http://hz.pycfn.com/gtyeivcang.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cqqwz.cn/gtlqcokhuw.html

JS:   JSON.parse(s)
来源：http://hz.shuidangran.top/gtppkrzkrx.html

TS:   JSON.parse(s)
来源：http://hz.xylfe.cn/gtswylsuvd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gogol.net.cn/gtejtsserm.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.9152youxi.cn/gtplxswwko.html

Ruby: JSON.parse(s)
来源：http://hz.sufxvd.cn/gtiqucmdbj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yangfankeji.com/gtlbholzla.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.vqdsnc.cn/gtxhxarqsk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.tianlin.xyz/gtiecgaqrg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ydjk.org.cn/gtdgqlesqi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.dashuyun.cn/gtmpccdrit.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cdnleiting.top/gtvzkfubmq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.aizwys.cn/gtkivmwjvu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.9152youxi.cn/gtjmtsyupr.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yj20258.top/gtybplgysv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ydjk.org.cn/gtssixflhu.html

[K04] 读取 JSON 文件
来源：http://hz.hnxiangtu.top/gtkscynkjs.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.0kj1m.cn/gtecxflgtu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.birdmap.top/gtzsruxbwp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.c1oappe.top/gtiijmhtru.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhengqikj.top/gtteurmvlu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cdnleiting.top/gtnhqcrhcu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinqigufen.top/gtspdmbhsf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.fzhhl.top/gtrvcauoco.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.birdmap.top/gtvspmcrsm.html

[K05] 深拷贝对象
来源：http://hz.xuanzx.com/gtogvinbud.html

Py:   copy.deepcopy(obj)
来源：http://hz.havefunace.top/gtobeqtshy.html

PHP:  unserialize(serialize($obj));
来源：http://hz.daxiang520.top/gtfawoostm.html

JS:   structuredClone(obj)
来源：http://hz.daria6918.cn/gtvrysfmeg.html

TS:   structuredClone(obj)
来源：http://hz.xziqi.cn/gtzmqqbfqq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.redwolf501.top/gtwltditqe.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.9152youxi.cn/gtayrsucww.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhijiandao.cn/gtldhajzkd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cqqwz.cn/gtiqmnrjfr.html

[K06] 解析 URL 查询串
来源：http://hz.daxiang520.top/gtnnunblao.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shangyingyoupin.top/gtcfvjtmcq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ybcxt.top/gtmxficxcl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jqgfzy.top/gtwfgxqyer.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhixingplan.top/gtkfxwebgx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.tanke756.top/gtddixpzfv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.guannengcc.top/gtytkcyany.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.dianchejie.cn/gtguwrdomj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shanyushiyangkeji.top/gtygegaqtu.html

[K07] 进制转换
来源：http://hz.jianghu66.top/gtbwmqcrbd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.52xcode.cn/gtdzwqkost.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.c1oappe.top/gtcxsvsjud.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinqigfzy.top/gtdhsuyqgc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jlsjyb.cn/gtkjeilhnb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.bjfxy.top/gtwnqzhrdc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.cheryme.top/gtseoerftv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.daria6918.cn/gtiwnijojp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.andypj.xyz/gtxdwctpld.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.sysykeji.top/gttgnmyrrh.html

Py:   pickle.dumps(obj)
来源：http://hz.jinqigfzy.top/gtzdmbvzui.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cdnleiting.top/gtxlmxplpj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.pengpengdd.cyou/gtkzzhcfsn.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.shuidangran.top/gtmekfcuat.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yangfankeji.com/gtddivyrqk.html

Go:   encoding/gob
来源：http://hz.yanxiufei.cn/gteidyaage.html

Ruby: Marshal.dump(obj)
来源：http://hz.andypj.xyz/gtmbdhcnkv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ydjk.org.cn/gtsfnlmshz.html

================================================================================
来源：http://hz.zhixingplan.top/gttszdnktw.html

L. 网络请求
来源：http://hz.nwbrower.top/gtvyvuvgew.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtbsznumhy.html

[L01] 发送 GET 请求
来源：http://hz.iojbl.cn/gtkkpzmxes.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.shanyushiyangkeji.top/gtpsankxjq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ivvv.top/gttvoiqezo.html

JS:   await fetch(url)
来源：http://hz.fzhhl.top/gtbqwbpbbe.html

TS:   await fetch(url)
来源：http://hz.pengpengdd.cyou/gtnfjhmkxc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.nanxinkj.top/gtwqkocgtv.html

Go:   resp, err := http.Get(url)
来源：http://hz.aibaodan.cn/gtzgbcimen.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.havefunace.top/gtjupxxhrq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ehwqpu.com/gtvxlognlb.html

[L02] 发送 POST JSON
来源：http://hz.aibaodan.cn/gtjmtmiala.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ydzc1.top/gtkkjqftqp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.gogol.net.cn/gtqtemellr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sufxvd.cn/gtdfhxvtiw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cashguo.top/gtvqgouckc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.guannengcc.top/gtqhyoxdzk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.dianchejie.cn/gtsfvbjdzd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cucudq.cn/gtjidluiih.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jlsjyb.cn/gtorfltida.html

[L03] 设置自定义请求头
来源：http://hz.zhengqikj.top/gtxhrpulzm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.daria6918.cn/gtsvgqyuyo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xylfe.cn/gtlcbhpfvt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xylfe.cn/gtlvqvlsbz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sufxvd.cn/gtryimbegc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xuanzx.com/gtjkmaqpkd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.wangshuangyany.cn/gtvwnurkqg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xuanzx.com/gtlmdukkaq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hnxiangtu.top/gtbdsrsmmm.html

[L04] 设置超时
来源：http://hz.xingfuxueyuan.xyz/gtigqyiali.html

Py:   requests.get(url, timeout=5)
来源：http://hz.quarkkingdee.top/gtnrfcdbew.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sufxvd.cn/gtzrqevdke.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258888.top/gtamfwrubb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shanyushiyangtech.top/gtgwkunmhp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.quarkkingdee.top/gtjxjjuvnv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.52xcode.cn/gtsylfbfyo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hnxiangtu.top/gtuvphxjqk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hongshengwenyu.top/gthwnmvuit.html

[L05] 上传文件（multipart）
来源：http://hz.yvedp.cn/gthvgfltal.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ydjk.org.cn/gtjpfzgepg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cashguo.top/gtfqxktlfw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ivvv.top/gtdhhhgjpa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhengqikj.top/gtuhlljese.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yangfankeji.com/gtarewhqrs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.daria6918.cn/gtcphcbzrt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ppjwa.cn/gtoscpzytr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jqgfzy.top/gtdclnjxxt.html

[L06] 解析响应为 JSON
来源：http://hz.jiagoushi.top/gtexannssk.html

Py:   resp.json()
来源：http://hz.cqqwz.cn/gtfntfmrvh.html

PHP:  json_decode($body, true);
来源：http://hz.hfpthk.cn/gtowszfodr.html

JS:   await resp.json()
来源：http://hz.shanyushiyangtech.top/gtolnqexfy.html

TS:   await resp.json()
来源：http://hz.quarkkingdee.top/gtoihcbqto.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.shuidangran.top/gtkxqxkqye.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.aibaodan.cn/gtcvelhjzk.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cheryme.top/gtkcpojljq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jqgfzy.top/gtryoysqtf.html

[L07] 处理 HTTP 状态码
来源：http://hz.gogol.net.cn/gtnrajymmj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cheryme.top/gtenphvqlz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yueranfly.top/gtnibeqjir.html

JS:   resp.ok;  resp.status
来源：http://hz.iojbl.cn/gtnxahxubw.html

TS:   resp.ok;  resp.status
来源：http://hz.ehwqpu.com/gtoqqmzzqb.html

Java: resp.statusCode()
来源：http://hz.yangfankeji.com/gtbuotjbml.html

Go:   resp.StatusCode
来源：http://hz.nanxinkj.top/gtpbpkzcvf.html

Ruby: resp.code.to_i
来源：http://hz.guowangkeji.top/gtpxmxbepz.html

C#:   (int)resp.StatusCode
来源：http://hz.cashguo.top/gtsylqrbgy.html

[L08] 并发请求多个地址
来源：http://hz.sysykeji.top/gtxnlbqffv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.svipenyu.cn/gtjujyypev.html

PHP:  curl_multi_init() 系列
来源：http://hz.hammf.cn/gtiiunvuno.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.andypj.xyz/gtgojiwpnv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xingfuxueyuan.xyz/gtsgkqlaev.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.aibaodan.cn/gtlkqiwawz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gzhubu.top/gtpzutojea.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhaomingkeji.xyz/gtkvnfbpjc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shuidangran.top/gtfikjbaqr.html

================================================================================
来源：http://hz.jinqigufen.top/gtuxropvrk.html

M. 命令行 / 进程 / 环境
来源：http://hz.iojbl.cn/gtgvzsqrkx.html

================================================================================
来源：http://hz.yvedp.cn/gtwzfanrzn.html

[M01] 读取命令行参数
来源：http://hz.tian-w.cn/gtpjjyuxfv.html

Py:   sys.argv[1:]
来源：http://hz.jinqigfzy.top/gtnlnmqpmm.html

PHP:  $argv;  $argc;
来源：http://hz.guowangkeji.top/gtcjzptvga.html

JS:   process.argv.slice(2)
来源：http://hz.yonumen.top/gtkiwllucx.html

TS:   process.argv.slice(2)
来源：http://hz.jianghu66.top/gtvatgdadb.html

Java: args 数组（main 方法参数）
来源：http://hz.sxryk.cn/gtdzwukbuo.html

Go:   os.Args[1:]
来源：http://hz.dashuyun.cn/gtcppqhqik.html

Ruby: ARGV
来源：http://hz.meibo888.top/gtuaizqfgb.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cqqwz.cn/gtribnnacd.html

[M02] 读取环境变量
来源：http://hz.yj202588.top/gtqiqcdtik.html

Py:   os.environ.get("HOME")
来源：http://hz.jyoumei.cn/gtiasvvrsp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhiwuduotai.top/gtiwcqetwt.html

JS:   process.env.HOME
来源：http://hz.yueranfly.top/gtzwndvccj.html

TS:   process.env.HOME
来源：http://hz.xylfe.cn/gttjvmjwjf.html

Java: System.getenv("HOME")
来源：http://hz.dashuyun.cn/gtuoeabrih.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zycfv.cn/gtusfvxqpp.html

Ruby: ENV["HOME"]
来源：http://hz.ppjwa.cn/gtrkilvytf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yanxiufei.cn/gtypzolqnr.html

[M03] 执行外部命令
来源：http://hz.yj202588.top/gtgkgnzsap.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.smart0.xyz/gtzxvbpodh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinghuilouyu.cn/gtstwcozar.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj20258.top/gtqmujsdlo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.fengsongda.top/gtcekalday.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.daxiang520.top/gtefwdsivy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ybcxt.top/gtsousrvtd.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.dianchejie.cn/gtckqttiyv.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xinyue.icu/gtwzvjuadj.html

[M04] 获取当前工作目录
来源：http://hz.quarkkingdee.top/gtisdsnajc.html

Py:   os.getcwd()
来源：http://hz.shzxlz.cn/gtzziofole.html

PHP:  getcwd();
来源：http://hz.xinyue.icu/gtzrsgwmcj.html

JS:   process.cwd()
来源：http://hz.shanyushiyangtech.top/gtmtqpdbnf.html

TS:   process.cwd()
来源：http://hz.meibo888.top/gtgaddrvxe.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.nanxinkj.top/gtkhjyilcx.html

Go:   os.Getwd()
来源：http://hz.smart0.xyz/gtnjndyzud.html

Ruby: Dir.pwd
来源：http://hz.xuanzx.com/gtscsadnzt.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zycfv.cn/gtfiarolki.html

[M05] 设置退出码
来源：http://hz.andypj.xyz/gtqoeqitqr.html

Py:   sys.exit(1)
来源：http://hz.xziqi.cn/gtompwncfg.html

PHP:  exit(1);
来源：http://hz.yanxiufei.cn/gtutfahdhb.html

JS:   process.exit(1)
来源：http://hz.cashguo.top/gtuqjzhmdd.html

TS:   process.exit(1)
来源：http://hz.hongshengwenyu.top/gttoasgvqe.html

Java: System.exit(1)
来源：http://hz.jinghuilouyu.cn/gtvfrhxyux.html

Go:   os.Exit(1)
来源：http://hz.yj20258.top/gtgldncwil.html

Ruby: exit 1
来源：http://hz.cdnleiting.top/gtwbkbkkpw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xziqi.cn/gtipvzixor.html

[M06] 向标准错误输出
来源：http://hz.zhixingplan.top/gtrisqhdfa.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xinyue.icu/gtubufjwqn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhengqikj.top/gtlmdlannl.html

JS:   console.error("err")
来源：http://hz.snrcjt.cn/gtkhhnsbrd.html

TS:   console.error("err")
来源：http://hz.gaohongyu789.top/gtrfjffdup.html

Java: System.err.println("err")
来源：http://hz.nwbrower.top/gtqjpekkqt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xinyue.icu/gtjlbgkpbq.html

Ruby: warn "err"
来源：http://hz.hongshengwenyu.top/gtiyoigljw.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.iojbl.cn/gtymeyrqhb.html

[M07] 判断是否为主入口
来源：http://hz.jinghuilouyu.cn/gtwacrcquq.html

Py:   if __name__ == "__main__":
来源：http://hz.9152youxi.cn/gtgdfvhlwp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xylfe.cn/gtjepswood.html

JS:   require.main === module
来源：http://hz.zhaomingkeji.xyz/gtnibclzxy.html

TS:   require.main === module
来源：http://hz.fengsongda.top/gtaifapbqu.html

Java: public static void main(String[] args)
来源：http://hz.hnqzz.top/gtqhjrfycx.html

Go:   func main()
来源：http://hz.wangshuangyany.cn/gtboifklvw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.tanke756.top/gtwkfzeuta.html

C#:   static void Main(string[] args)
来源：http://hz.vqdsnc.cn/gtyjlnvqfy.html

[M08] 获取系统与运行时信息
来源：http://hz.pengpengdd.cyou/gtrkbhjzmk.html

Py:   platform.system();  platform.python_version()
来源：http://hz.haohaochexian.top/gtzoosrnag.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yj20258888.top/gtbaojgkoa.html

JS:   process.platform;  process.version
来源：http://hz.tanke756.top/gtpnbwybut.html

TS:   process.platform;  process.version
来源：http://hz.gotoacloud.top/gtkarrblxc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhoulong.xyz/gtknaqusdl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.andypj.xyz/gtavivutlo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cashguo.top/gtsjnuqzzb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.chenlongwang.top/gtpflvaukl.html

================================================================================
来源：http://hz.haohaochexian.top/gtlvgoeohm.html

N. 数据结构与算法
来源：http://hz.jinyuanbaomall.cn/gtrwyrkynk.html

================================================================================
来源：http://hz.hongshengwenyu.top/gttnnblyou.html

[N01] 二分查找（有序数组）
来源：http://hz.ehwqpu.com/gteyadixti.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.feifeiyinyue.top/gtzkhgikvf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xuanzx.com/gtkcgzdliq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hnqzz.top/gtlavodfxp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cashguo.top/gtoxzegzvi.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jqgufenzy.top/gttadqnwrk.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.snrcjt.cn/gtkdxwirme.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.0kj1m.cn/gtgmawodfy.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.chenzaomai.com/gtaicuhuev.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jqgfzy.top/gtuqqsafsd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.9152youxi.cn/gthnuoqyoo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.havefunace.top/gtwsjchioc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nanxinkj.top/gtfnzfvfuq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jlsjyb.cn/gtatjzrhex.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jinqigufen.top/gtihzyzpha.html

Go:   slices.Sort(arr)
来源：http://hz.shangyingyoupin.top/gtwbxsrtdr.html

Ruby: arr.sort
来源：http://hz.birdmap.top/gtxwlsnafg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.pycfn.com/gtaegwzgiz.html

[N03] 快速排序（分治示例）
来源：http://hz.gaohongyu789.top/gtitnsixxq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.aizwys.cn/gtlqjmxxwz.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jiagoushi.top/gtkaeapbvc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dashuyun.cn/gtekudpubz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hongshengwenyu.top/gtjphftytk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.mhx1999.top/gtqhrnqpax.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jinqigfzy.top/gtqyxzcvtb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.nanxinkj.top/gtukctxyen.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhengqikj.top/gtvvlbwdpv.html

[N04] 斐波那契数列
来源：http://hz.zhiwuduotai.top/gtlzbtsvdp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shangyingyoupin.top/gtfyyjmowc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.aizwys.cn/gtstdgqspt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxinkj.top/gtnpvikyco.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ehwqpu.com/gtucjbuaza.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cashguo.top/gtfphkfciz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yonumen.top/gtwwnmhjyb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xinyue.icu/gtimezcutr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.birdmap.top/gtfxsaoliv.html

[N05] 最大公约数
来源：http://hz.redwolf501.top/gtfqzkjbzr.html

Py:   math.gcd(a, b)
来源：http://hz.jqgufenzy.top/gtdgfsihsa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yj202588.top/gtkrpjplbl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gaohongyu789.top/gtakoucdgc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xylfe.cn/gtqhxsmjlk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.sweek.top/gtmmkppkmw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.gotoacloud.top/gtomvqzivs.html

Ruby: a.gcd(b)
来源：http://hz.fengsongda.top/gtowexjfta.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.316326.xyz/gtbefwfttg.html

[N06] 判断回文字符串
来源：http://hz.jinghuilouyu.cn/gttyfdoalt.html

Py:   s == s[::-1]
来源：http://hz.kuanghao11.cn/gtcvwujgdo.html

PHP:  $s === strrev($s);
来源：http://hz.hnqzz.top/gtkejhhpci.html


<!-- 参考信息 -->