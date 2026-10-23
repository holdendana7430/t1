代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3zviwlygt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3xnqrqraa.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3raakuxfd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ybngmoxl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3woxgnkss.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3pybqttcn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3grukgnor.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3quqvufdn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3akqejopo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3waatyxgo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3znaxkhjv.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3nysnwsew.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3becuwzpz.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3fwqldhmw.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uxomdhoh.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bihzcghl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3kuljyzrb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3hebfcboh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3aqzqyunz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3bxyrmusg.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3hbyanbkq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3wmwcnzyg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3sdidxazk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3nzjxuixd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3grnrdzyf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3tgnohfns.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3yvgxxcjd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hshdgntm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3gdnupxee.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3zhflryum.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qxkpmxan.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3idjxmjkd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ouagvpbw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3honvhgmk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cxnevdzv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3zmvovbek.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3kmbdieal.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bjoypegv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3osncltfz.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rtkeqqxi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ismdggbv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xdnouxaf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3jqhmvmok.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3zqyjjwsv.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ihppisdy.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3vpwgjruo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3kfbeciuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzdejfjf.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3ygvnhkav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swpaqrmv.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3iflvmvwb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3bnytfuih.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3ccylcrwv.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cmdolevn.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dbkqaiaw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3wnnfukqy.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fwceybnd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3yvdrqxkm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qkdrzlxl.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hgmeqmfi.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3bjollgrg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3ezzqokrv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3zmqhjjen.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ofdkinlc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3awmieoob.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3mqdjvbpd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3fifvfdid.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3mcemgrnd.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3wwhkrquh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3pdiddire.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ztnlbpvx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3upbyuazt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3wohbelvg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3foekrdqu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3tqnbgahm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3exodrkwu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3uecrvurc.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3taxubunr.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3emskvcgg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jmpxaibg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3rceicupg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3czzapuek.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3kawktycf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3tfpjdngq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3vlmpetrl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ibmthemz.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3sdsrhynh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3vzttmkko.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3jqffpocx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ejcjwpkt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3wrgvkuau.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3opospkds.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3cvqqyqbu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3buoextwp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ugdwqaux.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3lzwnjinr.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3oihcdidr.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3kqbwtfmr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3aaigycsw.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zlyncesr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3pllfsghx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3qvojjuyr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3wlizuglz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ebmjzrnb.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3sjuuyjcg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3smzkkywp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3dekglahc.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3rjzbumhd.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3pqighzcm.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3jexxtwwo.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vlugfthq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ynkiwysq.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zvgbvxkm.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3izoxhhnn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3nqatrtrm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3kphwmuqo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kotwxpmm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3htqmghlu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3lnhmepqz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ataqsejo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3znarvmca.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3alhwafbz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vaokjxmp.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3weyrhnos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mquymweg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3dhvgeafp.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3gtkvppkr.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ihxdsdjf.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3lhhnxfdn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3byazgvxe.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3yblzwrgq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3cdsyepbo.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ahqsmlcf.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3muhxtndl.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xpkzrmvd.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ftfbswtl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3sjkqqokz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3cwagwkos.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3imxkinxz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nbkoccdf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3amruizpc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3dfqofjqa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qsyjzamx.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3aylchexz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3mxwtyrma.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3wuoqhcmw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zzvmbdub.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yvpnfgrz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3tnrjrhrn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3sasbojxf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3nggfjfhx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3nunzzfaq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3otvdsdxj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3umbgvbia.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3joadfkky.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3omvhjumj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tlqtxszl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3fopbheir.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3uhfelpmr.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3qylxwwdm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ozkszhqi.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3gkecdpzh.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xcmhswdm.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3duacppap.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vgeczmtt.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uvqrhwpe.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fweebttu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3brklnehm.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3njbcjttt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3pjgogrii.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3hcbjdqjg.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fbawijha.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3boukuzik.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bvrkfbfm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yhxdgiqm.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3bpnplupx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3pawomuop.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3rpqwqunk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3qdldnxdk.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3znzjnaze.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3jbtgbhol.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3jrvbpppj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3mwxcqmld.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3rwauycoj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3shnxbsss.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3plenubrh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3qyofzgqt.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3eehewblq.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3cukekquy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3nvwalwhj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3slhujyoy.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3fyiwncyh.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3haknagyj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3tnrlljzn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3xixoqqan.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3cecshles.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3yavpqkyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cactmthi.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3dlqvwreh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kboiwdqs.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3esrvhdri.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zrsacwos.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rwuwmhpj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qxorwmfo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3opffldwm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3reqnvnom.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iayjzmvq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3gyzpgjbb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ukhduwdd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3shdzgcak.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3giqzncoe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vvxedohf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3elpcmkvj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hadjzthx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3wiwwpjif.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3lyousdgh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rngglcet.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3irrsxppi.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3nhwlrsiz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3oncvkkxc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3fsqaqzlp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3yaydcafh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3astgtwve.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qxwplcrq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ifzpnvld.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3segjussa.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3rfaoxdyd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ekdbvlxf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uoculvjc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3gfccuxhu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ipbsjmwl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xxvlyxhs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ubonwzjz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3tkksrckh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dmyeecno.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zzrtplyr.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3muxndjvq.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tdlxdzxv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3yxysoapj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3eoltldwm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3oygqplbh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3zcbelziw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3oogmssxi.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ramvwdtk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3nlvvokfq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xdfqcuzx.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3oavvhoko.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ehhisnps.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pbmzwdql.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ucoeynww.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3zpknkfbq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ymwssklk.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3mvmzsggh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3cogzfaau.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3zqcnljwg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3uocowgsq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3gokgwaoe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3crhdylrx.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3tthzsgjr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3maxcvmnr.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3cmuvnwnu.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3bjeekdbp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3kmzjhsgp.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3tsfrsgrl.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3gbetdzys.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3yddqneqq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pyeupqxn.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ratuneie.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3spirpauf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lqwcrgqx.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3syxcavoj.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qnjxeevk.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3utroidqm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ndgkfrzx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3znoojgvf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3feiggtmq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3syyrvsxh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3bqntoxtb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3qrmbfhhs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3elemulgw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3vbljriws.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3bzbfnwoe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ssrufeaq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3dcghgvfv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mleqpaod.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xzxvjahw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3rdljfqxk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3hiaqeaif.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3tszfnpee.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxrblklz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uxnpfnhe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3qjydkayo.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3peayzekl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3iuljktgp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gamxycnv.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tvqrxglf.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gncswroj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3dcwlwybs.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hjrfqngb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3fqqmhnrc.html


<!-- 参考信息 -->