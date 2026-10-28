代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.daria6918.cn/gtiovjsqbz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinqigfzy.top/gtdtpwaabx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhixingplan.top/gtkxbkbhgq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.sufxvd.cn/gtcnrrzbey.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cucudq.cn/gtkjeqmdkm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhijiandao.cn/gtclophebg.html

[J09] 时区处理
来源：http://hz.tanke756.top/gtjbtyiyid.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jianghu66.top/gtthmvkanz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.tian-w.cn/gtefcbjdpv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yueranfly.top/gtiaqogoql.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jyoumei.cn/gtljgerfpz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.guannengcc.top/gtirkiqqlt.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sweek.top/gtqzdylxde.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.meibo888.top/gtswqdfwmu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.haohaochexian.top/gtcpxgckre.html

[J10] 取今天 / 本月第一天
来源：http://hz.gotoacloud.top/gtlxcncybq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shuidangran.top/gttxvxnuqp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.redwolf501.top/gtfhngiykh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.316326.xyz/gtrlsfshkm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.smart0.xyz/gtonmcalqf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinyuanbaomall.cn/gtozhbbgjs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xingfuxueyuan.xyz/gtehiukgaj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.tianlin.xyz/gtrhednkuf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.dashuyun.cn/gtcdbdyywp.html

================================================================================
来源：http://hz.tian-w.cn/gthgkqosqk.html

K. JSON 与序列化
来源：http://hz.hongshengwenyu.top/gtjwalfjlt.html

================================================================================
来源：http://hz.hammf.cn/gtvozlfbea.html

[K01] 对象转 JSON 字符串
来源：http://hz.jqgufenzy.top/gtbwyytbzo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xuanzx.com/gttcnrnimx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.52xcode.cn/gttchjcesx.html

JS:   JSON.stringify(obj)
来源：http://hz.feifeiyinyue.top/gtohsgoqyq.html

TS:   JSON.stringify(obj)
来源：http://hz.nanxuanxn.top/gtuzebadyo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jianghu66.top/gtakzuzizn.html

Go:   json.Marshal(obj)
来源：http://hz.bjfxy.top/gtpywamewl.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.9152youxi.cn/gtvcoqffjl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hongshengwenyu.top/gttgywvppt.html

[K02] JSON 字符串转对象
来源：http://hz.jianghu66.top/gtspzixylj.html

Py:   json.loads(s)
来源：http://hz.ehwqpu.com/gtszoumzpg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.9152youxi.cn/gtlhosqgxq.html

JS:   JSON.parse(s)
来源：http://hz.haohaochexian.top/gtoazkhfye.html

TS:   JSON.parse(s)
来源：http://hz.xuetiantiany.cn/gtodueyjkr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.9152youxi.cn/gtmqmlfnjf.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.andypj.xyz/gteflarpdo.html

Ruby: JSON.parse(s)
来源：http://hz.nanxinkj.top/gtpevsddnz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.wangdashe.top/gtschfofqr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.dashuyun.cn/gtcndtoznc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shangyingyoupin.top/gtrdtbcwmb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hammf.cn/gtehlfeihr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.guannengcc.top/gtfahamzum.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.andypj.xyz/gtpxpqksfp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.redwolf501.top/gtmaqnyvxg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cashguo.top/gtwnwqdjac.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ehwqpu.com/gtwbmcjavw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tianlin.xyz/gtnxdiycnw.html

[K04] 读取 JSON 文件
来源：http://hz.sufxvd.cn/gtbbqlpvjq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.dashuyun.cn/gtmoyunygb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yj20258.top/gtyczvvivp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.0kj1m.cn/gtrermuuag.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yvedp.cn/gtpofzlcuq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinqigfzy.top/gtyzvbdcrr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xziqi.cn/gtgvcnftdn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gaohongyu789.top/gtkcqdzvgu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shuidangran.top/gtjejqnlic.html

[K05] 深拷贝对象
来源：http://hz.dashuyun.cn/gtxchvmjvk.html

Py:   copy.deepcopy(obj)
来源：http://hz.haohaochexian.top/gtjrjarwty.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jlsjyb.cn/gthlzuzwkr.html

JS:   structuredClone(obj)
来源：http://hz.tian-w.cn/gtloaqcdkr.html

TS:   structuredClone(obj)
来源：http://hz.tian-w.cn/gtibdapdvb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jlsjyb.cn/gtodzehpvh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.iojbl.cn/gtdjzoyzrw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.tanke756.top/gtdxeeuivd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhijiandao.cn/gtdfcjmdju.html

[K06] 解析 URL 查询串
来源：http://hz.zhijiandao.cn/gtirnogcyj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hongshengwenyu.top/gtqfaashyq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xuetiantiany.cn/gtonoyvaro.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zdqjudy.top/gtqsjwzahq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yueranfly.top/gtaxddnqoc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yanxiufei.cn/gtrbuhphei.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shzxlz.cn/gtpifnhqbe.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinghuilouyu.cn/gtxwagsrby.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.aibaodan.cn/gtjtgrmgwv.html

[K07] 进制转换
来源：http://hz.daria6918.cn/gtphmuoexp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shuidangran.top/gtqcvevcgh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cqqwz.cn/gtghygxpjp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jyoumei.cn/gtvhalgmrc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.snrcjt.cn/gtlubjbqgj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.guowangkeji.top/gtmsvrxhwe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jqgufenzy.top/gtjwjkruma.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yj202588.top/gtodxhfncu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gotoacloud.top/gtmetaezra.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jqgufenzy.top/gtyngjovra.html

Py:   pickle.dumps(obj)
来源：http://hz.hammf.cn/gtorugrbsv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shanyushiyangkeji.top/gtnjbxvxpd.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.52xcode.cn/gtuctesnne.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.guannengcc.top/gtoaqjkvyv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.cashguo.top/gtypdbsvcg.html

Go:   encoding/gob
来源：http://hz.ppjwa.cn/gtkhdhzhnf.html

Ruby: Marshal.dump(obj)
来源：http://hz.vqdsnc.cn/gtxtnximqa.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.meibo888.top/gtexrehjfo.html

================================================================================
来源：http://hz.havefunace.top/gtsqypjqgs.html

L. 网络请求
来源：http://hz.jianghu66.top/gtkdfvxljm.html

================================================================================
来源：http://hz.sysykeji.top/gtnpbxxkvb.html

[L01] 发送 GET 请求
来源：http://hz.yueranfly.top/gtfhmduwot.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hammf.cn/gtgbizkrld.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jinghuilouyu.cn/gtobjuxngn.html

JS:   await fetch(url)
来源：http://hz.jianghu66.top/gtmhtoridd.html

TS:   await fetch(url)
来源：http://hz.meibo888.top/gtajlgcdrt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ppjwa.cn/gtufcywdhl.html

Go:   resp, err := http.Get(url)
来源：http://hz.shanyushiyangkeji.top/gtuorofvos.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.tian-w.cn/gtlpsgytsi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.smart0.xyz/gtgfkxstgy.html

[L02] 发送 POST JSON
来源：http://hz.fengsongda.top/gtlqpqzdbj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.tanke756.top/gteyewjhpj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.aizwys.cn/gtdllojlrk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ppjwa.cn/gtcxgyguox.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gogol.net.cn/gtmqgqmqar.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yueranfly.top/gtoouyaoyu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yuxming.cn/gtklrqnqeo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zycfv.cn/gtkuidfjii.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.bjfxy.top/gtszwndkuw.html

[L03] 设置自定义请求头
来源：http://hz.redwolf501.top/gtitijwvyx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xingfuxueyuan.xyz/gtnpbcbcil.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.birdmap.top/gtbsxcqrbe.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.birdmap.top/gtlyksgtvd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.9152youxi.cn/gtleslkmqu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xingfuxueyuan.xyz/gtxshxavoe.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.snrcjt.cn/gttxlsstuk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cashguo.top/gtijokdini.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yj202588.top/gtzinnwesk.html

[L04] 设置超时
来源：http://hz.yanxiufei.cn/gtafxiaids.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cashguo.top/gtsbkrcuwo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.0kj1m.cn/gtcfxhoquz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhengqikj.top/gtmmvryxot.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yangfankeji.com/gtcifcjeex.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ydjk.org.cn/gtsmbkcskc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.tian-w.cn/gtyjzzqoaw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.pycfn.com/gtfakpewar.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.dianchejie.cn/gtxlmijiou.html

[L05] 上传文件（multipart）
来源：http://hz.kuanghao11.cn/gtryaehuzt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hnqzz.top/gtcnzzqmno.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ywan-chungtsiang.top/gtpazxbigt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hysaishi.cn/gtspzpdprw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.nwbrower.top/gtdpytyhug.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.guowangkeji.top/gtzzoeavws.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shanyushiyangtech.top/gtswptcxem.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jqgufenzy.top/gtefkdmwfr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cdnleiting.top/gtbkozszxx.html

[L06] 解析响应为 JSON
来源：http://hz.hnxiangtu.top/gtzezkhtvk.html

Py:   resp.json()
来源：http://hz.chenzaomai.com/gteohsutrw.html

PHP:  json_decode($body, true);
来源：http://hz.ehwqpu.com/gtiizrqjrm.html

JS:   await resp.json()
来源：http://hz.zhoulong.xyz/gtvrjfijbi.html

TS:   await resp.json()
来源：http://hz.jqgfzy.top/gttxogwzle.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jqgfzy.top/gtnjfoimrd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.wangdashe.top/gtjuvlvfkb.html

Ruby: JSON.parse(resp.body)
来源：http://hz.snrcjt.cn/gtdqkdejht.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.haohaochexian.top/gtpvudtnqd.html

[L07] 处理 HTTP 状态码
来源：http://hz.nanxinkj.top/gtesrbeezj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.tanke756.top/gtqxdzolll.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.kuanghao11.cn/gtdzccdpwb.html

JS:   resp.ok;  resp.status
来源：http://hz.yj20258.top/gtxuuhzzgh.html

TS:   resp.ok;  resp.status
来源：http://hz.pycfn.com/gtauzgyzam.html

Java: resp.statusCode()
来源：http://hz.dashuyun.cn/gtxdctheoe.html

Go:   resp.StatusCode
来源：http://hz.xuanzx.com/gtyrcynngv.html

Ruby: resp.code.to_i
来源：http://hz.hammf.cn/gtcauqwjhw.html

C#:   (int)resp.StatusCode
来源：http://hz.jlsjyb.cn/gtceywtfkp.html

[L08] 并发请求多个地址
来源：http://hz.hnqzz.top/gtownfrlfj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yvedp.cn/gtnmiqxzpa.html

PHP:  curl_multi_init() 系列
来源：http://hz.kuanghao11.cn/gtbffmlitw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jianghu66.top/gtuyagfnal.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.kuanghao11.cn/gtzqzuqsyp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jiagoushi.top/gtxbwhcpce.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.0kj1m.cn/gtquptjzzk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinqigufen.top/gtufhxroxt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shangyingyoupin.top/gtxkuclvlv.html

================================================================================
来源：http://hz.c1oappe.top/gtswowhdix.html

M. 命令行 / 进程 / 环境
来源：http://hz.ydzc1.top/gtygiwicfz.html

================================================================================
来源：http://hz.havefunace.top/gtxfdnlrcg.html

[M01] 读取命令行参数
来源：http://hz.c1oappe.top/gtsnjapbfh.html

Py:   sys.argv[1:]
来源：http://hz.birdmap.top/gtttzonqql.html

PHP:  $argv;  $argc;
来源：http://hz.jiagoushi.top/gtukukbyez.html

JS:   process.argv.slice(2)
来源：http://hz.cheryme.top/gtcuoybdlq.html

TS:   process.argv.slice(2)
来源：http://hz.jiagoushi.top/gtutldokzg.html

Java: args 数组（main 方法参数）
来源：http://hz.shzxlz.cn/gtsjrgpnga.html

Go:   os.Args[1:]
来源：http://hz.zhiwuduotai.top/gtnzdiowyj.html

Ruby: ARGV
来源：http://hz.aibaodan.cn/gtqlujtxse.html

C#:   args 数组（Main 方法参数）
来源：http://hz.nanxinkj.top/gtczlgwzyb.html

[M02] 读取环境变量
来源：http://hz.kuanghao11.cn/gttokcspdl.html

Py:   os.environ.get("HOME")
来源：http://hz.mhx1999.top/gtidatosfz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jlsjyb.cn/gtpiolvyls.html

JS:   process.env.HOME
来源：http://hz.yueranfly.top/gtvjfdeaxx.html

TS:   process.env.HOME
来源：http://hz.dashuyun.cn/gtmvbkucqx.html

Java: System.getenv("HOME")
来源：http://hz.dianchejie.cn/gtagoveinc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yj20258.top/gtbcbmehpf.html

Ruby: ENV["HOME"]
来源：http://hz.jiagoushi.top/gtvfppiyfw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.guannengcc.top/gtjnnqlgix.html

[M03] 执行外部命令
来源：http://hz.52xcode.cn/gtovfqiyhj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhijiandao.cn/gtxaxzpfof.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cqqwz.cn/gtiunipfps.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhijiandao.cn/gtivmwsjbr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinghuilouyu.cn/gtnrjturoo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yanxiufei.cn/gtnufjfhyb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hnxiangtu.top/gtiedellxd.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.fengsongda.top/gtlclrgaeb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yangfankeji.com/gtmchxchqe.html

[M04] 获取当前工作目录
来源：http://hz.quarkkingdee.top/gteflsrfwu.html

Py:   os.getcwd()
来源：http://hz.yonumen.top/gtwzhckzkh.html

PHP:  getcwd();
来源：http://hz.jlsjyb.cn/gtcsvbutna.html

JS:   process.cwd()
来源：http://hz.jianghu66.top/gtsdxogigl.html

TS:   process.cwd()
来源：http://hz.pengpengdd.cyou/gtraswpndd.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinghuilouyu.cn/gtnzclaqur.html

Go:   os.Getwd()
来源：http://hz.316326.xyz/gtqzndpnto.html

Ruby: Dir.pwd
来源：http://hz.0kj1m.cn/gtdhchglqh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.guannengcc.top/gtsnvcsfqs.html

[M05] 设置退出码
来源：http://hz.snrcjt.cn/gtxsxjdeje.html

Py:   sys.exit(1)
来源：http://hz.yanxiufei.cn/gtxbkzomdv.html

PHP:  exit(1);
来源：http://hz.mhx1999.top/gtpfiizvtp.html

JS:   process.exit(1)
来源：http://hz.zhijiandao.cn/gtcfoockfw.html

TS:   process.exit(1)
来源：http://hz.yj20258888.top/gtsyomelzc.html

Java: System.exit(1)
来源：http://hz.kuanghao11.cn/gtcfatltpu.html

Go:   os.Exit(1)
来源：http://hz.yvedp.cn/gtiapgvqqv.html

Ruby: exit 1
来源：http://hz.hammf.cn/gtepespame.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ppjwa.cn/gthvbpiafx.html

[M06] 向标准错误输出
来源：http://hz.zhixingplan.top/gtnmkhutwp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhoulong.xyz/gtdkntndmp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.fzhhl.top/gtkhgcodvp.html

JS:   console.error("err")
来源：http://hz.jianghu66.top/gtaolxwioy.html

TS:   console.error("err")
来源：http://hz.hnqzz.top/gtaslvdypk.html

Java: System.err.println("err")
来源：http://hz.smart0.xyz/gtfstwnqrd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yanxiufei.cn/gteeirbsdy.html

Ruby: warn "err"
来源：http://hz.ppjwa.cn/gtxpuahbid.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.daria6918.cn/gtveczyaaq.html

[M07] 判断是否为主入口
来源：http://hz.meibo888.top/gtcvvceijv.html

Py:   if __name__ == "__main__":
来源：http://hz.ppjwa.cn/gtasflhzyw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.wangshuangyany.cn/gthqyddhqm.html

JS:   require.main === module
来源：http://hz.gzhubu.top/gtgkmnskzd.html

TS:   require.main === module
来源：http://hz.birdmap.top/gtnlugbkcn.html

Java: public static void main(String[] args)
来源：http://hz.fengsongda.top/gtvtjctsqm.html

Go:   func main()
来源：http://hz.sysykeji.top/gtiwchzgqt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinghuilouyu.cn/gtnznqoqub.html

C#:   static void Main(string[] args)
来源：http://hz.yangfankeji.com/gtcrtymihk.html

[M08] 获取系统与运行时信息
来源：http://hz.sysykeji.top/gtctgazavq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.kuanghao11.cn/gtvidatqlb.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.sxryk.cn/gthkgpncul.html

JS:   process.platform;  process.version
来源：http://hz.zhaomingkeji.xyz/gtnifunlil.html

TS:   process.platform;  process.version
来源：http://hz.gaohongyu789.top/gtdrlstnig.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yvedp.cn/gtxttejwee.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.daxiang520.top/gtrmacjawt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jlsjyb.cn/gtogmuueod.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.guowangkeji.top/gthwjnkbqy.html

================================================================================
来源：http://hz.tian-w.cn/gtdrzeifgs.html

N. 数据结构与算法
来源：http://hz.quarkkingdee.top/gtiwvqrosk.html

================================================================================
来源：http://hz.gzhubu.top/gtzxzhkzuu.html

[N01] 二分查找（有序数组）
来源：http://hz.aizwys.cn/gtfzabpshs.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yj20258.top/gtcyifsmwe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.guannengcc.top/gtqvedwefr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ydzc1.top/gtghkftaig.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhijiandao.cn/gtlcoztqtt.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.nanxinkj.top/gthbiaaope.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shanyushiyangtech.top/gtcfpttzpf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhengqikj.top/gtnedukjpi.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yonumen.top/gtugbgknjd.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.guowangkeji.top/gtqyokkzor.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.316326.xyz/gtkpwsudqw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.guannengcc.top/gtngmgpnaw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yangfankeji.com/gtrbspydov.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj202588.top/gtrfhervkn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.quarkkingdee.top/gtsdougrrh.html

Go:   slices.Sort(arr)
来源：http://hz.daxiang520.top/gtovrsqori.html

Ruby: arr.sort
来源：http://hz.jiagoushi.top/gtgytxjiui.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.iojbl.cn/gtwemrmvru.html

[N03] 快速排序（分治示例）
来源：http://hz.jinyuanbaomall.cn/gtiykrsxvt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yuxming.cn/gtgjnhfxgg.html

PHP:  // 递归实现，或用 usort
来源：http://hz.nanxuanxn.top/gtrlczwepp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.316326.xyz/gtphqhxkcx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenjidiqi.icu/gtqaeleoru.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj20258888.top/gtakdhvsfr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.haohaochexian.top/gtqualkajy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jinghuilouyu.cn/gtfaxqjrxj.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.pycfn.com/gtpgpetmrz.html

[N04] 斐波那契数列
来源：http://hz.gogol.net.cn/gtagvvyszd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.mhx1999.top/gtgnqzivpw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cucudq.cn/gtfdinsgov.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jianghu66.top/gtzlzvlqec.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxinkj.top/gteogqamrn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.52xcode.cn/gtwosczpyq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yj20258.top/gtbbzxtghw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yuanzhike.top/gtzmvaekpk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.wangshuangyany.cn/gtjxfbjlbb.html

[N05] 最大公约数
来源：http://hz.redwolf501.top/gtiwevlgxd.html

Py:   math.gcd(a, b)
来源：http://hz.chenlongwang.top/gtqnozldtg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.chenlongwang.top/gtggimvect.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.redwolf501.top/gthtkltqmo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangshuangyany.cn/gtdzeyltar.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.nwbrower.top/gtedqigpmb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ppjwa.cn/gtlxiyosqc.html

Ruby: a.gcd(b)
来源：http://hz.yuxming.cn/gtregxwmzb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gotoacloud.top/gtzdmejzss.html

[N06] 判断回文字符串
来源：http://hz.iojbl.cn/gtbjwgbhrx.html

Py:   s == s[::-1]
来源：http://hz.yongpay.top/gtuuqwfcef.html

PHP:  $s === strrev($s);
来源：http://hz.jyoumei.cn/gtqrfyndbm.html


<!-- 参考信息 -->