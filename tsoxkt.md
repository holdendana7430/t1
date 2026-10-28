代发 wailian999

================================================================================
来源：http://hz.gzhubu.top/gtfochkmzw.html

K. JSON 与序列化
来源：http://hz.hysaishi.cn/gtgrvnqqcr.html

================================================================================
来源：http://hz.tanke756.top/gtbfkogolv.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhaomingkeji.xyz/gtjxfbiuhb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.tian-w.cn/gtmsvghrsx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yj202588.top/gtyhxfdqdf.html

JS:   JSON.stringify(obj)
来源：http://hz.aibaodan.cn/gtvnxeczwe.html

TS:   JSON.stringify(obj)
来源：http://hz.cheryme.top/gtwwaqxwjq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.birdmap.top/gtpwwewjgm.html

Go:   json.Marshal(obj)
来源：http://hz.yongpay.top/gtbtyeoeps.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sufxvd.cn/gtxlrtsxfs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.havefunace.top/gtqqnrlhpn.html

[K02] JSON 字符串转对象
来源：http://hz.ivvv.top/gtiicavajm.html

Py:   json.loads(s)
来源：http://hz.cqqwz.cn/gtdqcnghyh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.wangshuangyany.cn/gthwkkvlef.html

JS:   JSON.parse(s)
来源：http://hz.svipenyu.cn/gtivtzfqbi.html

TS:   JSON.parse(s)
来源：http://hz.ppjwa.cn/gtvpyvwcqg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yangfankeji.com/gtggnzkmpb.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yueranfly.top/gtdhifauov.html

Ruby: JSON.parse(s)
来源：http://hz.chenzaomai.com/gterkncpyh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.guannengcc.top/gtlglfrzlt.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.meibo888.top/gtuwautwag.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ydjk.org.cn/gtkzmiqace.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shangyingyoupin.top/gtfzwfhsat.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydjk.org.cn/gtmcvlauln.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xingfuxueyuan.xyz/gtggbryhcd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yj20258888.top/gtbqiifbld.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gaohongyu789.top/gtwltcrubq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yj20258888.top/gtblyhfcbf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zycfv.cn/gtsshqurhb.html

[K04] 读取 JSON 文件
来源：http://hz.cashguo.top/gtblshexrk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.wangshuangyany.cn/gttfhvggwx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.aibaodan.cn/gtzkpajvnm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yongpay.top/gtxaiatugd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.bjfxy.top/gtwmkrndpu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.bjfxy.top/gtnagyjmva.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhixingplan.top/gtndgtszcm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yj20258888.top/gtonzbaead.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.smart0.xyz/gttrfnqnec.html

[K05] 深拷贝对象
来源：http://hz.ppjwa.cn/gtrhpwgifb.html

Py:   copy.deepcopy(obj)
来源：http://hz.jianghu66.top/gtuafvalop.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cqqwz.cn/gtpcszbnqv.html

JS:   structuredClone(obj)
来源：http://hz.tianlin.xyz/gtmnjfdzbq.html

TS:   structuredClone(obj)
来源：http://hz.hysaishi.cn/gtdqmanczo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xuetiantiany.cn/gtdzlulxlp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jqgufenzy.top/gtheoatohh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhongyouzk.top/gthxmdacwi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shzxlz.cn/gtgsdscrta.html

[K06] 解析 URL 查询串
来源：http://hz.ydzc1.top/gtyomtnxle.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xinyue.icu/gtwjlyuhin.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.kuanghao11.cn/gttekjteps.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zdqjudy.top/gtblcpdgcu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cdnleiting.top/gtxwfuhmom.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shuidangran.top/gttybkstsy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gotoacloud.top/gtfecdmhlu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.0kj1m.cn/gtxgcrzrpf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.kuanghao11.cn/gtksrohbpu.html

[K07] 进制转换
来源：http://hz.zhoulong.xyz/gtfphsbwsg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.fzhhl.top/gtiwlyutqj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cdnleiting.top/gtynymzczd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtvamihvbp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtfgtolzaq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.wangshuangyany.cn/gtkgllkfkt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.shzxlz.cn/gtyagcmqav.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.guowangkeji.top/gtobdlnsvs.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gtlguawigu.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.haohaochexian.top/gtxeljutlw.html

Py:   pickle.dumps(obj)
来源：http://hz.shanyushiyangtech.top/gtcviyphhi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cucudq.cn/gtmhhnqlmy.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ehwqpu.com/gtbxyqqjko.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.aibaodan.cn/gtzqxfpcgb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yvedp.cn/gtcjnuqwsh.html

Go:   encoding/gob
来源：http://hz.pycfn.com/gthdyyhlcf.html

Ruby: Marshal.dump(obj)
来源：http://hz.daria6918.cn/gtuhmqngfc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.chenzaomai.com/gtqltyfhul.html

================================================================================
来源：http://hz.yuanzhike.top/gtbcloaxex.html

L. 网络请求
来源：http://hz.havefunace.top/gttmengqci.html

================================================================================
来源：http://hz.52xcode.cn/gtyzqbmqjv.html

[L01] 发送 GET 请求
来源：http://hz.ywan-chungtsiang.top/gtuuzuduix.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.c1oappe.top/gtycnorfov.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yueranfly.top/gtweibquol.html

JS:   await fetch(url)
来源：http://hz.kuanghao11.cn/gtxipbmyca.html

TS:   await fetch(url)
来源：http://hz.cucudq.cn/gtiboylvnr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shuidangran.top/gtvvohigtc.html

Go:   resp, err := http.Get(url)
来源：http://hz.wangshuangyany.cn/gtqkusvkis.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xinyue.icu/gtcpjzansz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cqqwz.cn/gtozjaajpl.html

[L02] 发送 POST JSON
来源：http://hz.xuetiantiany.cn/gtutgrrxvq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.fengsongda.top/gtdrogjgej.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sxryk.cn/gtpoeyzoph.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gotoacloud.top/gtigsdteky.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shuidangran.top/gtoyoslfrf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj20258.top/gtvhcyaeci.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cashguo.top/gtxdrwsawn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yueranfly.top/gtmygtmxcz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xuetiantiany.cn/gtxzunxgco.html

[L03] 设置自定义请求头
来源：http://hz.hysaishi.cn/gtdnppogrq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xylfe.cn/gttsvdnouv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.meibo888.top/gtiscxnsda.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gzhubu.top/gtxyswkfuk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.316326.xyz/gtmhzrjybe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hammf.cn/gtgwascqab.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ydzc1.top/gtuiixupqa.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cdnleiting.top/gtqviwvsyc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.316326.xyz/gtavwjfgmw.html

[L04] 设置超时
来源：http://hz.hywenlv.cn/gtzhqgzdot.html

Py:   requests.get(url, timeout=5)
来源：http://hz.52xcode.cn/gtaededakl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xylfe.cn/gtdzqothnc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhijiandao.cn/gtgioaidsz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ydjk.org.cn/gticttjzyt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.aibaodan.cn/gtukhzeodp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ydjk.org.cn/gtgrlaviob.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tanke756.top/gtrxyawprc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.fzhhl.top/gtlividlrv.html

[L05] 上传文件（multipart）
来源：http://hz.tianlin.xyz/gtvurakqlo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.gotoacloud.top/gtukyzscbc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.meibo888.top/gtomxfmuns.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.nanxinkj.top/gtnmwpfzie.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.wangdashe.top/gtfvfwdhjo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cucudq.cn/gtvpoluefu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zdqjudy.top/gtmruxpxxt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shzxlz.cn/gtiszspvqs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhijiandao.cn/gtikzwovex.html

[L06] 解析响应为 JSON
来源：http://hz.xinyue.icu/gtmugxooml.html

Py:   resp.json()
来源：http://hz.chenlongwang.top/gtgkihuyui.html

PHP:  json_decode($body, true);
来源：http://hz.quarkkingdee.top/gtohakjmch.html

JS:   await resp.json()
来源：http://hz.yongpay.top/gtbglhqyvx.html

TS:   await resp.json()
来源：http://hz.quarkkingdee.top/gtszlppbgq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cheryme.top/gtrdnbpige.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gotoacloud.top/gtobdvoggj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jinqigfzy.top/gtnxamckvn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hfpthk.cn/gttkknjndm.html

[L07] 处理 HTTP 状态码
来源：http://hz.smart0.xyz/gtmqiqkkao.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.chenzaomai.com/gtuqfphaim.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.chenzaomai.com/gtfztdspil.html

JS:   resp.ok;  resp.status
来源：http://hz.jlsjyb.cn/gtjjkjaoli.html

TS:   resp.ok;  resp.status
来源：http://hz.birdmap.top/gtkiqpiaaf.html

Java: resp.statusCode()
来源：http://hz.hnqzz.top/gtpvinhxro.html

Go:   resp.StatusCode
来源：http://hz.zdqjudy.top/gtwepopbzw.html

Ruby: resp.code.to_i
来源：http://hz.xuetiantiany.cn/gtgozkhpvv.html

C#:   (int)resp.StatusCode
来源：http://hz.yvedp.cn/gtcmkgzvht.html

[L08] 并发请求多个地址
来源：http://hz.jinqigufen.top/gtcmednujy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xuetiantiany.cn/gtnmxukmca.html

PHP:  curl_multi_init() 系列
来源：http://hz.yj20258.top/gtjqkzggrc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.andypj.xyz/gtinwdnbyj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj20258.top/gtnywjvqvp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.guowangkeji.top/gtckmfjyvw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gogol.net.cn/gtalyxykyg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hammf.cn/gtfdtkpklv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gaohongyu789.top/gteztnknoe.html

================================================================================
来源：http://hz.zycfv.cn/gtdbttautk.html

M. 命令行 / 进程 / 环境
来源：http://hz.ivvv.top/gtmmpocoqh.html

================================================================================
来源：http://hz.yj20258.top/gtgedvfkfz.html

[M01] 读取命令行参数
来源：http://hz.shanyushiyangtech.top/gtluvycahd.html

Py:   sys.argv[1:]
来源：http://hz.aizwys.cn/gtmkzvihgs.html

PHP:  $argv;  $argc;
来源：http://hz.redwolf501.top/gtnjmqcuoz.html

JS:   process.argv.slice(2)
来源：http://hz.tanke756.top/gtyzborecs.html

TS:   process.argv.slice(2)
来源：http://hz.yj20258888.top/gtdqmibkio.html

Java: args 数组（main 方法参数）
来源：http://hz.smart0.xyz/gtnvslmutk.html

Go:   os.Args[1:]
来源：http://hz.gotoacloud.top/gtqvwmsnwb.html

Ruby: ARGV
来源：http://hz.hfpthk.cn/gtfjiugomk.html

C#:   args 数组（Main 方法参数）
来源：http://hz.bjfxy.top/gtboqsxilq.html

[M02] 读取环境变量
来源：http://hz.haohaochexian.top/gtwbcsycrb.html

Py:   os.environ.get("HOME")
来源：http://hz.xinyue.icu/gtswhdrpue.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.aizwys.cn/gtqpplyyvs.html

JS:   process.env.HOME
来源：http://hz.52xcode.cn/gtcmcecamo.html

TS:   process.env.HOME
来源：http://hz.yangfankeji.com/gtiapdvuua.html

Java: System.getenv("HOME")
来源：http://hz.chenjidiqi.icu/gtasakqldn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.52xcode.cn/gtkmlrbwie.html

Ruby: ENV["HOME"]
来源：http://hz.shanyushiyangkeji.top/gtaugbrmrd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.sxryk.cn/gtoiglnhmc.html

[M03] 执行外部命令
来源：http://hz.jlsjyb.cn/gtqgnlvgku.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jlsjyb.cn/gtiivvupzw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jqgufenzy.top/gthuxormrv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydjk.org.cn/gtakmsxdlb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.meibo888.top/gttjpskqnd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.tianlin.xyz/gtcbbycgpg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hywenlv.cn/gtqqzmpnet.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xinyue.icu/gtrhlqckck.html

C#:   Process.Start("ls", "-l");
来源：http://hz.redwolf501.top/gtnhluvyky.html

[M04] 获取当前工作目录
来源：http://hz.ybcxt.top/gtlbjrmnyf.html

Py:   os.getcwd()
来源：http://hz.jinqigufen.top/gtxavdoqnq.html

PHP:  getcwd();
来源：http://hz.zycfv.cn/gtrwdhhscn.html

JS:   process.cwd()
来源：http://hz.redwolf501.top/gtubdrvyht.html

TS:   process.cwd()
来源：http://hz.gogol.net.cn/gtysxjqcqy.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hfpthk.cn/gtnanytwwr.html

Go:   os.Getwd()
来源：http://hz.ppjwa.cn/gtjnrngjto.html

Ruby: Dir.pwd
来源：http://hz.sysykeji.top/gthjlrrhzn.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cdnleiting.top/gtxkxmgiox.html

[M05] 设置退出码
来源：http://hz.ppjwa.cn/gtzijeyspj.html

Py:   sys.exit(1)
来源：http://hz.ywan-chungtsiang.top/gtihifgmip.html

PHP:  exit(1);
来源：http://hz.jinqigufen.top/gtvghtugcq.html

JS:   process.exit(1)
来源：http://hz.aibaodan.cn/gtzmpqkxfn.html

TS:   process.exit(1)
来源：http://hz.shanyushiyangkeji.top/gtekegttui.html

Java: System.exit(1)
来源：http://hz.gaohongyu789.top/gtvvkgkazi.html

Go:   os.Exit(1)
来源：http://hz.jqgfzy.top/gtyvnlbtzr.html

Ruby: exit 1
来源：http://hz.jqgufenzy.top/gtkuuhljrx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jiagoushi.top/gtlhhfrsei.html

[M06] 向标准错误输出
来源：http://hz.sxryk.cn/gtdyidiuvl.html

Py:   print("err", file=sys.stderr)
来源：http://hz.daria6918.cn/gtmqhgydtw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.aibaodan.cn/gthzceiwdk.html

JS:   console.error("err")
来源：http://hz.gotoacloud.top/gtpbxzdcyw.html

TS:   console.error("err")
来源：http://hz.9152youxi.cn/gtkiprrwct.html

Java: System.err.println("err")
来源：http://hz.sweek.top/gtqkflfwdp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.chenlongwang.top/gtwgexzjrq.html

Ruby: warn "err"
来源：http://hz.cheryme.top/gtryzclors.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.nwbrower.top/gtdbwpuxnt.html

[M07] 判断是否为主入口
来源：http://hz.jinqigufen.top/gtvyvxqpvs.html

Py:   if __name__ == "__main__":
来源：http://hz.yj20258.top/gtixyrkvcl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ydjk.org.cn/gtqgllgcqt.html

JS:   require.main === module
来源：http://hz.yuanzhike.top/gtuvxtcgsj.html

TS:   require.main === module
来源：http://hz.jinqigfzy.top/gtqlmporwa.html

Java: public static void main(String[] args)
来源：http://hz.yonumen.top/gtknriuusg.html

Go:   func main()
来源：http://hz.xziqi.cn/gtbkdddynx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.svipenyu.cn/gtsgocphlb.html

C#:   static void Main(string[] args)
来源：http://hz.fengsongda.top/gtgeocphpu.html

[M08] 获取系统与运行时信息
来源：http://hz.chenzaomai.com/gtjpzjnnai.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ydjk.org.cn/gtkecufunl.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.wangshuangyany.cn/gtaggezmxv.html

JS:   process.platform;  process.version
来源：http://hz.gaohongyu789.top/gtrrlcqreu.html

TS:   process.platform;  process.version
来源：http://hz.pengpengdd.cyou/gtlvwwbnlt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.pycfn.com/gtylulygxf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yongpay.top/gtizzydfwx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.9152youxi.cn/gthggdavyy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yonumen.top/gtyhfdgutq.html

================================================================================
来源：http://hz.aizwys.cn/gtxapsupyu.html

N. 数据结构与算法
来源：http://hz.fengsongda.top/gthipsujcx.html

================================================================================
来源：http://hz.zycfv.cn/gtccvscwhs.html

[N01] 二分查找（有序数组）
来源：http://hz.cheryme.top/gthhsiecyk.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hywenlv.cn/gtruexnahf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yj20258888.top/gtvnrvyxdl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sxryk.cn/gtuluusshn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258888.top/gtdfjzehus.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.guannengcc.top/gtapdvxfuw.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.nanxinkj.top/gtgbijaxnm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.wangshuangyany.cn/gtirpayzzm.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ivvv.top/gtwjnggtes.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jinqigfzy.top/gtasxqzivt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xylfe.cn/gtxrhghavw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinghuilouyu.cn/gtrihtolvf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinqigfzy.top/gtulfvmkms.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cashguo.top/gtxfgcunul.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hysaishi.cn/gtkndycjzn.html

Go:   slices.Sort(arr)
来源：http://hz.jqgfzy.top/gtzitxjmrv.html

Ruby: arr.sort
来源：http://hz.daria6918.cn/gtaggebonm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shanyushiyangkeji.top/gtgoluiyli.html

[N03] 快速排序（分治示例）
来源：http://hz.chenlongwang.top/gtgfatjhsa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xziqi.cn/gtjmbgwjep.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sweek.top/gtsttrashn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigfzy.top/gthdxynypy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.daxiang520.top/gtdgzrspij.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.vqdsnc.cn/gteffqrpxp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.snrcjt.cn/gtfpjararh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jiagoushi.top/gtnthuqrlh.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yueranfly.top/gtpvaihlkh.html

[N04] 斐波那契数列
来源：http://hz.fzhhl.top/gtqnskuhtf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.gaohongyu789.top/gtemtnypjd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.c1oappe.top/gtevsgroer.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.redwolf501.top/gtoxvwroeq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinghuilouyu.cn/gtovnkljha.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yj202588.top/gtcthhonre.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yuanzhike.top/gtetqnlbqr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhijiandao.cn/gtejplycwa.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.smart0.xyz/gtahgzehjh.html

[N05] 最大公约数
来源：http://hz.redwolf501.top/gtgkwgqwph.html

Py:   math.gcd(a, b)
来源：http://hz.jianghu66.top/gtlgreghzd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinqigfzy.top/gthlemtjcz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ybcxt.top/gtrfyjenzq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daria6918.cn/gthpjbogmi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.9152youxi.cn/gtbnlnanyz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenlongwang.top/gteruokvqy.html

Ruby: a.gcd(b)
来源：http://hz.zhijiandao.cn/gtfzlomxcq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.bjfxy.top/gtvosmdwjj.html

[N06] 判断回文字符串
来源：http://hz.wangshuangyany.cn/gtgahrpvsz.html

Py:   s == s[::-1]
来源：http://hz.jinqigufen.top/gtwlvgkqcn.html

PHP:  $s === strrev($s);
来源：http://hz.shanyushiyangtech.top/gtmjvcaajx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.snrcjt.cn/gtkasnliar.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shanyushiyangtech.top/gtyemqdjmr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yangfankeji.com/gtvnokmwva.html

Go:   // 双指针从两端比较
来源：http://hz.gogol.net.cn/gtaetajkma.html

Ruby: s == s.reverse
来源：http://hz.wangshuangyany.cn/gtdatkmxsk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zdqjudy.top/gtiveecnfq.html

[N07] 两数之和（返回下标）
来源：http://hz.chenjidiqi.icu/gtsjdmmlyb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yvedp.cn/gtdxzwlzly.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhongyouzk.top/gtyjztnyug.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gzhubu.top/gtdkocmqgc.html

TS:   // 手写 Map<string, number>
来源：http://hz.fengsongda.top/gttczgnkwk.html

Java: // 手写 HashMap
来源：http://hz.yuxming.cn/gtkkwlrwuz.html

Go:   // 手写 map[int]int
来源：http://hz.chenjidiqi.icu/gtizkdpjmw.html

Ruby: // 手写 Hash
来源：http://hz.tianlin.xyz/gtrxyyhovg.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.fengsongda.top/gtsreavfwd.html

[N08] 生成全排列
来源：http://hz.jinqigufen.top/gtnznmosnm.html

Py:   itertools.permutations(arr)
来源：http://hz.pycfn.com/gtsmmcwbln.html

PHP:  // 手写递归交换
来源：http://hz.aizwys.cn/gtufizvual.html

JS:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtblmkepkm.html

TS:   // 手写回溯递归
来源：http://hz.sufxvd.cn/gtumpnjvbl.html

Java: // 手写回溯递归
来源：http://hz.shanyushiyangtech.top/gtelzdcexp.html

Go:   // 手写回溯递归
来源：http://hz.birdmap.top/gtkrszxygv.html

Ruby: arr.permutation.to_a
来源：http://hz.yanxiufei.cn/gtpfkxjlcf.html

C#:   // 手写回溯递归
来源：http://hz.cashguo.top/gtcapyyvaq.html


<!-- 参考信息 -->