代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ehwqpu.com/gtfozitzip.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hywenlv.cn/gtfejbhwym.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.andypj.xyz/gttcvtohbd.html

[J10] 取今天 / 本月第一天
来源：http://hz.ywan-chungtsiang.top/gtahnhmnrk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jqgufenzy.top/gtnwuiydko.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.316326.xyz/gtjenwtlbv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.pycfn.com/gtoijrvxob.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ehwqpu.com/gtrjmlgcax.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.dashuyun.cn/gtpclilccn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhoulong.xyz/gtlveebnba.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hfpthk.cn/gtadbxorfe.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.wangshuangyany.cn/gtfilpunud.html

================================================================================
来源：http://hz.cashguo.top/gtywfbmfee.html

K. JSON 与序列化
来源：http://hz.cucudq.cn/gttlnrznnc.html

================================================================================
来源：http://hz.bjfxy.top/gtyznjspjv.html

[K01] 对象转 JSON 字符串
来源：http://hz.jqgfzy.top/gtwberydef.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xylfe.cn/gtkflgvseb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigfzy.top/gtfrxpbife.html

JS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangtech.top/gtgvymkkte.html

TS:   JSON.stringify(obj)
来源：http://hz.aibaodan.cn/gtrwkqtrez.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hfpthk.cn/gtehigikpu.html

Go:   json.Marshal(obj)
来源：http://hz.ydjk.org.cn/gtssdwmtlo.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.nanxinkj.top/gtndolaghg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hammf.cn/gtdatpvhlu.html

[K02] JSON 字符串转对象
来源：http://hz.zhiwuduotai.top/gtxdhovlrx.html

Py:   json.loads(s)
来源：http://hz.jinqigufen.top/gtptdkmcun.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hongshengwenyu.top/gtuiyxxtaa.html

JS:   JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gttrwkftwr.html

TS:   JSON.parse(s)
来源：http://hz.xuanzx.com/gtovvrvpmw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinghuilouyu.cn/gtlygzxwzb.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.wangdashe.top/gtlzuvuuhg.html

Ruby: JSON.parse(s)
来源：http://hz.aizwys.cn/gtjlksxbsq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.aizwys.cn/gtfrlgoyzd.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.pycfn.com/gtjoezfmyo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hysaishi.cn/gtzqvifypj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hnxiangtu.top/gtkvfateej.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.sufxvd.cn/gtuyeezced.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.pengpengdd.cyou/gtqcfxzbey.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hammf.cn/gtcxnmthrx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gzhubu.top/gtftxxksse.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.shangyingyoupin.top/gtjlpujhft.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.fzhhl.top/gtdfamzzsb.html

[K04] 读取 JSON 文件
来源：http://hz.tianlin.xyz/gtfecgnyhq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.tanke756.top/gttnkeqjxv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ppjwa.cn/gtcnqepkij.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.daria6918.cn/gtodzdnxwh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yvedp.cn/gtcjbawlfd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.fengsongda.top/gtdvtxijna.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cheryme.top/gtearlpjqz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.haohaochexian.top/gtwpbltkxx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ehwqpu.com/gteorlblsx.html

[K05] 深拷贝对象
来源：http://hz.aibaodan.cn/gtqxyejsef.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinqigfzy.top/gtwrleuhsl.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jianghu66.top/gtcmlsovwy.html

JS:   structuredClone(obj)
来源：http://hz.nanxinkj.top/gtbkxcynyo.html

TS:   structuredClone(obj)
来源：http://hz.meibo888.top/gtrdjyulag.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jyoumei.cn/gtmoyuqffj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenjidiqi.icu/gtsmsxhwur.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.chenlongwang.top/gtifutgrlj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shanyushiyangtech.top/gtdfulrrrr.html

[K06] 解析 URL 查询串
来源：http://hz.316326.xyz/gtpsyljpfo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sweek.top/gtyknnibjm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yueranfly.top/gtswozenof.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cashguo.top/gtddxoqugm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cqqwz.cn/gtxaaeuxij.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.svipenyu.cn/gtgiukhkvd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.vqdsnc.cn/gtmffoeyhu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ydjk.org.cn/gtewshfqud.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.nwbrower.top/gthilbqrng.html

[K07] 进制转换
来源：http://hz.iojbl.cn/gtubkovqqa.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xuetiantiany.cn/gtukdhqyiz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhoulong.xyz/gtjrqnulgx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.fzhhl.top/gthjvvxsja.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtfumtmivi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhixingplan.top/gtwhjdyxej.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yonumen.top/gtgojsdmqk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinghuilouyu.cn/gtsyhgscoi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.tianlin.xyz/gtbqsvwiar.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xuanzx.com/gteajsiigu.html

Py:   pickle.dumps(obj)
来源：http://hz.ivvv.top/gtixmyoivu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.aizwys.cn/gtapsigncz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hywenlv.cn/gtragqlsdy.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jinqigufen.top/gtuqfgcrtu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yvedp.cn/gtnoyjfbnt.html

Go:   encoding/gob
来源：http://hz.pycfn.com/gtlnyyborf.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhengqikj.top/gtrtszejab.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.fzhhl.top/gtnvbwqedx.html

================================================================================
来源：http://hz.52xcode.cn/gtqwrazqcx.html

L. 网络请求
来源：http://hz.vqdsnc.cn/gtikrvnsrs.html

================================================================================
来源：http://hz.bjfxy.top/gtnmzprzcg.html

[L01] 发送 GET 请求
来源：http://hz.andypj.xyz/gtqsztgzzz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinyuanbaomall.cn/gtzeqmosro.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xuanzx.com/gtvtwtjcsc.html

JS:   await fetch(url)
来源：http://hz.zhongyouzk.top/gtregvpbri.html

TS:   await fetch(url)
来源：http://hz.chenlongwang.top/gtpzenphnp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yanxiufei.cn/gtwmhwufny.html

Go:   resp, err := http.Get(url)
来源：http://hz.hongshengwenyu.top/gtdksbogxt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xuetiantiany.cn/gtdgnmdhrg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.pycfn.com/gtcqidffuj.html

[L02] 发送 POST JSON
来源：http://hz.dashuyun.cn/gtpmlzkxrr.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.fengsongda.top/gtpwodwdlb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zdqjudy.top/gtabzcbigo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dianchejie.cn/gtxdxwwmpv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.kuanghao11.cn/gtwsmyhiea.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhaomingkeji.xyz/gtlubnwcbs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.gogol.net.cn/gtxapjnmyz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ydzc1.top/gtoxkyqvuk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.tanke756.top/gtmitsgpgw.html

[L03] 设置自定义请求头
来源：http://hz.birdmap.top/gtaebbonju.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.tian-w.cn/gtqarknzpe.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.fzhhl.top/gtgqlsaubv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cucudq.cn/gtkojcnbsm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhixingplan.top/gtmmtugpaw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.chenjidiqi.icu/gtmekukdda.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinghuilouyu.cn/gtgkidukhj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.nwbrower.top/gtympivisc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.meibo888.top/gtsfkscxda.html

[L04] 设置超时
来源：http://hz.yuanzhike.top/gtncalvbyp.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yj20258.top/gtrgpuqkec.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yj202588.top/gtetlsprpt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zdqjudy.top/gtgtaplndi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dashuyun.cn/gtlofkrrtt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gotoacloud.top/gtbuzilerh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.havefunace.top/gtwkpdmnrz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yuxming.cn/gtqlfdiqza.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cucudq.cn/gtbvfrdixw.html

[L05] 上传文件（multipart）
来源：http://hz.xylfe.cn/gtjztvynic.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.smart0.xyz/gtbswhjhtk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shanyushiyangtech.top/gtmypdevwi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.birdmap.top/gtfnoclzqb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.andypj.xyz/gtxlhrwdlm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yanxiufei.cn/gtoapqukwn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jinqigfzy.top/gtluvjuyht.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xuetiantiany.cn/gtbaznazrp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yj20258.top/gtdgcdvvei.html

[L06] 解析响应为 JSON
来源：http://hz.yuanzhike.top/gtqxuufuua.html

Py:   resp.json()
来源：http://hz.bjfxy.top/gtwpzvzryw.html

PHP:  json_decode($body, true);
来源：http://hz.sysykeji.top/gtpfpxjxid.html

JS:   await resp.json()
来源：http://hz.hfpthk.cn/gtekgwotab.html

TS:   await resp.json()
来源：http://hz.nwbrower.top/gtontfwrrv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yangfankeji.com/gtivasqnpv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.pengpengdd.cyou/gtialqxkxh.html

Ruby: JSON.parse(resp.body)
来源：http://hz.nanxinkj.top/gtptfvxuqf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shanyushiyangkeji.top/gtrkouzypa.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinqigfzy.top/gtqctgfssk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.chenlongwang.top/gtzdzkyfrj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ivvv.top/gtldfxeyth.html

JS:   resp.ok;  resp.status
来源：http://hz.havefunace.top/gtlyfailka.html

TS:   resp.ok;  resp.status
来源：http://hz.aizwys.cn/gtjxfizoni.html

Java: resp.statusCode()
来源：http://hz.cdnleiting.top/gtmscyejom.html

Go:   resp.StatusCode
来源：http://hz.andypj.xyz/gtjscimnto.html

Ruby: resp.code.to_i
来源：http://hz.xziqi.cn/gtaxsukgkh.html

C#:   (int)resp.StatusCode
来源：http://hz.jinqigfzy.top/gtkvnzbgyw.html

[L08] 并发请求多个地址
来源：http://hz.sysykeji.top/gtdzkkvihb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.snrcjt.cn/gtgffonimt.html

PHP:  curl_multi_init() 系列
来源：http://hz.yuanzhike.top/gttfuxhigv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yangfankeji.com/gtybqyccgl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj202588.top/gtuahaprot.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.tanke756.top/gtuwkailsk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.snrcjt.cn/gtytogftfo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.chenzaomai.com/gtzqvxtybl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xuetiantiany.cn/gtvkcgmcid.html

================================================================================
来源：http://hz.0kj1m.cn/gtgyirhdgy.html

M. 命令行 / 进程 / 环境
来源：http://hz.vqdsnc.cn/gthnvsapev.html

================================================================================
来源：http://hz.yuxming.cn/gtqmdktcvr.html

[M01] 读取命令行参数
来源：http://hz.snrcjt.cn/gthfimzxtl.html

Py:   sys.argv[1:]
来源：http://hz.aizwys.cn/gtoizlccwk.html

PHP:  $argv;  $argc;
来源：http://hz.chenzaomai.com/gttnoyxatk.html

JS:   process.argv.slice(2)
来源：http://hz.tian-w.cn/gtoiefhkcy.html

TS:   process.argv.slice(2)
来源：http://hz.dashuyun.cn/gtltyaksqu.html

Java: args 数组（main 方法参数）
来源：http://hz.jlsjyb.cn/gtpafzjaje.html

Go:   os.Args[1:]
来源：http://hz.ydzc1.top/gtsygmohmr.html

Ruby: ARGV
来源：http://hz.yueranfly.top/gtdgyxhtim.html

C#:   args 数组（Main 方法参数）
来源：http://hz.c1oappe.top/gtoymzydry.html

[M02] 读取环境变量
来源：http://hz.0kj1m.cn/gtgmmlskkt.html

Py:   os.environ.get("HOME")
来源：http://hz.zhoulong.xyz/gtlyphuesx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.gogol.net.cn/gteqabkqps.html

JS:   process.env.HOME
来源：http://hz.xziqi.cn/gtaaigvtor.html

TS:   process.env.HOME
来源：http://hz.sufxvd.cn/gtcgenxbwr.html

Java: System.getenv("HOME")
来源：http://hz.andypj.xyz/gtqkbxtpig.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xuetiantiany.cn/gtfuzdpuns.html

Ruby: ENV["HOME"]
来源：http://hz.shanyushiyangtech.top/gtuviyokeu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhijiandao.cn/gtgxvstwzu.html

[M03] 执行外部命令
来源：http://hz.yj202588.top/gtnghpaynk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ivvv.top/gttjgivhko.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.aizwys.cn/gtrnpdcyqa.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sysykeji.top/gtbekucjtf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cheryme.top/gtiksmrbny.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jyoumei.cn/gtchnicxat.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.kuanghao11.cn/gtxponbsmj.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cdnleiting.top/gtkprgrhwr.html

C#:   Process.Start("ls", "-l");
来源：http://hz.daria6918.cn/gtsyndisvi.html

[M04] 获取当前工作目录
来源：http://hz.tian-w.cn/gtoxfspglt.html

Py:   os.getcwd()
来源：http://hz.zhengqikj.top/gtirxrswpc.html

PHP:  getcwd();
来源：http://hz.hfpthk.cn/gtnmwrciim.html

JS:   process.cwd()
来源：http://hz.shuidangran.top/gtukifpjps.html

TS:   process.cwd()
来源：http://hz.hongshengwenyu.top/gtmjifyoeq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.pengpengdd.cyou/gtdqzdergy.html

Go:   os.Getwd()
来源：http://hz.jinqigufen.top/gtiszszhzc.html

Ruby: Dir.pwd
来源：http://hz.hnxiangtu.top/gtwukzjnff.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jinqigufen.top/gtacdctnck.html

[M05] 设置退出码
来源：http://hz.52xcode.cn/gtjyzamqux.html

Py:   sys.exit(1)
来源：http://hz.guowangkeji.top/gtwqrijhyz.html

PHP:  exit(1);
来源：http://hz.ydjk.org.cn/gtapgrjuow.html

JS:   process.exit(1)
来源：http://hz.yangfankeji.com/gtubrywfwh.html

TS:   process.exit(1)
来源：http://hz.ywan-chungtsiang.top/gtlfhtfnqi.html

Java: System.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtdmbswvmx.html

Go:   os.Exit(1)
来源：http://hz.sysykeji.top/gtflxzhgyw.html

Ruby: exit 1
来源：http://hz.havefunace.top/gtqgduyrsa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jinqigufen.top/gtpccoazjn.html

[M06] 向标准错误输出
来源：http://hz.c1oappe.top/gtvjslmoff.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhixingplan.top/gttfmhdslk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shangyingyoupin.top/gtzmaqkogt.html

JS:   console.error("err")
来源：http://hz.bjfxy.top/gtxdnnujrm.html

TS:   console.error("err")
来源：http://hz.yuanzhike.top/gtmuzwcenr.html

Java: System.err.println("err")
来源：http://hz.shangyingyoupin.top/gtgdlhdtyv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.smart0.xyz/gtcmfueqoy.html

Ruby: warn "err"
来源：http://hz.dashuyun.cn/gtkntgekjp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yvedp.cn/gtwzqmxqjz.html

[M07] 判断是否为主入口
来源：http://hz.yvedp.cn/gtcidkhudr.html

Py:   if __name__ == "__main__":
来源：http://hz.xylfe.cn/gtenskncdx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.wangdashe.top/gtitldzivt.html

JS:   require.main === module
来源：http://hz.dashuyun.cn/gtftrvglqi.html

TS:   require.main === module
来源：http://hz.jinghuilouyu.cn/gtsfgmeqwu.html

Java: public static void main(String[] args)
来源：http://hz.hnqzz.top/gtkbqgxoxd.html

Go:   func main()
来源：http://hz.smart0.xyz/gtajjyfvfg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.316326.xyz/gtucttivtt.html

C#:   static void Main(string[] args)
来源：http://hz.gogol.net.cn/gtyhfewvcu.html

[M08] 获取系统与运行时信息
来源：http://hz.zhijiandao.cn/gtmsrtcynm.html

Py:   platform.system();  platform.python_version()
来源：http://hz.aibaodan.cn/gtdyinkymj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.guannengcc.top/gtiovcedoi.html

JS:   process.platform;  process.version
来源：http://hz.zdqjudy.top/gtvaxfbrxa.html

TS:   process.platform;  process.version
来源：http://hz.chenzaomai.com/gtykiqjqjp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hongshengwenyu.top/gtbthqezwz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhoulong.xyz/gtqpnufchi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.sysykeji.top/gtynhyjkcd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.tian-w.cn/gthccjzdnk.html

================================================================================
来源：http://hz.chenzaomai.com/gtovtzlcbi.html

N. 数据结构与算法
来源：http://hz.gaohongyu789.top/gtspaitbde.html

================================================================================
来源：http://hz.gogol.net.cn/gtsvwpzyln.html

[N01] 二分查找（有序数组）
来源：http://hz.iojbl.cn/gtlhchdsdn.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.smart0.xyz/gtfvwiylya.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xziqi.cn/gtojvwsnxz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hywenlv.cn/gtdeqqnvps.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.feifeiyinyue.top/gtbfuehocg.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.chenzaomai.com/gtbtiwoywi.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hnxiangtu.top/gttyuiyqgi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.bjfxy.top/gthrcjizlb.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.dianchejie.cn/gtixbhgukw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ivvv.top/gtqkodknub.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xingfuxueyuan.xyz/gtztejstrj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yonumen.top/gtrrzzfrep.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenjidiqi.icu/gtlnfakqyz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aibaodan.cn/gtfgkpmfnr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ppjwa.cn/gtgihitucf.html

Go:   slices.Sort(arr)
来源：http://hz.cdnleiting.top/gtxeolguqn.html

Ruby: arr.sort
来源：http://hz.shanyushiyangtech.top/gtwvnzfxgy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hnxiangtu.top/gtwnmffnzb.html

[N03] 快速排序（分治示例）
来源：http://hz.c1oappe.top/gtyxrtzwvd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.9152youxi.cn/gtjihikcgw.html

PHP:  // 递归实现，或用 usort
来源：http://hz.havefunace.top/gtdjjwgypw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.guannengcc.top/gtnqhewasw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.redwolf501.top/gtrtljkbbo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hnxiangtu.top/gtujnaolbk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.snrcjt.cn/gtgeacvakc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shuidangran.top/gtkzydcafy.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhengqikj.top/gtinietshw.html

[N04] 斐波那契数列
来源：http://hz.yangfankeji.com/gtddjkygnx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.tanke756.top/gtppefexai.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.chenlongwang.top/gtweckuatg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hammf.cn/gtwrjkxmdv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shangyingyoupin.top/gtodhusktq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhengqikj.top/gtbnpaothr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ydjk.org.cn/gthlxnjcvq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.52xcode.cn/gtscfaafxt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhaomingkeji.xyz/gtapqftvzf.html

[N05] 最大公约数
来源：http://hz.hammf.cn/gttdjrrare.html

Py:   math.gcd(a, b)
来源：http://hz.tianlin.xyz/gtvyiaopns.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhixingplan.top/gtwvonpwpw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shangyingyoupin.top/gtiticjnyf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinyuanbaomall.cn/gtmtzjmnat.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shuidangran.top/gtncpldncx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xuanzx.com/gtmuzxecbi.html

Ruby: a.gcd(b)
来源：http://hz.pengpengdd.cyou/gtugtffvvq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.quarkkingdee.top/gtubicdslw.html

[N06] 判断回文字符串
来源：http://hz.jlsjyb.cn/gtniyfxlux.html

Py:   s == s[::-1]
来源：http://hz.yongpay.top/gtcdbfimrs.html

PHP:  $s === strrev($s);
来源：http://hz.birdmap.top/gtfioztrty.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shanyushiyangkeji.top/gtpkttycbc.html

TS:   s === [...s].reverse().join("")
来源：http://hz.birdmap.top/gtxketruuh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xylfe.cn/gteexyqetg.html

Go:   // 双指针从两端比较
来源：http://hz.hammf.cn/gtoljhhivz.html

Ruby: s == s.reverse
来源：http://hz.yj20258888.top/gtiqmxdpsu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.9152youxi.cn/gtcftxavzy.html

[N07] 两数之和（返回下标）
来源：http://hz.cucudq.cn/gtjrrqvvwl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zycfv.cn/gtuternhng.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.sufxvd.cn/gtznrbmpbv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.tian-w.cn/gtqelnxnen.html

TS:   // 手写 Map<string, number>
来源：http://hz.yuanzhike.top/gthrkixztb.html

Java: // 手写 HashMap
来源：http://hz.aizwys.cn/gtluihhcab.html


<!-- 参考信息 -->