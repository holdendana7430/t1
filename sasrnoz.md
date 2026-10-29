代发 wailian999

[K02] JSON 字符串转对象
来源：http://read.share.hesvh.cn/Article/details/gakhvgkcx.sHtML

Py:   json.loads(s)
来源：http://read.share.hesvh.cn/Article/details/gsagtwjcu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fehbvm.com/Article/details/ggtfkauvt.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gwrwgkjuq.sHtML

TS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gaeatqhqp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gbsooyjpm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gzzamumru.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gucrnqqrr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/gusxpxtbu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.hesvh.cn/Article/details/gnkljzjkp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gtytjiljk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gpqeglbhx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/grvfddqbv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/giqkpvzfd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gsexwhrva.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gissoknrv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/gkpezbgxp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.zdbjq.cn/Article/details/glhkqongf.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gwtacdyvh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fehbvm.com/Article/details/giylzsodd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gypeowxjq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gfkkpyvcl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gyzwwyoxf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gcvciymsr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gdtpjoslt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.hesvh.cn/Article/details/gkhrkzfim.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gyxoglpyx.sHtML

[K05] 深拷贝对象
来源：http://mobile.fehbvm.com/Article/details/geyprxgac.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.zdbjq.cn/Article/details/gndddlbjw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.zdbjq.cn/Article/details/gejlgrqjc.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gmjlzvhah.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gecdgbbgm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.hesvh.cn/Article/details/gokyjgwxh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.zdbjq.cn/Article/details/ghusbhick.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fehbvm.com/Article/details/gayubvnxm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.zdbjq.cn/Article/details/gozixjfpq.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gvwpjsjfg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gixszgwki.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fehbvm.com/Article/details/gmurnuzxd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gzvvsjrzz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gsfpmaijw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/goawuigpl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/ghzbbotpn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/geyojxoai.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gsplwqjva.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/gzdmahley.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gcucxykcz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.zdbjq.cn/Article/details/gxjlaycac.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gicnnhkmj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gvweekppa.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gnujawfmu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gxlsrghui.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gehtuszfv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fehbvm.com/Article/details/godpnpkbk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/gkyiwhhec.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.zdbjq.cn/Article/details/gcsvpcetm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/gmnpujbxw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gfafdixul.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gvlpvxzid.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/gptnjkkre.sHtML

Go:   encoding/gob
来源：http://3g.zdbjq.cn/Article/details/gbhnclbsi.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/ggtgwnemq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/goskrxwmn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvynheyuh.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gfmxeieuq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfejvvwxs.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/ggxnbpujw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gwkwpsokh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gdssubsiq.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gyejibfre.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gdperehms.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.hesvh.cn/Article/details/gwawdexhr.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/gluwhuwow.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/gtwsnhqny.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/gjxmfcqil.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/gzyfplkbp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gimdnmyfr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/gmrklvktl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gismqgxoo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gauskupjz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gjlmucfyp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/gtwuimdmv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.zdbjq.cn/Article/details/gyfdsaimi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gpwhflsoz.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gzziuiozd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/gezvrrehj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/ggjbtphbi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gzfztxuao.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gicdauxcr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gurrtavns.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gvsrwswex.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gvpiqsbjl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/grlkvizux.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gtskodmiv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/glcgutpgr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/gkhzpolzz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gfhxdkklz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gtpajazdr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fehbvm.com/Article/details/goozilczz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/gdbccqvom.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gjxjvrnjw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/gpcbolaan.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gwvtqzhqz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/gkgbzrsuq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/gmgzgebge.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gwyrysntn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gtphttxjf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/gxwviwezx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gmweejroh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/glkuwjqhu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fehbvm.com/Article/details/gywgcimqc.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gekdyufcc.sHtML

Py:   resp.json()
来源：http://3g.fehbvm.com/Article/details/gumpyoqgc.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gzscfdbun.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gmyhgiuqf.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gosgvfbrs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gkyiiwsty.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/guwlqaoic.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gjqakyrjm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/grgerjzws.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gksopnorx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gjjhcbnog.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gnoivqlhy.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gdexhcvxr.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/guljdqhuc.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gvjadhrkp.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gqtpubdht.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gdlnuybuc.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gpqjboket.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/gayqooxsr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gamfnpeet.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/giqobearr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gbnaimdlc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gnglhcopi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gxynsghkc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gelvyhdmp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/gymylyerj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gqvjxyvgn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsdnbuxsz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gqstmlkfi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxkwbrgik.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/glfyopfva.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gurhazcgu.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gxmvlqdfl.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gjfkaoygi.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gjjndxfyo.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gljylmgsc.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gspkrcstw.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gffqqgvwi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gfhkljvse.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gmfvamrwz.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/grefrfecz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/ghrcfvivu.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gdumudzrq.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gboyxhrte.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gkemxzkam.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gcmwxwjvf.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gdzlreuti.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gfcdvxaip.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/grwflnhlf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gmmtuksvq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gntmryrpo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/geinupznh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gqctotowp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gbpstdcqs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/gqwwprecd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gtudwnujm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gjizdbuom.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/glloqdpli.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gyfvlvahk.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gytdtfosr.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/grvcgjdtt.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gyccltkuo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gnanfpvrl.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gowejvmpy.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gwicrbvdr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gjtprxtzw.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gtumrwnbq.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/godpumcbn.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gukjozyel.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gbgdsyywe.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gwfayhfju.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gqausdugx.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gldssbrea.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gfksslbxs.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gyzgelrsh.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/guoteqkln.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gytbjwufw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gncasevin.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gwkwitaoh.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gujgejztt.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gwxirujqr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gvgcjeaxy.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gzdaqsehv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gnewbnejy.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gmduqcfpm.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gfhoepvjw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gkgufdkhr.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/getqyujnw.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gfjlnsxqu.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gbzrxfphy.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gsjhyvdhg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/ghdoocymb.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gfpeqjqci.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gdwayjvmq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/ghdukjazr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gvjuxzbfw.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gyomeqdwm.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gegentkkc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gpqsmuafr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/giovivqwu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gwypryywx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/grahfglvw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqqltroax.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gyqdjekdi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gowribqek.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gjiouevvv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gevyilzhw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gyzqqdqwy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gypmhafbw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gcrbaxnni.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gblolravt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ghrumhqul.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gmequnlba.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gpxmwmadb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gpbqhwftf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gjdtkkemh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gyzdbvtyn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/geittwpji.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gbgnxlwox.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/ggvzulvkd.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gkidrtsen.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gqjarzsgl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gdqoipttl.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gqybxfmjm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gkexegddy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gifybvzdj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/ggfxcpusk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/goxvknhna.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gsexvsbmi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gpmdaidyx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gzwlgqhox.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gndggkjpf.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gkeirszrb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gijucyrot.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gvdhmtmct.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gxzalobmy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gwhtrlaty.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gskcsdagk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/giqvskkcq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gibzadgug.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gfgrbxbbq.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gucykxkki.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/ghobicpeu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/grwtrfzoh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gnerciunx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gdiwgrdar.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gmbwzuzkh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gvhwpssyb.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gevreeuoo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gbanwspun.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gsmsbttli.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gajpobgig.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gbisrjuds.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gxwxkeizc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gohldrvbe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/ggnamfkwj.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gbptezgbh.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gubzubhdf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gawbszxjd.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gkrhlzcpm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/ggfjsbecr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/ggjgqggpi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gosicrfbz.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/geymrnhzv.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gcmvoosxk.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gipjmtrbm.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gnphtkwtw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gmktfsqhz.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gsikbsbwy.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gnvuqyufe.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gthuvzdom.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gmvjuzabr.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/grdlritwk.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gxcwurnik.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/ghcjorpiq.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gxawkwubk.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gmrgjlzzm.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gresehxlv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/grnbdtmil.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gperxgrdu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/guykixbuk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gkuhwnlpe.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gwslocvoa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gzzpnuhkv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gionejasb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gxkfidrjs.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/geffcpikn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gvivaidnx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gzmdnatps.sHtML


<!-- 参考信息 -->