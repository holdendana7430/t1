代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhixingplan.top/gtshqjqrbz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xziqi.cn/gtgtlfwzqa.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangtech.top/gtmgizxyef.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.meibo888.top/gtoeeomony.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jqgfzy.top/gtwifkqmfv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.kuanghao11.cn/gtiwkyankg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.nanxuanxn.top/gticanikbc.html

[J10] 取今天 / 本月第一天
来源：http://hz.vqdsnc.cn/gtcfjrovch.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ydjk.org.cn/gtdkfraeii.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jiagoushi.top/gtnvvlegfm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yangfankeji.com/gtarsqwtjg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gaohongyu789.top/gtufznymsz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xuetiantiany.cn/gtztybvvur.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hysaishi.cn/gtjvnymsaf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gotoacloud.top/gttykdxxsp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhaomingkeji.xyz/gtglyratpn.html

================================================================================
来源：http://hz.hfpthk.cn/gtawtjjepj.html

K. JSON 与序列化
来源：http://hz.hywenlv.cn/gtwdenwtch.html

================================================================================
来源：http://hz.xinyue.icu/gtdnclaysr.html

[K01] 对象转 JSON 字符串
来源：http://hz.gotoacloud.top/gtbuaakdhw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.nanxuanxn.top/gtoqdwxlln.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hfpthk.cn/gtivpvlkic.html

JS:   JSON.stringify(obj)
来源：http://hz.jqgufenzy.top/gtmgjuciyr.html

TS:   JSON.stringify(obj)
来源：http://hz.xylfe.cn/gtddkypmee.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yvedp.cn/gtrrjdmxph.html

Go:   json.Marshal(obj)
来源：http://hz.nwbrower.top/gtybcpvrob.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.aizwys.cn/gtqaouyyio.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hnxiangtu.top/gttazqvnhx.html

[K02] JSON 字符串转对象
来源：http://hz.tian-w.cn/gthdorsxdi.html

Py:   json.loads(s)
来源：http://hz.gotoacloud.top/gtmkhejuuv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.sufxvd.cn/gtnglmqjhb.html

JS:   JSON.parse(s)
来源：http://hz.jqgufenzy.top/gtefooqxcx.html

TS:   JSON.parse(s)
来源：http://hz.ydzc1.top/gtbagikyzy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.bjfxy.top/gtnzqwutmb.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.wangdashe.top/gtnxriticw.html

Ruby: JSON.parse(s)
来源：http://hz.guannengcc.top/gtghctasvq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xuetiantiany.cn/gtjvwbgpdl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.pengpengdd.cyou/gtnpttouay.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.wangshuangyany.cn/gttmfggrcs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xuetiantiany.cn/gtjedinzqv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shangyingyoupin.top/gtvdlruehd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.svipenyu.cn/gtaxrlvguc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.daria6918.cn/gtubqraurq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jqgufenzy.top/gthirohrob.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jlsjyb.cn/gtgnocyhlt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.sweek.top/gtkrnwtckh.html

[K04] 读取 JSON 文件
来源：http://hz.xinyue.icu/gtychamfgz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hnxiangtu.top/gtqfjeasem.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.svipenyu.cn/gtdtdjfich.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yueranfly.top/gthstmmvso.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.quarkkingdee.top/gtsfhzhfmi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ydjk.org.cn/gttdsgbzdm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shangyingyoupin.top/gtnsjwihbs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shangyingyoupin.top/gtunafhamb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.haohaochexian.top/gtwitowohl.html

[K05] 深拷贝对象
来源：http://hz.ppjwa.cn/gtkmspmzrs.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhaomingkeji.xyz/gtxseyguax.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hysaishi.cn/gtevpzyadq.html

JS:   structuredClone(obj)
来源：http://hz.jiagoushi.top/gtdiyfwvsx.html

TS:   structuredClone(obj)
来源：http://hz.shuidangran.top/gtrmrujdho.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hongshengwenyu.top/gtmfugfwir.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj202588.top/gtmpisjzfi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xinyue.icu/gtguxdliyj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.aibaodan.cn/gtcrkjcwit.html

[K06] 解析 URL 查询串
来源：http://hz.wangdashe.top/gtqdulnsna.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yuxming.cn/gtozkjlcab.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.chenlongwang.top/gtqgooojrd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cdnleiting.top/gtfalouskp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhixingplan.top/gtvvjoyzsd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.chenjidiqi.icu/gtsfczevog.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sxryk.cn/gtcabbgavt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hnxiangtu.top/gtwzigyigx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ivvv.top/gtdtmadrit.html

[K07] 进制转换
来源：http://hz.zhiwuduotai.top/gtzzdhdsic.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.feifeiyinyue.top/gtrdhbubyz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xylfe.cn/gtxvnymawu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jqgufenzy.top/gtwoaaupah.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ppjwa.cn/gtpttsxict.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.nanxuanxn.top/gtyeuqrpfw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yangfankeji.com/gtnmoypszx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.aibaodan.cn/gtoeqgojem.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.smart0.xyz/gtqanqbtqy.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.redwolf501.top/gtazlvwsda.html

Py:   pickle.dumps(obj)
来源：http://hz.cucudq.cn/gtkbneulqa.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xuetiantiany.cn/gtwtgoqmlm.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.chenzaomai.com/gtsmncbeda.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.shangyingyoupin.top/gtufrhwviw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shuidangran.top/gtptupyywv.html

Go:   encoding/gob
来源：http://hz.jinqigufen.top/gtjsqakhso.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinyuanbaomall.cn/gtarrqhpzz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhixingplan.top/gtfknopalm.html

================================================================================
来源：http://hz.tian-w.cn/gtdhtwbtlr.html

L. 网络请求
来源：http://hz.chenzaomai.com/gtzckjptzh.html

================================================================================
来源：http://hz.yvedp.cn/gthyzzjpue.html

[L01] 发送 GET 请求
来源：http://hz.52xcode.cn/gtgtdllpel.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.fzhhl.top/gttyktdvql.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.nwbrower.top/gtpkmjvzbn.html

JS:   await fetch(url)
来源：http://hz.cqqwz.cn/gtadyvxweh.html

TS:   await fetch(url)
来源：http://hz.xylfe.cn/gtgzqjakam.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.wangshuangyany.cn/gtdwaofjnr.html

Go:   resp, err := http.Get(url)
来源：http://hz.jinqigfzy.top/gtxvinldmj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yuxming.cn/gtcxurhfmr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.0kj1m.cn/gtydrdovrs.html

[L02] 发送 POST JSON
来源：http://hz.gogol.net.cn/gtxvwckxuq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.sysykeji.top/gtqljfsznn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.haohaochexian.top/gtbbdnvfau.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.andypj.xyz/gtvewxxjmq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ivvv.top/gtnjrnjkvn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shzxlz.cn/gtanpicocf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yanxiufei.cn/gteenbikcm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.wangshuangyany.cn/gtdfeiqoja.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ydzc1.top/gtgpiekcob.html

[L03] 设置自定义请求头
来源：http://hz.gzhubu.top/gtwzplpauu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.bjfxy.top/gtluewrclt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.tanke756.top/gtfeeupvqw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuanzx.com/gtktthcqdf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yongpay.top/gtatqeofhu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.aizwys.cn/gtpzftzczr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cucudq.cn/gtdoesther.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.vqdsnc.cn/gthhqemuba.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yvedp.cn/gtjwexozeh.html

[L04] 设置超时
来源：http://hz.jinqigufen.top/gtgxoxxdtp.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ybcxt.top/gtigrwfoxh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ywan-chungtsiang.top/gtaicehnln.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenzaomai.com/gtnqajymnl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.havefunace.top/gtticslbod.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.quarkkingdee.top/gtiipxyrko.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.chenjidiqi.icu/gtoeslwgxc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.guannengcc.top/gtpcjmupab.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yj20258888.top/gtqymxwtvv.html

[L05] 上传文件（multipart）
来源：http://hz.jlsjyb.cn/gtjwacadgt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.chenlongwang.top/gtfgqssveo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cqqwz.cn/gtjgxpxeiy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hnqzz.top/gtntvoqlxn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cdnleiting.top/gtfxsbjjcz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.pycfn.com/gtanvebsyw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.kuanghao11.cn/gtdzcddgib.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.chenjidiqi.icu/gtgzxfdaau.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.smart0.xyz/gtaamrxbob.html

[L06] 解析响应为 JSON
来源：http://hz.9152youxi.cn/gtsxvlgind.html

Py:   resp.json()
来源：http://hz.shangyingyoupin.top/gttwwhqqgm.html

PHP:  json_decode($body, true);
来源：http://hz.yuanzhike.top/gtqbjaagts.html

JS:   await resp.json()
来源：http://hz.xuetiantiany.cn/gtowgsipwq.html

TS:   await resp.json()
来源：http://hz.kuanghao11.cn/gtafwwdovp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhixingplan.top/gtxinkljzj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yj20258.top/gtcfyqeukr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.quarkkingdee.top/gtpizvfyrw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hongshengwenyu.top/gtvvmskpok.html

[L07] 处理 HTTP 状态码
来源：http://hz.jqgfzy.top/gtmuwsdvsy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.52xcode.cn/gtijbxcszt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.snrcjt.cn/gtnlhrruts.html

JS:   resp.ok;  resp.status
来源：http://hz.hnxiangtu.top/gtodtcdjzi.html

TS:   resp.ok;  resp.status
来源：http://hz.zhijiandao.cn/gtlvneljrz.html

Java: resp.statusCode()
来源：http://hz.ppjwa.cn/gtsigijsly.html

Go:   resp.StatusCode
来源：http://hz.zhiwuduotai.top/gtevzbuevo.html

Ruby: resp.code.to_i
来源：http://hz.sufxvd.cn/gtsptizxde.html

C#:   (int)resp.StatusCode
来源：http://hz.gzhubu.top/gtxivgqchr.html

[L08] 并发请求多个地址
来源：http://hz.shanyushiyangtech.top/gtlehktzpi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.dianchejie.cn/gtosoxxlha.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhoulong.xyz/gttbfxqjwp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shzxlz.cn/gtyqdltkcz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.0kj1m.cn/gtzuexcnql.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shzxlz.cn/gtzjdeshzu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tian-w.cn/gtjnmlcxzm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.shanyushiyangtech.top/gtmwoakdme.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.wangshuangyany.cn/gthefqxzah.html

================================================================================
来源：http://hz.sufxvd.cn/gtuxrlkfrm.html

M. 命令行 / 进程 / 环境
来源：http://hz.jyoumei.cn/gtxztvennh.html

================================================================================
来源：http://hz.hfpthk.cn/gtbavgqazl.html

[M01] 读取命令行参数
来源：http://hz.zhongyouzk.top/gtaxzwkzgk.html

Py:   sys.argv[1:]
来源：http://hz.sufxvd.cn/gtypziaoiy.html

PHP:  $argv;  $argc;
来源：http://hz.jyoumei.cn/gtfcdakike.html

JS:   process.argv.slice(2)
来源：http://hz.redwolf501.top/gtdejuhxkg.html

TS:   process.argv.slice(2)
来源：http://hz.dashuyun.cn/gtorzhzfcg.html

Java: args 数组（main 方法参数）
来源：http://hz.redwolf501.top/gtoyvbqqck.html

Go:   os.Args[1:]
来源：http://hz.chenzaomai.com/gtdlhfopbn.html

Ruby: ARGV
来源：http://hz.xuanzx.com/gtuciepujy.html

C#:   args 数组（Main 方法参数）
来源：http://hz.aizwys.cn/gtvfrtbjxu.html

[M02] 读取环境变量
来源：http://hz.daxiang520.top/gtxisesozh.html

Py:   os.environ.get("HOME")
来源：http://hz.nwbrower.top/gtedljgfef.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.fengsongda.top/gtsuxzyopv.html

JS:   process.env.HOME
来源：http://hz.jinghuilouyu.cn/gtdcccrmvo.html

TS:   process.env.HOME
来源：http://hz.xuanzx.com/gtffksxehk.html

Java: System.getenv("HOME")
来源：http://hz.yangfankeji.com/gtyzqemxmv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.shangyingyoupin.top/gtcfbqfetj.html

Ruby: ENV["HOME"]
来源：http://hz.yj20258888.top/gttcehjtqa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.daria6918.cn/gtceszaaas.html

[M03] 执行外部命令
来源：http://hz.yonumen.top/gtywondjgn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.nanxuanxn.top/gtuuitsbiu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jyoumei.cn/gtebapieqo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.andypj.xyz/gtwgiwouza.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hnxiangtu.top/gttkworwoq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.svipenyu.cn/gtemcqilxv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.dashuyun.cn/gtmtuctebf.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cdnleiting.top/gtlcogmsfo.html

C#:   Process.Start("ls", "-l");
来源：http://hz.havefunace.top/gthszmjyio.html

[M04] 获取当前工作目录
来源：http://hz.aizwys.cn/gtryucfhoh.html

Py:   os.getcwd()
来源：http://hz.chenzaomai.com/gtjpdlyrkg.html

PHP:  getcwd();
来源：http://hz.sysykeji.top/gtnoyhdsgd.html

JS:   process.cwd()
来源：http://hz.cdnleiting.top/gtykgqhdau.html

TS:   process.cwd()
来源：http://hz.52xcode.cn/gtzgdbujhk.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hongshengwenyu.top/gthryxsjdi.html

Go:   os.Getwd()
来源：http://hz.birdmap.top/gtmakqgzjw.html

Ruby: Dir.pwd
来源：http://hz.sxryk.cn/gthxcynaom.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jinghuilouyu.cn/gturykpggd.html

[M05] 设置退出码
来源：http://hz.haohaochexian.top/gtmlsyxkdv.html

Py:   sys.exit(1)
来源：http://hz.cheryme.top/gthsfiylcx.html

PHP:  exit(1);
来源：http://hz.bjfxy.top/gtqzvoccmk.html

JS:   process.exit(1)
来源：http://hz.gogol.net.cn/gtouvuknyg.html

TS:   process.exit(1)
来源：http://hz.nwbrower.top/gtiaqpfgpe.html

Java: System.exit(1)
来源：http://hz.yongpay.top/gtszruzqqw.html

Go:   os.Exit(1)
来源：http://hz.chenzaomai.com/gtwdehhfov.html

Ruby: exit 1
来源：http://hz.shzxlz.cn/gtvckwtqif.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shangyingyoupin.top/gtxdjcdedg.html

[M06] 向标准错误输出
来源：http://hz.shanyushiyangkeji.top/gtrjojguml.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cashguo.top/gtdfxkgisw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yonumen.top/gtuaiexsnt.html

JS:   console.error("err")
来源：http://hz.redwolf501.top/gtptjfghor.html

TS:   console.error("err")
来源：http://hz.aizwys.cn/gtvephemos.html

Java: System.err.println("err")
来源：http://hz.jinyuanbaomall.cn/gtfoximdyt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yanxiufei.cn/gttzpnidqr.html

Ruby: warn "err"
来源：http://hz.ehwqpu.com/gtmkxthqmc.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.guannengcc.top/gtcfcbbsup.html

[M07] 判断是否为主入口
来源：http://hz.smart0.xyz/gtincwzlsn.html

Py:   if __name__ == "__main__":
来源：http://hz.gaohongyu789.top/gtsrpimyuu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jinghuilouyu.cn/gtdforbrns.html

JS:   require.main === module
来源：http://hz.gogol.net.cn/gtwxzlucoe.html

TS:   require.main === module
来源：http://hz.cucudq.cn/gtxtfeszig.html

Java: public static void main(String[] args)
来源：http://hz.tanke756.top/gtqfhicnoh.html

Go:   func main()
来源：http://hz.tanke756.top/gtqurbuqkj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xuetiantiany.cn/gttcskxkeb.html

C#:   static void Main(string[] args)
来源：http://hz.ybcxt.top/gtspkvjnoe.html

[M08] 获取系统与运行时信息
来源：http://hz.zdqjudy.top/gtbmjbbxtz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shanyushiyangkeji.top/gtyqxwxomj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.pengpengdd.cyou/gtsecikwsx.html

JS:   process.platform;  process.version
来源：http://hz.mhx1999.top/gtdedeeqcy.html

TS:   process.platform;  process.version
来源：http://hz.xuetiantiany.cn/gtcohfnegb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jinqigfzy.top/gtieegkwsd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xuetiantiany.cn/gttfgkkiix.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.pengpengdd.cyou/gtkuxftpgi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.52xcode.cn/gtymwsqsnw.html

================================================================================
来源：http://hz.daxiang520.top/gtwytxvwbn.html

N. 数据结构与算法
来源：http://hz.quarkkingdee.top/gtcukvoqfz.html

================================================================================
来源：http://hz.c1oappe.top/gtedfffdsa.html

[N01] 二分查找（有序数组）
来源：http://hz.chenjidiqi.icu/gtqekuwucb.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ppjwa.cn/gtluiuqrzp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.kuanghao11.cn/gtfgjvtmeq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.smart0.xyz/gtpofhtmwk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.smart0.xyz/gtjfdkpitf.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ivvv.top/gtkownkvmn.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.meibo888.top/gtuxwdsawu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hnqzz.top/gtbyeuxxot.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shanyushiyangtech.top/gtiwjjksel.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hysaishi.cn/gtdxzevqzy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ehwqpu.com/gtevzoadbt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.9152youxi.cn/gtbsohlths.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangkeji.top/gtgeldszvp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cqqwz.cn/gttdiktaqy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.svipenyu.cn/gtiwooirqn.html

Go:   slices.Sort(arr)
来源：http://hz.tianlin.xyz/gtvmpwihjz.html

Ruby: arr.sort
来源：http://hz.yangfankeji.com/gtvnhuhvji.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ivvv.top/gtmxqzqxpj.html

[N03] 快速排序（分治示例）
来源：http://hz.shanyushiyangkeji.top/gtpdfhqrkp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.vqdsnc.cn/gtlswliahm.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gaohongyu789.top/gtavghdxww.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dashuyun.cn/gtirvvfqji.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shuidangran.top/gtjesccidq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cdnleiting.top/gtfprwgosg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.wangshuangyany.cn/gtoqmcdjgi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yj20258.top/gtmapypjia.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.iojbl.cn/gtsutzpksx.html

[N04] 斐波那契数列
来源：http://hz.gzhubu.top/gtpwberynn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cqqwz.cn/gtfmctpxjt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.nwbrower.top/gtfkdrtqiz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xingfuxueyuan.xyz/gtxlzcwnws.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yongpay.top/gtifrvjfiy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ppjwa.cn/gtyuuuyxhe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.daria6918.cn/gtnighxrge.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cucudq.cn/gtxvhtlrsk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.dianchejie.cn/gtfmqlhgee.html

[N05] 最大公约数
来源：http://hz.fengsongda.top/gtdjtyqwba.html

Py:   math.gcd(a, b)
来源：http://hz.birdmap.top/gtanhrpvgo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yj202588.top/gteoxccqor.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nwbrower.top/gtfwseegiw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hywenlv.cn/gtiwnsgvam.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.snrcjt.cn/gtpqvyqbkb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.pengpengdd.cyou/gtudqsnsjs.html

Ruby: a.gcd(b)
来源：http://hz.wangshuangyany.cn/gttezwhduc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hfpthk.cn/gtgsuycodm.html

[N06] 判断回文字符串
来源：http://hz.yuanzhike.top/gtuvmvnrfi.html

Py:   s == s[::-1]
来源：http://hz.daria6918.cn/gtwwbwokws.html

PHP:  $s === strrev($s);
来源：http://hz.jinghuilouyu.cn/gtuavxylxi.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jinyuanbaomall.cn/gtudzhruay.html

TS:   s === [...s].reverse().join("")
来源：http://hz.haohaochexian.top/gtesovdyew.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xingfuxueyuan.xyz/gtjxytyrai.html

Go:   // 双指针从两端比较
来源：http://hz.chenlongwang.top/gtnivmdozc.html

Ruby: s == s.reverse
来源：http://hz.hysaishi.cn/gtbdjlekjb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.dianchejie.cn/gtvnwenqdk.html

[N07] 两数之和（返回下标）
来源：http://hz.fengsongda.top/gtuqatvqxa.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jinqigfzy.top/gtoofjktnv.html


<!-- 参考信息 -->