代发 wailian999

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3gvpclobf.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3fsvlrnlr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3flebrrql.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3evsyoipk.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ntugwhaw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3dfyharps.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3easxbuaq.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wkcixfyo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3affarfmu.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3khtenhvg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3duqmbwyo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wjlkfexp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eodxdkzb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gfmqddws.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qmlyctwo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3ikzrnyld.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3ttgubajj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3afmcbzqi.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3zmzwfygm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3hktzpqlh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3qxftkqqi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3jcfrdyip.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3wdcirrnd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3kzxepwzt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3khoolbxq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3vdswqxue.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xpgfwhyr.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3zumfdntr.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3yxeqpjpz.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3sakzrtqn.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jnqwtbvj.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3bmbbxzff.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3kehtjoxh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3rfblnxpl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ggvriiyv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3elanvqqc.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3gtypborb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3iybgkzfc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3gnzykrwr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3npwaazlt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3sjjfgauz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3xoxspgfe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3usuezcwo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3vztkoikg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zqcuvrzl.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3wrarlfdf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3immlitie.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3xyudwsfx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bnuuvgxe.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gyxyqyuy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ujljdkex.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3qideewai.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3zwjisujj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tqvchhbe.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3dvvhgmpg.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ovvhwztm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pzwhzria.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3yxipbkmm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3fyudlsms.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3tpownano.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ehxiuusa.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wixltrcb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vqevaspk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kfieldki.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3mwbetsxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ramofpnn.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3cvwpyxob.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3sslsilek.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3wleieoel.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3lcipuuym.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3feqolokm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3xzfguxfp.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3vnbqhjuj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3pkwiifpb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dkbcppgm.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3iodsonqh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3vxdnpfmg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3wrkgsspz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ndyewrij.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3mscituqh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3rwouxabn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3yvvsgrox.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3jykgshms.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wxvycelf.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3eonuxqhb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3teomjoyj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zqhdektx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3zmjtbglu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3szmyxplt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3eamfhdbv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3nfliinzo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3swbtqgws.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3pkrdojok.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3yefdqmoe.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3zaujvvxl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3nvzfbdjj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3kdsmpsrl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3qgwkliky.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3uyspekcc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3emifplpt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3wtyinkvw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3alsbkhhc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3nqfcfysu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3znnnhays.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3dwpgtogf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jtgeamjk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3sjvthbcg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3gvvfqiqs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3pkmkpisz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3xhsnbsso.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lkkcwvcu.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3cmnkfwjb.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xihagyzd.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hunnwpde.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jebmiibj.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yuokfraq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3mmdpdzdm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3siraofsr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3lojyytoi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3uxqohagg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qxrqqqpm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3dsfgbzae.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ailcdatw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3fvabiqux.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3hbicwwjt.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3qlwbtpty.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3uagwjmrp.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3slquqgvk.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3hiyhusyb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3czjzuoba.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3exqdkdqm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3sthbnhyo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3womxhpep.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fcnywxth.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3yykyntgy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3nbsfsrhx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3kzxoxsml.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3stnomhyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bwmtccnb.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3glkjykaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kotituqq.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3wraptzra.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xlnismyr.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3mlufsrsl.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pmmajhif.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ysqnkpbk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3sigkwxej.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3jgrpvodz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3tzfxhauz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jhgxjtvd.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mxxlrwoo.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sfjufoqg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3cklafcif.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3iytwlxej.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3pejtchfb.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gkjenrhq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3znjnqpup.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3lxrbjygm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lqbtpxrh.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3iubcpuyg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3gkjgnwmf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3irdvysvo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xxeffbkw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3gbvkhhzt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3olfwltvt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3wuyvzfoo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ivzfjqqy.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3vpdtkezd.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3renduavf.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3etqtjdgh.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3rvjyspmd.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3kzxnmezz.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3cggjiadm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3mqsazdbx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3exhwmiqi.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3vwisjllv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3foqkvtqn.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3jakqiybb.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mwqluxpb.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3qwpnieir.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kkltcknr.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yritmipv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gmmsbggo.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jrgjtjgq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3lntqouxn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3gyiflixu.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3dsfoekid.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3vraalxid.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3thteeoxb.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hqcydjpc.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3axecermi.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3uptienee.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ckuiqvyg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3itpcamso.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3etjgcxfj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3nwvrunch.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3xqbvydwz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3yqyfxiec.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3eauepdhl.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3sjmfoaki.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3osblkjsd.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3wqrulsjo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3kfxvvlzm.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vjjmwofv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3nulmqcgo.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3hkcqkthp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3thkrjbss.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mxsuroyq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3pbodktzb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3bzypmtwm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3cdjoeyzv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3xgcajcre.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ckuogsgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3quemygao.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3riydflgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3teeymjoz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3clbxvrsx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3akzmtkfo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yzxseghn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ownmbzld.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pbkjvykf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vuqzcxwj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3muevtaug.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3mxiatgvx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ockokbjk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3yteheulg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3fybmpqkc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3pkfncuod.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3eyojidsu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3axacrhlj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3tlkeuzvh.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dpqwawgw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3thmecebh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pchrffvn.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3yoqiymbm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3guwdtmyl.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3gqnvnfrj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dhoqnyul.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3slywysuo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3eyguvvnm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3lueeprhb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3dtfzftdi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3crnsvtzy.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3eepyhbdm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3lztbaxkk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3dbihbjoe.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ybgdigdk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fjphbzvx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3zgpvjrvc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3khzyoyya.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3kylwgceh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hksuipwt.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3xltjavcr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bhvfyqts.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3najyyekx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3itqieogq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhyzkqto.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3tmrqgswd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3xcoytnai.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3uabpnwfn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3cwdeeihb.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3tssegcqv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xlkhlevw.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3feafjxyw.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wjhwuero.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yndurvct.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3kylaqtlq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3zqmhmalj.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3bvbxhgix.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vnyepgln.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3gvbjlems.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3dsbswvys.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3wlchuiwl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3lrkzoqhb.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3rqkareuo.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3apyywqmh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3dnbtzdhc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3rupdipnb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3eqqbsore.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3hbbtndae.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zzhtbyvz.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3mndqfath.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uzdiabcx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3aidnsccs.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dwwgfvee.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kkwyrbzq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3epscfhio.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rasgcayq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3lptnbipe.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3sagjglwj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3skxwbcjl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zdijqlqc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3mswiekpu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3podqokeu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3pamlarun.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ntyaqeam.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3qyfvztqr.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3bvacubop.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3bagmxhac.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqmprmkl.html


<!-- 参考信息 -->