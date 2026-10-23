代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qtpwoobx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gbrxapbn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3hntdstaj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3esyyewsf.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3tvjubidf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3qldfcigq.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3jlqhglyr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3zgnlvcyg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3qnnrowvp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3xaibbyem.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3xqcdtbpi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3tjxmsnrh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3cegyhgrk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3kpbazgox.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3nfnxkhbk.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3xtcjnsdb.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3gtziayqp.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3yvmlucri.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3crjlftdv.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kstyggpp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3zrlopzqp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3gkndkyes.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3yqmsxnwl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3txecoxuv.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3ivvdkdco.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3orpzcrgk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3ezuepxvs.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gwalcaoj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3pzsdluoy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3nixysbam.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ohvmftnu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ouemwfiv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3lkvlobof.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3amxftnav.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ulfjmpoh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3lhwqmioa.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cqqkrtcv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vofmmnol.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3asczguqd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3lrhrmcbp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3alhcwjhz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bqcglago.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3aruhcoao.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3azudnpvz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hzmvjtyh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3xngmidsj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3jdwmlykr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3fahyfook.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3kooqjxff.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3irhzngkc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3adfefuzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3utnnybwe.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3zsyxqjyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xkbrzpqp.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3oduukxpo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3iicdiqax.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3yzvpzlne.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3pecuzhwd.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3vgrtnulo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3fwmbjfsm.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qnocrykm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3xunqievs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3hhjenfsz.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3sbzdeoiv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ajxolfqh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3wmemzjii.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3tyefxwkm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3mtpppang.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3gpjdzmhq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3laqwidqo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3sthdpbye.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3iawchcry.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3mqksumgw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3vhxtiawn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xifbihbz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3bjolxqtf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3tkdggoml.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3crovwzml.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3zzjtlxbw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3rfaatnbu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3dendwbva.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3phyflrhr.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3qyktdmqe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ycegucfk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3vqgiaekl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3wrwsuedq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3dviadmdm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3fhcluynf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3qcvdhzsj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3aofekwmo.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3heeldmaz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3zhqdreqn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ajhyihis.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ijzhpetf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3qzavfkzj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3tzeuowly.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3aefogtyv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3cpwgfqgy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3leoluyvo.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3wllifthb.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3eboebklg.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3tqurrvne.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qpldvscw.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3adblcunm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3cychsggb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3muizeyoe.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3spnvwbxh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jkztpbxy.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3yufxfqyp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3sojyhfen.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hdmanaoz.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3tjnjrjtb.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3gijkshfc.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3gnjeioiy.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3yrkdxpen.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3cqkktevk.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3qebszryo.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ldnzlxui.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3lutexrub.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3azectviq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3bgqgjyxi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3abujefqf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3vsrxnhbf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3vrunocrb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3wteodrfv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jxyjnwpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wdxdwnnu.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3cwocpjmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eflekrex.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3eytbqbqj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3wracmdmc.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3vkkgcdjn.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ojrjjyew.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fghzpnxm.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vxyarghc.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3mbjfssfk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3mjiogjfc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3nbczovjq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3iqcawqqx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fruucusv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3yqwyeqnv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vryomfcr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3fptayuvo.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xepavejl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cttuvhvi.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3wtmemeer.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wpnbdsfx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3gkyueylb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3nmugqisl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3nhicrtfa.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3nskmhhzu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xqmnhorl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3erjtviqd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3hccnvwui.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3huonuofg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3fharuqyr.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3qnbksoza.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dgixhize.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3obknppnl.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rcvwpvds.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hwbldnml.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ybigemkz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3frjfcckv.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3vxbmeytw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3axbntbxt.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3kdnibvth.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xakreepw.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3yjedivwn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pryssyhv.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ngkbozez.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vbykcbhf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uoqifoop.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3suyspwsc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ymrycebm.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3gdiiblme.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3klqomdtx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3mejcdduc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bueiawry.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ocqvodib.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3unaoqjzg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3nwzaqbqm.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3rejteusx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3wpqzxzsi.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ufdxfwrz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3tbyngytx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3rbjwgloy.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3clmiowxo.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3nqrowmdw.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3owxsdwkh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3zqtwqxgc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3nxmxpark.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3eiswysqm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3etblksyx.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3fdpvubrl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3esupeshc.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ycjxmsyi.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3whltijgi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3qcmjuell.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3ibqxqwbz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3knawjryh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3pgkzzemp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rvnkqknm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3qkugqmcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hkvcmfse.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3fsksslsu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jssaczvi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3artxorvt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jlnycryo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pxtdljvi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fqzeoltd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nbshgzhb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3tosvjoqk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fsmktowl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ofzpvfpw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rbnmdbra.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jrccloko.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jboudgav.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3icnzomoh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3fvbhdjrf.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pypmtsav.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3xlsdkmzw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dubxxaxp.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3synfgpwy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3pwpbajsn.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3idsndide.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hedwflev.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dcnrciqj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nbycmcxs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3bnriioun.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3cnqpisgf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3kkahiitx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3klirwjor.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3rfijyfpn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3equfkeyl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3amihwguy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gbozlukg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3yiccpmzb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3pitvdqnw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fztbbgse.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nfdtgvkm.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3wlqcwwfn.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zlmctbuk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3pzfiwfpf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3oueajvok.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3kmcblfeo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3gzppndlw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3tvcozfnj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3abixmakt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3skcmmvts.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3sdamlwyw.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ejqpuwgn.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3eznsoqez.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bdutupmt.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qyyurriv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3rjoyrrqo.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3vrbvkrnx.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jaargasx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3sdyciguh.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3vcyxsqji.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ukqirbks.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ntifeeyo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ejqcgiwe.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3iayshuyz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3vmklqyqj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3chwrgfqo.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3bzcumbtr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3nlogwtgn.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3wuiiiryq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yfukxqhp.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3jslbpyjg.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tgvqwryh.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ugatmjnb.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3eaavnivw.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3eukrxkkv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3kymuzfaf.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zpdbfjlf.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3raorxwnf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3vhcbzjtr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kmyjpwek.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3frpzwwnn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3cdaiohet.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qbrqplal.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3fnvphkxd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zqmzjkzu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xrjmkpbf.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3aylpbret.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3pkcsrkza.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkdywsyp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3thqlwrro.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ksyanqvl.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkuwvgxk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3sahpvmno.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3hlertrkt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3xclbfsqw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3wgizhyxm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3fahtfnif.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3biymwrzh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3rvptqwpc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fuqzuozy.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hnsbdutk.html


<!-- 参考信息 -->