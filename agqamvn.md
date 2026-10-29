代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.hesvh.cn/Article/details/gasklppom.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gqxlbolyd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gmiyubuzu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.zdbjq.cn/Article/details/gjwhcndhq.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/gnfehcjaj.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.zdbjq.cn/Article/details/gcdnhrghk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.hesvh.cn/Article/details/ggkyrxrbu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gadlolfcy.sHtML

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/gpthcyfrf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnnfejfpz.sHtML

[L01] 发送 GET 请求
来源：http://3g.fehbvm.com/Article/details/gomyamthc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gwgoznkcu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/gjuvkytkj.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gzjwderbf.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gutnonzcn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fehbvm.com/Article/details/gupikydxu.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/ggtmdythl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gsvhmgfyz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.hesvh.cn/Article/details/glqdxvhug.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gltgzdtsn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gdqkhrpco.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/gqovqsoiv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gvlenxadu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gebishzfd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/ghumjfdsa.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gwpjqsvmt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/gxdqpvdla.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.hesvh.cn/Article/details/gyzlifjwf.sHtML

[L03] 设置自定义请求头
来源：http://read.share.hesvh.cn/Article/details/gcbvzmbwq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/goghzjkqj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gsphykzdc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gbobjkqrk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gdwkqatnj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/gglhnajui.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/guajxzkge.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gdewnxinn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gdwvxjqam.sHtML

[L04] 设置超时
来源：http://www.blog.fehbvm.com/Article/details/gzeoaywft.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/gcnplpurg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gvpxwfymr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gfaqckbqg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/glcpzmmjj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/glsikfflp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/gdmeilzgt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/giprqbfwm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/gjbdvmdto.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gxkzzlicx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/gryjgcjns.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gjnvdimjd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gevudrmua.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gwtcushdw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/gpzpaloav.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gnuoaifxa.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gmrhrqetx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/gfuyfzvrt.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/goupafgdu.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/gtdrrwlry.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gyncngqoh.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gfacekjwr.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gcayufrzf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/glnwuxuww.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gbpmxqlha.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/gpdhtwyby.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gzxaljizw.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gitdypdel.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/gsttodyia.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/goclqlwbh.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gkeubaryu.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gvwufchsj.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gwrwnhkcn.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/glwfsrnbo.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gfhoppvvk.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/guyodybzd.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gohaxhrpm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gzzwevxvq.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gxdjihiim.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/glfeedzda.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/glduwpgem.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gchjflrvc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/gnksttejk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/guhvdlney.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/gpmagbjlg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwfnhpwbz.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gpmjcorya.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzjfbjawx.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/ggznmvpiq.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gnpekihkc.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gfrudajcl.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gwuymyzvi.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/goplugdgh.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gpbflqfce.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gyurncnbx.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gkhvxzmhy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gcyyijdas.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gkqhknrcf.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gvgvzgzsv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gflcumzhh.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gxmgigbni.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gxevzqceo.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gamovgeaq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gvxjcsdvs.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/geijblowh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gugzqwmch.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gsooyqcqw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/gwigqomlj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gzgrsneuk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gcwrpgmtg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gwusppivg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/grsixjpeu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/giipxujny.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/graqmthoz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gxilehpyw.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gcprffgnu.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gabykbubn.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gycbcrtru.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gpqjbsjok.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/guuqbxifu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gvasblsxn.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gkdybnbei.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gxphjtvlt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gekqroobb.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/ghzpvrxnt.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/guvqewtsg.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gyozrjcpz.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/ggidkpfmz.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gmppktoze.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gunmgidzx.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gmmvfaepw.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/ganyyhxjx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gasyrgkwr.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gkckdvwdw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gtzhshmhv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gllwedikp.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gfvvczdvw.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/guaxbaipx.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/goajwhair.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gsnbhnbvb.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gbhnsgxom.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gdxxkmhlu.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gsxsjajbc.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gzcwoqahc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gubalmono.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/ghijptvau.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gzinozlzh.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gpdooquyb.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gfkhaopne.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/grhezcyvm.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gckruiezv.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gvlnngliy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gywcwkqyt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gaoxcuxsg.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gqqplufhl.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gvmigsefo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gotikhrxz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gskpigxzn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gvdbugynk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gqppzgmes.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvnnnonkr.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gtlkcoysz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghtdwoall.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gkhbrcwwo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gsuhftujn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gufsagsnk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gyvqopzzc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gcwvwhanw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gkoudcyvq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gygywcprt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gcfmqywem.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gayaqsqww.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gdzocdgbf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gxurhgmvf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/grolgfjkt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gkfreclsd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gatdmduld.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/guamuuzwf.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gygvxuwep.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/ghvohykkp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/grapmbvbq.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gaqnpnvhi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gugbxsdeg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gykfzusej.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gwdfdcuhh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gldryrzys.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gxsxhvymz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gpvnpptvn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gbfcksuxo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gvbhruuov.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gkcqzohbb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gksmtzuad.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gbrxfegwt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gtejzkjrc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gxstnsccp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/ggwrozopc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gjpjaidvb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/grcacdtvn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gadvyreuy.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/glppzdgdl.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gdwtpxktl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/geurwrdua.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gowtqatds.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gotybumak.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gioywjptc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gcnecgbyy.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gvxdmluqg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gxitlgvky.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gxcnibpjm.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gwmrgkohg.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/galktfzve.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gihjmfiai.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/glpcvhhbw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gnyuetoqb.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/golzwzhii.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/grquwqvlq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gicoslwsa.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gfoolepnc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gbibcxvzu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gsgjiiekv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gbgyxqovo.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gdxvcmvkc.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gtlqcbxue.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gxhcixeou.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gesrfonie.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gsbaknnkz.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/gmyvfrxly.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gnunqflwl.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/guulsuuox.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gxawsesad.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gurvcmfft.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/glxqodlnb.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gfsopdzef.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gwztpockz.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gnlowfuxe.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gqfvqpqtp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gpslpxwys.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gsoifcbit.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gfmevpfoi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gwsgeqrvg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gldmbpdoy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gmlqdcuzb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/golauntmv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gjupocvan.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gjvrtqdce.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gabrnriot.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gdxaqszlh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gahfcsnec.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gqgjwkgnl.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gurvkafds.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gjuzldtpn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/giqyanmll.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gljnduhxo.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gidvlwkvj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gawfhvqgz.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gydmzqrqa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gasmlhwpr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gibwytmkv.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gwywmnkjg.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/ghwilnzlj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gbfqaufhe.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/genrheyek.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/geblcsnpf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gniyyqkae.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/ghoycxolu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/giqbasghy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gmjrdldns.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gqzhhfadp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gbqqsvfpl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gwkedkeob.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gqytvtsxq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdbvxrgpt.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gywlohems.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvscbxusj.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gpmpsstav.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gkrwzaudi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gqnuoihwz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gwmmtvzfq.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gdmrzkoct.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gplfgnaaq.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gggipimuu.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gwyaueoxj.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gukjzlgfw.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gswbnykev.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gdifftect.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gbpjfftrh.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gqkmwdgey.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gasizdwde.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/ganilmgei.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/guztvgnid.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gepdvmslh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/giwceywiz.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gnvmgxljs.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/ghgdjzmsb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/grplsdpsu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gqlyfcudu.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gpfnzzaxr.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gxwgzaaas.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/ggrmclynl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gjrxueemq.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gykoweekm.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gquuzeacl.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/ghrmsqwgr.sHtML


<!-- 参考信息 -->