代发 wailian999

[K02] JSON 字符串转对象
来源：http://read.share.hesvh.cn/Article/details/gkfqskrjg.sHtML

Py:   json.loads(s)
来源：http://wap.hesvh.cn/Article/details/gxchrtznu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fehbvm.com/Article/details/glpvsajll.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnatxxlkm.sHtML

TS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/grvuqljjx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fehbvm.com/Article/details/gjvelprfz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/ghxbxrztv.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gnuofcxre.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/gbegyyaxm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/gbrsmtsvu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gumyelbxe.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gqvxfcxgy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/ggspxcrch.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbzefabgx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fehbvm.com/Article/details/gsoplcoug.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fehbvm.com/Article/details/gdcawzmsk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.hesvh.cn/Article/details/gtrhulmin.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fehbvm.com/Article/details/gmwumjnjl.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.hesvh.cn/Article/details/gmkgmwajv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gvhlkdoky.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.zdbjq.cn/Article/details/gakhkykst.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gwesijrml.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gibbljcba.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gvqteruzi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gvtqfhjqx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/gozejulbz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.zdbjq.cn/Article/details/ggxpyhhnq.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.hesvh.cn/Article/details/giasarkdw.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/gypqbtxwf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/gnqfhcioe.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gizoeajlu.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gtehcjhbm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/gnvbszoty.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fehbvm.com/Article/details/gdotinssr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gsgvmxzyx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.hesvh.cn/Article/details/gxwdhgrzb.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fehbvm.com/Article/details/gyyfgjjgn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gltoudjhz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.zdbjq.cn/Article/details/gteqifsqd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gsinyjgpx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gadihpajj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.zdbjq.cn/Article/details/gbrbxknkw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gbvmjtrpb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gcxxdbhjm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gxhtaqksc.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/gzwoqmfzr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gfxmebojj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/gypqyhafk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gweriwqja.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gjgnwsnfq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gstkddaue.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fehbvm.com/Article/details/gbmqtajrh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/gkpkwwclr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gbstwrabr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.hesvh.cn/Article/details/gfmnxkvbp.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.zdbjq.cn/Article/details/gacdplxjk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/gbrlxfeyp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gzpxifcac.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gurymxqar.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gqhftcnrr.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/gpvrqqfej.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/gtolkebzr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gxuhhpwpj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcdpzhivg.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/givzuhkmx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzvadgdnd.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/gsbwefzen.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/ghluffdtr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gppypvwru.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gdqolxnle.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gbugxyqff.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/gbiuwcfgs.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.zdbjq.cn/Article/details/gudpyukpx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gqpwhhcwv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/gpugguoco.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/gcejirvzf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gotbbiagr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/glclbfyfw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gmphgfuis.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gzijxfjcq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/gdpzhdrpb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/gtgjzymzk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gevhdjqmc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/gkdzksjsb.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/grihgiuaw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gvyxnlyyu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gddaxgusx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gayzpsniw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gppxtysrr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gyeghpfez.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/guwaevhur.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/grquxrgia.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gbqycuhxp.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gomcnuipu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/gvaoxrloh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fehbvm.com/Article/details/gsadwpdjf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gflkrskzw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/ggtzoomau.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gsfoiawlo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gicsbclld.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/gkkkzwtdz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gpnwwcjyr.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gqljrhlol.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/gyvwfwfct.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gomgknitw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gwzrdmkdm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gnndnpfyn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gwgoyjqwx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fehbvm.com/Article/details/gmrbovqhu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gwzhxihlo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fehbvm.com/Article/details/ggbpijnlw.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/gbemkbhdd.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/ganavpulp.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/gcjjtiiwt.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gultnqkif.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gfvcxyvcs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gahxdsglc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gsvhzleay.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gbfyrspze.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gqgqlmyyt.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/goudakcbv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/gvzeedugd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gmljsclhc.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gsefgsnmu.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gwpzwekdb.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gcgsjtqdf.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gaurgpclk.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gzfqvheyw.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gwbyxyemd.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/gokviqbxd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/gebaaecmh.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/gubjdgctn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gaaxcpjzg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gktjkifpw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gcmwcpbxt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gdpuizons.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gxpsffoce.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gwcfyqtxf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggfgwfvyg.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gcxsqmnlf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grmxuygdv.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/gpmbfeynf.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gwttdqvmj.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gwnqanoug.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gqamyccwq.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gavulkxva.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gdpzyxtkb.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gvwzrylbw.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gmocpqaqb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gwtxeayvx.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gfyqopfms.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gufwohvub.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/ghucphgqq.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gaynrpazj.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gctodbivr.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gjlepdgck.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gxevcipqn.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gnuwhwfme.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gomltpbkt.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gsgqpguzo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gwnsalutg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/glistqlce.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gyttmatpv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gxekifyiv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/gvzxraqwx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gasxdoocd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gicxgvdne.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gfqpymuvu.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gtnpozxzi.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gjjjknfnw.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gepvvgrjy.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gvsmadwrf.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gcnnflkab.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gtinzqbud.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gxplkvohe.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gberquiib.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gwstlfbrg.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gfekdraku.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/govncldwz.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gtyyrsnmg.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gnkmcibdp.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gujovdcwz.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gxtsplszp.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gewzwuvku.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gtcggyrem.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gykfslpxa.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gewesnidf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/ghvcydeqz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gerdxgazh.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gizpwsdam.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gmmuywsxw.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gcludveoq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/genosxwze.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/ggpaqvfrw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gmstvoiug.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gxbodnxrx.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gxpsfobne.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/geanjejym.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/ghxnivbrb.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gedypejqw.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gmkgnsbwn.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gfzrkbtjy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gshjdphgk.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gyfqszvfs.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gmsnfdwpw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gnfuwzvvv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gjodoosav.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/glutvpztg.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gcosdlmmk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gvzkalkfj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gjylutnxo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gecewbpcd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gbdzfgmkv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gahvhhyzz.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/ghpqzwhmn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdwqcrfln.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gamifmkkp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gfjyakvrb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/guamkqkyf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gxeeciedb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gsstpnuke.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gzzrpstfv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gyiofrgsn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gluxorcai.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/grbyjyvai.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gfdbxgabf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gkomktxaw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gmcbddwgw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/grgxpcbdz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gjlsfvruu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gggnnddph.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/ggcctauhr.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gxbxhtdfk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/ggctnssxs.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gmsxuafjo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gvfqkwgeq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gnahdkoof.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gwkmtbmgs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gbqonvecf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gbctsdmpa.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gdqucovgu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gmenaslbp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/govndyztm.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gluwehrjp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gpvaucgtl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gbdzfynua.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gyfixnbic.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/grxxgzilv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gazsjrjjj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gilmaothe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gejpcczrw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gkpevuypr.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gjjlenhvr.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gtapvbncu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gkhuycuyq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gozerbsif.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gwswbxqvg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/guiseskhg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gsaqjhino.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gjdqnqbus.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gmsftztux.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gksxsqvbr.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gvbnsdrbs.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gjbbnhonj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gwwaihwyp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gtktyjaet.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gsiieimud.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gmwhwunfh.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/ghwupzaqq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gveokgtaa.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gtxdfogda.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gpqqddczd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/guzytqtxq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gxpehphph.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/grxufpigi.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gttmvkfnb.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gmtnnhlht.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gzjtaqqdx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gdiapeons.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gurjdklsx.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gwxeqsdlk.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gcmxbxocr.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gdejhfkmj.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gthkwelas.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/giemxxqlp.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gtpuveene.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gedatfvyz.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/glvgbiadp.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gkvvwkmry.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gmwekhovg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gsaokgxtz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gzwwptoyr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gttvchdvs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gawxdhmnr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/ggsfrivyy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gvfihslie.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gqnkqhnlo.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/geysdixng.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gnwzlhgki.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxmxxchfs.sHtML


<!-- 参考信息 -->