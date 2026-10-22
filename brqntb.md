代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2hxonwxpy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2oyhnbmfc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2cqusygko.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xmoplypp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2jqvvvrgx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2onghrjwb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2xeizxzae.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2kwsgokne.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hcgzmdvb.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2xdibaggp.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ifhqynnn.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2jbygqbzt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2vzgognuv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2mhvmvgts.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ytminmgj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2lexnnxer.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2wzhqhfjd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2eycqodwl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2qwgsamii.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2oyewdciv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2mqyuficz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2ycyhbuqr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2pkyogwoz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2gmexyayt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rwlyboxf.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2dwxbwpsq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fnxbcjid.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2osvemnej.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kifzacna.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2awlxvhzc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xzdungmd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2vmxmxpjq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2otcqcdll.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gwaakgwa.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2hdhxkvxz.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2rskmyngw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2coohkfeh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2jbfscpxy.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2qectwcgj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2jbiemjtl.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2tvngjcmj.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xeuruxgd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2oagwehch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sxfjqfgw.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2dzqnrzfr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xylazngu.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2grkrsuoq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2imhxsbqw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2swxbsbqc.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zowxubgt.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2qfvmkkyu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2nrbcxxsi.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2qmreiczo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2lpqaajrl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2iojnfoyw.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nkpfqedx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2smhwwkco.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2qhrmpdld.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2mmtcpcfj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ohqqgguo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2pbwugxja.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2nbtbpuoz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ortwwtoh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2eqdigoif.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2fbowddpy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2muluiqqb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sdfrnzgp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2zbbeoxxk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2vmlpmrwc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2utjlbruu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2lzqnszth.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2oilwmzad.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2nhnggjdx.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2aqwdaewv.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2evvqiccs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2tvszhnwz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2hyduynql.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2adcdadra.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2jsgdfhku.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2gwsituko.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2hualgbfq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2yziafcrb.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2mcqwhfsp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2jsevwxcg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2hqomwvuj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2xgvdlyhm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2nkipsdwp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2uefwlzzp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2vrkgubpo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2cnazvgue.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2weftqgti.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cdkejzph.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2hnllzalm.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tdpsmaqm.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2aiofliyc.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dojcbtsv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2clhidkuu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ewmnrkqr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2jvpfaruu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2nkwyfiku.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xjcyjqtj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2xnnbckrt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2zzfxlayk.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2dszpacfk.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hwiwqwzz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2awpwzjip.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2leexwqeg.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2cnohxlaq.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2jvbfeexf.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2nwthmcdt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2wgaiwvat.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2giprnhrs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fcwvmboi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ydjlklvq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2oeufvgqd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2rxrljary.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xtztaels.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2fkytocrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nfxxmros.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2mbkbxdpe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2edzgyfde.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2qtmdpdut.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2gihvhsgs.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2dkdjxtfp.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2agwgluwv.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2eornbtbm.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2diiwobxr.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ecmyzdsh.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2bwtdmzvo.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2syjerrds.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2rafdxstj.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pulweoqc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2sbaireov.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2visdveeg.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2bkdrkukh.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sepcbiji.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2evcvfezv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2msfqxmjv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bowwntsz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2gwqunruy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2jnkgfsnp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2elhjtmrl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wdqssnyv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tjcpvytz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2waomfahm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2xnxjecgn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2rlunsxnv.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2jxubkqhp.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2xyvvshzb.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vqundlex.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2amsbxuhl.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2sqeenlpv.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bowtgaka.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2oxdkmorv.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qldtwyfm.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2gyiphwgm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2onhwwllm.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2khwijdyu.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vuxtdihw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xnxuxbda.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pqiusaov.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2enbcikop.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wizahbch.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uqnybhcd.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2yyxqirzy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2ivfpsksz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2larqcnsd.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2vaekjzrb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2kiufymvh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2osldvbcm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2crkcmzfe.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ckzjmhyl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2cdggtkra.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ffpqinwd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2sqgrmzvu.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2kueqojhe.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2puloxzeq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2qcctnwga.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2gdazirsc.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2nxfmfsjj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2laowxfix.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2errouhju.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2kmtencaw.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2nsgsbibr.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2dzigbgdp.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2lnhfbedb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2khpjudoj.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2aawuszzt.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qvrgzqob.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2orgleavq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2aelfdkop.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2dtqbrwxk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ceszyohl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qvircrua.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2yuryfysc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lfcklsap.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2waxjzkmq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uxrhngvs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ehnixujw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2oviggfph.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gqonhokg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lwxnaiis.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yhwkkayr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2rbmkyojb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zmozfylw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2rhmmcpof.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2oskykomd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2gpwsatsx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hcdgartt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2iowcjkmj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2gjlvmjze.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jrqgrgmk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2nxntxrhq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hitpntlb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2awjzdjzb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2amdkzkzz.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2lszketic.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2mokysxuh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pgqrhxoi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2mfwpvjur.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ljkdsmzf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2xsrvxequ.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2sjnvbnjo.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2mnotrczo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iysrvkwm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yakogqni.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2amxicgrv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ovnrftwi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2pbnhvsvu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ibtnmelz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ffsujwjc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pekrdzuh.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2plfnavkx.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2txfqndqn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrjkpxmx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukjdkhrm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2gtcjtwkt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ctctwhvk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2gvfcgwmr.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2hyvibkrk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2mhnpijrj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2xdlydwow.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xpmkrvmx.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2pcrurkdf.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2emhddzns.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2esfmeyeb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2bvsqjzjv.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2mykvanen.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2odbhkkll.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zmvaamzf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2bjxjmcne.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2rcdsaiyi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2whqtieet.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2hilqcxxl.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2rrqlcgvq.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2iwmagenr.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2mzjusatb.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2lepnypcd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2bltsznep.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2gsnqpbxg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2sujwdjas.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ciqlfoiu.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jvzewaat.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2znpalbfx.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qctxwgee.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bhydxypz.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2unipbaak.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jnrrjdry.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2tnfyohog.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2szqeptam.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2orheiyku.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qrnnjkmh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2utwwqyol.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2kpzqcxjy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2mqhtchfr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2daageasz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qlvqytml.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ihizukvs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2xsqolxiv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2roucxzpm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2rkuscamq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bwmjlxlx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jflcegyf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2igmpswig.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2owszlaes.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqrumorx.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rbkbbskl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2czvvjkke.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2lhytbjfc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2cplbqhfo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2gqczzpua.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2samyevxt.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2iifmrzjs.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2zjrviqeu.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nrqsmsde.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2dqzglwnk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2tpbqhfjk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2bqsmbkfm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2bwfzjaca.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cpqwgqhp.html


<!-- 参考信息 -->