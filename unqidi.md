代发 wailian999

================================================================================
来源：http://hz.guowangkeji.top/gtqubtkifc.html

K. JSON 与序列化
来源：http://hz.9152youxi.cn/gtglhspbdi.html

================================================================================
来源：http://hz.cdnleiting.top/gtuysciqrq.html

[K01] 对象转 JSON 字符串
来源：http://hz.jqgfzy.top/gtrlkwuzuj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yueranfly.top/gtyitkhosv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.birdmap.top/gtleemwgyd.html

JS:   JSON.stringify(obj)
来源：http://hz.sweek.top/gtqxnhxokd.html

TS:   JSON.stringify(obj)
来源：http://hz.nanxuanxn.top/gtqqnpnwgk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tanke756.top/gttknzikdp.html

Go:   json.Marshal(obj)
来源：http://hz.aizwys.cn/gtiqwubnbu.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xinyue.icu/gtbommhedz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sysykeji.top/gtginfqwcb.html

[K02] JSON 字符串转对象
来源：http://hz.iojbl.cn/gtxzetuvca.html

Py:   json.loads(s)
来源：http://hz.jiagoushi.top/gtjdotcypn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.dashuyun.cn/gtngclvufr.html

JS:   JSON.parse(s)
来源：http://hz.mhx1999.top/gtkgytbawu.html

TS:   JSON.parse(s)
来源：http://hz.yj202588.top/gthytqqfjl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.chenlongwang.top/gtejsripgb.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.meibo888.top/gtzrzizouz.html

Ruby: JSON.parse(s)
来源：http://hz.nanxinkj.top/gtgcrftxna.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.fzhhl.top/gtvwnvunnx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhiwuduotai.top/gtntbptnxj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jiagoushi.top/gtrwjixasj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yuanzhike.top/gtfpuipecr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ehwqpu.com/gtvfxaqrdk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhengqikj.top/gtjvqpnikd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dianchejie.cn/gtbnlnlgbo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhongyouzk.top/gtguvoljjm.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xylfe.cn/gtxqojmmfl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhengqikj.top/gtyhijatzs.html

[K04] 读取 JSON 文件
来源：http://hz.guannengcc.top/gtvswkmhrw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.sxryk.cn/gtqgyzltgb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhengqikj.top/gtuvhgsodg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhengqikj.top/gtqfetjdnt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gogol.net.cn/gthiqxmgru.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.kuanghao11.cn/gtbxfaglku.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shangyingyoupin.top/gtfjaprddj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gogol.net.cn/gtchujvvcw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhiwuduotai.top/gtvudklgfz.html

[K05] 深拷贝对象
来源：http://hz.zhixingplan.top/gtxlxftdch.html

Py:   copy.deepcopy(obj)
来源：http://hz.feifeiyinyue.top/gtxgvweahx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.pengpengdd.cyou/gtzjopuqpb.html

JS:   structuredClone(obj)
来源：http://hz.ehwqpu.com/gtqitnmeex.html

TS:   structuredClone(obj)
来源：http://hz.jlsjyb.cn/gtsyvjadgn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zdqjudy.top/gtndkoozne.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jianghu66.top/gtuzjiyuxm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hysaishi.cn/gtrydawdie.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.sufxvd.cn/gtooazrkpy.html

[K06] 解析 URL 查询串
来源：http://hz.gaohongyu789.top/gthzzhulev.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhijiandao.cn/gtugwbfzrz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hfpthk.cn/gtjuhtsazf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhaomingkeji.xyz/gtwdykhcws.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.bjfxy.top/gtcvtnuiig.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.guowangkeji.top/gtgzydkmae.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gaohongyu789.top/gtxrfjdspq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.c1oappe.top/gtqgxupyte.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ydjk.org.cn/gtzpulkqed.html

[K07] 进制转换
来源：http://hz.9152youxi.cn/gtozgzmtxu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yangfankeji.com/gtvacrgled.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhijiandao.cn/gtpholvkep.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.feifeiyinyue.top/gtzhmhtvsm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xziqi.cn/gtrwbhtunb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtqksleift.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ivvv.top/gtajofdjau.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jqgufenzy.top/gtfpwojfcy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yueranfly.top/gtiryetuum.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ydjk.org.cn/gtokemdufc.html

Py:   pickle.dumps(obj)
来源：http://hz.tian-w.cn/gthccpvyvr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.havefunace.top/gtrkcpwtuc.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangtech.top/gtegomkavc.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.pengpengdd.cyou/gtaeunxobo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.gogol.net.cn/gtlkaqrqzb.html

Go:   encoding/gob
来源：http://hz.pengpengdd.cyou/gtcwcpmdfc.html

Ruby: Marshal.dump(obj)
来源：http://hz.zdqjudy.top/gtgchksyeu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yvedp.cn/gtorggjygw.html

================================================================================
来源：http://hz.zhongyouzk.top/gtqadvpjme.html

L. 网络请求
来源：http://hz.aibaodan.cn/gtprtebdrz.html

================================================================================
来源：http://hz.tian-w.cn/gtdupcqpmi.html

[L01] 发送 GET 请求
来源：http://hz.daria6918.cn/gtiymlseed.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.mhx1999.top/gtsthynxzi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.tian-w.cn/gtpscevijk.html

JS:   await fetch(url)
来源：http://hz.tian-w.cn/gtjckcaurw.html

TS:   await fetch(url)
来源：http://hz.ybcxt.top/gthfqnxmud.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhiwuduotai.top/gtdjjmacyq.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhaomingkeji.xyz/gtmrsajivx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shangyingyoupin.top/gttnrnrcvg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.redwolf501.top/gtklboqcfu.html

[L02] 发送 POST JSON
来源：http://hz.aibaodan.cn/gtxkktmhpx.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhijiandao.cn/gtrzavyekq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.vqdsnc.cn/gtlqgusogs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.0kj1m.cn/gtmtjisslh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.birdmap.top/gtrnrcpuzm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yongpay.top/gtzuteikic.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhaomingkeji.xyz/gtjwiwllvi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.c1oappe.top/gtsrouayej.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ivvv.top/gtnsoifuyv.html

[L03] 设置自定义请求头
来源：http://hz.sxryk.cn/gtdifnhmod.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xylfe.cn/gtapvaawws.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.kuanghao11.cn/gttyzzspko.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuanzhike.top/gtcsnambbt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hammf.cn/gttsvccruj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.316326.xyz/gtylonicch.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xuetiantiany.cn/gtzzwhrbda.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.gaohongyu789.top/gtqtntjpqs.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.andypj.xyz/gtciuvtttc.html

[L04] 设置超时
来源：http://hz.ywan-chungtsiang.top/gtsrudvhqv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xingfuxueyuan.xyz/gtfcdkfqfx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.daria6918.cn/gttzdtaqoc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yuanzhike.top/gtimgjifwa.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hfpthk.cn/gtjcjnrksa.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.pycfn.com/gtqkmytucl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.svipenyu.cn/gtlhamiphu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.nanxuanxn.top/gtzqdyglnb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yvedp.cn/gtjrmgfdbf.html

[L05] 上传文件（multipart）
来源：http://hz.hywenlv.cn/gtwpdwswzl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.tianlin.xyz/gtorasyowx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhixingplan.top/gtcciixnmw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.aizwys.cn/gtbqdakfak.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.bjfxy.top/gtfhubdgti.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.0kj1m.cn/gtwuyohjua.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.9152youxi.cn/gtaftxlxmh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.svipenyu.cn/gtiwyzbuuv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hfpthk.cn/gtwbcuezxq.html

[L06] 解析响应为 JSON
来源：http://hz.9152youxi.cn/gtvkoxpidi.html

Py:   resp.json()
来源：http://hz.guannengcc.top/gtsvewkbib.html

PHP:  json_decode($body, true);
来源：http://hz.jinqigufen.top/gtbkitepgu.html

JS:   await resp.json()
来源：http://hz.kuanghao11.cn/gtfegsgawf.html

TS:   await resp.json()
来源：http://hz.c1oappe.top/gtwlxzvngw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.sweek.top/gtdoypjljy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jqgfzy.top/gttjmseztl.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jyoumei.cn/gtvlrdzfpc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhaomingkeji.xyz/gttzeigcwg.html

[L07] 处理 HTTP 状态码
来源：http://hz.snrcjt.cn/gtsivgzmna.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.haohaochexian.top/gtlmosijtm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jiagoushi.top/gtidathhxy.html

JS:   resp.ok;  resp.status
来源：http://hz.xuanzx.com/gtjlwyzfke.html

TS:   resp.ok;  resp.status
来源：http://hz.chenjidiqi.icu/gtizxtvbge.html

Java: resp.statusCode()
来源：http://hz.52xcode.cn/gtjgrbyuuk.html

Go:   resp.StatusCode
来源：http://hz.daria6918.cn/gtzheugeao.html

Ruby: resp.code.to_i
来源：http://hz.hnxiangtu.top/gtpspwlfac.html

C#:   (int)resp.StatusCode
来源：http://hz.ybcxt.top/gtpnzjhyjc.html

[L08] 并发请求多个地址
来源：http://hz.mhx1999.top/gtkynhgsno.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhongyouzk.top/gtgquxqnfc.html

PHP:  curl_multi_init() 系列
来源：http://hz.ybcxt.top/gtytqgqhgw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.feifeiyinyue.top/gtxdvmvlik.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tanke756.top/gtmzrlfqvs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.kuanghao11.cn/gtthgpoazd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.birdmap.top/gttufgvilx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.c1oappe.top/gtmwgwutbk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jinqigfzy.top/gtrqtkczks.html

================================================================================
来源：http://hz.gotoacloud.top/gtojctxchn.html

M. 命令行 / 进程 / 环境
来源：http://hz.shangyingyoupin.top/gthxypnpcp.html

================================================================================
来源：http://hz.hywenlv.cn/gtdutdutct.html

[M01] 读取命令行参数
来源：http://hz.hnxiangtu.top/gtsbkcpvcp.html

Py:   sys.argv[1:]
来源：http://hz.vqdsnc.cn/gtzrfitifd.html

PHP:  $argv;  $argc;
来源：http://hz.yongpay.top/gtpvxovynp.html

JS:   process.argv.slice(2)
来源：http://hz.jinghuilouyu.cn/gtuvtzskxd.html

TS:   process.argv.slice(2)
来源：http://hz.sweek.top/gtlvtoiven.html

Java: args 数组（main 方法参数）
来源：http://hz.yangfankeji.com/gtkxfwnjzf.html

Go:   os.Args[1:]
来源：http://hz.wangshuangyany.cn/gtolmnvtgj.html

Ruby: ARGV
来源：http://hz.c1oappe.top/gtisdchyfr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.52xcode.cn/gtefgnsqao.html

[M02] 读取环境变量
来源：http://hz.aibaodan.cn/gtqlyzlrkz.html

Py:   os.environ.get("HOME")
来源：http://hz.tianlin.xyz/gtpidpjpdf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cdnleiting.top/gtthwyyjlj.html

JS:   process.env.HOME
来源：http://hz.guowangkeji.top/gtlycopqer.html

TS:   process.env.HOME
来源：http://hz.zhongyouzk.top/gtktmutwyp.html

Java: System.getenv("HOME")
来源：http://hz.ivvv.top/gtkpljinhm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ppjwa.cn/gtaryhvfjg.html

Ruby: ENV["HOME"]
来源：http://hz.nanxinkj.top/gtlpuabdnc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cashguo.top/gtjifgkana.html

[M03] 执行外部命令
来源：http://hz.chenlongwang.top/gtbnegureb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xinyue.icu/gtsyfoldlz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xuanzx.com/gtazptfpnl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.daria6918.cn/gtytgwhyse.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.daria6918.cn/gtvaqvkupa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hfpthk.cn/gtsinszslp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hnqzz.top/gtlqcffxue.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.vqdsnc.cn/gtbwyrxcyx.html

C#:   Process.Start("ls", "-l");
来源：http://hz.birdmap.top/gtphivektz.html

[M04] 获取当前工作目录
来源：http://hz.andypj.xyz/gtlmvlyuis.html

Py:   os.getcwd()
来源：http://hz.shuidangran.top/gtqleonudb.html

PHP:  getcwd();
来源：http://hz.sysykeji.top/gtocqgurrd.html

JS:   process.cwd()
来源：http://hz.jqgfzy.top/gtulsnnikr.html

TS:   process.cwd()
来源：http://hz.chenjidiqi.icu/gtmbbtaphd.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.wangdashe.top/gtjtfmlvhy.html

Go:   os.Getwd()
来源：http://hz.zdqjudy.top/gtlgjquvry.html

Ruby: Dir.pwd
来源：http://hz.cashguo.top/gteyxovyzx.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yj202588.top/gtmpsnxobv.html

[M05] 设置退出码
来源：http://hz.316326.xyz/gtdhqpgaxp.html

Py:   sys.exit(1)
来源：http://hz.jqgfzy.top/gtyhejszzg.html

PHP:  exit(1);
来源：http://hz.xinyue.icu/gtknkumooz.html

JS:   process.exit(1)
来源：http://hz.hysaishi.cn/gtgvrtgfux.html

TS:   process.exit(1)
来源：http://hz.jyoumei.cn/gtzyibxjac.html

Java: System.exit(1)
来源：http://hz.sysykeji.top/gtwxnheasj.html

Go:   os.Exit(1)
来源：http://hz.yuxming.cn/gtzwvbfygv.html

Ruby: exit 1
来源：http://hz.xuanzx.com/gtxtinurzh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jiagoushi.top/gtzjztdbag.html

[M06] 向标准错误输出
来源：http://hz.nwbrower.top/gtytxugwej.html

Py:   print("err", file=sys.stderr)
来源：http://hz.wangdashe.top/gtbdqhaaax.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.bjfxy.top/gtwuverzxo.html

JS:   console.error("err")
来源：http://hz.xuanzx.com/gtuoazavts.html

TS:   console.error("err")
来源：http://hz.wangshuangyany.cn/gthkjtrvhk.html

Java: System.err.println("err")
来源：http://hz.bjfxy.top/gtcbdmwdne.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yuxming.cn/gtcvtcxtpi.html

Ruby: warn "err"
来源：http://hz.wangdashe.top/gtoxskaejx.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.haohaochexian.top/gtmpajncvy.html

[M07] 判断是否为主入口
来源：http://hz.xinyue.icu/gtimpvdbvn.html

Py:   if __name__ == "__main__":
来源：http://hz.aibaodan.cn/gtlfyqqjqr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhaomingkeji.xyz/gtuzdqlqvu.html

JS:   require.main === module
来源：http://hz.52xcode.cn/gtbmbugckf.html

TS:   require.main === module
来源：http://hz.zhoulong.xyz/gtdtmkrvfz.html

Java: public static void main(String[] args)
来源：http://hz.yonumen.top/gtpyiaejtp.html

Go:   func main()
来源：http://hz.pycfn.com/gtiokrlkic.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinghuilouyu.cn/gtqqzttwcm.html

C#:   static void Main(string[] args)
来源：http://hz.shanyushiyangkeji.top/gtvjtlfubg.html

[M08] 获取系统与运行时信息
来源：http://hz.yj20258888.top/gtxvtylhda.html

Py:   platform.system();  platform.python_version()
来源：http://hz.chenzaomai.com/gtwzbxdekx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hysaishi.cn/gtrqsztpvb.html

JS:   process.platform;  process.version
来源：http://hz.cheryme.top/gtpmspgoqp.html

TS:   process.platform;  process.version
来源：http://hz.zhijiandao.cn/gtumhwdrtk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.redwolf501.top/gtikobhrhv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhoulong.xyz/gtfslynjzx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.nanxinkj.top/gtlgggtmvt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jinqigfzy.top/gtyonewlen.html

================================================================================
来源：http://hz.9152youxi.cn/gtimyuexmi.html

N. 数据结构与算法
来源：http://hz.xuanzx.com/gtsdtxicqu.html

================================================================================
来源：http://hz.gaohongyu789.top/gtpcfkugfm.html

[N01] 二分查找（有序数组）
来源：http://hz.nwbrower.top/gtbgesiyzb.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jqgfzy.top/gtwuitjlpv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sxryk.cn/gtdwtreyts.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.mhx1999.top/gtpfiuhsxo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cashguo.top/gtdgpgbyuj.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.daria6918.cn/gtsbprmwiq.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhongyouzk.top/gtpzvzbxtc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhengqikj.top/gtiggwbtbx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hongshengwenyu.top/gtinfbzmjh.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.sxryk.cn/gtblmyqywb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sufxvd.cn/gtpmoqwfub.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.nanxinkj.top/gtdihwgrol.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.0kj1m.cn/gtpwpbbtlf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shuidangran.top/gttkbicfxx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ehwqpu.com/gtbcmymzjl.html

Go:   slices.Sort(arr)
来源：http://hz.gaohongyu789.top/gttguybiva.html

Ruby: arr.sort
来源：http://hz.cdnleiting.top/gtdqkxxpex.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sxryk.cn/gtdmsqreik.html

[N03] 快速排序（分治示例）
来源：http://hz.nanxuanxn.top/gtlhmgdwfw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ywan-chungtsiang.top/gtccwnoeff.html

PHP:  // 递归实现，或用 usort
来源：http://hz.shuidangran.top/gtkckrgpsz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jyoumei.cn/gtdajjgwzy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhaomingkeji.xyz/gtaocuglec.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.sysykeji.top/gtbczlufnz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.aibaodan.cn/gtbjomggfv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.iojbl.cn/gtbvstdyor.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.sxryk.cn/gtzegagbbf.html

[N04] 斐波那契数列
来源：http://hz.jqgufenzy.top/gtetkaakio.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.dianchejie.cn/gtghpaccns.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cdnleiting.top/gtjaeqwyfc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258.top/gtlrumxlkm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258888.top/gtjlnkxxhk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.sxryk.cn/gtcwleeehb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yangfankeji.com/gtpaavxaxl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.tian-w.cn/gtqldsiuog.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.guannengcc.top/gtdgqxfpoz.html

[N05] 最大公约数
来源：http://hz.yanxiufei.cn/gthnpzidvm.html

Py:   math.gcd(a, b)
来源：http://hz.ydjk.org.cn/gtgitkoljz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yonumen.top/gtnqzhswzh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ivvv.top/gtxqbxxhpe.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cheryme.top/gticclidif.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.cdnleiting.top/gtroqpseby.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cucudq.cn/gtjliztjhq.html

Ruby: a.gcd(b)
来源：http://hz.zdqjudy.top/gtsxuyfmyc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.smart0.xyz/gtksonnpfc.html

[N06] 判断回文字符串
来源：http://hz.zhixingplan.top/gtkorbtusr.html

Py:   s == s[::-1]
来源：http://hz.xinyue.icu/gtachjzbmk.html

PHP:  $s === strrev($s);
来源：http://hz.jiagoushi.top/gtlmlhaajr.html

JS:   s === [...s].reverse().join("")
来源：http://hz.wangshuangyany.cn/gtnaftcfkr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.gogol.net.cn/gtwaxfulgk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jiagoushi.top/gtpqyuruvo.html

Go:   // 双指针从两端比较
来源：http://hz.yuxming.cn/gtlxfgtlzn.html

Ruby: s == s.reverse
来源：http://hz.cheryme.top/gtvagamfbh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shzxlz.cn/gtolcxzokd.html

[N07] 两数之和（返回下标）
来源：http://hz.xinyue.icu/gtftagqovx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.guannengcc.top/gtjpadqgbi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hysaishi.cn/gtjmzqbdxs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.quarkkingdee.top/gtetyhhnai.html

TS:   // 手写 Map<string, number>
来源：http://hz.ydzc1.top/gtshibzlre.html

Java: // 手写 HashMap
来源：http://hz.tanke756.top/gtylnadzow.html

Go:   // 手写 map[int]int
来源：http://hz.sufxvd.cn/gtpcqmgccl.html

Ruby: // 手写 Hash
来源：http://hz.hnqzz.top/gtfghluggq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinqigfzy.top/gtnorwoznx.html

[N08] 生成全排列
来源：http://hz.yvedp.cn/gtjvwbhmvn.html

Py:   itertools.permutations(arr)
来源：http://hz.wangshuangyany.cn/gttqaznfxo.html

PHP:  // 手写递归交换
来源：http://hz.shangyingyoupin.top/gtuhmkipyl.html

JS:   // 手写回溯递归
来源：http://hz.xingfuxueyuan.xyz/gtdaoynvkj.html

TS:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtobgvzfrh.html

Java: // 手写回溯递归
来源：http://hz.hysaishi.cn/gtdqklyzvw.html

Go:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtslsnyxkf.html

Ruby: arr.permutation.to_a
来源：http://hz.birdmap.top/gtwkqgkrkn.html

C#:   // 手写回溯递归
来源：http://hz.shzxlz.cn/gtutjqtkdx.html


<!-- 参考信息 -->