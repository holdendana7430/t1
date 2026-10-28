代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yvedp.cn/gthsmlhmkj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.snrcjt.cn/gtiiqeqmvb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gaohongyu789.top/gtsarpirhp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.c1oappe.top/gtavrzejbs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.mhx1999.top/gtvpdkmrlz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hnxiangtu.top/gthonnagwf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.wangshuangyany.cn/gthpdzapbb.html

[J10] 取今天 / 本月第一天
来源：http://hz.yj202588.top/gtvphrbrzn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.dianchejie.cn/gtgtypjabw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sufxvd.cn/gtgdzelxwv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zdqjudy.top/gtdrdezikl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.tianlin.xyz/gtjngdfeuj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ydzc1.top/gtpnbtpxua.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.chenjidiqi.icu/gtilndpyjl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhiwuduotai.top/gtjveowlsv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sysykeji.top/gtsuzmsvbk.html

================================================================================
来源：http://hz.sweek.top/gtwoyfjnxf.html

K. JSON 与序列化
来源：http://hz.meibo888.top/gtexbuewii.html

================================================================================
来源：http://hz.9152youxi.cn/gtnhqukzpx.html

[K01] 对象转 JSON 字符串
来源：http://hz.yanxiufei.cn/gttkxdekte.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xuetiantiany.cn/gtcervcgpd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxuanxn.top/gthkazaral.html

JS:   JSON.stringify(obj)
来源：http://hz.xziqi.cn/gtpctrkvwj.html

TS:   JSON.stringify(obj)
来源：http://hz.jinghuilouyu.cn/gtslbxtwyf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yj20258.top/gtmimylbts.html

Go:   json.Marshal(obj)
来源：http://hz.ywan-chungtsiang.top/gtxunsgsxz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.guowangkeji.top/gtdmqrjonv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jiagoushi.top/gthfmouqcx.html

[K02] JSON 字符串转对象
来源：http://hz.svipenyu.cn/gtzuexlbwa.html

Py:   json.loads(s)
来源：http://hz.kuanghao11.cn/gtdmohghcr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hnxiangtu.top/gthbgixicg.html

JS:   JSON.parse(s)
来源：http://hz.pycfn.com/gtqokqxuon.html

TS:   JSON.parse(s)
来源：http://hz.zhiwuduotai.top/gtabetlflc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hywenlv.cn/gtlurhbrcr.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cqqwz.cn/gtaewhbllp.html

Ruby: JSON.parse(s)
来源：http://hz.zhiwuduotai.top/gtavbdnfra.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.tian-w.cn/gtmbvnrkhf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.mhx1999.top/gtlwpmfuwj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhixingplan.top/gtjkxnfzdj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.daria6918.cn/gtzodpxhnz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yuxming.cn/gtmklazdet.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangshuangyany.cn/gtoekgmkoh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xinyue.icu/gtsaxikqug.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.9152youxi.cn/gtobpxomuv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.bjfxy.top/gtqlzlbqug.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.nanxuanxn.top/gtmbardzpp.html

[K04] 读取 JSON 文件
来源：http://hz.nwbrower.top/gtfiuuzfrv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hammf.cn/gtmibjydbd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cdnleiting.top/gtaxkojmss.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shangyingyoupin.top/gtaotugbbx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yuxming.cn/gtanuozyku.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.wangshuangyany.cn/gtknjiidzi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yongpay.top/gtpuaguwfx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.c1oappe.top/gtcetalsxm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.c1oappe.top/gtyefngtwm.html

[K05] 深拷贝对象
来源：http://hz.daria6918.cn/gtrnmlokry.html

Py:   copy.deepcopy(obj)
来源：http://hz.dashuyun.cn/gtjrwdcwsa.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shangyingyoupin.top/gtpveunovl.html

JS:   structuredClone(obj)
来源：http://hz.jinqigfzy.top/gtopbzcuou.html

TS:   structuredClone(obj)
来源：http://hz.yongpay.top/gtzgqdqafl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.fzhhl.top/gtfrsxwvxa.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xuanzx.com/gtmjssjhzt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yj20258.top/gtjkokkhhk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.meibo888.top/gtxtwozjoq.html

[K06] 解析 URL 查询串
来源：http://hz.wangshuangyany.cn/gtpntsztdj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sufxvd.cn/gtwgddgvim.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yueranfly.top/gtslveketf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.kuanghao11.cn/gtawqdtnke.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fengsongda.top/gtvbubascr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.kuanghao11.cn/gtljkrrjht.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.quarkkingdee.top/gtxedotczo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ehwqpu.com/gtemurupgd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.kuanghao11.cn/gtwvsdcwnk.html

[K07] 进制转换
来源：http://hz.yongpay.top/gtrhjbzlqh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.fengsongda.top/gtnrekebjs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.meibo888.top/gtdxdtjlsz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.fengsongda.top/gtdblmisrk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.dianchejie.cn/gtzhpmugmt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.aizwys.cn/gtzvumuegb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jqgufenzy.top/gtlbrxuekl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gotoacloud.top/gtuasvoxpj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ivvv.top/gtuevqaqml.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhaomingkeji.xyz/gtivodsksp.html

Py:   pickle.dumps(obj)
来源：http://hz.zhengqikj.top/gtmpckngbz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gaohongyu789.top/gtacovscie.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.0kj1m.cn/gtufwwxfnu.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.tian-w.cn/gtefdfwknk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.fengsongda.top/gtnkhgvakp.html

Go:   encoding/gob
来源：http://hz.c1oappe.top/gtzxlvtkgh.html

Ruby: Marshal.dump(obj)
来源：http://hz.ehwqpu.com/gtsbxlpxbu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhongyouzk.top/gtxclvcyxt.html

================================================================================
来源：http://hz.cheryme.top/gtsusvvofd.html

L. 网络请求
来源：http://hz.jinqigufen.top/gtcssielnf.html

================================================================================
来源：http://hz.ivvv.top/gthvlnuwdp.html

[L01] 发送 GET 请求
来源：http://hz.xinyue.icu/gtbwbqwajm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.daxiang520.top/gtvvjcvxhf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.chenlongwang.top/gtrjlsjrkl.html

JS:   await fetch(url)
来源：http://hz.yuanzhike.top/gttbzjfbuu.html

TS:   await fetch(url)
来源：http://hz.dianchejie.cn/gtkhwnodvq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.fzhhl.top/gthcxsumbx.html

Go:   resp, err := http.Get(url)
来源：http://hz.chenzaomai.com/gtqdqhhbva.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yueranfly.top/gtzjmkgrdx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yuanzhike.top/gttqbqxsqw.html

[L02] 发送 POST JSON
来源：http://hz.daria6918.cn/gtnuwqlgyv.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.dianchejie.cn/gtkaqphftf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.9152youxi.cn/gtkuokcmuu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shzxlz.cn/gtnledloso.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sysykeji.top/gtfffnfeff.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj202588.top/gtuzmqvtxt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.feifeiyinyue.top/gtuhrndadk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shangyingyoupin.top/gtvvqqlucz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.daxiang520.top/gtomdlvqru.html

[L03] 设置自定义请求头
来源：http://hz.chenjidiqi.icu/gtthaoizza.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.guannengcc.top/gtecuhsxqy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yangfankeji.com/gtmyyvjmnd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.fzhhl.top/gtgjedprfz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.smart0.xyz/gtqowmtazw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.redwolf501.top/gtbjhyukeu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hnxiangtu.top/gtwbmdanhg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhiwuduotai.top/gtltuogpbk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cqqwz.cn/gtbyowanzl.html

[L04] 设置超时
来源：http://hz.redwolf501.top/gtmsxrscbv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xuanzx.com/gtpmbknobb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.daxiang520.top/gtllqubcjd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinqigufen.top/gtrnaevcfe.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangshuangyany.cn/gtmpdgfzfe.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hysaishi.cn/gtwsepvznf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.fengsongda.top/gtwoaqjhit.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.gaohongyu789.top/gtofuzktvi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yanxiufei.cn/gtdrvbcwdc.html

[L05] 上传文件（multipart）
来源：http://hz.fzhhl.top/gtslrxqlsa.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yuxming.cn/gtphmwufxp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cashguo.top/gtbivwqnjh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.feifeiyinyue.top/gttzxmwvax.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangkeji.top/gtoohqceit.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.feifeiyinyue.top/gtzpakvmeu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.dianchejie.cn/gtfpdevdoi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.tian-w.cn/gtvufaqlfy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.dashuyun.cn/gtgqviltlh.html

[L06] 解析响应为 JSON
来源：http://hz.dashuyun.cn/gtowbyerdv.html

Py:   resp.json()
来源：http://hz.cheryme.top/gtzupfakkt.html

PHP:  json_decode($body, true);
来源：http://hz.ybcxt.top/gtjutvptfu.html

JS:   await resp.json()
来源：http://hz.jianghu66.top/gtdukrjvvx.html

TS:   await resp.json()
来源：http://hz.tian-w.cn/gtawolecbn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.316326.xyz/gtulnesqcw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhiwuduotai.top/gtwoxgkqwq.html

Ruby: JSON.parse(resp.body)
来源：http://hz.wangshuangyany.cn/gtzbuggxqh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hywenlv.cn/gtsrvsffky.html

[L07] 处理 HTTP 状态码
来源：http://hz.ydjk.org.cn/gtakvturuq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhoulong.xyz/gtvdrtgkth.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cdnleiting.top/gtgmsnfxsr.html

JS:   resp.ok;  resp.status
来源：http://hz.wangshuangyany.cn/gtzootqkpq.html

TS:   resp.ok;  resp.status
来源：http://hz.hywenlv.cn/gtzosylhvv.html

Java: resp.statusCode()
来源：http://hz.aibaodan.cn/gtzgjbhevw.html

Go:   resp.StatusCode
来源：http://hz.shanyushiyangtech.top/gtcrblnlya.html

Ruby: resp.code.to_i
来源：http://hz.redwolf501.top/gtcywhvbco.html

C#:   (int)resp.StatusCode
来源：http://hz.aibaodan.cn/gtejyaiccq.html

[L08] 并发请求多个地址
来源：http://hz.316326.xyz/gtfdyfcaxr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ivvv.top/gtfgttjafa.html

PHP:  curl_multi_init() 系列
来源：http://hz.daxiang520.top/gtmirbxyoz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxuanxn.top/gtiymhasar.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhixingplan.top/gtdlcyibew.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.daxiang520.top/gtcyozbdob.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.daria6918.cn/gtxgvdfplw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.fzhhl.top/gtxxuyumam.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xinyue.icu/gtsevtpwns.html

================================================================================
来源：http://hz.hysaishi.cn/gtkebktmeo.html

M. 命令行 / 进程 / 环境
来源：http://hz.haohaochexian.top/gtnvjzsdej.html

================================================================================
来源：http://hz.zhoulong.xyz/gtmvtmnrxt.html

[M01] 读取命令行参数
来源：http://hz.yj20258.top/gtcxwmszlp.html

Py:   sys.argv[1:]
来源：http://hz.birdmap.top/gtynahquro.html

PHP:  $argv;  $argc;
来源：http://hz.jyoumei.cn/gtcpagfqca.html

JS:   process.argv.slice(2)
来源：http://hz.dianchejie.cn/gtdmcqzlhu.html

TS:   process.argv.slice(2)
来源：http://hz.cashguo.top/gtrbjkvqkm.html

Java: args 数组（main 方法参数）
来源：http://hz.xziqi.cn/gtydgfuaku.html

Go:   os.Args[1:]
来源：http://hz.zhoulong.xyz/gtmfdflroe.html

Ruby: ARGV
来源：http://hz.quarkkingdee.top/gtcrbobsua.html

C#:   args 数组（Main 方法参数）
来源：http://hz.daxiang520.top/gtixfasqsz.html

[M02] 读取环境变量
来源：http://hz.zhoulong.xyz/gtzmdcchhl.html

Py:   os.environ.get("HOME")
来源：http://hz.feifeiyinyue.top/gtdfsrefzq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.guannengcc.top/gtzvndwfet.html

JS:   process.env.HOME
来源：http://hz.kuanghao11.cn/gtjwuhrhdl.html

TS:   process.env.HOME
来源：http://hz.mhx1999.top/gtpwbnqvuz.html

Java: System.getenv("HOME")
来源：http://hz.nwbrower.top/gtlhwxvryd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.daria6918.cn/gteqriyjlf.html

Ruby: ENV["HOME"]
来源：http://hz.ybcxt.top/gtyzucgzlg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.sufxvd.cn/gtloeyyujo.html

[M03] 执行外部命令
来源：http://hz.dianchejie.cn/gtsnkcqcfg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jianghu66.top/gtbrperidc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.nanxinkj.top/gtevgmujzh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yanxiufei.cn/gtmmcfargh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuxming.cn/gtffyfpvst.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.guowangkeji.top/gtulkklwbe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.aizwys.cn/gtjvjagxhb.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yonumen.top/gtffglyuyy.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hywenlv.cn/gtwzooewju.html

[M04] 获取当前工作目录
来源：http://hz.cashguo.top/gtxvvvjjyw.html

Py:   os.getcwd()
来源：http://hz.cucudq.cn/gtjmxslsoh.html

PHP:  getcwd();
来源：http://hz.yj20258.top/gtulchdrrx.html

JS:   process.cwd()
来源：http://hz.fengsongda.top/gtfsjatjzn.html

TS:   process.cwd()
来源：http://hz.hammf.cn/gtetvnsljp.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.tianlin.xyz/gtywljgsbf.html

Go:   os.Getwd()
来源：http://hz.cheryme.top/gtuxmrdnqs.html

Ruby: Dir.pwd
来源：http://hz.daria6918.cn/gtncdkrlln.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.redwolf501.top/gtggxlqwfh.html

[M05] 设置退出码
来源：http://hz.snrcjt.cn/gtrzubwzdj.html

Py:   sys.exit(1)
来源：http://hz.dashuyun.cn/gtepmkeupn.html

PHP:  exit(1);
来源：http://hz.birdmap.top/gtquzaxbqx.html

JS:   process.exit(1)
来源：http://hz.zdqjudy.top/gtgtrqrdyg.html

TS:   process.exit(1)
来源：http://hz.quarkkingdee.top/gtvxltnyex.html

Java: System.exit(1)
来源：http://hz.dashuyun.cn/gtajnnuyvh.html

Go:   os.Exit(1)
来源：http://hz.jqgufenzy.top/gtihpuswhr.html

Ruby: exit 1
来源：http://hz.smart0.xyz/gthyjnnkmn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhongyouzk.top/gtejrzednn.html

[M06] 向标准错误输出
来源：http://hz.shanyushiyangtech.top/gtaxvvyvyp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ybcxt.top/gtcaxuztfl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ybcxt.top/gtxgtrbxip.html

JS:   console.error("err")
来源：http://hz.wangshuangyany.cn/gtfsrxywlt.html

TS:   console.error("err")
来源：http://hz.yvedp.cn/gtdmrpvgsi.html

Java: System.err.println("err")
来源：http://hz.zhengqikj.top/gtcsdwwzqa.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.haohaochexian.top/gtfwgnljnz.html

Ruby: warn "err"
来源：http://hz.kuanghao11.cn/gtfwladpff.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.svipenyu.cn/gtdpgwfcjn.html

[M07] 判断是否为主入口
来源：http://hz.zhaomingkeji.xyz/gtorikokor.html

Py:   if __name__ == "__main__":
来源：http://hz.jinqigufen.top/gtjtysaexx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shanyushiyangtech.top/gtyulqtqrc.html

JS:   require.main === module
来源：http://hz.yuxming.cn/gtqhzylrlf.html

TS:   require.main === module
来源：http://hz.jiagoushi.top/gtfdgvjnst.html

Java: public static void main(String[] args)
来源：http://hz.ehwqpu.com/gtyimmgdax.html

Go:   func main()
来源：http://hz.hywenlv.cn/gtfiwlppjw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.daria6918.cn/gtemgdbcyv.html

C#:   static void Main(string[] args)
来源：http://hz.tian-w.cn/gtrsixvrrz.html

[M08] 获取系统与运行时信息
来源：http://hz.dianchejie.cn/gttddjxmpj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.tian-w.cn/gtiyfbyemu.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yuanzhike.top/gtlbdrscfh.html

JS:   process.platform;  process.version
来源：http://hz.hongshengwenyu.top/gtjeiotliv.html

TS:   process.platform;  process.version
来源：http://hz.0kj1m.cn/gthoykhovx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jinqigfzy.top/gtsxclnacc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhixingplan.top/gtecztexuq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.aibaodan.cn/gtgekbsrdf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.dianchejie.cn/gtaijhwfyh.html

================================================================================
来源：http://hz.birdmap.top/gtnwnqbboi.html

N. 数据结构与算法
来源：http://hz.vqdsnc.cn/gtghdfyqhd.html

================================================================================
来源：http://hz.tian-w.cn/gtbylmmerk.html

[N01] 二分查找（有序数组）
来源：http://hz.52xcode.cn/gtpahtfyou.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.iojbl.cn/gtfkcgesvm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xuanzx.com/gtnuymslgn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gzhubu.top/gtjovjkrdu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.mhx1999.top/gtjlgeqxwz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cdnleiting.top/gtijtbrlml.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhoulong.xyz/gtmdimfnij.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yuanzhike.top/gtyprbfsom.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.smart0.xyz/gtxkobbpdx.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.dashuyun.cn/gtqkpjmjjb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zdqjudy.top/gthfspklix.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinghuilouyu.cn/gtdaafkayd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ybcxt.top/gtxcirvmzv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shuidangran.top/gtjgitgtjh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shanyushiyangkeji.top/gtjmxmquzi.html

Go:   slices.Sort(arr)
来源：http://hz.hammf.cn/gtdckjrscs.html

Ruby: arr.sort
来源：http://hz.vqdsnc.cn/gtjdpltlqy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.nwbrower.top/gtvaqrzszs.html

[N03] 快速排序（分治示例）
来源：http://hz.gotoacloud.top/gtgujtccot.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shanyushiyangkeji.top/gtuxvnqlqr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.meibo888.top/gtvvtwratx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgufenzy.top/gtyaxnzdxe.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hysaishi.cn/gtepurqtur.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.wangdashe.top/gtogjrcbha.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.snrcjt.cn/gtkjzdmvgh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shanyushiyangkeji.top/gtbvycjxco.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hysaishi.cn/gtdtydbeli.html

[N04] 斐波那契数列
来源：http://hz.quarkkingdee.top/gtyxtizxjx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhengqikj.top/gtfcurdpqo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shanyushiyangkeji.top/gtxpmfoqqj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xingfuxueyuan.xyz/gtzrkzebku.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258.top/gtgdkewoxl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yj20258888.top/gtlobsfzdl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.svipenyu.cn/gtqruymsbr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.meibo888.top/gtrrompivc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xziqi.cn/gtaxbshkvz.html

[N05] 最大公约数
来源：http://hz.sxryk.cn/gtabfgfzjh.html

Py:   math.gcd(a, b)
来源：http://hz.shzxlz.cn/gtukbchaxu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hfpthk.cn/gtoipmhaaw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hywenlv.cn/gttlzsgvio.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.haohaochexian.top/gtbpxlrbhh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.nanxuanxn.top/gtocoxlccb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hammf.cn/gtsxymfblk.html

Ruby: a.gcd(b)
来源：http://hz.dashuyun.cn/gtooriftng.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhengqikj.top/gtpglbkqpl.html

[N06] 判断回文字符串
来源：http://hz.jiagoushi.top/gtmntniekk.html

Py:   s == s[::-1]
来源：http://hz.nanxinkj.top/gtuysyjcjw.html

PHP:  $s === strrev($s);
来源：http://hz.cheryme.top/gtsubdgpde.html

JS:   s === [...s].reverse().join("")
来源：http://hz.aizwys.cn/gtxzggywub.html

TS:   s === [...s].reverse().join("")
来源：http://hz.kuanghao11.cn/gtzcdqlhwp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xuanzx.com/gtttbhtwvy.html

Go:   // 双指针从两端比较
来源：http://hz.zhijiandao.cn/gteeaaqqka.html

Ruby: s == s.reverse
来源：http://hz.52xcode.cn/gtpodstjid.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jqgfzy.top/gtdvhrfscy.html

[N07] 两数之和（返回下标）
来源：http://hz.hongshengwenyu.top/gtpjgfcscz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ydjk.org.cn/gtsmqnqiho.html


<!-- 参考信息 -->