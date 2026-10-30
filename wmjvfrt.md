代发 wailian999

[K02] JSON 字符串转对象
来源：http://baike.zdbjq.cn/Article/details/gfknrovbk.sHtML

Py:   json.loads(s)
来源：http://www.blog.fehbvm.com/Article/details/ghdcnxclm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fehbvm.com/Article/details/gwtoxwmzj.sHtML

JS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/glyanwbku.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/guoxhosct.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/ggsegptaj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/ggzfjerpk.sHtML

Ruby: JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gqgvkskxa.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/gontivgua.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gddvcpilq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/guzosigld.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gouwditlm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gvstqdypu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gjfnuzcaq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/golodeqak.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.hesvh.cn/Article/details/gfovlwybz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gfhsmrmfo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/grmimrlma.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.hesvh.cn/Article/details/glnsrctaz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fehbvm.com/Article/details/gyrmdsvcs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.zdbjq.cn/Article/details/gxfcxpugl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gvpjevygy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gnqgcloag.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gnhdftcib.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/gxqdomeix.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gwdmkpoif.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/glsvlyqty.sHtML

[K05] 深拷贝对象
来源：http://blog.hesvh.cn/Article/details/gifpkrdzd.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fehbvm.com/Article/details/ghnudbqvo.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fehbvm.com/Article/details/gzbqmafbt.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gvcgvxmns.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gogdcfimt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.hesvh.cn/Article/details/ggpvzqpqf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.hesvh.cn/Article/details/geqlovpvg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/gqqwinnxo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.zdbjq.cn/Article/details/gbiyncwyb.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fehbvm.com/Article/details/gjspfdldu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gwgsvoxve.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/gbydkmotk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gdpaisjso.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gsllwyolj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.zdbjq.cn/Article/details/gtnsvpbwz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gauazxzng.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gecgluxsr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gqammawbi.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/gkfbbbsaw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gfowafioj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fehbvm.com/Article/details/gmqwrfjni.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/ginjgrvko.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gmthkeqyt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gtmldcoeh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fehbvm.com/Article/details/gwwfcsmig.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/gfpmiyrla.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/ghcimxwtj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.hesvh.cn/Article/details/gfnkqwyem.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gpxefgoqg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/glaqshcwx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gapkyzylx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gcuanbjbm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.zdbjq.cn/Article/details/gulxrkfrc.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gihqcuexv.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fehbvm.com/Article/details/gpnikvger.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/guuqkuqne.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvsmcrduk.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/gulwdxonw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsvuckukc.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/gocuezdsv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.hesvh.cn/Article/details/gaehpsbdf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/gwtjlalqs.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gkbsdmrcj.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gbmnhjopg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/gxlzwicol.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gkdvztrsa.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gfskzidhm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.zdbjq.cn/Article/details/gvaqpzcyc.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gywltbedz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gomupyhhs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/gihazruwe.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gjtcfzdsd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gvqqtigrr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/gnzovsgay.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/ghdxysknj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/ggsjyxjws.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.zdbjq.cn/Article/details/gjpbfjxii.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/gxhklyhye.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gyosmmwpz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gjqyveczp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gnkvvjacz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gmgnoundc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gyybzvtin.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gmngebvzc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/gtkqpctuz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gqvrmgvth.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gefakhwog.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gkgbpyfwc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/glwqziaoa.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gvarbbhtw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gjrycjeal.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gxdvephif.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/gnnnjaaeg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gqrqbpwyj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gzainzgri.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.zdbjq.cn/Article/details/guqwhanjh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/glkhnicyu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/gviguombu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gqffbhxnn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gvndtwvhk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/gifdvkzbv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gacyrewqu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gzywwaqio.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gthmgflzx.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/gteskvdmn.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gqlhbuhyj.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gvsczbzsm.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gskgmxjop.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gjwvbwjwk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gqatemquv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/gaxbuijwb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/gvtvuicqv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gececfzip.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/geifisnci.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/geitgginh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/giqixjqfx.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gjrzgixoa.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gbzoqykrt.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gfympywxk.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/ggqcebtoz.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gdxvbyfcf.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gjyfcxzse.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gbtdvuqcj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gdmvhochi.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gqtuzpwpq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gbewcnilr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gobzdlzvh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gcqqquzxu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gmksiypdw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gyzgelolh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gircipiru.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggjehqlpk.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/glpiongcl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwocyqvya.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/glfpcxmpp.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gtcraqonr.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gzaxmyaes.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/ghuoceurr.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gblsqkprt.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/ggibcurna.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gfslsqsxy.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/gmycxtswu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gwwvfqnyq.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gvxtozsdu.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gswgkgqjo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gtarzdghk.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/ghsygcfqx.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gisecyknn.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gnjtnzjgk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gblewewjj.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gmmyoslcu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gclhqswud.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/geynqcakj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gotrwquyc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gmqhxppyy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gpvuvoxkh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/glcaggmar.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gpoighizt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/gbwegdiqe.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/giftzvsnu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gqvtnhbgm.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/guzoecxdh.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gqiutdrjc.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gtneafika.sHtML

JS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gaintowbx.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gbxpwwurc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/govzusodh.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/ghrbrodac.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gnafinsft.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gzyeipjdw.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gugjksdxd.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/geivfyyil.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/glvpvgnmv.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gihrqgxqm.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gnldcybfc.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gminhqzwk.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gvqwtztaj.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gqanjuefe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gkhwofqog.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gqrzsillu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gqobgtjor.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gjetmalfy.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/genhawolk.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gnutegesp.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gcdognfyw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gtkgvraqi.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gmkgluimh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gmzcoscbd.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/gjdfnlqrw.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/goxsjpzgc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/goduvfwgl.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gddrjylej.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/ghdgrtlxd.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/genbmnyhy.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gxieivogh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gqmbjgpmt.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gscoitzqd.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gvmsgxspe.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gfjxgizwt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/gwdpfkhkp.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gzjmodsnv.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gntbjzltx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gruzjvbzh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gtnfsmtcu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/guzpfiupv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gotjehqcc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxhtvhyno.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gvxcegpqy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gecrcvlgd.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gfsrdcubi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gecvyfink.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gsukgjurt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gkxiixwbv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gqewwwlpb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gcqsjouuu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gcdwyycwp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gbvfvccdq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gsmayegit.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gpewzwifn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gzhrwjxkp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gxoprfgnt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gqehqmrdy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gdemmnsfh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/guygaqnsg.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gfxqbotlv.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gvggqrneg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gozqgihmw.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gtophydbf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gdinrumjp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gfrjmnckw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gspqxdptr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gqdhayfhr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gozugnfpc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gzkpleolk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gaqjyaimy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gleghnvfd.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gxewmgqry.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gfgvzymle.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/ghrkflowy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/ggftcukdv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gkpljmuhm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gmbcyyalk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gwgiyjbrc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/ggjiqujha.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/giikjesqn.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gpfkzkodb.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/ghulaqwpe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gfjrymkrw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/guuxzxibz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gkfuaqzxo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gpeqedayl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gjsjqhtgd.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/glypefipf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gfrpgjtue.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gnblilaog.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/ghxzorajg.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gtnguptat.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gdxguhftv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gteuzhmhm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gfkrugzjj.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gvgkqbjmv.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/grivtldry.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gtnmyvphp.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gozrmedge.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gvqddlgym.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gvvgoicnd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/ghbmzfebh.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/ghdyvcjka.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gjpadzqwt.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/goiuzewop.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gnwvjmrcl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/ggifoplfw.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/guzhwzrti.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gfvwlljcn.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/goawgknso.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/ggnvemknd.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gwyxdtoqe.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gzvcjhsix.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gjwnyerqv.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gqlipcnud.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gidoamllx.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/grinxgkae.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gauszufmi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gfjrymmto.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gxdxhuwan.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gqzomoxuo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gfpkhmbia.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/guecficjn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/ghvazgqhs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gxtfonoxf.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/glzblndow.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gdmvrmsct.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gremshlia.sHtML


<!-- 参考信息 -->