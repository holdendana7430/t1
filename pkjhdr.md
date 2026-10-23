代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3hupjtnfv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3mimawbur.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3ukazikrp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jlvyzckj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3gwfbisvu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3gpukmhiq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3bnxerkoz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3exjcqykl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3kbzgpimm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3zjzyuvdg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3onyfmqxp.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3etcsovvm.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rbnxyiac.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3fnflvztr.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3abpjryjl.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cdkztfor.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3nhsjnngc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3rcutryaq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3mzgdysfw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3rrycbnww.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3aeicgqqx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3oyvjvyrk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3tqixmdjm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3mzxcasls.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3xplecfgx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3aynjfbyq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3bzjyhhiz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3duhfdpuz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3brcrldek.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3dqzgkaye.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bqbxyvne.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3ggvvpitr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3byoxvtuh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pwbpqycn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3knpsgvsn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ezihijde.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3sqeicbmw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ktkfsowg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3rxnyfdrl.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3yokhhxjo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3ndwqqxux.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3yvfubakg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3yebolobb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3hngjkloj.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3plpsowzf.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3rbrpamfe.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3lmnprbtv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gjviivfb.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3kldnyqdj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dnnvgyya.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3aeeiaiwb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3qmktwdrc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3tptnjcpv.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rophjcth.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fusjibvy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3eanyhidb.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3pudqycvb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3rauxwbiu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xbmnwhax.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3owxfmrko.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3obcluyxl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3egbztjve.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3bfnzwxgh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ztfpbxts.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3fxiurmyj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3odnjpuei.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ernfwoju.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3wfmzgrfx.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3awabtyyl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ravglpyn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jxkotsht.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3grlcnjni.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3nfirxvwv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3vinogqmq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3rjhxiath.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3rczkaxfz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3rhlzcrmn.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3qvuwcheh.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3duzstpvn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3yphmhehu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3xrjulsen.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3rxkmzabd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3cbjtccxp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3yoyhtinq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3lurulswx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3eoponkjg.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3xmvclspv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3khtszneu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3puswkkxi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3etofvwvg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3yvpbdasa.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3vdgtcfya.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3pizhfkgo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3lmyccvsc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vivihmkd.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dcxchbzp.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qbjsfoaj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fgiyknso.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3flshjfox.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tarldbfv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3fwjiowxe.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3asuuvuyb.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ugcvqpdk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3vlpqwkaw.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xnvqahwc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3pwdyhpdq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3niwahfce.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3yilasssx.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3jclzxojh.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3enxdepmy.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3moffdmyr.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3klpnqfbd.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3xgreqitp.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3yiospmhj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3mvbojrjg.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3eruinydx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nbyqzgfw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3dlzmozfd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3duokvezd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3jzdqrvmh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3aixacccl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3vwxidfso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wjlfxeby.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3imqbwaxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vhrnwfhj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3dgmwwukp.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3louutjdq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3apboueqm.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3bymnkmtl.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gcxmfrac.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vrbbaxda.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3srgptfvv.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3tiugdgxv.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3bjwqxvxm.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qksrwmbj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3byoqhpeh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qhbqaubr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ryontazw.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wvvvcmrj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ashadfjy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lzmxrepk.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3muvjegur.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dgfmiaps.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3dtacgfqw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3xnubtijq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3pvxcteyb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rvbbpokd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wtvtelfa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3tjotjgot.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3oskovddf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3uafosdjr.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3sauejkvs.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3xtnnytva.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kjgsfcto.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3fybmftsi.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3fzxlzies.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zznmvspa.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3dyzxztge.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rbuzkgfv.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3tibctreo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3uxzqslht.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3soaoyvvy.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sryespew.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3rmopyghs.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3brbfannj.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rkyplxdu.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rltdpjjx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xnoxvmkf.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3qhxaubmr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3hhiwejzf.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3hwtpvtdk.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dzqzqqdt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3twcevnoe.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fvkaeufp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vjpqqvnn.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ettatpyh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ueqaookx.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3bcraechw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3wocycwab.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3fevvaxrk.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3uolowzlj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3gnnklyox.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3kriginbr.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3dmbvqqkv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3fgbxrbjh.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3gdmufqap.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3noyqqgvv.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3mowfqgkj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3pufoipho.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3aqfsqtcu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3krbzbnic.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vqwnajha.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3chigfkqr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3xfvgwjme.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ypzuxets.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3yipivnmz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3iffgxenj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dhqmmqah.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3pqggnxsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkexvuuk.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qqqekxoe.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bmenneyt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3eopbwghm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mzgyxpmi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bjgnqidw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pgkxsjpm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gjbrrkpj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3uclfszak.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ktsdqhkq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3wizgkvbb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zgoeujkv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3aaigopzc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3iemkjcvl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3uzdgxtks.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zmsrjxny.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hehohhut.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3hbtklgwp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3gyuctbzb.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3xalzguhe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3atafhpxq.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3mvoizdty.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bwbkikxf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bohlidex.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vcclnktt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3txswlwlb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3wsmwbhhv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3tqbffukj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3cugfnwcd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wyjsajym.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3tfhsehft.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nskqfhcj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3uhaqhywy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3plxrznct.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3cftjpcjz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ncwfupom.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lllfukwx.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ostnoirj.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3frwxjxos.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ijpnbqnu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbvriboz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vwqdnztn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ivitwzfp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3xsbnakvn.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qaofxetd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ryklizgj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3forvhzjf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3gvgyqzna.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ugzgdluj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bhrlbmdp.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oqjjdshk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3fyvsaszk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3vlmpfqho.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dyuwcvda.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3krkmiiax.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3cpsdygft.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3sflwxake.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3whzlnlol.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3uvcwexqq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3sdfdkynb.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3fpwdaslo.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3fzewgcbt.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3imzlzigl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ftsyzdfm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3vrxsksit.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3sbbdiipc.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ntciywva.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pkjvatki.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3graanoji.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hqdfieof.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wsbplemg.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qrklviex.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gncsnnlc.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3okplrljq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3stpmfvjd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tupjuyza.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3eqxmobdz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3xoosruzl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3cqsiykhf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ushcpyyl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3akpsypwm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3rzjebnnb.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3rszepbdc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3drqkkrxm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3nxxulkxf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3venavnuy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3sgsvsrtt.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3qloctfvl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3pxfqoblk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3fdrezyvu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3cmoyqskw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3givshqjl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3mkixtegd.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3psghthnl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3dyrhdboq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3hyqphjig.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ezqpmnas.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ytnnypbu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3jkbimkbr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xdgkxocx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3httkdbis.html


<!-- 参考信息 -->