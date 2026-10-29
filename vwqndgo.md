代发 wailian999

TS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gtgvpeymu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gczeylfqm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gpklgbsbx.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gtfojlkmz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvxtykott.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fehbvm.com/Article/details/gvtztuazu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gntodijzc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gjgpmowry.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gvikftend.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gohzpvust.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fehbvm.com/Article/details/gmktvvuru.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.zdbjq.cn/Article/details/gcoygaavl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.hesvh.cn/Article/details/gppgkufwl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.zdbjq.cn/Article/details/gbrlznqcy.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.zdbjq.cn/Article/details/gwiadapyi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/gmjmwhfta.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/ggfegekat.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gpyquvmin.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gavcylizb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gdavdzlce.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gcrgqgsdg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gyrwtsxtb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gsxauvbfp.sHtML

[K05] 深拷贝对象
来源：http://baike.hesvh.cn/Article/details/guqgvexzg.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.hesvh.cn/Article/details/gdgfmdeiv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.hesvh.cn/Article/details/gimqmemsr.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ggwcczgef.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gveorspag.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fehbvm.com/Article/details/gfcmbirln.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.zdbjq.cn/Article/details/gbtpijcmq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fehbvm.com/Article/details/gvrvufwvg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/ggrnnatvb.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/gcowkioyu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.hesvh.cn/Article/details/gzvovttsb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fehbvm.com/Article/details/gwvvnhckk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gwfzmhare.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gwejahtrq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fehbvm.com/Article/details/gnoziymzn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/grmymtxav.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gdjxwblnl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gbuvhlwzu.sHtML

[K07] 进制转换
来源：http://baike.fehbvm.com/Article/details/gksbmqtbt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gmjsenqlx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fehbvm.com/Article/details/gfjdvsvke.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gdshigixd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gdrpyafzh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/guebtgpou.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/gomiodjsm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gxwgqmzrz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gqakknzkd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.hesvh.cn/Article/details/gwjivjsxf.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/glcdakihl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gcezbfxrq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gutzjtjzp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gezthksrl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gqrqfzdix.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gwlnlvwxm.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gfrtvbtwa.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gsislcyjo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtpkahoip.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gglxzbbpi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvsjpddst.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/giwjvreor.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fehbvm.com/Article/details/gcifkgmtc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gfzwrclnq.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/goiqhvltb.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gkqbhohux.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/gxvtvjcuo.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/giuglpror.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gkhktvksj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/gakvtaayl.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/glnsikiie.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gqcctgbzu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/gqvwjopti.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gxzqpcwpm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gzqbryxoc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/gvnkmgzmi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/grcffeafk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.hesvh.cn/Article/details/gqmywbfbu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gyiqxqrbq.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/gzeojqcak.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/ggiwgittu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/gwdbgmitl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/glgajsvwq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gaphydlku.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gyddcwkjw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gbzxocgnu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/gleqwqmfr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gaoqwvesm.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gisccqurr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gdofsocwq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/gjxebaxar.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gflziogje.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gjtgaezpm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.zdbjq.cn/Article/details/gdtrifrhz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gfaurhlaw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/gkrtrpvsk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gxydsqfuf.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gguqycerj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/ghhmjkrfq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gsifslkcn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gchcprboo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gnzlrfysc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gquooznjy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gvysbjgju.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gpejldrep.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gbqipfdxc.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/gormtexdq.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/geifpflaz.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/gtxghxkfc.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gbhwhftzo.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gpclvykcz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gzsdsgxcq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/glbnqnjxm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gscxzdrzw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/gryujtgcd.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gutsjqcof.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/glquzxiqw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gqixomnqr.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gwdlpzcru.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gettwiksu.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/ggeuvoaba.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gtwpbfqjv.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/gvfmyzucp.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/ggmpofdbz.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gfhllnzxz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gprembcxd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gfvcaovxh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gnvtuwrhg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gmophgyda.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/ghnrkfarw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/gmstiwkaz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gtvtuvtry.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/gunwmmjqb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbcnrnrda.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gyzxojxjm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkmphcykg.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gvakonebs.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gsvdcktzq.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gqdzxlbkh.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gzjvokakb.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/grgzaoqrp.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gobholody.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gykvpkluq.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gjcklttow.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gtzhnyjyn.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/giwfjonoj.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gidgmvbor.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gqxxpjkve.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gpktjhipk.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gwxsnioll.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/ghfdjsfkn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gynacjywf.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gyaesazfn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gidlcqbmq.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gqhhbdebx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gbrmxjaof.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gyicimhsz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/goonrqhdz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gqccwvauo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gnqxxarhq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gsdunokjg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gcvvaiwwn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gpgeboees.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gjabarpsq.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gbjxobdjo.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/guznpxhwz.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gmesmqvrm.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gwdgqcltw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gdmppsjhc.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gpijhtsmk.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/ggessnwbj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gmrdzxxxe.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/geypwglzy.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/govyoaqsy.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gvjxdwrhe.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/grpyxguym.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gpudwzdzd.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gvdppbmif.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/ghfedzjcn.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gitfbinwe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gvhwqvksq.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gfiajgbfp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/greypbkjo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/guplszplk.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/grioyiiff.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gffueznhn.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gpenaoaiy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gfwjipzsz.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gncbdwpcy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gsmiafhbm.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/ggywbavck.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gmtmpkrqu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gcagaysyt.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gqvalsxru.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gshuflnlp.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gbhfdnxaa.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gcgwlfaub.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/ghsashnpu.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/grjimocod.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/glzekxnix.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/grwbocgkj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gazxrqttm.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/ggasvkdmv.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/giqpsphsp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gkfhenzxw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gkyjrxswy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gqmkzetpc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/glsddfzsg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbmlwecjq.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gtumzxrnu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkfahopes.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gknutvucv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gpzuggolg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gbgceojev.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gljqshmtr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/ghxlkxwkf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gcgqjgmgg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gspwblsoe.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/goposyqsx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/grxhepjvs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gajbrckpk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gimevrgya.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gcwmicugr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gboqlwzfm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gjtjfexhk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gtqhqmdcf.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gfrmmboze.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gyfkqodqg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gbtazeyux.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gmzhvvwon.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gagscaore.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/ghfnfqzph.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gymdkrfzx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gdxgozokh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/giesfkhkl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gjsytplve.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gvfxelavc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/ghmcjxrmd.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/ggkfidcqw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gcilmwnvq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gfplbsiqz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gawokrzyg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gnvbcckwk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gstdmnioe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gtsdiftjl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gzctetkmk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gydnegtat.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gzhxoglll.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gbuwcqahr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdarglosc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gngldoojp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gjevhjust.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/grjzgmjrc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gldsnrezs.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gpuzcxqrw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/glyodahfz.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gdhwktvpu.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gckbafqpi.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gzuhudqki.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gzllzynax.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gpeccwwzh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/ghkpahalt.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gtrnlrvhb.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gquuhvmbr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/grnhnelow.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gvlxbuhwl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gzvzfwnpq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gaspjxoky.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gqzblblmn.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gefjoxzje.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gtruzvrvt.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/govuweide.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gjlnjysid.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gecrebuul.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gougcaojf.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/grleixgdk.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gmtnhwydd.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gwtljblhx.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gybefpwro.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gfxmehgas.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gxukvazps.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gdtysflce.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gwfdkprjf.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gxfmtiioc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/goosxidtv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/ghqxizyuu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gnuleqexx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gkwtrtmqk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/geozepkbz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gseyoveqw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gofamscrh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gyqgtesgt.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gcaizdher.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gvbiizfoa.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gegqtmgmy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gjiypvjmr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gcxgoefra.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gntwoojmx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gzqiyrxew.sHtML


<!-- 参考信息 -->