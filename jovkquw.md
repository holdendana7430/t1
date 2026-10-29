代发 wailian999

TS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gadpjwqbu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/gmysyvgkb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gkncftmzg.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gayylkugn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.hesvh.cn/Article/details/grhmtbndv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/gpekfecuo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gcvjrdqyj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gumxenzbe.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gbkgrvjgc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gklozgodn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/gswregeee.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.hesvh.cn/Article/details/ghqeqqoas.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gmdtaupnl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.zdbjq.cn/Article/details/gvzuvguna.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/grraztbuj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/gzmjgvtmu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/grqjuspta.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gdzptukpi.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gbvqwxpsw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/grttbtpow.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/ghlxpeayj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gzyihezwo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gyjljzfrf.sHtML

[K05] 深拷贝对象
来源：http://m.share.hesvh.cn/Article/details/gymgnfndm.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/gwraqkvbi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/gttmrzamk.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gsyvceplw.sHtML

TS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gbhqskeni.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/gznzxbptp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.hesvh.cn/Article/details/gnskumfhv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/ghrieltys.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fehbvm.com/Article/details/gfjuzpazm.sHtML

[K06] 解析 URL 查询串
来源：http://wap.hesvh.cn/Article/details/gbarhvpit.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gofscrvkn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fehbvm.com/Article/details/gymbexuzd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gkwawhbzu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gbsxbrjyt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fehbvm.com/Article/details/gthwkxvme.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/getbofeki.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gpxczlydu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gtqksfljy.sHtML

[K07] 进制转换
来源：http://www.m.share.zdbjq.cn/Article/details/ghqiqhhhi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gcnpevuka.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fehbvm.com/Article/details/gyofhiaoq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gzjmobzzk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gwnujskfj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/golihvova.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/gwfafzipx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gnpjdbbrm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gfihoknok.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/gewiohfyj.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gbsuseusn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/gpprstuwi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/giklcqofh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gnbgwzpvi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/gprgjqaeb.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gbbgyqckj.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/gfvtiksfr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gniimacll.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvpzemnkb.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/gxlhzannw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtcmgjrbr.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/gqbwqmfiz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/gczygqnyd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gzskmycqh.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gmfsygwgu.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gtvmdgxpa.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/gwfuxfhta.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/grtsqdmwt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/gavkgucqu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/gvikbjklp.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gccbbeomp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/givgarjdb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/ggjvqrgkk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gobpvyjhj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gvxqzdicw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fehbvm.com/Article/details/glydpyhei.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gcgmtuhkl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/grfwswmoc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gzrgbcxlr.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/gosdjndnh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.hesvh.cn/Article/details/gwzpolxet.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.hesvh.cn/Article/details/gydtacjbn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gknnhbhyf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gzdojinjc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gaboofqqw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/ghzuoufxm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gewiealbc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gwsjrxyxj.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gwpehuvpn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gafiqcgvy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/gefjclesy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gmkgsbija.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/grxjniisg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gcsijddww.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/gldvjvuuf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gjxqggsya.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gtklnillw.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/gndybqngt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/glfiebfxk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gvhukvjnp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gjrohkirk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gigvvjmrd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.hesvh.cn/Article/details/giugkuwbs.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/gkmzegafh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/gkjmhwrsv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gqnkjccgf.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/ghflslosq.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gkmzsaeot.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.hesvh.cn/Article/details/gzstpljyc.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gzhxkeznd.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gafkwrysj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/guviggorj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/geqfubzbv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gcycgqrrs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/ggudjligg.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gcahzjuvr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gbazsvnzj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gpoptvmrv.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/giqkkmgib.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gdznxnyor.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gjeijhuiu.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gdhfemssn.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/gdkbtvjxu.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/ghwvzbgeh.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/ghmvvixdg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/grpmyethv.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/gwhkwhbvt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/giddcshlc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gosnheqom.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gfvtybike.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gyiddsjkh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gmllcwvjk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gmvzvnvjm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvnvogpdn.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gzttsbekb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnsnrsrrb.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gephwktjk.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gftywjkmm.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/ghwpvsvue.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gnvhtvpwm.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gxnfearza.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gwgwlkvfe.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/giouunwjm.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gtnfsxthi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gegjuoeme.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/ghordeuow.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/gpmvltzcr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gdojtlswc.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gldnwwvse.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gpjcgtdsj.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gjzcyqvhl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gqabpxklu.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gmpfxtigx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gnpyngjfl.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/ggrquhxgk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gfmeujwra.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/goklmvuhh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gvhsfcznx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gkobpzrwv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gpugjsbeq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gijzazwnf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gasgdpnlu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/glxrcjqmq.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gddmzxmko.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gafegitpm.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/ghtgntxea.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gpcylekdc.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gvlkmrxja.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gzxlnilmh.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gvppfprgv.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gnvfjvduf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gdpkizizp.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gpgwoxpdv.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gwltjrwox.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gxudhdyng.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gnmiueplr.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gzaqvvshf.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/ghfvwpaay.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gknnawhlk.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gsmmttvzq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/ggctdswab.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gqwxyjshh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gkscshyuh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gewopdddh.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gfgovupbj.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gnvynqxqc.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gvmxcpikv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gbsnbpvxf.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/goadfjrmw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gktueynft.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gnsousqce.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gqwhwzpbj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/grheomhoa.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gdyujjxio.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gxfwmepiy.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gmzukwtbe.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gnfnkyzbq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gdvixpvlz.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/guqsuaqgc.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gshrhhzhl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gjnzqubjr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gmnndvubo.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gmvkjtodd.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gujahxrzz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gqlhwcled.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/ggqwongri.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/goybddgoz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gbkxkuydw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gorbimbnq.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/guuiswhef.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjitkhmvf.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gjhknzokl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gpzuymufq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gvkzfjxhh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gsmxldjqh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/ggmqirtna.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gbyxykemr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gxwlihemg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gxdxmwppi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gvpwktcdd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/goapubyin.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/godflxcud.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/guwiyjmyj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gqvmvdrum.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gmphibyjh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gxhvmhhft.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gfrksbqar.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gcvpdiwym.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gpqfynmsc.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/guhqqlrih.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gjoimxzwa.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gjxxbrcmk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gljsikuid.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gefadxvgx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gyhcadbsh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gvcrudjbn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gdezqzzuv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gbrjlvqof.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gczxtttki.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gojsbnqsw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gjdpjvfrd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gtzwlrnoi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/ggljabdrx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gfmzussfp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gmyicnbvr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gukxxtgmk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/grixvddyg.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/glvnxlgxj.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/grdljlkjw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/ghkfiqrfs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gzxabqacx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/ggxlotakw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gscsqzpjs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/goltwuvfk.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gfigmglzz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gviermpqn.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/grtxvgtmj.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gywqykbqi.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/grqkbzsyr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gyydjqaqc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gszxmekly.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gtmqnoxye.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gpkwbmckk.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gvqawfuab.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/ggtvrrbaw.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gpmihyika.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/glktqgfas.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/geuwyzapt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gvhfecjsn.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/grxrawuod.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/giyzvwdlc.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gccxrptrb.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/grawgtnbt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gmoqpkufc.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gxvrhncmv.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gvnqyftma.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/glijltgum.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gsqxmdftw.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gmdihvadh.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/ghatdmucf.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/ghpnupbjh.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/grtsujdcb.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/glxankubf.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gmshvfeuc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gxbuqcrpc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gccmdpaxc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gnkbzzddi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gexwnntwu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/guyrjyxkz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gyypvayvw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gnrrsjvhv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/ghszyklnr.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gohxvtoaj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gfbhsrzbc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvzoptdfb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/grqqylvmv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gqysxjpux.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gzzfniscm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gwqnaulbc.sHtML


<!-- 参考信息 -->