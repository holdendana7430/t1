代发 wailian999

[K02] JSON 字符串转对象
来源：http://mobile.fehbvm.com/Article/details/gfttrgbys.sHtML

Py:   json.loads(s)
来源：http://read.share.zdbjq.cn/Article/details/ghjenazen.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.hesvh.cn/Article/details/gsveresoy.sHtML

JS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gusbbfxzl.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gtxhakzkq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/gajhbrooe.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/glmfrawtx.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gqdnjeqte.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.hesvh.cn/Article/details/gwvzfbomm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.zdbjq.cn/Article/details/gdkmlumeb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/galrbaqti.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/ghdjfbcgc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gutwrguxr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/geyhepqcs.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fehbvm.com/Article/details/gypubemrt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.zdbjq.cn/Article/details/gksqptkiw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.zdbjq.cn/Article/details/grnpzruyq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/gngylxaga.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fehbvm.com/Article/details/gfvqgolcm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.hesvh.cn/Article/details/gwbcevkjc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.hesvh.cn/Article/details/gdocmkxij.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gblzlqota.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gwmjfwkqi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.hesvh.cn/Article/details/guuehysaf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/ghywhwvgq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gtassbwdj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gcrwevahz.sHtML

[K05] 深拷贝对象
来源：http://wap.zdbjq.cn/Article/details/glppqqtrm.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fehbvm.com/Article/details/gmkirtgks.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/gqhbalwxb.sHtML

JS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/godruxblg.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gyuhdmoxm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.hesvh.cn/Article/details/gmbjqnlka.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.hesvh.cn/Article/details/gwhiachcx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gzmaspayo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/gzekgvpsk.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fehbvm.com/Article/details/gtkrcalou.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gplrifwwq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/gkihjezah.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/glkllgdji.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gqfdwaekp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/gnqdivocl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gbrnmyday.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/govjijzdc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/ghkakdwmt.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/gwhogxmdd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gzwhhvfpc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fehbvm.com/Article/details/gniqvsaks.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/ggataulyv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gyvxwohar.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gjazxtsti.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gfhllwkaz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/gyajxxhjz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gmpqtiagk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.zdbjq.cn/Article/details/glwvclkby.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.zdbjq.cn/Article/details/geyjlqfiu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/ggpolmsrb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gylylaxpl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gtsadcqdf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/gkovxtfkd.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/ggdokjpmu.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gppbvcoia.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gebsfvpyy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdxakessk.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gcdcozlqd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxkzyeifn.sHtML

[L01] 发送 GET 请求
来源：http://read.share.hesvh.cn/Article/details/ghfsvurdi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.hesvh.cn/Article/details/gcggbthkr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.zdbjq.cn/Article/details/gfqffmhlq.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gvjzxfofv.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gwrakglve.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gcjuuesgv.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.zdbjq.cn/Article/details/gqjipwgyb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/gydjhwjyf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gevwyvhix.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gbgfqybrf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gwgzlnsak.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gbzloevin.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gxxfvxkly.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gjhymykfw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gwewcoucc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gezmmlmzc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/gdciyjqho.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/gqrrzdouw.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/glgsuohfk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/gfcugktgs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/gdregnklx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gzegikhyk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/guqwpdedj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gnlkawqur.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gpfwuxpoo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/gsszbkkbk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gcmpikicy.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gvnuyiawt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gefaifqbk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gwgpkhxdn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/ggritidzt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/goareedta.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gawnoustz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/gxppyibhm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/gqzdltvqm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/gzafdggkb.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/grygsxmam.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gjgvtkozg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/grnhegtmm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/guyziysby.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gptnjvgtm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gatuklcvr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gwsodnlgh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/gfiowdoub.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/glxiarsbq.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gsxiskvep.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gvwetpfxq.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gcvzazeek.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gosdzszuq.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gbakfrtjz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gfoslaqyd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/genavhnar.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gtokovkvz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/ggowcfdhf.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/ghljcirne.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gsykcvmsr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/grjfmnytn.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/goqzepifq.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/geqlkiutu.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gjqoxpjmy.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gcntcyrqp.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gxtznnzxg.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gznyqobel.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gzlkctslm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gvxntpwth.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gqerrofih.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/ggcflpgwn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gilxoppzn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gnligppzh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/gxfgmxuzz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gswdghfnh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gwxkqaueo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsyeurjhy.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gdhlzgvlw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsafbtcsy.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gfdjzvqtr.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gcqkeuepm.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gcxjjzknf.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gbefesnby.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gwepmypiv.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gzqvtpfed.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gcbwpaqsv.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/gtjaitcwn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gbsydlzam.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gnxbrtwpr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gxqczpioi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gcrudozxe.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gkkphskbl.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gxgiejvae.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gvwauoaza.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gocbuhhvn.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gsmgcryej.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/geligizzp.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gcmzkxlrh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gisbnwgln.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gninpdtez.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gvqzodjfi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gmbyzoobv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gyjjpgmnx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/glfmdshmc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/gtxpihnqf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gxxdwqaia.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gztdzeflw.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gjkngmqmd.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gcytatqsu.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gnlgfqncb.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gkmimsbdj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gntlgtnqj.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gbyhrovjn.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gnjxebmep.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gfjgxrlda.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gnzknapbv.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gstgzkjto.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gpgtwhmbu.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gkkkyhqls.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gslhwjysj.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gtydffuhn.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gsdwmpdwg.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gbxgkqkdu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gtqvmvdiv.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/ghvkcepof.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gqvqrmmcf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gclvzetus.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/guidzxptd.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gbhhtjwdd.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gwxiyfdgj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gxrqaozmz.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gautizlwu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gjhykotqo.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/guugyedcw.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gwcwpfmoi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gyqladsos.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gjhzxoqli.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gngdsukjf.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gxbsevigr.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gtqzomshk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/glkeusmdi.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gkehzyoef.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gdwqcnckc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/giexyrtxf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gjhtfvtzg.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gwzlsktys.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gduogvmoe.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gcrwfnhpf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/guqacbqbr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gslxdfovl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gjrtflrpb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtjhjlaca.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/guixyewje.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdseikfyc.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/giyirprgr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gcztwlijm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gutctqtua.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/ggkrpcxlh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gugxwrgzr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gtdnosool.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gqmuxqvrm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/ghfalrwjc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gsluaannw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gxzetmtvj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gaenofjyf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/glvfsrsbw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gmuvgvigg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gkqskkgbn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/ggtvyprtq.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/ghzdfxwdy.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gedggsgrr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/guxrmimtb.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/geaenbvoo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gkrdazbfz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gwzbjevdy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gjfvwmrxe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gcddalvhy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gcvqwfsxq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gkxsmhwvu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/guugyyaiy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gbiyhodhe.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gkcprqymy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gysmnbgjj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gbfxlofgk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/grekihdpe.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gqdfcaklg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/ggwxkzsrc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gplukxbqq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gkbrieysu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gtplvgqno.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gpxhhmfkz.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gxglgwqrg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gprtnpfqb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gkugintdz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gczhuivvs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gycagxmqk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/grxfmnlut.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gkdvisdvl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gclumorjr.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gxfnspwer.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gusswvlbf.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gslafpgrr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gwwfxjnzn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gvnsqxrue.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gtoabyzrx.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gpjbncnhz.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/girfigsur.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gsabjqbgh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/guuakvhkt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gkewxsfmh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/glprqlcik.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gtqkbxqbo.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gbymjpdik.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gcmyqlgjc.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/ghlpkggsa.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gddcudkje.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/ghwkvdzik.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gjiqgzzos.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/grfwaxozf.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gfgdwxihh.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/griydlyht.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gpfiueitf.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gpcxbsavb.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/guvmvxbal.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gudynqzqu.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gjgqgxyyw.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gydrdvwdl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gccwauluq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gfomsrwrb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gisiayoao.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gtfhgktnf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gpivplfny.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gfervqiwp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gjaifxdqb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gbbsvtnra.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/ggdyyvmja.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gyijhcxct.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gzbwbruds.sHtML


<!-- 参考信息 -->