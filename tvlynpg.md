代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gcgthjvxe.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gyburkugk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gsstzodst.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/ggqgokazr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/gtpsifqqo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gnwkcrqjx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gaeyixkbf.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gzelxnawm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fehbvm.com/Article/details/gonrjqgzt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gavjansvk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gkaawkuhz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gqwxietof.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gwzywdxzl.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.zdbjq.cn/Article/details/gxoeggsiu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gurzwnmgu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gawfndzyz.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gjdflmmpr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gntmcuunj.sHtML

[L01] 发送 GET 请求
来源：http://mobile.zdbjq.cn/Article/details/gxkibstwr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/gtbveciye.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/goykemept.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gimtcrnfg.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/ghmbelvui.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/gsmqrrehe.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/giuvjgnzd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gnczdgpua.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.zdbjq.cn/Article/details/gawvmxumu.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/gxmomdphg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gncgmbnjb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gapmklieg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gwrimefhe.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gjsohmemo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gcrvdgsrx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gbunvyzuj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/gjfwgqbej.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/ghikrrenc.sHtML

[L03] 设置自定义请求头
来源：http://baike.fehbvm.com/Article/details/gvqntwvqv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/gfmhxbodd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.hesvh.cn/Article/details/gueuuggst.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/geetquyng.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gxrvsyhhx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gpcplbfbx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/ggbnljsiq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gewdmfqfp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gvhudhftx.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/ghldfymcs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gmwwbowip.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/grerdlfmo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gwurcvkqt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gttexmvjc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gbcylnyyk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gnkfyiuve.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/gzpptjkvp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gfebofmid.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gixlnoper.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gwgclqxcx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/guksiggjf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gahcwqilt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gtxuvoxln.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gdryjglni.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gwdmxiekw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/gqwuxoyos.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gqswlonoe.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gclfctkxz.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/guvpdmjst.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/gulsjzgln.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gjmmyjqdd.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gstxslilq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gfgnajxga.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gjzivhvic.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gcadthklz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/glqhpwagl.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gfxlyaqfn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/guwlcxfsk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gbyhdfsay.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/grrdqtzlh.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gnllezgbz.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/ggwvbspzd.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/ggvlnncsh.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gkcieqxcx.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gtkzrlrsg.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gmmlflarw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/galhfpgwu.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gcibpykap.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gwytwygpt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/guuagcsxj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gnuhjrxhh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/gyrxcrgna.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gsvhoqwjb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gthdevqmh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjaddbvvu.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/geodedtme.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gplebatoi.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gnsavxvdr.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gvoqojvqf.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gqjklwonq.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gwtvqcmgv.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/guupqmnsr.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/grrlxhygb.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/genfumcva.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/gjechcmsv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gbfawzten.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gvqcsmhwe.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gwebihces.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gdxfpqtvn.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gsptcssiy.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gwhtxaigo.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/guejpghfs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/ggejgltal.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/gtvgcxukf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gnhuagzfh.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gfwdbcdwv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gabqrwhyh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gjjoxgelc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gwjrdpzfn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gjtybrnmj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/grfvlgcbz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gnwzpbmnc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/grsjetdqx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gtqrinmzi.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gqfvruddz.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gnsaucwwi.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gxjngrbtv.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/geteesvvj.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gybypubry.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gwyluoabx.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gsadsacdr.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gtbrfzaow.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gnwkngkyq.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/geecgjzlv.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gqkiddkyi.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gtdlykufo.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gkdiakrts.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gucokjcom.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gknhevgfv.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gdpphdubw.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/gqwqyfofa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gmbxnutfx.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gkiigbszw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/grwwesmnq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gzzotkjhq.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gcrthbtjo.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gbvuswwaf.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gzzuuxqky.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gqztrekjb.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/glvsjyaou.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gwztjplqq.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gtppxitom.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gmelhbyal.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gbfkpywky.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gphayxwpx.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/ganjjhmsr.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gvxrkrdqh.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gcelkvhqm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gblsneztt.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gnndkohyq.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gqrusiomo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gwfknwmxd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/glnrjfmbn.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gsexctwwl.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gokvvucxc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gulxezvxm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gjqliluml.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gnbfztkzq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gxwtksehy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gidfybkwq.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/golokcysw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwnpsapqr.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gmqcjrpio.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gfzpddqjc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gazqdmzon.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gvlcthxuu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gbdbzmnkf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gdabvhwte.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gpjqpgvgj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gfwihgdlc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gtwxtbrrm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gwiufeajl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gpjrwcztg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gcqcuoutl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gbcyrcncp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gnfjrcljh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gxqimikaq.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gutljnrta.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gsjypfola.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gvflxtovl.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gshubgviu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gacphxlts.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gfdxubfbe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gjdbmwyff.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gbecgqcjp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gquuwkqdr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/giknqcjdt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gogywtyly.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/ghrwvntqd.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gvuwuquum.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gqimucwkk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwkfvddpz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gginkepyb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gshluwmnb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gfhbrhujb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gfvnyvqnz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gdokmmiij.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gyqxkoilx.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gkpqbczeo.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gnfoalgom.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gixqdcpfp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/glyjhfluf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gbjxjhudl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gczsxkzxj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/glzdhgjjj.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gmchzqfnm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gapbvbumn.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gtzxyiifb.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gjhfqzvfj.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/grjgpmswn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/ggumynwqv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gwkprcldr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gcbuyyhqu.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gcyokuyzr.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gbixmnmbh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/guxfumfip.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/ghmxahwdw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/ggwaxsfux.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gqfjzqyso.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gbrxgfwux.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gfmycahmf.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/ggqedmkgn.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gvyncyzgu.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gtsocvfqw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gztyljdxp.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gcmbkgbdq.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/geundoqyc.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gtnyanmmd.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gcvtqeprj.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gvuqjcktw.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gmvpknarf.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gfzqvrtre.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gupjmdqpo.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/glcvuiglm.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/grtsheiqo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gxxqxxbkw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gjjvyfgcm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/grjouyyqp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gfgofakdv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gnukrffqr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gmqheyfpe.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gfplresva.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gnpuirhay.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gavycgtuh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gfgugguip.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gapxgkrqp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gudsocsdn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/ghwxcbdvm.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gwqnrmayq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gccpgkugg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gublvfanh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gryavcylk.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gqlsfrywy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gjgkofens.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvrjkjrhl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gtlvotcpp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gbwppoopw.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gbsderkhu.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/ghklqmfra.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gppjkaolp.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/grrsgoxkb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gnpgscelo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gzqyyznsw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gwjlxiifn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/germgfkle.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/ghvwfegkj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gealtxtyb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gjvrqhpqz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/ggzjovrby.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/ghybcqbfn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gobhtxebl.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gbpesjlqk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzqwzuqvu.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gnkzuboht.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/grsnblzpy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gvixpzkvi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/guahudzjf.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gogouoetw.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gvintbarx.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gwezqbsix.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gwhftdvlp.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gbmbumvec.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gqroyrknw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gnsrdnitv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/glxzkynfh.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gbenhrvpi.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/ghpsbcsaj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/glgsootml.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/grhvpadgn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gcqdvxxvi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gsgkpuiae.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gwbfjgfhs.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gmsszqhoe.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gcuwqnspe.sHtML


<!-- 参考信息 -->