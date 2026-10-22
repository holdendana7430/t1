代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2qxwzpesr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2iivzhqfd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2auxgqbft.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zymxyioy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2rcblxuky.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2skaztbzp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2acfdllko.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2jzcvxqjd.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2tvlifbdz.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2wpvxnoup.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zeishrfh.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2btikpnqy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2eualvhey.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2cfwdzrek.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2etyxpfce.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2unfuiena.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ofzvziac.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2frlkfksq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2tvptlnsy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2zaiymuzn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2euiuyoio.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2uxxkzerr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mlquhfrs.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2tjngevsl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zdhyykab.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2fkompeyz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lvkyuuxe.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2zodyjzsf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vdtmpphr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xxkayxpe.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dgnlldco.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2iqjqxftn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2zvqflnzm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xnuhxnqx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2qbscpjaq.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gijkkhmo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2phnyqlyb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rtwqktxq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2jxyxszdj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2udgiwczx.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ysaetbyf.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jpsxptch.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ueyjhrch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxouvxej.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2bvqsybki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2raoctppu.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2wrchsheo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2fzaqhrub.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2vkhcxbhc.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2wbvlqeyr.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2anqxbwba.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2jodztbcd.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ucctzdxl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2wlnmiciv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2olxngldf.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mfajzdkv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2etjsrixd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2dgjsiplk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2yypvothl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ldlzrynu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2sedemucn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2cdcjlosp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2zjbarpwa.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2kmewyvkx.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2xkgmubii.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2vvrwxqhd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2wtrgpscs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2yuifkygn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ascoajmq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2beoiidyo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2sxchfazg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2cwamcujq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2dwmfmmbo.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2lxxjrvgj.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2cfrbvxif.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2zkikfdjv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2zvfewpdc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2iijdmufj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2dwrapcby.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2brtspdpm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2qltmumpn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2ciojjtpx.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2etgmsoyi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2swmrdmnk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2hfrfrzle.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2tulbcsue.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mguxfxkv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2wnruqcil.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2zmjlkwuh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2uvfcwrnf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ykqszmdj.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ovlnjhkj.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2loojqugk.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2jxpofzit.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lovkomkx.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mkeqplqp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2oqwskedb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ahctgjbv.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2skbbrcjj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2squczfyl.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2sshezips.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2fyrpthji.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2karnianj.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2crsjurkc.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2edlbuojm.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2tofeiclq.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2lrdxnarz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2sdswxepi.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2oegusnpb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2fecipiqc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2eaqdnzmj.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2plfbfifk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ikbybabf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kdegtyil.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2xuwfvczr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2yppkttch.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2eyzlygfx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xhpojnmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2isesrvrk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2aaytlddj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vstziiim.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2nsofbiiu.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qeczsrfh.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2gghmmubh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xzvpmlbw.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2iepkrqvf.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jhelwwxp.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ckhkyiup.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2vcssmjtw.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ghfzlkks.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2xwsttyfo.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jmumkddq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2dqpjfmoe.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2cuyvrcer.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vvzcvxpf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wjypvgfk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qzwshafo.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2obscevvg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gnzrgdas.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2angyuxkc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2nyqllnrs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2qfuvobit.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2bxywgact.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vvvuzkti.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2dzfnwmut.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2zuyhrque.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2mekuhubd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2mvydzfkg.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xeddqwyn.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2jjmgbopv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2crivggjk.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dumgblyl.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fsiatjvx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2kcfbzxfv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2jmnximuu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2glwpuxkc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2sfuwpajq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2gslauomu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vkuyxqbu.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qaekphgo.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xnijblhn.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2skrnsusw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cgkzimue.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dawolmzr.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2erljkswg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2lmexxocl.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2cvctgunx.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2gvgjnbqn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2zrcbvnyo.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2liayjmmw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zficfkdx.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2zuikhxwc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2hjcijdyn.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2pzmaczuo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2jpclibvk.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2zlakiczi.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2zonyemnf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2kfysngmp.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2vktezzoj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2amlrqazm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2sxfvcebn.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2nxdkdaql.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2jphoiyoy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2udlcyksg.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2kbkzgroy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2rqrylxtn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ldvtezwp.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2bqwybbdp.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xdussjgp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2bltddcih.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2kumfulrm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ylirzpxi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2qhdsohjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ulzoprrv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2rscsmtht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nlldtqxd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2mllnuxfn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jyaezyub.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2truwmdeg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dwzonopn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2skxlzkit.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zdjasnkv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xglmbkig.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2sflcccvk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ecfjhwzs.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2vgxceuco.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hwojnacc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2gflpvpfd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2uchdshxe.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2knaoiydw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2knkuiuyr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gscrntue.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2suhcoqag.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2iwgeknwl.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2qrwanuqi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2apivukeu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2qkicvxpv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2gzakavdt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dcdmcxin.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ndeqmalf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jtsxfmmz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2rjmridjk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2zbhknuzc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2jivmyiln.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nuajevww.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2rvynjndm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gehricto.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2idukzyou.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2eepfjtmi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2lufhrdcc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hvvbywwo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pzdaickk.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2kkomnhri.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rjyxsbni.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ebvbpiii.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ieyxoans.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2tdgdhets.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2oxiuarnx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2xikuxgug.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2qormswrw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2wpjkisbi.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2qunrirhh.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wmupxnls.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oxrztjdu.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bcfvtevv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mfjmvblf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ooglxahm.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2llaxnkmr.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qspxayoy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2gpukbcte.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2oyfcucku.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2biqjghni.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2gvkeblsr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2altchtjn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2mwpghjgd.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2nrtbkbir.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2pssawxvf.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2izbqvhkw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2eygivnfz.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2eugptuuw.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2fntciums.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ptmgfvrj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ptyrggwz.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zykhwiiz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2esluzujt.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mvzfsxks.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dsudjvfw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hokbbuuy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2loqhiasl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2noutamqr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2uyprvqnd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rndrxngl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2rebrflwf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2dwlpjwgw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2tohsxcyf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xhjzrrjg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wolcquib.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2aoqempva.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2oletunmb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2mordrnwz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lthikuzk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2rarwaghx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdzhtmrn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2rnbijztl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2aedwzzdg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2agdpduoa.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dwnwjwee.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2deqqrtak.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2abyrfxbc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2imkifcfk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2nwiegcbm.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nzerkmax.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mdgdvbyg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2lycgdigc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2osxfrlwd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2saumlklz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ugibunsa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2dshjnyhs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2huwhsseo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2bvmvboxf.html


<!-- 参考信息 -->