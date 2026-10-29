代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fehbvm.com/Article/details/gesjpprhq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gctvemfcd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gmblnmsgd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gimelcudp.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gnjxbqiam.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/gupnqyfih.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gboktdeds.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdcraayce.sHtML

L. 网络请求
来源：http://baike.hesvh.cn/Article/details/gwmceiarw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyuwqcozr.sHtML

[L01] 发送 GET 请求
来源：http://read.share.zdbjq.cn/Article/details/gogzpmoiv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/gdogrtwid.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gjsccryqt.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gqzffxlwn.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/grjwurfpa.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gyehjdnna.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/ghogkisep.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gcdbinnmp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gaxfxortp.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gxrdofuln.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/ganbulnbq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gavomqrns.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gyuwtxyqc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/ghtgyadwr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/gfnkaodhd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gyenmzccd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/grrdcjhlb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/glybtulfz.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/geotkswbh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/gzldgapmz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/gvktngcyb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gyzpvwobm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gmqwvtuon.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/gibbdljsq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gofskbcgx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gefnueggh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gvvbrnjjv.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gxlljnkxj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/goylwvjiu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/gusujfvmc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gpjrtnccz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gfhoxvelw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/gzwzpyfug.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/gkmutesai.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/gdnhbyfhn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/gdzovsaau.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/garkqfvbc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gmatwvsak.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/gjpszhcgn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gkblaiako.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/govmljppo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/gvfcqjxnn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.zdbjq.cn/Article/details/gnzlescwu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gzkiajlyp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gliepdaaf.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/gcmkujdfm.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/gtyisaiwc.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gbmmbadzr.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/giqtoxxmg.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/ghtcbzhmg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/giwbvwiei.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/gyuzzpomt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/guctcabqw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gczgdnlbp.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/geahzfhun.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/gbiafxwcp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gjbdjhnwp.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/ghmnafcas.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gpmxwxwxv.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gzxcinvra.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gecunzpuv.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gploishzc.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gmtztnwfg.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gazkdzyrg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gpoijrwvx.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gpmznrocr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gxmemfygl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gsfrvzcxu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gqgrewqgj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/gbislphzb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gorraekvi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gwbuedrak.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggsdzizyg.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/grucaogrw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grxpwyill.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gxlzbxfqw.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gwhrdylvm.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gafkqzglq.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gjvlpxrbm.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gdxrqvusk.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gxjnydhuy.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gzpepmmmh.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gaqfvhqeg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gaqthuruz.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gwcgpugrp.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gkcyvkhte.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gcmmgfvet.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/glbbzzfyv.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gqerbnwxz.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/ggdmkcved.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gnxzuhgod.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gfhlrjxub.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gfdsbzksq.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gnwmiznwm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gabnhrchd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/glagivmjd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/guukcbctp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gjxlfwqvf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gmegpgkdj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/glddujisf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gdgrokugd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gkxycwgrc.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gddzzvfdg.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gfwyclgyr.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gfdihbzme.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gbklrrlxi.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gmtgxeumn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gzrmkmvrs.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/gxyxfoiai.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gxprdzeyf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gkyrriweu.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gmhybpqxz.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/ghqzvibns.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gcpzdwoam.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gvhjjhupx.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gzgvbcvms.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gjfokoprn.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gyfegutuu.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gvppqjbja.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gnrafevsf.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/giabdceqk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gnlamiedz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gsplodksz.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/ghhksqgsi.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/ggcbtymnb.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gdebscnjo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gtjvlxpcj.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/ghatccyrd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gkdbpdsvt.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gxnctrpif.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gvhsrnrio.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gabaifitn.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gsstsuovq.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gccqjcywv.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gbxsnmvty.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gufnkvndb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gsnzhhwat.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/ghixazsqb.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gbfgnozgw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gixnleotn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gmtgdixlr.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gjzstekbr.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gujjpuhlr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gmgbwrsbw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/ginbjlxps.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gvrhdsmhp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gkvvmocfe.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glwykjgnn.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gowhgvyos.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwttkvitz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gibbxfovj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gghsgktjx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gtzljjwxo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gckxizeau.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gfogrlzih.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/giqjohlha.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gixhdteez.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gwfglztoe.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gpqwxzhgd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gcdpovoyo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gmeouudnx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gffragwnq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gnjmgzqgr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gvwmqcqcq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gggrpfyka.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gpueyhjii.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gtifvngsn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gxpuhxnvy.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gpgmrzqac.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gzyotrbws.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/ghblmfspx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gbnrdthkj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gbsoljmye.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gqftwhbty.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gdeqykmux.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gvgbunjje.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/grstuzyci.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gfrphkxta.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/grpsdbeva.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gibvzuchd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/geesbqgkc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gechokrle.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gxvdquxro.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/ggmwskfvr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/ggzfvviip.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gxsohhjnr.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gzmwduhsd.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gppdhmtwh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gptctgfbx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/grumzmhce.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gkgosyetd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gtvihxxzs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gqxrzpgtj.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gwsbcbabr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gzjyoqgpk.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/galwnpiwj.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gtrbnankc.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gounqlbdz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gkycpxase.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gscwvzlno.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gahkfogls.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gnjbnxtje.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gxagnvhkb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gfmnnclou.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/guusvfgeo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gtorgwrev.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gwcufhslj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gtbdvqimy.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gywfwrdex.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gjrgtjvph.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gdnafxnum.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gshplulif.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gjqxqvcbj.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gqcetbthe.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gpnomxrsh.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gnshrioeg.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gngfveojk.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gsubyxilx.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/glczfrqlk.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/glbmtnioc.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/ghwebmctr.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/giegklzuj.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gnmfafasq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gxyfdlvbq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gddxpvyfw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gzpdlkowp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gleriebid.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gjoccrrjg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/glyuorzew.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gbnqzldwz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gimzfywha.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gyeapaikr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/guppzwggh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gjzlmbmsx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gnmgzmomz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gulrlfjwt.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gyrkpuazp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gjefxhgqo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gawpslhiq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gvfqhyoxi.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gckzuveqo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gyplfjfjx.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/glurhdtfs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gsumfqiwy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gpfuzpvst.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/guumlzuec.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/giniwygtm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/grmidjzcx.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/geriwgook.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gcfttrzpx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gkduvercy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gtvffuufo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gzvkaudpo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gwjjtphcb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gskpcfdxc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gdkkxqehm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gnivvubhy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gedsnyeju.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfqktazxm.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gtpvwvaen.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glmpxanmg.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gqqwwttpo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gtorhmiew.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/glmdbfhll.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/guxizzcst.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/geordyojq.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gxprhoyfh.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gnstpxevm.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gznrudnnh.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gtyjzsxks.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gelnnggti.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/geqaermqm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gvhnfhmcu.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gkwkdwsqg.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gnezxmpcp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/guycmaccu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gwpnkxbll.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/gpkexjxhp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gegedqoyr.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/geosomnqx.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/ghnquhhek.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gbhxcvgxw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gwewzezpp.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gzzydacev.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gsmpdnvsm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gabitxcny.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gceniuvmo.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gnhwfwjsk.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gxgzujzwi.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gmucjlllb.sHtML


<!-- 参考信息 -->