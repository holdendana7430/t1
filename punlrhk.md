代发 wailian999

[K02] JSON 字符串转对象
来源：http://baike.zdbjq.cn/Article/details/gzoxzorgy.sHtML

Py:   json.loads(s)
来源：http://read.share.fehbvm.com/Article/details/gwmjartvm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fehbvm.com/Article/details/gnshigrol.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcluaadxw.sHtML

TS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/ggxbaxybf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fehbvm.com/Article/details/grhuwgxgh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gnnacwinn.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gyxqqnzyb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/ghszijvmq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.hesvh.cn/Article/details/goblidfwn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/guilnarew.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gitylixee.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/glvktgsjz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gtxpuoqio.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fehbvm.com/Article/details/gtspqcosj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/gffnwxyhq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gbuvlagqb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fehbvm.com/Article/details/gdtrxgkng.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.hesvh.cn/Article/details/gsgbjgdsn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gkqvjsoxz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.hesvh.cn/Article/details/gqrgusclb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gmtjrcqtf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gnhtvsyuz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.hesvh.cn/Article/details/gpvhpajml.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gndslblnk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gbndkaksy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/ggcrngetj.sHtML

[K05] 深拷贝对象
来源：http://mobile.fehbvm.com/Article/details/givbktqzs.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fehbvm.com/Article/details/gdvnqnifw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fehbvm.com/Article/details/goocxmpny.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gxvhcsgwf.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gkuyydegb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.hesvh.cn/Article/details/guoqzpsft.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.zdbjq.cn/Article/details/gizfehdnm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fehbvm.com/Article/details/gonwkjxxd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/gcjcjcpow.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.zdbjq.cn/Article/details/galhhemhz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fehbvm.com/Article/details/gcucnyivh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.zdbjq.cn/Article/details/gndnogutp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gselrwjlg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gijfawnaj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.zdbjq.cn/Article/details/geafmnwyf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gvdqknjmt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gohqbufwo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gpuydnwvb.sHtML

[K07] 进制转换
来源：http://m.share.fehbvm.com/Article/details/gepvsoobx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gzntnshmn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fehbvm.com/Article/details/gsiclircd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gzahyitvm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gxmkobigt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gfodoeutq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fehbvm.com/Article/details/gjiicgiqt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.hesvh.cn/Article/details/gtupmhqbd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gvlkbpbys.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gyipzijfl.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.hesvh.cn/Article/details/gsiwxabsw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fehbvm.com/Article/details/gorqzgjas.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/ggefilcrn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/ggnfrozav.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/gqfjoxcgx.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/gycsibwzw.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gfsvfmsad.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gxbgafocp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxvhusham.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gvmigsctm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gagvbfkhh.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gjirysjma.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/gwxhrdgjk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gygqdpyra.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/ghfivmufl.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gazzdzkqj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/gpkfwwspu.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.zdbjq.cn/Article/details/gbojclexe.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/ggkskxylm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/gtllvqkkm.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gxftuufck.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gayuclcon.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/gwyjqgjgz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gycjnvazq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gjrfmhtfg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/gmhfgmafh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/ggfbjdpyx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.zdbjq.cn/Article/details/gioqocxso.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/gruabfhga.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/glpzlwinf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/gyyxbniqo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gfxqqillk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gmwjygilg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gxhmfgzse.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gbmywuias.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/ggwwymnvc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/gaekjaexr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/ggcsishgh.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gvufkcfuz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gxzynujnv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gipvfcgau.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gqajcuaca.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gwqigumor.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/grbhtylap.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/ghiyyizkw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gvpcrocmn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gdpqncaqn.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gmfmqpnvn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gyihsnout.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gtuzbgbgc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gjehfghum.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gzfwrzeek.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/girkwqhzm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gavjqlvwe.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gyjiilxqo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/glcvkamyf.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gtkextrxo.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/grpldtsxq.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gifcrfboz.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gqjrumpjy.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/ghggscmre.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gupslsads.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.hesvh.cn/Article/details/gmdfoagfz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gybuvaysg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/gzgheilwj.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gurusnzok.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/gcrrsmugu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/glbgpwaqu.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gpepchpfn.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gkzvqqqxc.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gzwiyecdx.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gonvpdzyv.sHtML

Ruby: resp.code.to_i
来源：http://wap.fehbvm.com/Article/details/gctifxaly.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gwwkqrptr.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/gzcbrjbqx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gtfiiblch.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/goxiiuqzo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gdcmhwgex.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gbmdfcjpc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/gbwkioyyi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/gjdymndmq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/ggrkzltqh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gprdbhxkc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gaxkdpwpf.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gazztoupj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggkewujbi.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gtbpovvtm.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gwyjgamer.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/germqklmi.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/ghekjijev.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gmafwmugf.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gdmolvuuq.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gveecunmv.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gxkjfgxed.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gxjuuivsq.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/guvivwern.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/ggxtrwfng.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gwqeiqpna.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gpzmioqlj.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gmkkxdljs.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gwajihxzt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gkyyokjxe.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gxqdltmtd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gtidcurkc.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gurrahpxt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gknpcduoi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/ggadcxxzf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gyhfuajre.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/geyzhxqjl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gdpfjrozf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gzkxkouzq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/giepiqcmy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gvtnxrzii.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gosmmdchh.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/glqijqbzb.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gypphlrjv.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gshynxsdc.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gtixvorqk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gtskjqotj.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/grbuzyvhy.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gtceloxnu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gxcabcsvy.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gsjkgtijt.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gmmfniiau.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/guzwizqsz.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gikpfzrpb.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsevqstbd.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gmaetfyhu.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gwwcewysc.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/ghlkikuit.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gspzaidwd.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/ghrkshsfs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gdhjcpfmy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gancubxjb.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/ghmhsspjy.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gmohwoock.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gysevotzt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gtlmyietk.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gqjoioofq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gpuyjdqoq.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/grakbmlkp.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gcsmknyfd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/ginpgbcje.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/glsdsgkqj.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/getxgcius.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gqrlwjlny.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/grdvuhnmd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gqxetnste.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gqaqwkqms.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gytltgrry.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/grujyfkuc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gafjswbeh.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gzpwwutkp.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/glzhehrqc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gotzyblry.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gapfdjeag.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gpxusvwrv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gybkohkex.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/goateiovx.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gmwyxqbcy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkpuyrxfn.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gevkzurli.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gbemxeptv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/geycthigc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/ggbxxmboj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/goszjizqs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gwyowtoaf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/ggiprofhu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gxtdhyzbj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gumswkujq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gpohumxpa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gocbvnbxc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/grifnerdd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gnhvrooic.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gjrrwljlx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/ggbffboaj.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gmgqflqxj.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gahlktfai.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gujzliqnj.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gpbporqdl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gxdcjhzet.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/glhacbkdl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/grcpwxgyh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gczntfqvp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/ghycgqrtn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gqoykwdnb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gkgeubfmt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gyiazclld.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gryomltqx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gwtwujfhe.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gerbroymi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gmpetsczm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gelhtzhzl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/ggfslqvkn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gnwnkldeo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gzhxbetzi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gcmausevu.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/guglpxbgb.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gdswyofzt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gcofnknye.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gzjseklhw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gdzsioutk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/getclgaai.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gcqmckmjp.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gsxootgkq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyaxfjoyi.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gomecnpyb.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gwmkrrwbv.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gxzlgcxsa.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gmnjfgxzn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gtgisslaj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gxspmdejj.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/ggonrpfkd.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gcvooigpq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gvqlnrnyr.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gzjsnruaf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gnrksmiwg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/gircwzofx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gdzhbqnew.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gkzdriezh.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gaylbtioa.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gfitciifa.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gddeqknrz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gtwbfwwxv.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gjwlqbhll.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gmmriivhe.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gmlxhmzrv.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gtnknbteg.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gkuaspqoy.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gctfuvemd.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gowkflkrq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gapqrsvcm.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gzbwkghuf.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gwjdopgee.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gojcdfvzm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gjvnwodyd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/giowvqrlw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/goeoynyhg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gjkwlzpzo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gomwakugu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gehhqvxnm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gpqlcseii.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/ggjllyuyb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gzpfaavxr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gleqyidrs.sHtML


<!-- 参考信息 -->