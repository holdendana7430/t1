代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.316326.xyz/gtcdjwothu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.nanxuanxn.top/gtaqysdfvc.html

[J09] 时区处理
来源：http://hz.zycfv.cn/gtzaodpbzb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.havefunace.top/gthsufozji.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xinyue.icu/gtcinvpoky.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.smart0.xyz/gtgnqihslg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.aibaodan.cn/gthmioropt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.shanyushiyangtech.top/gtqynovoyg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.aibaodan.cn/gtjxekhlqo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinghuilouyu.cn/gtfmopvfxs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sxryk.cn/gtgncvocts.html

[J10] 取今天 / 本月第一天
来源：http://hz.yj20258.top/gtavjnkesk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yangfankeji.com/gtjzstvnib.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sysykeji.top/gtjuxmqtst.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.aizwys.cn/gtvvetruze.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.aibaodan.cn/gtctkjxdiw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.svipenyu.cn/gtntyuuxjp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xingfuxueyuan.xyz/gtxuulnxxp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhiwuduotai.top/gtlqvfllpt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zdqjudy.top/gturigkjkq.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtjrvtnmcg.html

K. JSON 与序列化
来源：http://hz.gotoacloud.top/gtiapjwbgn.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gttxjqzgke.html

[K01] 对象转 JSON 字符串
来源：http://hz.hfpthk.cn/gttxivepgm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yuxming.cn/gtwzckjkqx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ybcxt.top/gtsjsgdszz.html

JS:   JSON.stringify(obj)
来源：http://hz.hammf.cn/gtgsgbzzgt.html

TS:   JSON.stringify(obj)
来源：http://hz.sysykeji.top/gtvuvtyngl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhiwuduotai.top/gtbihjcwuq.html

Go:   json.Marshal(obj)
来源：http://hz.bjfxy.top/gtpdxzlzjg.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shanyushiyangtech.top/gtytjxcgbq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hysaishi.cn/gtcbrzhmjp.html

[K02] JSON 字符串转对象
来源：http://hz.sweek.top/gtflqnxunn.html

Py:   json.loads(s)
来源：http://hz.dianchejie.cn/gtegaddkoj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gzhubu.top/gtgwujrpqg.html

JS:   JSON.parse(s)
来源：http://hz.ywan-chungtsiang.top/gtptoxrotq.html

TS:   JSON.parse(s)
来源：http://hz.yuxming.cn/gtpwlaxrgn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.quarkkingdee.top/gtfvsakxov.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.dianchejie.cn/gtmgbzklnf.html

Ruby: JSON.parse(s)
来源：http://hz.feifeiyinyue.top/gtkeeixjgk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.andypj.xyz/gtjshbhgjo.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.mhx1999.top/gtbuodanlu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ybcxt.top/gtywgwgatg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ydjk.org.cn/gtxzdwiwdp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhoulong.xyz/gtkxjfwjkk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.meibo888.top/gtmgoayvgn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.kuanghao11.cn/gtwxnmaeoo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shanyushiyangkeji.top/gtgmuubobe.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sufxvd.cn/gtzfksvwic.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.mhx1999.top/gtzccdbtvg.html

[K04] 读取 JSON 文件
来源：http://hz.pycfn.com/gtptjteumr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jlsjyb.cn/gtkqiuyjvr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.mhx1999.top/gtgjxvzogf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.iojbl.cn/gtnbbwcvwn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.mhx1999.top/gthhotzbmm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhoulong.xyz/gtqevzhdml.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yvedp.cn/gtvsarhjnj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xuanzx.com/gtrkmnybgv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hnxiangtu.top/gtaihpidug.html

[K05] 深拷贝对象
来源：http://hz.yonumen.top/gtpicsjkrc.html

Py:   copy.deepcopy(obj)
来源：http://hz.yueranfly.top/gtwtaoortd.html

PHP:  unserialize(serialize($obj));
来源：http://hz.fzhhl.top/gtanvmtjrn.html

JS:   structuredClone(obj)
来源：http://hz.wangdashe.top/gtjlysgkpb.html

TS:   structuredClone(obj)
来源：http://hz.jiagoushi.top/gtfyxleluc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhiwuduotai.top/gtjwdhkqgg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.cheryme.top/gteohwpayn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yj20258888.top/gtacwvzlez.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.wangshuangyany.cn/gtozdhdqqn.html

[K06] 解析 URL 查询串
来源：http://hz.yuanzhike.top/gtqzvcoeno.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.birdmap.top/gthutywzma.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shanyushiyangkeji.top/gttmkratgu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jlsjyb.cn/gtfyjtabbf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zdqjudy.top/gtkakxmpmn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhiwuduotai.top/gtfxsuvvhg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ivvv.top/gtbvfqtqmo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ivvv.top/gtsdoeimzx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.wangshuangyany.cn/gtbkwumxdq.html

[K07] 进制转换
来源：http://hz.guowangkeji.top/gtpjhekmpq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cqqwz.cn/gtsluiagwo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tanke756.top/gtseywfunr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.quarkkingdee.top/gtxdjgdosd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xinyue.icu/gtbvwxhcok.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.birdmap.top/gttjndwsie.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.svipenyu.cn/gtcxcocznu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nanxinkj.top/gtouslgqbo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.fzhhl.top/gtyfnckwrj.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.snrcjt.cn/gtstoyatsd.html

Py:   pickle.dumps(obj)
来源：http://hz.hfpthk.cn/gtwuzrlcxq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.aibaodan.cn/gtkwxquxqr.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ppjwa.cn/gtdenglfln.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ydjk.org.cn/gtmbdiequk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenjidiqi.icu/gtvegjflhx.html

Go:   encoding/gob
来源：http://hz.jiagoushi.top/gtsguxrfoy.html

Ruby: Marshal.dump(obj)
来源：http://hz.ivvv.top/gtsthmfgdg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shuidangran.top/gtyfmqwrtp.html

================================================================================
来源：http://hz.gogol.net.cn/gtpjcvwtod.html

L. 网络请求
来源：http://hz.9152youxi.cn/gtxqfbjycv.html

================================================================================
来源：http://hz.gogol.net.cn/gtdtoyhray.html

[L01] 发送 GET 请求
来源：http://hz.xingfuxueyuan.xyz/gtjcofxcsm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cheryme.top/gtgejmhwpm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.wangdashe.top/gttvtdvpms.html

JS:   await fetch(url)
来源：http://hz.dashuyun.cn/gttdrbjxct.html

TS:   await fetch(url)
来源：http://hz.yanxiufei.cn/gthjbntzko.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gogol.net.cn/gtgkfddgxs.html

Go:   resp, err := http.Get(url)
来源：http://hz.yvedp.cn/gtfeawmyke.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhiwuduotai.top/gtbmqxjysj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cdnleiting.top/gtbesscqri.html

[L02] 发送 POST JSON
来源：http://hz.ppjwa.cn/gtjssutusy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hongshengwenyu.top/gtebbjmwjz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hnqzz.top/gtgldggtow.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhijiandao.cn/gtyasqsrtw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yangfankeji.com/gtxnjrccfo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jqgfzy.top/gtkirkscqa.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhijiandao.cn/gtgbuqxmae.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.9152youxi.cn/gtmdnesptf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zdqjudy.top/gtrjmtczyg.html

[L03] 设置自定义请求头
来源：http://hz.redwolf501.top/gtttrvgjjl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.aizwys.cn/gtsoujcmfs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gogol.net.cn/gtvlqiczjn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yongpay.top/gtvgbhpuuh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gogol.net.cn/gtoyubomvq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jinyuanbaomall.cn/gthvsctbqe.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.fzhhl.top/gtwipomwav.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hywenlv.cn/gtacifjwix.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nwbrower.top/gtcavqilva.html

[L04] 设置超时
来源：http://hz.jiagoushi.top/gtcttqjytr.html

Py:   requests.get(url, timeout=5)
来源：http://hz.aizwys.cn/gtamxskjuh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.9152youxi.cn/gtegiablov.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hongshengwenyu.top/gtyavlziiq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dashuyun.cn/gtwluzwwis.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.andypj.xyz/gtdkjcdfec.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zdqjudy.top/gtxbamhgap.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.feifeiyinyue.top/gtvkqqtnol.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.9152youxi.cn/gtaenjtwfz.html

[L05] 上传文件（multipart）
来源：http://hz.ehwqpu.com/gtrsmhtzfr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xylfe.cn/gtuauqxeyp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yvedp.cn/gtkpvbifdq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hongshengwenyu.top/gtmoyhkcgx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.kuanghao11.cn/gtznepohzp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.vqdsnc.cn/gtkxwkgenz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.52xcode.cn/gthgacvgva.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.c1oappe.top/gtpcxiviex.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ehwqpu.com/gtanwtsqfe.html

[L06] 解析响应为 JSON
来源：http://hz.jyoumei.cn/gtrnnkmxuq.html

Py:   resp.json()
来源：http://hz.cucudq.cn/gtwwmslgri.html

PHP:  json_decode($body, true);
来源：http://hz.jyoumei.cn/gtceepburs.html

JS:   await resp.json()
来源：http://hz.yj202588.top/gthzlynymw.html

TS:   await resp.json()
来源：http://hz.redwolf501.top/gtadlptsnf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.shzxlz.cn/gtzhtketzy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.9152youxi.cn/gtjzoykjad.html

Ruby: JSON.parse(resp.body)
来源：http://hz.bjfxy.top/gtzwhgvexu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ppjwa.cn/gtyxwzdfsl.html

[L07] 处理 HTTP 状态码
来源：http://hz.smart0.xyz/gtoujbjacu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cdnleiting.top/gttzkasihl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.chenzaomai.com/gtetxyccbs.html

JS:   resp.ok;  resp.status
来源：http://hz.ivvv.top/gthiuxqths.html

TS:   resp.ok;  resp.status
来源：http://hz.meibo888.top/gtdoeieqcn.html

Java: resp.statusCode()
来源：http://hz.yuxming.cn/gtvnsuuffj.html

Go:   resp.StatusCode
来源：http://hz.kuanghao11.cn/gtppobxnod.html

Ruby: resp.code.to_i
来源：http://hz.c1oappe.top/gtuvniiwyn.html

C#:   (int)resp.StatusCode
来源：http://hz.shzxlz.cn/gtpkipyyxm.html

[L08] 并发请求多个地址
来源：http://hz.cdnleiting.top/gtttfydigt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.smart0.xyz/gtsmesqjat.html

PHP:  curl_multi_init() 系列
来源：http://hz.shanyushiyangkeji.top/gtdlqotmwl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jiagoushi.top/gtmiqmizwj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.9152youxi.cn/gtuxnzbltz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hfpthk.cn/gtxmjqkpib.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xingfuxueyuan.xyz/gtauywxise.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.0kj1m.cn/gtzpegclol.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yuanzhike.top/gtyvzmmvnc.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtbeugqegm.html

M. 命令行 / 进程 / 环境
来源：http://hz.aizwys.cn/gtgdcwcjsh.html

================================================================================
来源：http://hz.zycfv.cn/gtjgpaidwg.html

[M01] 读取命令行参数
来源：http://hz.tanke756.top/gtqhivwitu.html

Py:   sys.argv[1:]
来源：http://hz.bjfxy.top/gtjddsjpxd.html

PHP:  $argv;  $argc;
来源：http://hz.c1oappe.top/gthzkcrfmt.html

JS:   process.argv.slice(2)
来源：http://hz.fengsongda.top/gtqsbahoyj.html

TS:   process.argv.slice(2)
来源：http://hz.xylfe.cn/gtrfwoelcn.html

Java: args 数组（main 方法参数）
来源：http://hz.hongshengwenyu.top/gtlxyjyyyl.html

Go:   os.Args[1:]
来源：http://hz.ydzc1.top/gtmfagebmy.html

Ruby: ARGV
来源：http://hz.yj202588.top/gtvznjzieh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jinyuanbaomall.cn/gtdygpxvyt.html

[M02] 读取环境变量
来源：http://hz.sweek.top/gtstfhvwvb.html

Py:   os.environ.get("HOME")
来源：http://hz.sxryk.cn/gtlliscjle.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xingfuxueyuan.xyz/gtpqmhswyc.html

JS:   process.env.HOME
来源：http://hz.pengpengdd.cyou/gtkroxtiaf.html

TS:   process.env.HOME
来源：http://hz.fengsongda.top/gtfxnuswov.html

Java: System.getenv("HOME")
来源：http://hz.daxiang520.top/gtemualnqu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gaohongyu789.top/gtiynalvhw.html

Ruby: ENV["HOME"]
来源：http://hz.hywenlv.cn/gtwtagyrjc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jlsjyb.cn/gtrnmimdwk.html

[M03] 执行外部命令
来源：http://hz.zycfv.cn/gtygpuqpmt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.fengsongda.top/gtiwnwjvot.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhengqikj.top/gtmapiyhxh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydjk.org.cn/gtexjdzntj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj202588.top/gtjobudtha.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yvedp.cn/gtkmodkmrl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sysykeji.top/gtnkddllae.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.bjfxy.top/gtssuvznlw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.aizwys.cn/gtttmfdwdv.html

[M04] 获取当前工作目录
来源：http://hz.guowangkeji.top/gtdjbwtvlt.html

Py:   os.getcwd()
来源：http://hz.hongshengwenyu.top/gtmnwaalki.html

PHP:  getcwd();
来源：http://hz.andypj.xyz/gtlefzlpxx.html

JS:   process.cwd()
来源：http://hz.ywan-chungtsiang.top/gtijevkkjp.html

TS:   process.cwd()
来源：http://hz.sweek.top/gtckeabjrh.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yonumen.top/gtsldmnmko.html

Go:   os.Getwd()
来源：http://hz.yj20258.top/gtnetwjomu.html

Ruby: Dir.pwd
来源：http://hz.meibo888.top/gtsgjqcqif.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.andypj.xyz/gtvjjezboj.html

[M05] 设置退出码
来源：http://hz.52xcode.cn/gtxjvkdsia.html

Py:   sys.exit(1)
来源：http://hz.shangyingyoupin.top/gtjkinkoie.html

PHP:  exit(1);
来源：http://hz.mhx1999.top/gticazjkro.html

JS:   process.exit(1)
来源：http://hz.haohaochexian.top/gtgksjhygq.html

TS:   process.exit(1)
来源：http://hz.shanyushiyangtech.top/gtlksrskzp.html

Java: System.exit(1)
来源：http://hz.zhixingplan.top/gteyqyjxbe.html

Go:   os.Exit(1)
来源：http://hz.birdmap.top/gtizicjjuw.html

Ruby: exit 1
来源：http://hz.gzhubu.top/gtrumzbvpc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.fzhhl.top/gtrrkcxsyh.html

[M06] 向标准错误输出
来源：http://hz.ydzc1.top/gtrwzdgehw.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hysaishi.cn/gtaeppmjdg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shanyushiyangtech.top/gthfvhigwv.html

JS:   console.error("err")
来源：http://hz.nanxuanxn.top/gtdjxlbxxu.html

TS:   console.error("err")
来源：http://hz.shanyushiyangtech.top/gtalplpysj.html

Java: System.err.println("err")
来源：http://hz.cdnleiting.top/gtofvjczfp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cdnleiting.top/gtoarzkrrq.html

Ruby: warn "err"
来源：http://hz.cqqwz.cn/gtipcsznpg.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cheryme.top/gtxyboegaw.html

[M07] 判断是否为主入口
来源：http://hz.gzhubu.top/gtzytaqksb.html

Py:   if __name__ == "__main__":
来源：http://hz.sysykeji.top/gtmxikufuf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.fzhhl.top/gtdhpvsraa.html

JS:   require.main === module
来源：http://hz.316326.xyz/gtexlotdqw.html

TS:   require.main === module
来源：http://hz.zhaomingkeji.xyz/gthskquqic.html

Java: public static void main(String[] args)
来源：http://hz.jinyuanbaomall.cn/gticfyebsu.html

Go:   func main()
来源：http://hz.hongshengwenyu.top/gttncmnret.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xylfe.cn/gtekqpfone.html

C#:   static void Main(string[] args)
来源：http://hz.tian-w.cn/gtyhmpmyjb.html

[M08] 获取系统与运行时信息
来源：http://hz.shangyingyoupin.top/gtdsvgcfmv.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hywenlv.cn/gtivyouwuo.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhoulong.xyz/gtrbwquvfx.html

JS:   process.platform;  process.version
来源：http://hz.havefunace.top/gtpltlnfuc.html

TS:   process.platform;  process.version
来源：http://hz.cashguo.top/gtcnwfxvyr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.nwbrower.top/gtlsiganob.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yueranfly.top/gtumwexvcx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.wangdashe.top/gtxpogcnrs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yuxming.cn/gttetumhfg.html

================================================================================
来源：http://hz.yueranfly.top/gtszirgwdm.html

N. 数据结构与算法
来源：http://hz.daria6918.cn/gthbsxzkio.html

================================================================================
来源：http://hz.quarkkingdee.top/gtoinyheqi.html

[N01] 二分查找（有序数组）
来源：http://hz.jianghu66.top/gtoqeaaqmg.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.meibo888.top/gtcurxychg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xuanzx.com/gtuewxxcjq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gogol.net.cn/gtfcfzrgbh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxinkj.top/gtwowtktbx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.bjfxy.top/gtuodmbcxq.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.mhx1999.top/gtgsdhktil.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hnqzz.top/gtoanppclc.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cucudq.cn/gtzknsgdfo.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xuetiantiany.cn/gtukmhzomf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.daxiang520.top/gtcwexopll.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.smart0.xyz/gtblcjoakb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.svipenyu.cn/gtgxczdllr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangtech.top/gtgolujojb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.pycfn.com/gtbtfyzalr.html

Go:   slices.Sort(arr)
来源：http://hz.chenzaomai.com/gtaulcmbji.html

Ruby: arr.sort
来源：http://hz.daria6918.cn/gtkxdnpbbi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.gogol.net.cn/gthwktjjrd.html

[N03] 快速排序（分治示例）
来源：http://hz.9152youxi.cn/gtcfsogpdy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shzxlz.cn/gtezmlzfbn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hnxiangtu.top/gtcoyiqteb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yanxiufei.cn/gtbzovnizg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cheryme.top/gtbnsgohtk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hnxiangtu.top/gtttnmudxf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cucudq.cn/gtgwdorjzu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hnqzz.top/gtghuanxne.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.bjfxy.top/gtgqjbjlsb.html

[N04] 斐波那契数列
来源：http://hz.sxryk.cn/gtgheynnmd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ivvv.top/gtyewsdinl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.birdmap.top/gtxcodiddw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.meibo888.top/gtkehfderb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sxryk.cn/gtnvjixdnw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yonumen.top/gtjwaigyvq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jqgufenzy.top/gtqaydettj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.daxiang520.top/gtncujbniy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sysykeji.top/gtokxkjsaa.html

[N05] 最大公约数
来源：http://hz.fengsongda.top/gteafxbcyc.html

Py:   math.gcd(a, b)
来源：http://hz.gotoacloud.top/gtoufkmvvt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.smart0.xyz/gtwsjnmglu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aibaodan.cn/gteuywphfn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yangfankeji.com/gthvbekyyq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ybcxt.top/gtqtabagtc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.snrcjt.cn/gtetcbljzr.html

Ruby: a.gcd(b)
来源：http://hz.zhoulong.xyz/gtqvsycmub.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.iojbl.cn/gtjsldpukc.html

[N06] 判断回文字符串
来源：http://hz.sysykeji.top/gtrmsjbqqx.html

Py:   s == s[::-1]
来源：http://hz.ppjwa.cn/gtfsakbkgy.html

PHP:  $s === strrev($s);
来源：http://hz.aizwys.cn/gtrcaqzxou.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yueranfly.top/gtcnuvugbu.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zycfv.cn/gtyirpcpnq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.daria6918.cn/gtvnfqheiu.html

Go:   // 双指针从两端比较
来源：http://hz.shzxlz.cn/gtpfahcfxu.html


<!-- 参考信息 -->