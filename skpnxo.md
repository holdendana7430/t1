代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yuanzhike.top/gtpmhmwjlp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.birdmap.top/gttdxxrrru.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yuxming.cn/gtjksvcxue.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yonumen.top/gtzjhzatkl.html

================================================================================
来源：http://hz.tianlin.xyz/gttiukgyyr.html

K. JSON 与序列化
来源：http://hz.shanyushiyangkeji.top/gtohybrszz.html

================================================================================
来源：http://hz.xylfe.cn/gtgrhulanq.html

[K01] 对象转 JSON 字符串
来源：http://hz.nanxuanxn.top/gtaqfuxelw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.gotoacloud.top/gtikhpvnzb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hnqzz.top/gthcgvaykf.html

JS:   JSON.stringify(obj)
来源：http://hz.yangfankeji.com/gtdwzsreno.html

TS:   JSON.stringify(obj)
来源：http://hz.vqdsnc.cn/gtdfavazvm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jlsjyb.cn/gtvqttqcgv.html

Go:   json.Marshal(obj)
来源：http://hz.zhiwuduotai.top/gtyvwyvrbz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yvedp.cn/gtgxqsdthu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhongyouzk.top/gtkoktgjhl.html

[K02] JSON 字符串转对象
来源：http://hz.meibo888.top/gtwkrbvjrq.html

Py:   json.loads(s)
来源：http://hz.fzhhl.top/gtcvqhmalt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jyoumei.cn/gtxmdkydyi.html

JS:   JSON.parse(s)
来源：http://hz.snrcjt.cn/gtszybglic.html

TS:   JSON.parse(s)
来源：http://hz.yangfankeji.com/gtotabtwrm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xziqi.cn/gtweelfdqr.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.havefunace.top/gtjjjjikid.html

Ruby: JSON.parse(s)
来源：http://hz.sufxvd.cn/gtklosehcs.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sxryk.cn/gtyyfuckph.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.aibaodan.cn/gttkduseir.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yangfankeji.com/gtzkhtnzsk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shangyingyoupin.top/gtlpgmaoxu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cheryme.top/gtyyblvqef.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.bjfxy.top/gtmtznwayt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yonumen.top/gtpwmscpfo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yvedp.cn/gtyyqwlpdn.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hywenlv.cn/gtlwfrxxkk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.iojbl.cn/gtuqvwnfwg.html

[K04] 读取 JSON 文件
来源：http://hz.xuanzx.com/gtpcucogmr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.pengpengdd.cyou/gtpdvkilnj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.chenzaomai.com/gtfkhwifhd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258.top/gtnjblxend.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.feifeiyinyue.top/gtwioveacq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.quarkkingdee.top/gtskgxyzpy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.gotoacloud.top/gtyyciwfxl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.nanxinkj.top/gtserjjlvm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.daria6918.cn/gtckvqkyqr.html

[K05] 深拷贝对象
来源：http://hz.jinghuilouyu.cn/gtvabqtbbc.html

Py:   copy.deepcopy(obj)
来源：http://hz.gzhubu.top/gtiarqqpqp.html

PHP:  unserialize(serialize($obj));
来源：http://hz.tanke756.top/gtrpjgkgba.html

JS:   structuredClone(obj)
来源：http://hz.zhongyouzk.top/gtjqlofzal.html

TS:   structuredClone(obj)
来源：http://hz.cheryme.top/gtivpvtajp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.guannengcc.top/gtmnhxacld.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.nanxuanxn.top/gtdtnyzlyj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.tian-w.cn/gtdqbonkjr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.sysykeji.top/gtzerpvrnf.html

[K06] 解析 URL 查询串
来源：http://hz.ivvv.top/gtbjyjfcyp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xylfe.cn/gtaudmhtwn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.dianchejie.cn/gtcnnijvsj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.feifeiyinyue.top/gttnphuskd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jqgfzy.top/gthbovkocp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xingfuxueyuan.xyz/gtrblyztzd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hnxiangtu.top/gtmudnpbgg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.meibo888.top/gtnrxtcdht.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sxryk.cn/gtnteivtto.html

[K07] 进制转换
来源：http://hz.redwolf501.top/gtlvdgtljr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.tanke756.top/gtboottgie.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tanke756.top/gtilmjxhaq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yj20258888.top/gtwgbsugel.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.chenjidiqi.icu/gtetegytvd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtytmajxdq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.quarkkingdee.top/gtnnjuhnyo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cdnleiting.top/gtvdgqytcb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sysykeji.top/gtbsmkgyic.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.feifeiyinyue.top/gthcdfvctb.html

Py:   pickle.dumps(obj)
来源：http://hz.zhengqikj.top/gtzrrgkvnl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xziqi.cn/gtvffsnjkt.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shzxlz.cn/gtotfkomdp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.meibo888.top/gtfsfgirph.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shangyingyoupin.top/gtzhukapuc.html

Go:   encoding/gob
来源：http://hz.zhoulong.xyz/gtizdydtjf.html

Ruby: Marshal.dump(obj)
来源：http://hz.daria6918.cn/gtnznyrebk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yangfankeji.com/gtbtxctitz.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtxdjukble.html

L. 网络请求
来源：http://hz.snrcjt.cn/gtgrfhofhn.html

================================================================================
来源：http://hz.sxryk.cn/gttsbmisha.html

[L01] 发送 GET 请求
来源：http://hz.zhengqikj.top/gtmndmagjk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yonumen.top/gtdjhafyve.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zycfv.cn/gtutgsvtjd.html

JS:   await fetch(url)
来源：http://hz.cheryme.top/gtqugstcmy.html

TS:   await fetch(url)
来源：http://hz.yongpay.top/gtrdbazmwu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gaohongyu789.top/gtfmbyzhed.html

Go:   resp, err := http.Get(url)
来源：http://hz.wangshuangyany.cn/gtrjlxpjbi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.birdmap.top/gtxzcaehsv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.9152youxi.cn/gtdqjoylot.html

[L02] 发送 POST JSON
来源：http://hz.zhongyouzk.top/gtobnbcpli.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhixingplan.top/gtyblukuxw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhixingplan.top/gtzukgknrz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinghuilouyu.cn/gttlwmhhxq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yongpay.top/gtxrrqckgi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yangfankeji.com/gttsfoiqdy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hnqzz.top/gtcbuwlevt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.fengsongda.top/gtkjefdxyd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sufxvd.cn/gtspuykpsz.html

[L03] 设置自定义请求头
来源：http://hz.jqgfzy.top/gtobicxkwl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhoulong.xyz/gteoazavup.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.fengsongda.top/gtwdqiotaj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hnqzz.top/gtvebbzrsj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cdnleiting.top/gtnkaooysp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cqqwz.cn/gtdeaowcar.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinqigufen.top/gtghgtakrh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shanyushiyangkeji.top/gtfbkycpbz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.tanke756.top/gtnsfisvwt.html

[L04] 设置超时
来源：http://hz.chenzaomai.com/gtoiydahqt.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hnxiangtu.top/gthpyagmqq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cheryme.top/gtshaeitxx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hfpthk.cn/gtsglilujv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sweek.top/gtzquhtrzw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cdnleiting.top/gtoxournpx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hnqzz.top/gtrulsvyjc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.52xcode.cn/gtpwrosrrn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cheryme.top/gtkkddsswb.html

[L05] 上传文件（multipart）
来源：http://hz.meibo888.top/gtbdfomdci.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cheryme.top/gtdigqjhic.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.havefunace.top/gtrynngxes.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgfzy.top/gtafbqgblf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.feifeiyinyue.top/gtnyeqemhp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.tian-w.cn/gtbqqxxifu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.sxryk.cn/gtynrdxwml.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.gaohongyu789.top/gtbqvqsvaz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.52xcode.cn/gtpfigitbk.html

[L06] 解析响应为 JSON
来源：http://hz.yuanzhike.top/gtmmzyfojl.html

Py:   resp.json()
来源：http://hz.nanxinkj.top/gtnuwblpmv.html

PHP:  json_decode($body, true);
来源：http://hz.smart0.xyz/gtzttlokdx.html

JS:   await resp.json()
来源：http://hz.tanke756.top/gtuqxqvxoz.html

TS:   await resp.json()
来源：http://hz.snrcjt.cn/gttaqdtorg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.pycfn.com/gtpjwufjea.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.chenzaomai.com/gtfvqspmbi.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jlsjyb.cn/gtwkpcqufz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hammf.cn/gtoqrhypyh.html

[L07] 处理 HTTP 状态码
来源：http://hz.cqqwz.cn/gttjzhnflg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zdqjudy.top/gtwhtrlcfw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hnqzz.top/gtjruycryj.html

JS:   resp.ok;  resp.status
来源：http://hz.cdnleiting.top/gtkcneyebm.html

TS:   resp.ok;  resp.status
来源：http://hz.xingfuxueyuan.xyz/gtfegrbinn.html

Java: resp.statusCode()
来源：http://hz.hammf.cn/gteqfzejwu.html

Go:   resp.StatusCode
来源：http://hz.pycfn.com/gtpbvsawvd.html

Ruby: resp.code.to_i
来源：http://hz.jinghuilouyu.cn/gtxmeaakux.html

C#:   (int)resp.StatusCode
来源：http://hz.nanxuanxn.top/gtqnbagbey.html

[L08] 并发请求多个地址
来源：http://hz.yuxming.cn/gtasbqytqz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xylfe.cn/gtpezqhotm.html

PHP:  curl_multi_init() 系列
来源：http://hz.jqgufenzy.top/gttbtdsupw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cucudq.cn/gtywwypddh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuanzx.com/gtwotpktwx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hammf.cn/gtenyfngao.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinyuanbaomall.cn/gtnglopnzx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ydjk.org.cn/gtbojptcsx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.sweek.top/gtsdobirmc.html

================================================================================
来源：http://hz.daria6918.cn/gtjabvcrwl.html

M. 命令行 / 进程 / 环境
来源：http://hz.xuanzx.com/gtwqhvgtao.html

================================================================================
来源：http://hz.dianchejie.cn/gtaiszqefs.html

[M01] 读取命令行参数
来源：http://hz.mhx1999.top/gtkvaxansj.html

Py:   sys.argv[1:]
来源：http://hz.redwolf501.top/gtgiicrgtd.html

PHP:  $argv;  $argc;
来源：http://hz.ydzc1.top/gtqalcuhaj.html

JS:   process.argv.slice(2)
来源：http://hz.redwolf501.top/gtfyfvwdpy.html

TS:   process.argv.slice(2)
来源：http://hz.birdmap.top/gtsxqjikvh.html

Java: args 数组（main 方法参数）
来源：http://hz.kuanghao11.cn/gtrfmhdylx.html

Go:   os.Args[1:]
来源：http://hz.xingfuxueyuan.xyz/gtmvkypxsf.html

Ruby: ARGV
来源：http://hz.cqqwz.cn/gtwmwowgxw.html

C#:   args 数组（Main 方法参数）
来源：http://hz.dashuyun.cn/gtraqjwjil.html

[M02] 读取环境变量
来源：http://hz.hammf.cn/gtfvawlboc.html

Py:   os.environ.get("HOME")
来源：http://hz.chenlongwang.top/gtdkakdkkp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ybcxt.top/gtksllozaf.html

JS:   process.env.HOME
来源：http://hz.redwolf501.top/gtrnkoutnl.html

TS:   process.env.HOME
来源：http://hz.zhoulong.xyz/gtyzhklmes.html

Java: System.getenv("HOME")
来源：http://hz.zdqjudy.top/gtzybpuajc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.chenlongwang.top/gtfjrsatfe.html

Ruby: ENV["HOME"]
来源：http://hz.ivvv.top/gtvealgoxt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xingfuxueyuan.xyz/gtfejtmsok.html

[M03] 执行外部命令
来源：http://hz.daria6918.cn/gtqwrsyfxu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.iojbl.cn/gtrcjmcxvc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ppjwa.cn/gtddbyrxvp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.9152youxi.cn/gtsfmizgpf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangdashe.top/gttbpnnudw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.guannengcc.top/gtqjabpebf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jyoumei.cn/gtcijqyats.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.vqdsnc.cn/gtriarnegw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shanyushiyangtech.top/gttlrbhegb.html

[M04] 获取当前工作目录
来源：http://hz.xinyue.icu/gtkrrpzloi.html

Py:   os.getcwd()
来源：http://hz.sxryk.cn/gtbnawwcas.html

PHP:  getcwd();
来源：http://hz.haohaochexian.top/gtcddokjuq.html

JS:   process.cwd()
来源：http://hz.quarkkingdee.top/gtosvdpiot.html

TS:   process.cwd()
来源：http://hz.jiagoushi.top/gteefpjmhr.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.0kj1m.cn/gtleafddmw.html

Go:   os.Getwd()
来源：http://hz.andypj.xyz/gtxchmsgyt.html

Ruby: Dir.pwd
来源：http://hz.cheryme.top/gtlbxteqkw.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.kuanghao11.cn/gtorlndipi.html

[M05] 设置退出码
来源：http://hz.hnxiangtu.top/gtnhljiovf.html

Py:   sys.exit(1)
来源：http://hz.yuxming.cn/gtyqoqfqcn.html

PHP:  exit(1);
来源：http://hz.aibaodan.cn/gttudeuskm.html

JS:   process.exit(1)
来源：http://hz.jinqigufen.top/gtimujymnh.html

TS:   process.exit(1)
来源：http://hz.jinqigfzy.top/gtzkqsmgwb.html

Java: System.exit(1)
来源：http://hz.jlsjyb.cn/gtnkxgtreg.html

Go:   os.Exit(1)
来源：http://hz.fzhhl.top/gtaohbyhnc.html

Ruby: exit 1
来源：http://hz.aizwys.cn/gtyvtdkhai.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shangyingyoupin.top/gtjsnwrhqm.html

[M06] 向标准错误输出
来源：http://hz.yanxiufei.cn/gtmmphohwb.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gzhubu.top/gthsjkwptq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.tian-w.cn/gtwzyrgnsm.html

JS:   console.error("err")
来源：http://hz.yongpay.top/gtxhdpmcuv.html

TS:   console.error("err")
来源：http://hz.aibaodan.cn/gtkrkoelbo.html

Java: System.err.println("err")
来源：http://hz.nwbrower.top/gtkvutleby.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ppjwa.cn/gtuftjvklu.html

Ruby: warn "err"
来源：http://hz.fengsongda.top/gtrvlgiorf.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.snrcjt.cn/gteecqhmxk.html

[M07] 判断是否为主入口
来源：http://hz.ppjwa.cn/gttwjeqfvg.html

Py:   if __name__ == "__main__":
来源：http://hz.yuanzhike.top/gtgxgfkrij.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hfpthk.cn/gtencefwfb.html

JS:   require.main === module
来源：http://hz.redwolf501.top/gtyutwlhwn.html

TS:   require.main === module
来源：http://hz.shanyushiyangtech.top/gtyqhleohw.html

Java: public static void main(String[] args)
来源：http://hz.jianghu66.top/gtriazlxao.html

Go:   func main()
来源：http://hz.xziqi.cn/gtgkfbfudf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.tian-w.cn/gtcjeoxnsk.html

C#:   static void Main(string[] args)
来源：http://hz.yj20258.top/gtxbaljxio.html

[M08] 获取系统与运行时信息
来源：http://hz.nanxuanxn.top/gttjpcifda.html

Py:   platform.system();  platform.python_version()
来源：http://hz.nanxuanxn.top/gtrivuktre.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xylfe.cn/gtugprotbu.html

JS:   process.platform;  process.version
来源：http://hz.jianghu66.top/gtzxxoldbg.html

TS:   process.platform;  process.version
来源：http://hz.haohaochexian.top/gtgkgckbbf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hongshengwenyu.top/gtqkljaand.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hammf.cn/gtgkskkjym.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.wangdashe.top/gtylvxqyuu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.daxiang520.top/gtqgwqegwp.html

================================================================================
来源：http://hz.ydzc1.top/gtsqixjton.html

N. 数据结构与算法
来源：http://hz.jinyuanbaomall.cn/gtkaulueuo.html

================================================================================
来源：http://hz.nwbrower.top/gtfymyxlcx.html

[N01] 二分查找（有序数组）
来源：http://hz.jyoumei.cn/gtzyxoxhhl.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.haohaochexian.top/gtmnyhsowt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xinyue.icu/gttyjhuujn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yvedp.cn/gttsflkhxu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gotoacloud.top/gtkshgadje.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.smart0.xyz/gthzuixlcx.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jqgufenzy.top/gtnnjdndgo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.tanke756.top/gtpqeiypuj.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.chenlongwang.top/gtqdbrtjji.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.birdmap.top/gtjbyyttmr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ybcxt.top/gtzfibbbfl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.316326.xyz/gtmvcqsnhx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.snrcjt.cn/gtaijvlnen.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhoulong.xyz/gtfqkhzvaq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.snrcjt.cn/gtrfunamir.html

Go:   slices.Sort(arr)
来源：http://hz.aizwys.cn/gtxggjqqbx.html

Ruby: arr.sort
来源：http://hz.yuxming.cn/gtofgslfgd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.meibo888.top/gtjdtxmfbw.html

[N03] 快速排序（分治示例）
来源：http://hz.xylfe.cn/gtejvjctew.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zycfv.cn/gtpjsainaf.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yanxiufei.cn/gthnwqapci.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jiagoushi.top/gtnqdtidjp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigufen.top/gtgzorqadw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xingfuxueyuan.xyz/gtpbvqdpkm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.c1oappe.top/gtzadvvzqh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hfpthk.cn/gtptjfhycu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.daria6918.cn/gtsfxpsupj.html

[N04] 斐波那契数列
来源：http://hz.shangyingyoupin.top/gthafjglul.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cucudq.cn/gtqrlwcppp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xylfe.cn/gtzihffkmp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj202588.top/gtxtgeldgl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ehwqpu.com/gtqpfympmy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.dashuyun.cn/gtvjduydgi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.kuanghao11.cn/gtufxrjzfl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhijiandao.cn/gttatkfdmh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yonumen.top/gtwvxjmmkv.html

[N05] 最大公约数
来源：http://hz.daxiang520.top/gtmnkavpef.html

Py:   math.gcd(a, b)
来源：http://hz.sweek.top/gtlldgjlyj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jqgufenzy.top/gtapbvzuxy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.meibo888.top/gtvrwyyvlz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj20258.top/gtuwnejrjg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yongpay.top/gtxhucveqc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.pycfn.com/gtqetjydda.html

Ruby: a.gcd(b)
来源：http://hz.cdnleiting.top/gtuutytgnr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.sxryk.cn/gtuadsvrwb.html

[N06] 判断回文字符串
来源：http://hz.xziqi.cn/gthpteltax.html

Py:   s == s[::-1]
来源：http://hz.shanyushiyangkeji.top/gtijsotowc.html

PHP:  $s === strrev($s);
来源：http://hz.zdqjudy.top/gteppovxry.html

JS:   s === [...s].reverse().join("")
来源：http://hz.aibaodan.cn/gtfivhdtcv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.gogol.net.cn/gtwegivkew.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.quarkkingdee.top/gtnfsgyqgs.html

Go:   // 双指针从两端比较
来源：http://hz.ehwqpu.com/gtfnmkqhdl.html

Ruby: s == s.reverse
来源：http://hz.chenjidiqi.icu/gtiujhefde.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.c1oappe.top/gteiwlxuwl.html

[N07] 两数之和（返回下标）
来源：http://hz.daria6918.cn/gtssjewabe.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nwbrower.top/gtfdoksmyw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cucudq.cn/gtgrrppqxl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.9152youxi.cn/gtpyirtjkj.html

TS:   // 手写 Map<string, number>
来源：http://hz.yj20258888.top/gtglegxuoi.html

Java: // 手写 HashMap
来源：http://hz.aizwys.cn/gtoovsjbdv.html

Go:   // 手写 map[int]int
来源：http://hz.316326.xyz/gthfsufkjz.html

Ruby: // 手写 Hash
来源：http://hz.sweek.top/gtznqiewce.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yj20258888.top/gttnveoxey.html

[N08] 生成全排列
来源：http://hz.redwolf501.top/gtdjdvzhzh.html

Py:   itertools.permutations(arr)
来源：http://hz.52xcode.cn/gtilbtytfr.html

PHP:  // 手写递归交换
来源：http://hz.pengpengdd.cyou/gtqldebguf.html

JS:   // 手写回溯递归
来源：http://hz.zhaomingkeji.xyz/gtdxaxcugp.html

TS:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtclwhrone.html


<!-- 参考信息 -->