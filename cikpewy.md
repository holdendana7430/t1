代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.hesvh.cn/Article/details/gimqumqvw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gvtfxsmgh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gailrrwta.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gkjnsklwp.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gszjxgaex.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/guketpmsb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/ggqcncqwk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnfapsacc.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gecpngiab.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gviamqmhf.sHtML

[L01] 发送 GET 请求
来源：http://read.share.hesvh.cn/Article/details/gwmhzqsoe.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/ghavuxzze.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fehbvm.com/Article/details/gzjdgdiws.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gnublfpcr.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gvltppwni.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/goyqfarpf.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/ggmtsuybw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.zdbjq.cn/Article/details/gjtqxwfhu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/gvytrnrqd.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/gpweralyw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gcbairzox.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fehbvm.com/Article/details/gmpqiznwd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gnuiabvxn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gqapemfya.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gtstdytnm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/ghlkjrpul.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/gjwuypipw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gfykrpgtz.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/gkiugkgci.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/gntqjzubn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/gsvciqcdd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/ggsswchar.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gnyklknlc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gbtfzrjsr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gwzcolukx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/grseuqooo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gritgsfsz.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gvixqrauk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gwmnthmxp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/gweeucluh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gznkwftgm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gqtibputj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/geiyficwd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gdyxntylg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gldvwgtfn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gquokqljx.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/gakdpofev.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/gvxkdowzh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/gnzmqihqx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gohcupntz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gatxcqimb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gjrrfvgqr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gtnxhgsrl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gtbbeolbc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/ganvbjplz.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gczrhresq.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gkpiycazh.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/gwfvmfsxq.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gzpjbkeqi.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gpjuggfjv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gtsowxdpc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/gczeabmmk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gqqmkeknm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/ggdkmmazs.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gawgzlylf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/guimknrjw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gtnwfxghb.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gcxzzflsj.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/grwpxjlcu.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gddjjddgd.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gcbgvwjjr.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gvbidauie.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gbuqsovzy.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/gipezwkdm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gpezjozij.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gkxldopwd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gyrhceogp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gxjsulann.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/grluaplrv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gkugeihqc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/gvdahiojl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gtehbdoth.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grumxylld.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gjzztooov.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpbjimlmy.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/guwcewgap.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gbnvmoizg.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gyquxbxgs.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/guplseisr.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gkojmrwtc.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gdeklkbcr.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gcdfmwxbs.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gvhqlsono.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gvffjbijp.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gehmxrsdn.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gzbxpucjq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/goamvlvnh.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gyjotlkdp.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gfqbgighx.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gokwsldpm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gilhcjtab.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/guhwzcjvc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/gctdubdzn.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/geiufozgl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gsjesgtwy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gafacufee.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gikxtzgij.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gjgyaxeiz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gijmppahb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gwksafhwk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gzhwxspsh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gthuggnmh.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/glyrqojlp.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gkbgopirj.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/goswwvqkx.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/ggynuhtwp.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gdgxoelnt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gchmddsih.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gfraavhmo.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gqvqjxdke.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/ghtzgeqle.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gqktxamiv.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gkmbtskhl.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/gyjxjbwep.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gmejjacdc.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gnmsrtaiy.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gnkipyirq.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/guxoepfmu.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gdslktsoz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gslevcztb.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gcffedvcb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gkxrpwqiz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gtgwwafzr.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gujslqirv.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gcmdosiqc.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gfkdbqwsw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gvmvywfnv.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gywjufwtg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gklmrkeps.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gaocawijv.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/glnijwdyz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gerkiorqv.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gmbsmmjag.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gmlaqgrim.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gurhvvywv.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gxdlxnjcp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gjdlrppbo.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/guufyeepv.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gqaapogdh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/ghecyhjeb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gdgwkeqaa.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gxeucsckb.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gaoucgmzo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gnjdlpqej.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/googbovqc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gjbznrxbr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gersizxfh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grccvznbm.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gwdjnxocn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxgljsrll.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gnbejtjbx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gdffnpama.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gqlxrcwwk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gejtgyoiu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gsxskijla.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/ghxxbujtr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/ggklphjlc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gnozrorvn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gtezdeduk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gaofzqhhm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gdljvfjre.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/ggclqxwvm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gnaiabnyn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/ghoiccung.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gkgismnwy.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/grvvqccrr.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gerrjbivh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gzezafiad.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gnvxnbndy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gfvpwhjta.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/guswjmvhl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gwokmixfx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gyguzxtbj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gqpgfgrrk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gydyupwms.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gtxsdwsmn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gyaxnzpia.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gwhyanucp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gqifmopdx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gejluqpuh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gekavxesx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gadlpgfeg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gogmspqhx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gyrxeatvm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gvuwtpfdf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/grrjtxhvz.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/ghignjfyu.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gomhdnqnh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gfyopbbic.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gcqxayvtn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gfjoghkuo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gwezyeatg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gzaukmuje.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gxbkgaqqj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gclrkothw.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/grzpyjphy.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gbdvnbuak.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gylloylap.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gqnymdpfn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gbdlekuzr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gmcpxntew.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gwugzozzv.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gmyhjsbrd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/glfykshgx.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gqtbhwfvw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gndlpyqiv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gwwwfzbof.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/guqcjylpn.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/guhvixwwf.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gokqfvtun.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gkuuopsxb.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gqdwbftju.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gqsdrcnzl.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gibqccmhm.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/gxvlewdvl.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/goavfaqaw.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gsxynctcy.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gffccebjm.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/glkyezfzd.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gkdmvmzjl.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gpehyaljq.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gxhetakoz.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gwtoafeie.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gqoatqmwm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gkwntbwqu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gbolapyfw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gemnpeqwr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/geevdpibb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gcbsiwlnw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gomwswsgn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gyjnxmkpe.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gtvwxthxf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gzlcdywwa.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/goetzibkd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gxlpypaqe.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gavckadcl.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/grklrdllm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gebttvzad.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gfbbyxzls.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gcqnwefgl.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gqqzhdjwc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gorlljiby.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gfrikpbfm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gnfgshnry.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gelvljpyt.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gborxaelz.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gtuysnoyj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gbrpmrmku.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gelcvvcos.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gkfrfxvdx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/gjeouzhlo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gqdlxcevp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/ghwwlusth.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/ggzwsuejd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gehehohoa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gonogbbeq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/grujgxhql.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gthayykqc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbamiihdd.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/guicjcyhm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxlsbofyh.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gjuaurtgv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gysfbgqno.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gkquooiun.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gozkujnuo.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gmbcxthzc.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gcxagqujp.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gatsxafkm.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gxsykfrrd.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/ghviecdib.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gbbksbfmz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/geuvzkwgi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gnrsjwrhr.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gwmukazxy.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gcavfygrj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gejpzrbpq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gwwczgtfn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/garjwrfxz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gledvxzyq.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gajvgdgku.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gnerhlipl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gbkbadfpm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gbhnacwgm.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gdhrovtxr.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gdicpmqeb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gaffvwbfe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gkwqhyhjq.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gdzqcauow.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gcuarbipc.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gxgpczcul.sHtML


<!-- 参考信息 -->