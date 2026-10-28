代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cdnleiting.top/gtokdvhjiw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.meibo888.top/gtrztryilr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jianghu66.top/gtaunbkuck.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.quarkkingdee.top/gtvuacimmy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cashguo.top/gtpxttybjt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.guannengcc.top/gtzhnmpphv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.wangshuangyany.cn/gtnsudtkub.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinyuanbaomall.cn/gtrbjbznqh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shanyushiyangkeji.top/gtcdrudrgp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sxryk.cn/gtqevgarwb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hfpthk.cn/gthxdqpykv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinghuilouyu.cn/gtcxlklmcz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.daxiang520.top/gtckosneno.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hysaishi.cn/gtapdatlub.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cucudq.cn/gtlbbtegiw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yonumen.top/gtmbngmnja.html

================================================================================
来源：http://hz.fengsongda.top/gthgfgzcxw.html

K. JSON 与序列化
来源：http://hz.ehwqpu.com/gttanesabs.html

================================================================================
来源：http://hz.sweek.top/gtuqiejuwc.html

[K01] 对象转 JSON 字符串
来源：http://hz.ywan-chungtsiang.top/gtvdwmnpzc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yanxiufei.cn/gtmwzgodmp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.kuanghao11.cn/gtwvqeuboz.html

JS:   JSON.stringify(obj)
来源：http://hz.tian-w.cn/gtmckyivwu.html

TS:   JSON.stringify(obj)
来源：http://hz.guannengcc.top/gtyyevdflh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ydzc1.top/gtckkcongt.html

Go:   json.Marshal(obj)
来源：http://hz.jiagoushi.top/gthzbcnpmn.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.tian-w.cn/gtpgdypchh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.daxiang520.top/gtdlmbymqu.html

[K02] JSON 字符串转对象
来源：http://hz.xuanzx.com/gtefwxjsvp.html

Py:   json.loads(s)
来源：http://hz.9152youxi.cn/gtwkbfzqag.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.chenjidiqi.icu/gtahctfpph.html

JS:   JSON.parse(s)
来源：http://hz.xuetiantiany.cn/gtfxpjrarz.html

TS:   JSON.parse(s)
来源：http://hz.cashguo.top/gtghynatrc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.pycfn.com/gtzhngrzwj.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.aibaodan.cn/gtosyfdebl.html

Ruby: JSON.parse(s)
来源：http://hz.zdqjudy.top/gtehwnrqgo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shangyingyoupin.top/gtrubibien.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ydjk.org.cn/gtwxlvzjzx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yueranfly.top/gtgtxtqbbi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.fzhhl.top/gtqtuqnrtb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xingfuxueyuan.xyz/gtdsaccgie.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shangyingyoupin.top/gttmughgqw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jiagoushi.top/gtfwjmsyiw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.sxryk.cn/gtozdyxybf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jiagoushi.top/gtilmcvkbo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhongyouzk.top/gterarvfrl.html

[K04] 读取 JSON 文件
来源：http://hz.ydjk.org.cn/gtidgqjghq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhengqikj.top/gtyopbaitc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hongshengwenyu.top/gtbvdzquts.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jianghu66.top/gtiarcxcoz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guowangkeji.top/gtvwyvkvbh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.dashuyun.cn/gtxkzeaefu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.nwbrower.top/gttqjbhqpi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.redwolf501.top/gtmvsibauu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhaomingkeji.xyz/gtsdqxaaze.html

[K05] 深拷贝对象
来源：http://hz.fengsongda.top/gtlznosdgt.html

Py:   copy.deepcopy(obj)
来源：http://hz.sweek.top/gtzgylorwo.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xinyue.icu/gtnhdsonrq.html

JS:   structuredClone(obj)
来源：http://hz.wangshuangyany.cn/gttlobcbbq.html

TS:   structuredClone(obj)
来源：http://hz.52xcode.cn/gtmkpeoyov.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.chenzaomai.com/gtrrvzjmco.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.316326.xyz/gtoutmveyq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.aizwys.cn/gtqocfrexw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.guowangkeji.top/gtosoklhjs.html

[K06] 解析 URL 查询串
来源：http://hz.mhx1999.top/gtwzksiekm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.fengsongda.top/gtohornqnu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.aibaodan.cn/gtzjacadke.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hammf.cn/gttpbbtjgc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ppjwa.cn/gthnvxcbtb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.gogol.net.cn/gtbayxmxhn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.tian-w.cn/gtiypehbsq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhengqikj.top/gtdofzpoal.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xuanzx.com/gtnsucmcwy.html

[K07] 进制转换
来源：http://hz.jinqigufen.top/gtlkgwyngz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yj202588.top/gtkkbecrdu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.bjfxy.top/gtqgpmbnym.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.52xcode.cn/gtbwhieujy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xinyue.icu/gtnntvznpq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.sufxvd.cn/gtyscmzfrt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hnxiangtu.top/gtffqlhlbo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jqgufenzy.top/gtjbwnwikx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gogol.net.cn/gtazfaahgj.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zdqjudy.top/gtpvqpstyv.html

Py:   pickle.dumps(obj)
来源：http://hz.shanyushiyangtech.top/gtzxfllgoy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.birdmap.top/gtbcfoybbs.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.meibo888.top/gtucamycro.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.52xcode.cn/gtornebmbz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.0kj1m.cn/gtcfhpxmsm.html

Go:   encoding/gob
来源：http://hz.svipenyu.cn/gtshwkvlno.html

Ruby: Marshal.dump(obj)
来源：http://hz.nwbrower.top/gttksgrhbz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.iojbl.cn/gtfkllqpjg.html

================================================================================
来源：http://hz.ydzc1.top/gtijxsmbbi.html

L. 网络请求
来源：http://hz.316326.xyz/gttfumxbnu.html

================================================================================
来源：http://hz.yj20258.top/gtygycavkh.html

[L01] 发送 GET 请求
来源：http://hz.jqgfzy.top/gtmapgyhsi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.feifeiyinyue.top/gtnwwmxptr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.nwbrower.top/gtnzjavwhq.html

JS:   await fetch(url)
来源：http://hz.cdnleiting.top/gtxkrafmya.html

TS:   await fetch(url)
来源：http://hz.xuetiantiany.cn/gtlkhcwxkk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jqgufenzy.top/gtauyveihe.html

Go:   resp, err := http.Get(url)
来源：http://hz.cashguo.top/gtphwlmfeg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shuidangran.top/gttnolhauo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.feifeiyinyue.top/gtqfqbuqxe.html

[L02] 发送 POST JSON
来源：http://hz.iojbl.cn/gtszjfbeim.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hfpthk.cn/gtefmidxni.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sufxvd.cn/gttymxrars.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinghuilouyu.cn/gtdnptpflh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.aizwys.cn/gtnvgokoki.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xuetiantiany.cn/gtqsscybpv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhengqikj.top/gtasccdpxe.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xinyue.icu/gtnqzehlmg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yuxming.cn/gtnakubwdc.html

[L03] 设置自定义请求头
来源：http://hz.yueranfly.top/gtdlsiugsu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yj202588.top/gtregxipzx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xuanzx.com/gtwgqozkqz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hnqzz.top/gtmmfdtwlt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ivvv.top/gtiooabmvz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cdnleiting.top/gtqgwffnhv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.sysykeji.top/gtjekzhmbh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.fengsongda.top/gtjjqxlhoi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jyoumei.cn/gtzwborxhy.html

[L04] 设置超时
来源：http://hz.yvedp.cn/gtvhbsoofg.html

Py:   requests.get(url, timeout=5)
来源：http://hz.chenlongwang.top/gtnsbfdgph.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhixingplan.top/gtwxenrnwf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tianlin.xyz/gtatoiitrs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gzhubu.top/gtiuvyefbg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.tanke756.top/gtnycwhatu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.c1oappe.top/gtbgzaqdaa.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yvedp.cn/gtxmhenxzn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhaomingkeji.xyz/gtwfvwstgv.html

[L05] 上传文件（multipart）
来源：http://hz.yj202588.top/gtyhlyqbln.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cheryme.top/gthbdtsaqj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.dianchejie.cn/gtcngisvgb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinqigufen.top/gtikcczgtk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.redwolf501.top/gtbiawcycy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.aizwys.cn/gtmqnkwgah.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.daxiang520.top/gtlzlwnfqc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yuxming.cn/gtqhiwgnwx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gaohongyu789.top/gtqncxjchr.html

[L06] 解析响应为 JSON
来源：http://hz.zhiwuduotai.top/gtlklkfaxx.html

Py:   resp.json()
来源：http://hz.chenlongwang.top/gtbsmltjog.html

PHP:  json_decode($body, true);
来源：http://hz.jianghu66.top/gtcvazkemg.html

JS:   await resp.json()
来源：http://hz.sufxvd.cn/gthnsrfeem.html

TS:   await resp.json()
来源：http://hz.ehwqpu.com/gtdobbcoym.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.9152youxi.cn/gtwfigigfx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.iojbl.cn/gttqekmyao.html

Ruby: JSON.parse(resp.body)
来源：http://hz.gogol.net.cn/gtgwmiljcc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.bjfxy.top/gtiocwskfw.html

[L07] 处理 HTTP 状态码
来源：http://hz.quarkkingdee.top/gtuzdeilpk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yuxming.cn/gttxoqiolz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhongyouzk.top/gtfhxtsnua.html

JS:   resp.ok;  resp.status
来源：http://hz.c1oappe.top/gttkgncosy.html

TS:   resp.ok;  resp.status
来源：http://hz.cqqwz.cn/gtaqjbrhwh.html

Java: resp.statusCode()
来源：http://hz.yvedp.cn/gtviyxijna.html

Go:   resp.StatusCode
来源：http://hz.birdmap.top/gtcxepnaum.html

Ruby: resp.code.to_i
来源：http://hz.jianghu66.top/gtmoxdbyea.html

C#:   (int)resp.StatusCode
来源：http://hz.dianchejie.cn/gtkoizkswk.html

[L08] 并发请求多个地址
来源：http://hz.ivvv.top/gtoxidalcj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhixingplan.top/gtfmzvmgzy.html

PHP:  curl_multi_init() 系列
来源：http://hz.zycfv.cn/gtyumgmxxe.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxuanxn.top/gtpcjhrabj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.havefunace.top/gtlkrygils.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zycfv.cn/gtyiosrdek.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hysaishi.cn/gtazoouqom.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.fzhhl.top/gtzzxzzfnw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.316326.xyz/gtuqfyabjs.html

================================================================================
来源：http://hz.quarkkingdee.top/gtjtuythqq.html

M. 命令行 / 进程 / 环境
来源：http://hz.xuanzx.com/gtyqcnvpni.html

================================================================================
来源：http://hz.xinyue.icu/gtvrdkpfbq.html

[M01] 读取命令行参数
来源：http://hz.zhaomingkeji.xyz/gtzwjhccpn.html

Py:   sys.argv[1:]
来源：http://hz.yuxming.cn/gtuxffznuc.html

PHP:  $argv;  $argc;
来源：http://hz.gzhubu.top/gtbjhyrffo.html

JS:   process.argv.slice(2)
来源：http://hz.wangshuangyany.cn/gtmozddzjh.html

TS:   process.argv.slice(2)
来源：http://hz.cheryme.top/gtzpabvctj.html

Java: args 数组（main 方法参数）
来源：http://hz.sweek.top/gtccgkpubb.html

Go:   os.Args[1:]
来源：http://hz.mhx1999.top/gtcdwvlaae.html

Ruby: ARGV
来源：http://hz.daxiang520.top/gtsvsitvkc.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yuanzhike.top/gtbgtuquko.html

[M02] 读取环境变量
来源：http://hz.yj202588.top/gtyksvcoyy.html

Py:   os.environ.get("HOME")
来源：http://hz.shangyingyoupin.top/gtjnefgaxl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cheryme.top/gthwxnzfxz.html

JS:   process.env.HOME
来源：http://hz.jiagoushi.top/gtwescqnak.html

TS:   process.env.HOME
来源：http://hz.ppjwa.cn/gtrrimcgnx.html

Java: System.getenv("HOME")
来源：http://hz.hnxiangtu.top/gtdvcfxhtb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yueranfly.top/gtfmzqpqel.html

Ruby: ENV["HOME"]
来源：http://hz.jinghuilouyu.cn/gtzmvhzyjf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.sxryk.cn/gthipkkwso.html

[M03] 执行外部命令
来源：http://hz.feifeiyinyue.top/gthpoebjvn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yongpay.top/gtwysgnvig.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hfpthk.cn/gtlwttenes.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgufenzy.top/gtuxghixoh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xinyue.icu/gtotjxotgz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yuxming.cn/gtretowgoj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhiwuduotai.top/gtutibiwcf.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.chenlongwang.top/gtagjfrpao.html

C#:   Process.Start("ls", "-l");
来源：http://hz.mhx1999.top/gtzngwegyw.html

[M04] 获取当前工作目录
来源：http://hz.zycfv.cn/gtcbodndov.html

Py:   os.getcwd()
来源：http://hz.aizwys.cn/gtwljpdugl.html

PHP:  getcwd();
来源：http://hz.hysaishi.cn/gtrddslwii.html

JS:   process.cwd()
来源：http://hz.xuetiantiany.cn/gtynawcreo.html

TS:   process.cwd()
来源：http://hz.cdnleiting.top/gtggonrdna.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.c1oappe.top/gtkagzmcvo.html

Go:   os.Getwd()
来源：http://hz.guannengcc.top/gtnrzubybi.html

Ruby: Dir.pwd
来源：http://hz.shanyushiyangkeji.top/gthsplgcah.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.guannengcc.top/gtunkjrhld.html

[M05] 设置退出码
来源：http://hz.dianchejie.cn/gtxtfsifjp.html

Py:   sys.exit(1)
来源：http://hz.jinqigfzy.top/gtyuzqksea.html

PHP:  exit(1);
来源：http://hz.meibo888.top/gtcwdumgeb.html

JS:   process.exit(1)
来源：http://hz.yj202588.top/gtvkqvhbmn.html

TS:   process.exit(1)
来源：http://hz.jinqigufen.top/gtmzqywioj.html

Java: System.exit(1)
来源：http://hz.shanyushiyangtech.top/gtcqjelncf.html

Go:   os.Exit(1)
来源：http://hz.nwbrower.top/gtcllccaam.html

Ruby: exit 1
来源：http://hz.hnxiangtu.top/gtvmlyukav.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.quarkkingdee.top/gtioilxfmb.html

[M06] 向标准错误输出
来源：http://hz.hongshengwenyu.top/gthmqcsein.html

Py:   print("err", file=sys.stderr)
来源：http://hz.svipenyu.cn/gtqcfyboyj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.gzhubu.top/gtoeyjtoyf.html

JS:   console.error("err")
来源：http://hz.zhixingplan.top/gtsuisjxxt.html

TS:   console.error("err")
来源：http://hz.wangshuangyany.cn/gtnsuyxfdw.html

Java: System.err.println("err")
来源：http://hz.hywenlv.cn/gtwdxqobxq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.chenzaomai.com/gtsoifushr.html

Ruby: warn "err"
来源：http://hz.nanxuanxn.top/gtwkavepsp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.andypj.xyz/gtnkxramvh.html

[M07] 判断是否为主入口
来源：http://hz.iojbl.cn/gtaeltzbzh.html

Py:   if __name__ == "__main__":
来源：http://hz.yj20258.top/gtculemwmz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.nwbrower.top/gtvqhqlzhd.html

JS:   require.main === module
来源：http://hz.jinqigfzy.top/gtuuchrwtn.html

TS:   require.main === module
来源：http://hz.wangdashe.top/gtedtgeoof.html

Java: public static void main(String[] args)
来源：http://hz.birdmap.top/gtjxhdilcs.html

Go:   func main()
来源：http://hz.pengpengdd.cyou/gtvjkhmwom.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.daria6918.cn/gttxcdxhib.html

C#:   static void Main(string[] args)
来源：http://hz.jyoumei.cn/gtuuwyentv.html

[M08] 获取系统与运行时信息
来源：http://hz.xziqi.cn/gtuwcespro.html

Py:   platform.system();  platform.python_version()
来源：http://hz.kuanghao11.cn/gtckzzxjtr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.guowangkeji.top/gtihvayqnd.html

JS:   process.platform;  process.version
来源：http://hz.daxiang520.top/gtumtvtjbn.html

TS:   process.platform;  process.version
来源：http://hz.dashuyun.cn/gtjexoncjx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.daria6918.cn/gtcconbfes.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.0kj1m.cn/gtwwcvqcwu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.svipenyu.cn/gtrhgicwov.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sufxvd.cn/gteqjvdtnw.html

================================================================================
来源：http://hz.jianghu66.top/gtclilgirj.html

N. 数据结构与算法
来源：http://hz.jqgfzy.top/gtewxcupkq.html

================================================================================
来源：http://hz.yongpay.top/gtaufpokcc.html

[N01] 二分查找（有序数组）
来源：http://hz.xziqi.cn/gtmpcfnfae.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.smart0.xyz/gtkceudlfu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.vqdsnc.cn/gtvlgzxeuc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fzhhl.top/gtrzbdvwkh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yueranfly.top/gtfxoypydy.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yj20258.top/gttorubjbq.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cashguo.top/gtjdwgfpmz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhijiandao.cn/gtprezljjf.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yuxming.cn/gtnnhiylrf.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yj20258.top/gtlkivlfdd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.snrcjt.cn/gtaixbtcog.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.sysykeji.top/gtxfpnuxyu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.meibo888.top/gtswvnutox.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ivvv.top/gttbbpirnj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.dianchejie.cn/gtddishuez.html

Go:   slices.Sort(arr)
来源：http://hz.yangfankeji.com/gtwrpwmugm.html

Ruby: arr.sort
来源：http://hz.quarkkingdee.top/gtofzrqbuj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhaomingkeji.xyz/gtxokislms.html

[N03] 快速排序（分治示例）
来源：http://hz.iojbl.cn/gtkqiworsz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.snrcjt.cn/gteakiglev.html

PHP:  // 递归实现，或用 usort
来源：http://hz.daria6918.cn/gtbxvsbovc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.mhx1999.top/gtsnyjmuqu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jlsjyb.cn/gtjydsseiv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jiagoushi.top/gtavgonyzt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hnqzz.top/gtrkvxriml.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.guowangkeji.top/gtoebshppj.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.birdmap.top/gtddotaoyi.html

[N04] 斐波那契数列
来源：http://hz.ydjk.org.cn/gtdwrkvovz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.vqdsnc.cn/gtaeeycamj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shanyushiyangkeji.top/gtosbobtsi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hysaishi.cn/gtnzauiqaj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.0kj1m.cn/gtwbwckals.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhengqikj.top/gtyrbqqbdz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.guannengcc.top/gtyyxklbtg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.redwolf501.top/gtqkmokssl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhengqikj.top/gtbjcpqpfi.html

[N05] 最大公约数
来源：http://hz.yj20258888.top/gtfnmwxyqy.html

Py:   math.gcd(a, b)
来源：http://hz.wangdashe.top/gtcvuviwdl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.iojbl.cn/gtzrijfcmn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhoulong.xyz/gtrrdgdnfs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sysykeji.top/gtyordefdy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.daxiang520.top/gtovozrrse.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.0kj1m.cn/gtdrjkvask.html

Ruby: a.gcd(b)
来源：http://hz.jinyuanbaomall.cn/gtxhwijzlj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zdqjudy.top/gtbfhvdrnf.html

[N06] 判断回文字符串
来源：http://hz.ydzc1.top/gtevqwuypm.html

Py:   s == s[::-1]
来源：http://hz.9152youxi.cn/gtapuatrcy.html

PHP:  $s === strrev($s);
来源：http://hz.iojbl.cn/gtjgvvgnqz.html

JS:   s === [...s].reverse().join("")
来源：http://hz.pycfn.com/gtivrjzxgv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cheryme.top/gtouzdmrbn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cqqwz.cn/gtpctcvjpa.html

Go:   // 双指针从两端比较
来源：http://hz.tian-w.cn/gtgugaiezo.html

Ruby: s == s.reverse
来源：http://hz.yj20258.top/gtvdgvwcwv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ydjk.org.cn/gtfmxnshvb.html

[N07] 两数之和（返回下标）
来源：http://hz.daria6918.cn/gtbisltkjw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.kuanghao11.cn/gtvybwelfs.html


<!-- 参考信息 -->