代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gvfihzdsv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gcnvlmegg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fehbvm.com/Article/details/gjmovbzes.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.hesvh.cn/Article/details/gqknbuzna.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.hesvh.cn/Article/details/gjiduwjkv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fehbvm.com/Article/details/gkjsbcqwu.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/ggnpdgdwh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gapfrctlq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/gkncziyff.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gaapefrof.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gxjboajze.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gmjahjysz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gzlxhszrw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/glfhawjdg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.hesvh.cn/Article/details/goesiferd.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gcsgzomxg.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fehbvm.com/Article/details/gysbnopkd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fehbvm.com/Article/details/ghfamakyn.sHtML

JS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/ghqefhkam.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gamajpcgd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/ggtybayku.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gfgztbxcb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.hesvh.cn/Article/details/gyyzhvvmy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/gvcxwkxpu.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.zdbjq.cn/Article/details/grplwfzes.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gdnmdfrja.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gbozcbxxy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gxoriqllk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gvyoicghj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fehbvm.com/Article/details/gzbtjzvae.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gobefesih.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gbihigtru.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gxbbgnhcx.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/gjqjouano.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/ghujzarss.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/gxrpagakr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/grejbsrpm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gpmctlccv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gtmrvdndv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gdenwvvzm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gftzgvosj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gtjzfjrkf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/ghzxpasmq.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gkamgywor.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gfgeffbns.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gqgemehxw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gfaqvaliw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/gfixwqffp.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/gkxaslrso.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gaczgfjpq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gekpnovfg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbfjscxqh.sHtML

L. 网络请求
来源：http://3g.zdbjq.cn/Article/details/gazutohsp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsgcxhaer.sHtML

[L01] 发送 GET 请求
来源：http://baike.zdbjq.cn/Article/details/gqkieeldq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/gmcoqcvpi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fehbvm.com/Article/details/gvztsjmzz.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/giwpparkb.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gladugmqb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gfwtfrein.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/gmnwveuss.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fehbvm.com/Article/details/giojbxqsa.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gjqweuvei.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gkizqszak.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/gjezpzgen.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/gluwtntnj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gpxvopszn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gvjajunon.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/gpnnnhoby.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gkkfdtond.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/gkpsdlcxy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/ghscxqpcm.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/gslzhnckq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.hesvh.cn/Article/details/gvlpwvlri.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/giuiigith.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/ggblrvhao.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gdphpoemy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gwjypdacx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gebiuwnfr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gijxvymde.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gloszorxm.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/gqxlecmcq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gfkshrjji.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gwanudttu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gmlhzohys.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gtvchgirq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gcmmridug.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/gtxsfhaww.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gngynhuwe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/giuglmiyy.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/ghmseldwo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gaspmjjek.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gmduyhnyn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gyqggioxe.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/ghceygqsh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gzacguukb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gwuxnbqyt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gkrcfnrkb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/grmaachzv.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/ggwwljqbg.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/guzaeqhrn.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gycoeoagq.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gpwqrwqty.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gzmwijloe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gjnabjmmz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gwoqxlhfe.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gtcaoaymh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gydgwlcsp.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gnvsgcxtd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gkvowgvkz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gqbrbyqwm.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gvakpkpbz.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/guvdribtb.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gmyaxgnne.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gvfdyeeuj.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/ggnyrgllc.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gzcedyilg.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gqhxmslll.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gjpxkwwbi.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gtvpbvkbu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gxhjxxwqx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gsbhruleo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gwvbdbxcu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/gxlvhtfvj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gypgvcuaa.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/ghtzlxtyb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsatdrdlv.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gqardvpdw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grmcrpzgq.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/guhhaykmr.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gcnfgfhsb.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gsuxwwoyv.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/guuedqmqv.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gabinmovs.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gqtpkdbyq.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gfgeqqwet.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gmtmmlvri.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gmvyxfokv.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gztfqvfyq.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gsoehjhjf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gaqxqzabb.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gfyktlyaw.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gtytrzznu.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gyypsubuc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gxztzshau.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gvdddbhwl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/glbnpwtbj.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gddtdhzhj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gqkholsuu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gspcdrbrt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/grbyxbbdj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gclcniavf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gbbkuchmk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gxwaoepgk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/gfdcswzkb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gxdajswmg.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gcklmjinj.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gjtlakitc.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/geqrcjtcj.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gfzfxrlkz.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gufbxphrf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/guzyixdpf.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gwsnipgyy.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gyfoqnjvm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gxbbiphym.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gvmvoghxu.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gqagzvmed.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gmlnwgwgm.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gzdmgoddw.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gidgmfxtn.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gjqpfbnjl.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/ghldacjxv.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gfxuqeqmz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gphfbvlrz.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gkioysler.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gfrpznwid.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gwavhmstj.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/giuckoree.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gtpdtzljn.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/ggnmcxwlv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gsuslyhzv.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gutcsqopm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gtlfczepo.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gftowltus.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gmynlfubn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gmssvywja.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gvifbozqg.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/ggdcqysab.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gievqjine.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/grrkefsne.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gnaaplsqz.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gsbkvgprg.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gsqxbrlbh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gtsobqcij.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gullywqew.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gwvoqrtop.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gneenqqrq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gfxxgdcer.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gclmeklno.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/griewvalu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gxeldgkla.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxandjugv.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gshlofpop.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpswifdtz.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gcscnakji.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gjienbwjm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/ggdoxrpyu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/geaxvqaue.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/giagjzuon.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gedrdpybb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gbmzxvktf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gozpdysoz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gvclwsmxv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gxlxdkcql.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gmzuuujkn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gmtkmcfxd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gaoegjkhq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gsnyxzupd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gpbifwymr.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gpaumlfdw.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gcucckeul.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gutbbklnp.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gvqxxvayk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gldsowfyp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/giwtkassb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gijljdfuk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/ggqtunurv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gtcrutruu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gnbkkkjig.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/goeiivika.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gggwyhlkn.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gniaqtilh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gjtdyrjfr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/glgcosxcv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gtumrbfpo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gmmahywsq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/grhjutjcf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gftmtwxez.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gqtnbbqlt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gbzlwbhoa.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gtprjxyhe.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gejpfppwy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gxwxmkfcr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gnhezzrmd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gljjmbmua.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gvffjypsq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gaqhqsiiv.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/ggxxhgdtb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gmuchpkly.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/guusnonot.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gmygcplvj.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gismnvtwp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gaknlcukk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gqgwnepbe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/ghxoknrvq.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gmattbuyg.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gvvxaeowr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/guwkhdckv.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gzqztcnnl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gdlhmxkbu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gydxryuia.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gvestwoir.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/growrisle.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gylubhego.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/guppnwgkc.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gjavdtgah.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gnxlcwvaz.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gjofcwmkg.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/glvachmci.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gcbfgfvot.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gpzgodlcs.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gqemntaxl.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/guoijtmpo.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gifilvbtu.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gvtuvrmdt.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gkjfgehfm.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gbicpmajb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gdqjvgoyo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gwrndzcwd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gznypywjt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gluryepoq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gyekdqnxc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gpqzxxcbs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gmzocrldp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gzwnhksny.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gbqgbhsck.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gsqrwmmof.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gofsnbzav.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gvggnfqdr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gnhbetzri.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/guoqrzyna.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gknrgrvuu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gdcshfvff.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gxiashmkw.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/ggqjhyshh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gqjjtnofd.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gamkoxwdg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gmlvjbsju.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/grefdfbdt.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gbxbnngfg.sHtML


<!-- 参考信息 -->