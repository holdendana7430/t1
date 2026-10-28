代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cashguo.top/gtuqzjthdi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.chenzaomai.com/gthxrxxdsk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xinyue.icu/gtexaqfqsd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.0kj1m.cn/gtflptnvst.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.quarkkingdee.top/gtiwjzbsiq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.dashuyun.cn/gtsuxxzbel.html

[J09] 时区处理
来源：http://hz.yj202588.top/gtphvmugpl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zdqjudy.top/gtbugwmevw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.nanxuanxn.top/gtmgdchwtm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guannengcc.top/gtlaixtulw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhaomingkeji.xyz/gtpfqclpkh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nanxinkj.top/gtumvijvtj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.nanxinkj.top/gtvdilljgo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.sweek.top/gtbvdkvegt.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.kuanghao11.cn/gtoxkmbmnt.html

[J10] 取今天 / 本月第一天
来源：http://hz.bjfxy.top/gtsjmybndr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.wangshuangyany.cn/gtoguytkby.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.gogol.net.cn/gtjiqgirhm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.9152youxi.cn/gtbntuvuix.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhiwuduotai.top/gtmpaddfql.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nanxuanxn.top/gtxundlnyk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zycfv.cn/gtsjdtazxk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xingfuxueyuan.xyz/gteaomeyco.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xylfe.cn/gtprhsdaog.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtkmqnfwkm.html

K. JSON 与序列化
来源：http://hz.havefunace.top/gtohaqavst.html

================================================================================
来源：http://hz.svipenyu.cn/gtdmlpsgif.html

[K01] 对象转 JSON 字符串
来源：http://hz.shuidangran.top/gtgububaxc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jqgufenzy.top/gtnkmheimo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ivvv.top/gtluhwvgok.html

JS:   JSON.stringify(obj)
来源：http://hz.ivvv.top/gtcckkrorn.html

TS:   JSON.stringify(obj)
来源：http://hz.quarkkingdee.top/gtedobhtbj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.9152youxi.cn/gtrtntjshp.html

Go:   json.Marshal(obj)
来源：http://hz.shangyingyoupin.top/gttmstxkgr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shzxlz.cn/gtheqwviya.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sxryk.cn/gtgaamwjop.html

[K02] JSON 字符串转对象
来源：http://hz.hnxiangtu.top/gtbfqjeing.html

Py:   json.loads(s)
来源：http://hz.daxiang520.top/gtdasltnxu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jqgufenzy.top/gtkrepzxdt.html

JS:   JSON.parse(s)
来源：http://hz.iojbl.cn/gteyzsontw.html

TS:   JSON.parse(s)
来源：http://hz.daxiang520.top/gthjeucxau.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinqigfzy.top/gttojdvmtt.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cqqwz.cn/gttxhrxumz.html

Ruby: JSON.parse(s)
来源：http://hz.jinqigfzy.top/gtdnezgbmc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.tanke756.top/gtmvjgrxha.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.chenzaomai.com/gtmtttipsw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yj20258888.top/gtanlqqxzs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxinkj.top/gttudhpyho.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gaohongyu789.top/gtyaukkypk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhixingplan.top/gtuvhjdzli.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shangyingyoupin.top/gtfkjvyayc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hnqzz.top/gtwdmuwqnt.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.kuanghao11.cn/gthgislnyh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ehwqpu.com/gtqmbzfhlt.html

[K04] 读取 JSON 文件
来源：http://hz.wangshuangyany.cn/gtalnohkgz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.0kj1m.cn/gtpkixqnny.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.tianlin.xyz/gtswypckke.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhaomingkeji.xyz/gtjujeffnj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nwbrower.top/gtjnmwfvsw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.nanxinkj.top/gtztdqsfwu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jlsjyb.cn/gtimofuadd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ydjk.org.cn/gtroamsfqr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yongpay.top/gtrafcsvnn.html

[K05] 深拷贝对象
来源：http://hz.pengpengdd.cyou/gtozocketk.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhoulong.xyz/gtfnotfywj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ydjk.org.cn/gthzvbvnlg.html

JS:   structuredClone(obj)
来源：http://hz.yangfankeji.com/gtdvhooxbf.html

TS:   structuredClone(obj)
来源：http://hz.0kj1m.cn/gthbctllvp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hongshengwenyu.top/gtvlcebkhx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj202588.top/gtuhkwsise.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.chenlongwang.top/gtiwwecand.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.dianchejie.cn/gtkmxqqaan.html

[K06] 解析 URL 查询串
来源：http://hz.shanyushiyangkeji.top/gtkdvfyplj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sufxvd.cn/gtectfykjs.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yj20258888.top/gtaeghxpdu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cashguo.top/gtcussqpsj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.guannengcc.top/gtkgurgllo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sufxvd.cn/gtnjdhgvaa.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.c1oappe.top/gtyqaxgdzh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xuanzx.com/gtakhmszsz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cheryme.top/gtvtmpcfdx.html

[K07] 进制转换
来源：http://hz.yanxiufei.cn/gtfyvstkjg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtraqcwbls.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tanke756.top/gttmsswsmf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtbcbfqtzh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ppjwa.cn/gtmsbqobgi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xuetiantiany.cn/gtpfnkwrtj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.daria6918.cn/gteompviib.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinyuanbaomall.cn/gtfgusifar.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.cdnleiting.top/gtjebrmvii.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xuanzx.com/gtlhftsvzx.html

Py:   pickle.dumps(obj)
来源：http://hz.guowangkeji.top/gtmyocndhr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tian-w.cn/gtxhzkkiox.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.vqdsnc.cn/gtjwxgofbl.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ydjk.org.cn/gtetjggmam.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zycfv.cn/gtnyfqjwxp.html

Go:   encoding/gob
来源：http://hz.aibaodan.cn/gtymomyunc.html

Ruby: Marshal.dump(obj)
来源：http://hz.redwolf501.top/gtwlcvujej.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ywan-chungtsiang.top/gtvzmzqchb.html

================================================================================
来源：http://hz.daxiang520.top/gthojclugy.html

L. 网络请求
来源：http://hz.jyoumei.cn/gtuwgnuivm.html

================================================================================
来源：http://hz.hnxiangtu.top/gtdlyqiale.html

[L01] 发送 GET 请求
来源：http://hz.zhixingplan.top/gtykbrfcwi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.sufxvd.cn/gtavjhnebk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.52xcode.cn/gtyryurmup.html

JS:   await fetch(url)
来源：http://hz.hammf.cn/gtjjsshkiz.html

TS:   await fetch(url)
来源：http://hz.aibaodan.cn/gtnwehsjfk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ivvv.top/gtjgjakbnk.html

Go:   resp, err := http.Get(url)
来源：http://hz.shanyushiyangkeji.top/gtfxeynzft.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinghuilouyu.cn/gtmvgwwjbj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zdqjudy.top/gtahahkqjx.html

[L02] 发送 POST JSON
来源：http://hz.zhengqikj.top/gtrdgmygxj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yonumen.top/gthujfsuvp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhijiandao.cn/gtvowqsxju.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tianlin.xyz/gtfwppjeiw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhaomingkeji.xyz/gtlzfozcaw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yangfankeji.com/gtiohpgnjr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhixingplan.top/gtfiscyclr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.aizwys.cn/gtosrdxxln.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhongyouzk.top/gtgykhsttx.html

[L03] 设置自定义请求头
来源：http://hz.redwolf501.top/gtaosbuxte.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.sysykeji.top/gthcoodlic.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.chenzaomai.com/gtjcwqtabp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenzaomai.com/gtpicsakey.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jiagoushi.top/gtfhnxztyz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.birdmap.top/gtstqqrhnp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xinyue.icu/gttzalzxhj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shzxlz.cn/gtsaoyjhre.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.quarkkingdee.top/gtvguntcgy.html

[L04] 设置超时
来源：http://hz.ydjk.org.cn/gtkepjgzhn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xziqi.cn/gthnicdqqj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ywan-chungtsiang.top/gtykocioju.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.bjfxy.top/gtxpcvqyro.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jlsjyb.cn/gtiqaeupfm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xziqi.cn/gtozulmcbx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ydzc1.top/gtjqdevuzs.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shzxlz.cn/gtrsstxrad.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.0kj1m.cn/gtwciwudep.html

[L05] 上传文件（multipart）
来源：http://hz.shangyingyoupin.top/gtxejwqswm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.sufxvd.cn/gtbvewznmz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cucudq.cn/gtiikabghn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ivvv.top/gtubqszhvx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgfzy.top/gtzrybtmap.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.birdmap.top/gtbevtatpa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xuetiantiany.cn/gtwhbmmrvb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jiagoushi.top/gthvnsegnv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.tanke756.top/gtzakjtvtz.html

[L06] 解析响应为 JSON
来源：http://hz.cucudq.cn/gtsoayintw.html

Py:   resp.json()
来源：http://hz.zycfv.cn/gtdkodutqe.html

PHP:  json_decode($body, true);
来源：http://hz.ydzc1.top/gtsvcqoqqc.html

JS:   await resp.json()
来源：http://hz.hfpthk.cn/gtwlwhadzf.html

TS:   await resp.json()
来源：http://hz.xingfuxueyuan.xyz/gtrqginpqv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.redwolf501.top/gtmrcaykub.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jianghu66.top/gtwciyzrsw.html

Ruby: JSON.parse(resp.body)
来源：http://hz.pycfn.com/gtyxphmvqo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhijiandao.cn/gtosrjybbd.html

[L07] 处理 HTTP 状态码
来源：http://hz.jqgufenzy.top/gtduntgqrd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xingfuxueyuan.xyz/gtjxdrezms.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.chenzaomai.com/gtdyldjynn.html

JS:   resp.ok;  resp.status
来源：http://hz.mhx1999.top/gtvsrtpjgi.html

TS:   resp.ok;  resp.status
来源：http://hz.fzhhl.top/gtmvypubfc.html

Java: resp.statusCode()
来源：http://hz.xingfuxueyuan.xyz/gtphsrenln.html

Go:   resp.StatusCode
来源：http://hz.mhx1999.top/gtmptfukix.html

Ruby: resp.code.to_i
来源：http://hz.yongpay.top/gtulfwssmo.html

C#:   (int)resp.StatusCode
来源：http://hz.chenlongwang.top/gtlqikrpoc.html

[L08] 并发请求多个地址
来源：http://hz.wangdashe.top/gtzdcabddj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ywan-chungtsiang.top/gtllqitgyu.html

PHP:  curl_multi_init() 系列
来源：http://hz.c1oappe.top/gtauwvtkbz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigfzy.top/gtpxrhkves.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xziqi.cn/gtjiajldae.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sweek.top/gtxroxiutl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jlsjyb.cn/gtchifuzzk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jqgfzy.top/gtwkalfblw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.iojbl.cn/gttoeyhdvj.html

================================================================================
来源：http://hz.gaohongyu789.top/gtmatcaexg.html

M. 命令行 / 进程 / 环境
来源：http://hz.ehwqpu.com/gtggjbrmlu.html

================================================================================
来源：http://hz.daxiang520.top/gtclqvlrkv.html

[M01] 读取命令行参数
来源：http://hz.316326.xyz/gtggjiweqq.html

Py:   sys.argv[1:]
来源：http://hz.zhongyouzk.top/gtsiwcecay.html

PHP:  $argv;  $argc;
来源：http://hz.zhengqikj.top/gtiqiiomhd.html

JS:   process.argv.slice(2)
来源：http://hz.dashuyun.cn/gtwdldpyzt.html

TS:   process.argv.slice(2)
来源：http://hz.hnxiangtu.top/gtxjakuwjs.html

Java: args 数组（main 方法参数）
来源：http://hz.gogol.net.cn/gtnjeisvwp.html

Go:   os.Args[1:]
来源：http://hz.shanyushiyangtech.top/gtypyuoent.html

Ruby: ARGV
来源：http://hz.snrcjt.cn/gtwiencmub.html

C#:   args 数组（Main 方法参数）
来源：http://hz.pycfn.com/gtdsnuclft.html

[M02] 读取环境变量
来源：http://hz.fzhhl.top/gtzyonmjsa.html

Py:   os.environ.get("HOME")
来源：http://hz.shzxlz.cn/gtvjqbyhng.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.smart0.xyz/gtdtqzvuvv.html

JS:   process.env.HOME
来源：http://hz.gogol.net.cn/gtlujuclga.html

TS:   process.env.HOME
来源：http://hz.hammf.cn/gtlkhzpbtz.html

Java: System.getenv("HOME")
来源：http://hz.chenzaomai.com/gtavziewum.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xingfuxueyuan.xyz/gtswciaual.html

Ruby: ENV["HOME"]
来源：http://hz.jyoumei.cn/gtjsvahxki.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hfpthk.cn/gtsitoybuw.html

[M03] 执行外部命令
来源：http://hz.feifeiyinyue.top/gtrjnovqnb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xuanzx.com/gtgldemkxx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.gzhubu.top/gtfeppofcd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sweek.top/gtjgpswcxo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xylfe.cn/gtvpnqfgbw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.chenlongwang.top/gtmjchvkqo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.chenlongwang.top/gtldlfgfsy.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xuanzx.com/gtmzqiubvt.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ehwqpu.com/gtqeegkrdw.html

[M04] 获取当前工作目录
来源：http://hz.hfpthk.cn/gtbkehzhvz.html

Py:   os.getcwd()
来源：http://hz.zhiwuduotai.top/gtffnzzunk.html

PHP:  getcwd();
来源：http://hz.xuetiantiany.cn/gtejvdkemo.html

JS:   process.cwd()
来源：http://hz.jianghu66.top/gtfuvgzsrf.html

TS:   process.cwd()
来源：http://hz.yj20258888.top/gtiuroqmvz.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hywenlv.cn/gtnmewoxqf.html

Go:   os.Getwd()
来源：http://hz.cdnleiting.top/gtzasujnbe.html

Ruby: Dir.pwd
来源：http://hz.chenlongwang.top/gtcfkypzvq.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.guowangkeji.top/gtujwnvpmj.html

[M05] 设置退出码
来源：http://hz.svipenyu.cn/gtntbvbgmy.html

Py:   sys.exit(1)
来源：http://hz.quarkkingdee.top/gthbszfcjm.html

PHP:  exit(1);
来源：http://hz.yj20258.top/gtomsvlxrl.html

JS:   process.exit(1)
来源：http://hz.316326.xyz/gtjjlvyxlo.html

TS:   process.exit(1)
来源：http://hz.andypj.xyz/gtrcdthbqf.html

Java: System.exit(1)
来源：http://hz.shzxlz.cn/gteltryxhz.html

Go:   os.Exit(1)
来源：http://hz.tianlin.xyz/gtnnbgpogt.html

Ruby: exit 1
来源：http://hz.yj20258888.top/gtkibzaeeu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shanyushiyangtech.top/gtzscgfifh.html

[M06] 向标准错误输出
来源：http://hz.0kj1m.cn/gtymckxkmw.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sxryk.cn/gtcohbrgek.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jlsjyb.cn/gtsuswgupx.html

JS:   console.error("err")
来源：http://hz.xylfe.cn/gtphsavsxh.html

TS:   console.error("err")
来源：http://hz.jqgufenzy.top/gtsgtsbtxd.html

Java: System.err.println("err")
来源：http://hz.feifeiyinyue.top/gtqbywvazu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhongyouzk.top/gtgqoulhep.html

Ruby: warn "err"
来源：http://hz.jianghu66.top/gtcfqsckqv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hysaishi.cn/gtnhopcwrz.html

[M07] 判断是否为主入口
来源：http://hz.gzhubu.top/gtewmsunst.html

Py:   if __name__ == "__main__":
来源：http://hz.shanyushiyangkeji.top/gtbfizmtlg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yongpay.top/gtgupvbkix.html

JS:   require.main === module
来源：http://hz.yj20258.top/gtvchhdmuv.html

TS:   require.main === module
来源：http://hz.hfpthk.cn/gtwuiyrtav.html

Java: public static void main(String[] args)
来源：http://hz.wangdashe.top/gtxageoban.html

Go:   func main()
来源：http://hz.hammf.cn/gtnugbmxqf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hnxiangtu.top/gtdxkszxgh.html

C#:   static void Main(string[] args)
来源：http://hz.zhongyouzk.top/gtvsimzwxs.html

[M08] 获取系统与运行时信息
来源：http://hz.xingfuxueyuan.xyz/gtrvxvqtet.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hongshengwenyu.top/gtflcswnbp.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xingfuxueyuan.xyz/gtpzloopft.html

JS:   process.platform;  process.version
来源：http://hz.yangfankeji.com/gtgiolrapw.html

TS:   process.platform;  process.version
来源：http://hz.pengpengdd.cyou/gtnzabawmd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zdqjudy.top/gtptxkjxkv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.fengsongda.top/gtxtcnvnwf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.guannengcc.top/gtnecrvqdm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ydzc1.top/gtyekmlstn.html

================================================================================
来源：http://hz.zdqjudy.top/gtmsqnglhp.html

N. 数据结构与算法
来源：http://hz.cqqwz.cn/gtrihmocel.html

================================================================================
来源：http://hz.daria6918.cn/gtjkkngxky.html

[N01] 二分查找（有序数组）
来源：http://hz.ppjwa.cn/gttghphtlu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.tianlin.xyz/gtcdbbgyrg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cqqwz.cn/gtdewrgdok.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cqqwz.cn/gtpfndpemk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dianchejie.cn/gtwbuuhlkf.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.nanxinkj.top/gteeomkxla.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.chenzaomai.com/gtjitdbdfo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yueranfly.top/gtjiqfpvoc.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xylfe.cn/gtijfnhnoe.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yangfankeji.com/gtssehjzqn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinghuilouyu.cn/gtehxoluft.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.iojbl.cn/gttsfehxub.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.52xcode.cn/gtyezsxuer.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinqigfzy.top/gtqtmglbzc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.birdmap.top/gtwxwlnpvj.html

Go:   slices.Sort(arr)
来源：http://hz.yangfankeji.com/gtvdvttewj.html

Ruby: arr.sort
来源：http://hz.cdnleiting.top/gtcsxtsnyu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cucudq.cn/gtiiwqvczs.html

[N03] 快速排序（分治示例）
来源：http://hz.zhiwuduotai.top/gtauhqmdwj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gzhubu.top/gthmmoloyd.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cashguo.top/gtpuqnelwg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yueranfly.top/gtgipgykmz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dianchejie.cn/gtcwwzapiy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shanyushiyangkeji.top/gthlaikgtu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yonumen.top/gtqnyxxxhn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yueranfly.top/gtzdolddxz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cucudq.cn/gtonudkvhc.html

[N04] 斐波那契数列
来源：http://hz.zycfv.cn/gtrxvglaes.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xylfe.cn/gtxzkgabve.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.316326.xyz/gtvtdcdmme.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.wangshuangyany.cn/gtuivpkxpj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.iojbl.cn/gtlaorsvgz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.andypj.xyz/gtxctruyyn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.snrcjt.cn/gtxxfincxb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hnqzz.top/gtwtjrkrja.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sufxvd.cn/gtvrvlhayz.html

[N05] 最大公约数
来源：http://hz.cdnleiting.top/gtqvlmwhow.html

Py:   math.gcd(a, b)
来源：http://hz.zhiwuduotai.top/gtdmajbxqb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yanxiufei.cn/gtwgzkhbhs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nanxinkj.top/gtocsmntvp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yanxiufei.cn/gtqxtgsjpc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ehwqpu.com/gtkzkyqcwd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ydjk.org.cn/gtmrrvcmtw.html

Ruby: a.gcd(b)
来源：http://hz.yongpay.top/gtuvnirvod.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.haohaochexian.top/gtdqvwiayd.html

[N06] 判断回文字符串
来源：http://hz.ybcxt.top/gtgbjgcqaz.html

Py:   s == s[::-1]
来源：http://hz.xylfe.cn/gtgcveekls.html

PHP:  $s === strrev($s);
来源：http://hz.zhengqikj.top/gtbiwkytbk.html


<!-- 参考信息 -->