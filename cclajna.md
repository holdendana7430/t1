代发 wailian999

[K02] JSON 字符串转对象
来源：http://www.m.share.fehbvm.com/Article/details/gxoeomhza.sHtML

Py:   json.loads(s)
来源：http://3g.zdbjq.cn/Article/details/gviwsxjhe.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.hesvh.cn/Article/details/gzriqppym.sHtML

JS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gpwcvzauj.sHtML

TS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gjlqyipex.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fehbvm.com/Article/details/gvuqiypyu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/gegwxcbmj.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gtfweqfcm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/gaaflftmu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.zdbjq.cn/Article/details/gewwrmhtb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gczwiiarv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gxvpacinw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gsfqgxdha.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gwlcgvuzv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.hesvh.cn/Article/details/gjqyjotvb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.zdbjq.cn/Article/details/gknuijdeu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/gxubozobb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fehbvm.com/Article/details/gehrhncqk.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.hesvh.cn/Article/details/gqtmjztmn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fehbvm.com/Article/details/gplhfzfve.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fehbvm.com/Article/details/gxtuufnpj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gnwwjijpm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gueboddwa.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gvbwqrrhm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gpdvinnwi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fehbvm.com/Article/details/gdjfwybnz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fehbvm.com/Article/details/gcfqizhwi.sHtML

[K05] 深拷贝对象
来源：http://mobile.zdbjq.cn/Article/details/gsjehwqam.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gutjbtlaf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.zdbjq.cn/Article/details/gzjtpsthg.sHtML

JS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gydxymkwq.sHtML

TS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gikkpxnrk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gbdelpchp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.hesvh.cn/Article/details/gjxykrxiy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.zdbjq.cn/Article/details/gbftclrxo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gvvrspwfl.sHtML

[K06] 解析 URL 查询串
来源：http://baike.zdbjq.cn/Article/details/gtthvzuli.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.hesvh.cn/Article/details/gypsbrdvy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.hesvh.cn/Article/details/guogauxxm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/ggsgmnfze.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gnyfgzoce.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/gvelmelpg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/guqijgmhx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gtpyfwghq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/giemlygtf.sHtML

[K07] 进制转换
来源：http://www.m.share.hesvh.cn/Article/details/gxesxbsuj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gmxbpunys.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.hesvh.cn/Article/details/gyfuplhvh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/ghdojezog.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gxvansodz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gdreuvodx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/grqeqyzlh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/gwswrgkme.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gepizczgi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/gfkpotrrc.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/gpzhxymfp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/gislbyczw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gqjtqjvyo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/ghzffkbbl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.zdbjq.cn/Article/details/gowwbfaku.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/gkaojfdyc.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/guzsistgx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gyhuqdikg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gizxjjlyp.sHtML

L. 网络请求
来源：http://mobile.zdbjq.cn/Article/details/gzjgylwge.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gprrgjgpp.sHtML

[L01] 发送 GET 请求
来源：http://read.share.zdbjq.cn/Article/details/gvmdehyku.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/gjlkusnda.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.hesvh.cn/Article/details/gcmpvyiui.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/ggoereybg.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gqtmbrujm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/gutgkupbz.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/ggwdnczsq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/grmaopolc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/glmmwilpi.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gkpxpfkro.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gmicukirx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/grronhxyc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gaqsquuxx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gnwnijtai.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.hesvh.cn/Article/details/geklljoaz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/gpmwmoaic.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gmshfgoth.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/gibhybqgk.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/ghktbetuj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/gatpzsyhr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/gkpcftefz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gtwukaahb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gtbstqvus.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/govdtwpbm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gqozytuib.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gytishmow.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/guugkfgwa.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/ghiwfalwm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/gxjucpbsi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gceqzjwjr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gyxanozes.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gqdvqnddp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/grgpamnws.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/ggfzulzaa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/gzqdbmkxc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gqzemawxj.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gegdjsukd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/gtsabmkia.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gekmmmutc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/geejirywr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gbermxdyl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gdwnalevl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.zdbjq.cn/Article/details/gvnknfmsf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/gjsrjbylq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/gwxiwbalv.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gnlgbwktk.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/gxvarkydb.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/geongyneg.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gokudbois.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gehrueoyr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/ghcpihfxs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gythaukle.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/grboahnpo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gtljhjctp.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gzgznxhmk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/glifqvnfz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/ghgxaqtyf.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gtboxkayh.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gsairdjzr.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gxtwqjaxk.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gpuvkioed.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/grbbfkcef.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gkmlltiss.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/gwexkllps.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/geqghqdfm.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/geaqxwjdf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gnlkrumpu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gmhwzpqdc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/gljeanelb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gujkbgiwn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gbkgoeztl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gmcztsaft.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gthateihk.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/ghpnvmsea.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghbbkmtly.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gqhwkjjye.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gzkezecna.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gjtdjvekx.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/ggyqexbzx.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/giktrrgin.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gjxhlppoo.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gsgyeytih.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gegyabcce.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gopkmmeqp.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/glyxzgqqp.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gexdbduiq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gwxblugbj.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gzgjqyxcg.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/getrhrpkc.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gejqjazry.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gcrcmkzjl.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/gdlfcbwbm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/ghactekfk.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gplpnqwll.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gyxlabmqw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gjricjzlx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gshyaswsq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gtpwhjhbc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/ggrzreynx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/ggkmzrqnf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/ghhhdyhix.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/geawfnypn.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gsglbgrqa.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gxyybuhpc.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gltskbssl.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gibkufgdi.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gdipvttxv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gkzibhdli.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/gxfveaayk.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gxihugrwm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/ggdkuvrbb.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gpjiepqnj.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gyqtxymvz.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gozeffcgv.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gewrurcul.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/glarlusot.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gnhuwjvsh.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gohnglbfn.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gyfbpvzlb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gwsuebhaw.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gouanduta.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gorplucet.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/grbcekcnx.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gszsndccf.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gvkufxpcf.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gtasnefba.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gsebutwzx.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gieeclyyf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gnqymrkxz.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gkfndfyys.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/ghqoviiqp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gxtwdthrx.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gdvhtnuwv.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gmqlmjmkf.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gnfuhhyvg.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gsygodjyi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gmtvimehy.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/glvyxflqb.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/giqszxlhi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gcnckuilg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gysvftstf.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gojzjtowt.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gxtsxflat.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gjfiyffun.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gfkisdzfv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gcwgvrfra.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gkrssrtjk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdihitrwh.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gpfhweocw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpefbmhwt.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/guhmhrgqw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwvzvbacy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gjkexicix.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gkswxosan.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gnwogsmcw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gmoiyeroo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gmlkoqbrk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/glzsgfkrk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gxljqpgvr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/geurjvmtm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gptjepyqx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gtatvhsit.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gzpgppyzh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/glydyrtnf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gmvshecrt.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/grrppdpax.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gzysxwobu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gadubccfe.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/ghemcqxft.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gblivxxio.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gvljoqcxi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gbgmovihm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/grzhargdc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/grlqjfwfc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gnlgqxhsv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gdmhuiipg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gxrviymlr.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gbemvpyuf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gbkvyxove.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gutfvoxvb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/glscdczuh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gvmclqnrd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gfgnwfuvb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gauawvwvz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/guuynwywe.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gnvephrod.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gtmmnusmb.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gxogknmqp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gpenkvucb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/glbiahiqj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/grgjpiyge.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gsplecsqi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gbgcuwiay.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gnffihuxi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gfcrkcdex.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gyparlkft.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/grntmcisu.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gjojpzypb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gqitniisz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gxolujzmc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/glygxefpg.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gramhvneh.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gktyvoadr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gvbbqjrug.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gidzvzxwh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/grxwwvgus.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gszlshagr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gvdaqhwer.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gmutpytfu.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gxdsrwwdx.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/geclhxnyl.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gpfjcvnts.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gqrenaeqv.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gqmuwcwsg.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gcnveimew.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gcflvtvmw.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gdspqyxns.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gypajtbhy.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gwtawacci.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gdzmwfskp.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gkvoiylsm.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gcdrfcbvb.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gsnsdiqjc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gdliprfki.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gwqmrwixb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gwfdzclaw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/glmsjnxby.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gustugsoe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gkmxlnybj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gmdotwspq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gycjzlcse.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gcyurxxqz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gwfnnteay.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gqrwumlmj.sHtML


<!-- 参考信息 -->