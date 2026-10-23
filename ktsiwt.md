代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pupmlddj.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3gswdtwse.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ypqbbwio.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ejprxxjh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oiyclqsd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3qtempfxy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nfkvfxjr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3xjbyakrr.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3cjjdyjon.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3ainwhfka.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3aihhmkvk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3nugtlbkn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3irdmdiwh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3lttbpyzb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3kayhuqhb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vbndyrca.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3cxfdjtsu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3chjwqwes.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3jiuxetqj.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3xeyhxaev.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vfbsxphq.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3poklfhbb.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ttbzceny.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3iowfpexx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3jvtttyuo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3kgneejnb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3trdctlao.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3jcmdfgpt.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3qhojunmn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ptdtgkou.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3mhofvsla.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3duucuhsf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3chiorzsb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3defzryqe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3dthlauel.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3hibcxaww.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3nqeytlws.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3kpfmmwfy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3itthyvaf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3jtfghsul.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xjziozrw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tklcmgkj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3oyjvxxwk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3cestfoax.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3omfhisbu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mmraizcw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3nqzdnyxr.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ewlnqbrt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3akadmcea.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ybllroxf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3eeqxffke.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3kuehetun.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3mhuitzcq.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3bmsnzoyf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3xzwnbfrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zyiusppm.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3wemrazqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ozhupbka.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3dpafycdz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3ummzjbmh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3amhieseo.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3uxtyvdkh.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3gjxxegkk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3fwyxvxfr.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3nnhvnxks.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3avjwyxmw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jmjkogvw.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dmprdwkp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3inbgyicl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3fognjafo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3cxnbwfjq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3pnxmvecq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3zklrqcld.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3yqppafuf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3pucgwhht.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3btobiait.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3emaiwlxy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3oqzzukgi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3yvwzchuj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3zycheecn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3zewyzyxl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3mhglhrqa.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ycdwwtyo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3rcnamnjb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3hilsvvir.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3twlpxaza.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ybqxixux.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3akumxdtk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3viicotzj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3lbxolvoh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ggeyamlo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3uwmyuory.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3curhdevt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3xrntmkud.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ezhbisqz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3oqvkxzkv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3xpwpqyon.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3tryvgxso.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3jehijkey.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3diulwbcy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3gbkumxro.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3furganos.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kmuyffdq.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rnzdaqmw.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3atsgwnpi.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zzdndxfz.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xokwxvuz.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ijxywglu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qnizcvlt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3fzxanlrr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3csqtiwqq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3gdbvplxz.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3scyrfcyj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3lggmrjjm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3lzjeyhfa.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3hvhydriw.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3rfefjqqq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3telkwhdi.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3uaujmcvb.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3nosxhlau.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mvqgxfvi.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3mnjgydgf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3jvqzishd.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3bmgguukm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3onrwabyk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rtnmtykv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3gwgrahxi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3uefkygxs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3bvvlpzbz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3lrqhjzkf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kasdzyxc.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3egmyvtmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cshanvjp.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xlqpotdh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3oockdbxu.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3qdsznyrl.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uhzeiyaz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qtsooyul.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vcqtwtjw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bskctojo.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3btgzsuxh.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3amimzouq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3siablvor.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3niodtgbs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3tcncyqlx.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3pzvktyoh.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qwaajqnw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ptyvwwjb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3obykpejy.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3vvnukggs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dlumcyri.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3jxxuewnm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mqensfun.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3whsuwxzi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3krmqypsw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3vnpesuxs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3kfkhmcdt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3frnhqafi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3qswcxynd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3gwtllrsz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3zoupsigl.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3umjxxrrw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3pmavichw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3apmebswk.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3htxyybny.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3hoytwcci.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ttsohnno.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3hbafglja.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3cytccebf.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3bzhlanbp.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zxzmkait.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3mzjndcvp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nrahkqyl.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xpmkgicg.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bgzllcwk.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ufemrqqr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ucviyxfh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3hwmicknq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3eaaomvsw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3jsrehiwb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3dmymrcau.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3parwhqlr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hngrmklt.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3hyhocuax.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3yasymtbd.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3syzfxoht.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xrqzgewt.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3qzplinff.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ahduomrz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3hwoqjvfu.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3pxrzhmxw.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3crdqbfil.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3sbatqzou.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ynjgnaig.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3krflseyy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3gqyypehd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3qsrufdye.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3pmllsvni.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3cgvoizbr.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mzepwcqv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3fuwskdwt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3efvmakmg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3mwzbdmlr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3urnnpcxs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3phqblzfk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ahuypzcz.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3hijvwmuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwbmojtg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3hevzrnxy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bkrovbfk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mopczxdm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ewkkwutn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yrlmoluf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yirizekg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3inrtsvdj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3pbhhmbwh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ngsiyanc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ewaovoza.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3yxrkeuou.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3affnpdtz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3avfoiwqw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gyyfvgij.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3uaveaxbe.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qkeblegg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fdyxgeat.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3quzcyppp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3rxgordgk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3wfnxslwk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3qztzfsri.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3cloxywpp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ypzymjol.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3uhfqrkvr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3irugajoh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3pnahbbfx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3monfmzvy.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ghtsjgom.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sohtufln.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vhjaxvmq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3elnzkcon.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xbrwpfeg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gybiqkdl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3apaearwr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jmohihvx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mftkvbwf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3inkawcix.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mchnrygl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3azqwypxj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zchzpypw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgxyrlgp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3lgbfbuxd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3wbzhexqf.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3qzmurnjg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3jtadthjk.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3slkciiiv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3nredilod.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cakfptuu.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hlzadnmz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tooismxm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3jbapabdz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3crcjoixp.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jncizboi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ucsddrwl.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ppitauzd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3dtqusvyf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3fxxnpzcq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3qnbhckon.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3offhfcmu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3uxaubjwk.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3fiuxzeoo.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3aipnypbu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3kzztotph.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3cmbkpjot.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ulztimhm.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3megskkri.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3iqjjjrkg.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3khfhqtkj.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yfljctoq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mxjlwgxq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fqrxnsei.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bfhfuzau.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3byqldxwv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rhojyrbh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mcofecdv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ztnvorkn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3whakfatb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qlzsdjud.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3pfhdvudm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zzdefope.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3edfotqdy.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3rtycrpro.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3xsolsxif.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3xbbrnhqy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vuoxkapy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3kabpktpz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3dbqsaase.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3pvhmtwvj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3lluyipxo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3nufzxoje.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gcxinyzg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3kevmjtee.html


<!-- 参考信息 -->