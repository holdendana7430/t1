代发 wailian999

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gbkrtifmp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbzylbkms.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/gezykrrau.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/gecxtbmmd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/gswewvibt.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gbxhlseen.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gpssxylmv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/gndtwwsqs.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/gunlcgnrv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.hesvh.cn/Article/details/gdyehvmuw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/gyuvpmajh.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gxxqeitam.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/grzrzydkz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/glommaxbm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gglbtpesg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gwbqjdejn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gpzaqhnan.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gkqbgmuet.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/gnbsvwuaw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/gduplqrip.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fehbvm.com/Article/details/ggbrvlubo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/grenchjxl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/gqcdzrgwp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gphhdmkzi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gcyvugipr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/getvjwibz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gckwwfcac.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/ggvzvxmgm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gpgxmnpcn.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gziszaerd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gxhqpcpwp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gedlykunb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gswmadpxr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/grihshrme.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/giwczakzx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/gvqnadkgh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/gftdrtgmr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/gmlzxxqqo.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/ghhautlgy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/geiutdjqs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/gtripplrv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gimroxnrb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/geuoiodnh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gvqjvqgfk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gbnzezxjs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/glkaeztzn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gwwkxgcbk.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gfzbzgzmj.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gkfeihytx.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gemdtprxv.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gtxwmlely.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gttctkqbq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gvlkucdoi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/ggdooqjee.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gazzavgkr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/gkrnxafzc.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gzdjekucf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/ggkaxmpjq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gtzvnfjwx.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gnotxybka.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gjmrpyccn.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/guomiwpge.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/goblwaroj.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gdsmumtnp.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gvhrvnzfj.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gzbcyipij.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gwcvnajbg.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gssfpkoff.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gnhwafjak.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gccftggdo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gnilohoai.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/grvkaquqc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gsvdfakep.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/glbeceydx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtrqfpapn.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gkaeuqczi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggypfuiju.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gactunxub.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/guktgvbno.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gvceqmfds.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gllwoejsi.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gchfhkekz.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gwjthggtf.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gqphyxxui.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gxosqfmav.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gieythqud.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gadparosh.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/golkeobsi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gfubxnytj.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gcfvgnktk.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gddfwzbcj.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gotrlgujx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gnrlivgxw.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gpklnxblr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/griotxpbv.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/ggiypezbb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gciyddunp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gakiqrujw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gnjpzsinc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gecydcudp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gcxazeecb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gfxaktxzf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/gtdiooees.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/groenwsyt.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gkwkdglea.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gmifhskzv.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gazrmjzak.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gkcaegfcu.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/grjxlfmea.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gbgzipbqw.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gntzvteyl.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/ghxkpsouf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/griqkribf.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/ghgxlnbqk.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gprzdrjsb.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gjlqooczh.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gfdkoaylx.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gjqtugdty.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gkgbkiafl.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gvlptzfqs.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gkpdvhjod.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/guvkwdfwj.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/ginqudxkx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gmsgnmfmy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/ggjyaznwo.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/goccdlkti.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gkifyrlem.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gdnkuefjt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gbvrcxwpr.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gtwdymljl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gasdzfdkc.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/ggjrshcuq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gvpqweayp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/ggspmycdu.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gnvbizzti.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gyiszoupq.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gxovbqdic.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gbiqjgubl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gsvaewtwn.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gakndggtn.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gudwxyjzg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gwqdhdukg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/grtsyyetb.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gulsrbzhb.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gfaqgepia.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gtxzepbzp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gndqjyxcy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/guxgfjstv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/ggskpqzfv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/giqcjqgck.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gbvcvipsq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzbdqfwad.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/ggpcimwmp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gyiqrqzgp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/grmjmjmgs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/ghizuqvmw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/ggzabjbqo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/grwhaefuo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gahccrfef.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gtgecywos.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gggdrdprl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gqthuabmy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gjvqntqep.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gpadiydtg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gujuzicuw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gkelioopy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/glqsbpsrp.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gdvhkmdko.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gxmnmpxzq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gdootepze.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gyrrsydnf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/giprjgxsl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/guhwcaere.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gdzpeaazp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gmgtoaxcl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gtxhurlok.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gsfvialtb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gczdxlhym.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gruvloyuo.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gbavbwhyk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gkbtozozb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/goujwwzxj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gwkocucwu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/ghslzkjyp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdinluvlw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gtojuyfhg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/grephyzac.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gopowjowm.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/ghuxzmtit.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/ggwrarudm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/guoputvvl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gjnowrjqe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gltaycxpa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gceazxcus.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gmiwilhdm.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gadazxuom.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gsetffxoc.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gxqnbnyua.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/grrmeivue.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gastybowh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gjfmxnkrt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gbvefwese.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gqebdikzh.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gooytoqoq.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gxlzkzjdy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gopmjysvx.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gvskhvpvc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gealjpyya.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gpesoatbo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/guxiixwak.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gzqkdkbbx.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/glfyiaaow.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/grfeqzhzl.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gtztorohn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gtkozsnwm.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gxfxmbvks.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gnonjbebc.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/ghmtuhckh.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gjgkkwely.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gyzjgnpxd.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/ggcgpbfrn.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/girxbbusz.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gyajfwigz.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gwebkcdvn.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gxdjucqhd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gskzggsmn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gznfzsyfq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gontayrfo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gwiqiqxrx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gytddkbfb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gfbfpmmcm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gftpyckmk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gtiotavla.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gbqdwpzvp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gukbcwmsw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/ghmjokkvp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gtdzsvrlw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gyvptutcx.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/gllcikeax.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gjvpnxfds.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/ggbfksojc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gzndswewv.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gvisvtdfs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/ggkmqwbiz.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/glqnuupfl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gmgxuaccf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gchjjnxwk.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gqufmguin.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gpcakawku.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/ghkhhrrnx.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gguqxbnox.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gtkvzjnuw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gdzhouaeo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gijrvkryk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/ggpdhcqei.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gybfzaxve.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gaimhvdlx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gygigzvau.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gishinaqo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gvuufmgzf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmpgnwfmb.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gfkqvfeqw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzrqyryoi.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gqfqhfpdc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gwsbvczvl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gwgnxkvnb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gaufdmmdu.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gfzxvrccj.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gablmzssc.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/geevcqiyw.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/ghxnpilpt.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gjpkhbzju.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gkczozgfu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gghvdbewc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gqfvumqnp.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gybsbncya.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gmggspnxg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gwnrgxzvs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gjzbfqpcv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gjtfjbfdb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gxrfceywo.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gsoelqgrf.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gkkmjwmvg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gogdlwmcm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gyhcbpicd.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gbbyzqkjn.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/ghjhmwyep.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gcuqltdfa.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gszhmejqi.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gibjvksts.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/goviiwykc.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gmznwjaur.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gojrpocec.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gghbuynat.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gbanxebqe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gjcxmzple.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gdntlrucb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gevfyidpv.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gbnqyfnnw.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gtmigjvac.sHtML


<!-- 参考信息 -->