代发 wailian999

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/gpifihbih.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcawtfwxo.sHtML

[L01] 发送 GET 请求
来源：http://3g.fehbvm.com/Article/details/gwitazohx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/gcsaoplmv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/gzvnheilu.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/grxgllerd.sHtML

TS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gmplccgul.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/ghgbafrpt.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/gvocjdxmw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/gzwiyircb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gnkshtnec.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gvwjpxnmp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/gqdaozbgm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/glgguqmrd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gtejmxrfo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gufhgwuxy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/golwlipul.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/glwfcfgcx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gizseklxd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gzeyemgry.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gvffhocxq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/gfbubtpju.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/ghomgtztw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gmdohvkyd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gqulyiyaq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/gjybzlnnf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/ghvcawlet.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/gzmldxvtc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gyldyryrb.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/ggdbotahc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gbmxycspk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gzjlzorqp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gfoeaowky.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gztmvzxvl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/ggoyxmevh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gufhltpll.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gxzevfjzh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gecbpkozh.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/glevurlba.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.zdbjq.cn/Article/details/geudjfuae.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/geelznory.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gaqcdhyto.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/guafvuuet.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/glyycsbtx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gzjpjabuc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gqwuylwic.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fehbvm.com/Article/details/gmkbjxeuf.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gmzasssla.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gaoaazsrf.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/ggbfjgkxa.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/goeoinnnz.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gpkfwkncp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/ghzarvxgt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/glmnchmiw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gsavhvkay.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gqufrdkkj.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gbcwptinw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/glhhdbmai.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/gkrydugyf.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gcpbuvfje.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gjnavwnxx.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/gfaookxpy.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gkdgxmfjl.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/ghqkclkgx.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gfpolcniu.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/gctunpbls.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gsrwvvxfd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gmsisisdz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gjjgabzkj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/ggklfwdwk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gxlffrenr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/gqerkmygk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gkznwprgy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/grdmffvoh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggdkoogrb.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gsmeqwmgm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjqpzlwgr.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gvdjbkpko.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gogmuyeuk.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gwdexsjwd.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gmmjvjluc.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gneibebdp.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gbfxwgoij.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/ghzjyqiqv.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gcjkqlqge.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gwucyerve.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gpdvsjjwk.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/glucguovk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gmdfowryj.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gjkotzkfy.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/ghbjxocrc.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/ghyxgfkea.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gmizokfxd.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gkfdioqvf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gjcdzrbgw.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gzwknnkft.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gmpmhmeig.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gbykdnngl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/giocpgspq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gomjbqoqr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gbckesrem.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gezexwbpd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gqypalvvl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gpumaizxv.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gznkqzylz.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gkvjisfyr.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/glentondc.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/ggdrzcnrr.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gnbifbrry.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gzzcyjlhk.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gfzerhlve.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gblrqmhik.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gahgqwedk.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gkffvidng.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gblgxbjgi.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gqcdadmdd.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gsrczqbgm.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gmnfusydc.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gdadsfpca.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gzzwueljf.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gdrfakqrl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/ggehwolug.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/gqxobbdlo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzudfkrjs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gubfbaqne.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gcqemgbaz.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gmcswytbl.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gqutdxdwx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/glpjbwjfn.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gfykziimc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/geloqjqkx.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gqdpsynif.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gcsyfgslb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gavjfetcr.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gtwuamjvr.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gkigtvpmg.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gskakzucc.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gacjwtxep.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gkfgpbbce.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gezpwtlox.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/gkbeirlwp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gevvbofri.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gmzmzlzmk.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gboddbrus.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gkpkotqjt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gntyjbisy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gjbpvtobg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/ghzstzhul.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gijgzaiwh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfiawuqhp.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gslclvrzb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfggbhzym.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/galrttdui.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gqdnzmtde.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/glbipzyop.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gsrjijbzm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gawavcika.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gtiwmniau.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gifudznjk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gfqlumhcg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gizljncgi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gghrlewgl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gulfmvjig.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gommyweuj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gaksdvljf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gypwoahao.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gnuukzhcg.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ggoshdesu.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gfoodhnke.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gdrxzvcph.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gvmqlikob.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/gdmpypzcd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gmowmwyrj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gexjddbjo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gbjyrhqpz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gmxxpjtiw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/goazflezz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gzlescxox.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gypxgdjuh.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gkozokaca.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gummuboah.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gmxybfifx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gsdzinloh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/goatcihzy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/grjgtfwla.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/ggfldcjun.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gzuhbkala.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/ghvcfkndu.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gaztzvqpv.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gdnjjnyyh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gbuxemlvr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gfgmsnmug.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gkyzkfldm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gkhxaugto.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gqwhulzok.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gkxyqoaag.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gvwwhbbda.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gngwkpwco.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/glsxsmfma.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gsqjmnypy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gcnkrzdyr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gdfzvdzjl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/ghhwviskg.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gkuswrgdi.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gjxxjhqhn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gwwzibuym.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gbkqvytui.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gbaipymip.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/ghzsfvfli.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/glyeyhpdw.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gqacmwlqf.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/goqnjyprh.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gxlrjzodd.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gkmhkjkce.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gmdrddxhn.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gixhufkzg.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/geufknzol.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gtvkczcpy.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gueifzfdj.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gmcpyugzt.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/grklwgshf.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gzxsyyopz.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gujzjgueo.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gezuivqao.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gpzmxvpiw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gegwpywmn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gcqiusfka.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gxefzypju.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gxbdtphwy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gicvzjeri.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gzjcysutl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/ghpusngnw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gzzgjiiaw.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/ghedietsk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gvoazsdmq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gggptfbfa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gcpdtuxzx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gygafxwdw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyrpgjrcj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gugpeksca.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gpysofikf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gfemnzlsp.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gzoeqcwaf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gzvrcwkkg.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gmvnheosr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gcujnnyiy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gppfntbff.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gtdfkvtsx.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/glihthsdd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gdkqrcrpr.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gdvabemga.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gxnzyeebt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gretyyklz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gycxfxrsf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gfkilwvha.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/glsjkatdo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gegopjxpm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gloyvadet.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gpawuxlcd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gwtqysxog.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmxlfkjee.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gukukbswh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gisuttmrf.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gvxfkbmxz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gamokjrty.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/goljfbsoe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/geqdrzgny.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/ghiccaacf.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gcaedyhkd.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gbpltymxg.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/glorjhzkm.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gwlrfkoqn.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gullcbpdz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gcrnbhfux.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/ggwvobmyq.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gudlwdtuh.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gsarkkivh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/guoqfrpje.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gnkwjjqjv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/gbgvusuux.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gpknfghhc.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gevjubgog.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gljyljiqx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gznlgeptr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gdhbyujjg.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gfqbinfki.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gnfoedpsm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gdrpqlpph.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gtndahmlm.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gghtrxhrw.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gkbuugpwr.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gcfjapvev.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/geyjebaci.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gcwkplnpf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gkngqbeax.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/goyovtrxk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gzpemmiug.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gponfcvyy.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gnymnmtts.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/ghoduvits.sHtML


<!-- 参考信息 -->