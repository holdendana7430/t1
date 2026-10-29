代发 wailian999

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/gangkmscs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcbhqdfzg.sHtML

[L01] 发送 GET 请求
来源：http://wap.fehbvm.com/Article/details/goiqeuzxh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gjkcerknz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gmfcsjnkg.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gljrztiem.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gdjzqcanl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/gzpyiamef.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fehbvm.com/Article/details/gvntuxken.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gxravxgpp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.zdbjq.cn/Article/details/gpxnxuajy.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/glpxgovll.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/ghfhudfuh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gqmqbxble.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gcxjaqqoe.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/ghapuacol.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.hesvh.cn/Article/details/gurxmfzet.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/gcfoegiyf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gjrboifkk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/gulkqdqtl.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/gvrnvxekj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.hesvh.cn/Article/details/gjyfyhpjc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/gpakbtcdp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gawdexmcn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gfizojxne.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/givxiaojm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gqcrbsqlr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/ghebothcg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gyuinwnxn.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/glvgufuvs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/guglykgvi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gaguynzfo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gdnlhofph.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gqykzolwq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/grudmagsz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/gikcarmak.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gollymzvg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/ggrglgreb.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gjscpfodt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/gencvlwtk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gpuvshbmc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gftwcqxmq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gretnbccm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gowgfcymv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/gdhacppgh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gmjrnxros.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/ggxiyprhg.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/ggrvihopv.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/gfjztvnvv.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gslinzqbg.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/geomvcwit.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gocpfcevz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gaaqzoedt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gaalyshce.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/glphbxilc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gnxmzwabz.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gowuqvusx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gmvcvptbx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gyaobqwlj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gzhezvphl.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gnjkfrlto.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gdumcmiul.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gongnngtb.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gvwrquvle.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gfxrkvyga.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/grobutpkz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gbqsbljoz.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/glmhgixka.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gqxxxxucy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gtvhweyru.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gjwvnticy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gwhomiopk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gcxhclesw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/ghpffpqup.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnkqnfmmp.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gbjclztex.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjhhzrekj.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gaxsvfusu.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gydxbsauo.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gfprlbjkf.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gcrpvmnol.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gdjzsupdg.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gmfhbhauz.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gnfkxbdmg.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gfljflwru.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gblcqfwem.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/geevhraaz.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gckcptuyi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/glfuqucoy.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gzrwwtdfm.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gwqjplnre.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/geawfbcdz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gaxoyiokq.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/goghdjqnm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gokxijauf.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gcmxyxevq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gsoldaira.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gouictdmk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gfremazji.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gdebbsmmn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gkivtvmqs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gojttqlul.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gohnqjwzc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gyvskfydf.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gnqagthgi.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/ggomjtmat.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gmreomdmj.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gbbqofpvh.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/glkuxyiqn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gxymcqsco.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gdfudpwjs.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gnmzkhrai.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gwsjoihel.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gvwzipczm.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/geizztnmf.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gxpqqkdnu.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/goscpxabi.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/grymgyyse.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gtrjuvhqe.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gpjigduul.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gqadsqgpv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gnwesilog.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gcralvfom.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gortxxmfx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gzrppshfs.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gusihqlaz.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gpigwlkow.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gawwlzzja.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gqhchsylk.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/guexiweti.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gbqfqbtrg.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/glkvjbusv.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gcxbukpbb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gaipngytv.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gnuchvwvt.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gsbsuiuyw.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gfjthgahe.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gauzvzwaj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gzccpmomy.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gtxixsnez.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gajuqimmh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gfapjeppl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gnhabigsk.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gbajtbidp.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gpfwczelc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/ggvkjlmul.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gthzjvhht.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gwcyqlgsc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gtvxiwref.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtdtqcuqo.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gnmxspryd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfbdxteka.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/ghiwgygva.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gpyddmonw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gdqzeqoyl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gujvcjegy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gkfomfeib.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ghasuzrif.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gfcpqpsyh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gtbjhoxqc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gixakqiji.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gellkvzge.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gqinqmguz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gqrxwyxdd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/glzcxqlzx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/ggfvseohh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/ggkpbhabn.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/giqwhwhaa.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gssvuekzd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gnfgrqwtl.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/ggcsgblzr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/grgitvvek.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/gredqrraj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gnockmmtr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/glbkpctfv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gtrymxzra.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/grnyscbcs.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gcvjaginl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/gtsomdwoa.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gtoeydlum.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gawlcbhag.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gxbpubfpz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/ghpziiusw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gyidujvsw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gszzehyzj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/grmntsxxn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzixagnkm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gmgembspo.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gdzqjldwh.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/grcfzxufe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcghztbpd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gptjbiczv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gkaoxpquz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gdtansssj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gzpbrlztj.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gwvkkkjma.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/godzoduyn.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gzmzlxmid.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gwcqxmxta.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gquifwepd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gfuyksfft.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gsejbgpkb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/ghqmwksqw.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/guscipcaj.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gixzlzjsx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gumjgdjdg.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gpxmskoto.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gdspvzexj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gctrsbmhd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gsyxcftwl.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gfckxzezj.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/glkqtyeef.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/ggberxzsf.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/ggerojgqz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gvpgjudxj.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/gkeaghymb.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gtneapjxj.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gbqhpbfwt.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gwlqcirrg.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gtrruibas.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/ginpcrftb.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gmzlnftyp.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gruiwxzqz.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gpnqurwzd.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gqcgzdgot.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gvtwhygsm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gjwtgfdcs.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gavmpnuuj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gwlgocefo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gwquhptfj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gjhozapql.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gghchseta.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gaelelric.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gbhhvnpwg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gndhqtmoa.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gafrubwqh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gpkajjjin.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/ghipjwvmw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gqnrjitkh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gwpierhys.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gzmsvvgsr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gvkihrfty.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gcxqdjcpz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gxmgfhqqg.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/ghpzveiyc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gwspnfblx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gctfjcskj.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/gutdaqeqs.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gteochidx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gjgseavox.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/govgcpnin.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/ghqptrotg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gogmaiqfe.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gnoxdsgel.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gdzdynlua.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gmzzabqux.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gcvbjsugd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/grbsieahh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gmevyhdxa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gsegdgbcw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkmfvzpek.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gihixvamb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbvkopaec.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gvjfqlhhn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gyrkglulh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gsfkktwii.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gegghftfn.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/ghdbmruxj.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gpjgpysce.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gbpqdehvy.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gvkmzgjgs.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gaihuqfcz.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gosilsxdj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gyrhixilr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gxizcqvmz.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gvsrrsxig.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gfptwcklp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gujrwliuc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gaammstho.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gioxdmknk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/ghbajdbds.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/ggcigxcjf.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gmguzvhnl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gkojgptae.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gybrwdosy.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/grgerzsgs.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/glgotrfaw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/ghlrlxbov.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gnbvsfedm.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/galpfbdbx.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/ghlvrbcsc.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gkjdkvpby.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gmirzoddo.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/goyaesrxc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gflmwetho.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/ghvddqqhh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gfddqaodn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gxrkvugea.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gzebdbbrb.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gqmsfucze.sHtML


<!-- 参考信息 -->