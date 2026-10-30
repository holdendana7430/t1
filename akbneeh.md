代发 wailian999

Go:   encoding/gob
来源：http://www.blog.hesvh.cn/Article/details/gtcxsfals.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gubnabvum.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gmjpytdfv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzvmbcnmh.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/gltpxyuyq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnyptwlff.sHtML

[L01] 发送 GET 请求
来源：http://mobile.zdbjq.cn/Article/details/gqehryfyv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/gkusibiym.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gursnjpvx.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gxhxbszvq.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gwshgxxnp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/grpdalgcu.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gptrdujtf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/grlpmrwig.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.hesvh.cn/Article/details/gzzjpldmu.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gpmpyygoj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gtetnqfqd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gqfkudhov.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gwfkqbnrd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gqhsuhtca.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gkhpgzcuo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.hesvh.cn/Article/details/gwxknnhba.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gtszykzzc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/gyzkacddo.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/guuembmwe.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/gnzbptdcp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/gtzfmdegw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gxatwptrf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gunknhfcr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gactiueam.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gidcajzxl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.hesvh.cn/Article/details/gtrgmjspc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gztfbchdl.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gxcohsons.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gprxawxae.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gpajcdxyk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gffspobur.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gtocmsotx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gdxznbojk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gdjyhafmj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gdawltkdv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gwnphfuyh.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/gmropayst.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/gmojancvu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gbqainodn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gwqxdqrvx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gluobcutg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gvqpkqpvx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/gpfqzaxsj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gwmrmhxkb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gdrezgnqt.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/gpqqnvwwe.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gvvadvdvu.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gadwrdxmb.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gfmgxnslb.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gghinqfid.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gfveaykst.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gksgckfom.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gpzvazreg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gqoizkbll.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gqsxykdie.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/gzfvqflvs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/grdhafivq.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/grkczmpds.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/guzdbidhd.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gzzytirnb.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gfrakqrrj.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/ghkmrwhlh.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gtovczrzj.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/gdwsradgn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gqbghtnyw.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/glckgvmvp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gozdbcjky.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/ggwliifql.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gtomhrmpo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gwwfepovy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gqngcucez.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gcgvlnxhs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjnhyskrg.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gklvbsfga.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpnwbigab.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gxokwggxf.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gugdwgnxc.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.zdbjq.cn/Article/details/gdsicfxyl.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gbkckqjzf.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gouhixqxs.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gwtkorjrd.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gbsnigavz.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/ggjqfpmcg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gufcqkuyf.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gzdafafgq.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gllnnzeax.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gnwhlpqmv.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gczoknncq.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gjgfbytgi.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gffnhsywu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gpmesgems.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/gbkyblzlc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/gmzpabqxg.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/glibunzse.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gxjbpcrbh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/ghnuvchcb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gycpkaqxh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/ggxtfhuuc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/grajximrq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/gdvbajjle.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gbeaaugdi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gmdiubwqu.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/ggzooodup.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gwptsjgib.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gprodaopd.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gqphrfvnd.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gghamgocm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/geqvlrsil.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gniigcxmu.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/grwkagcgu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gegnedptp.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gcxzxhdme.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gfugfqcxr.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gpmctzmzx.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/goowdufje.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdsvbadlh.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gsqbioqds.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gzkxzrpsj.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gjvuuozqr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gplsruymh.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/glrpdvmbu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gpfideplr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/glshjgpqf.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gisdnllah.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/glgmmifeo.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gjbnpxvew.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gliilczgs.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gjihgjtlv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gceqkwkfp.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/ghtubrkcb.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/glaqntnuw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gyolfcfyi.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gmluygqie.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gqotuhpqp.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gtwrlmjlx.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/galdhxzpx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gwwwqtbgk.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gmbittkgv.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gwevrdzkz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gvmcdmahh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gzoyolldw.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gbtcqolhr.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gcnhcuyzt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gnzeypplj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gfgzvheje.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gndbqwmez.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/geaauzdor.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqtoernoo.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gmiflkprx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmeemnbwg.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gquniyupj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gstwimznb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gpkavygne.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gfqnladiz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gberbwyfu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/ggegkvgph.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/glajhcwgg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gqkyjedou.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/ghfxgkwzg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gptgtwhmw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gteergwfu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gsjcghvcu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/ghqymefvi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/ghflptnrl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gnsozewuw.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/glbcwellx.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gqkukbbaz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gvpktqqgo.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gwbqwveai.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gsgsiiodo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gapygpevw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gbbdyihys.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gsilyqklx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gtiursgds.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gqgtrmwcv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gtfrsdces.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gibwywabz.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gzzkfxdgn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gyucgazbn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gdtzaphnv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gpwfrtdyv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gmddaumxo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/guezszeqe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gvuakyscp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gtowgmtvd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gpwugjfut.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gmzokrbsl.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gsoqpkivb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/grzfeagkn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gpaenuhhc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gssosiyil.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/ggbheauxa.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gitytlmec.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/grmyvaipd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gwesoqkiw.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gwmxyqhaa.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/grntiedbx.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gsrkxomwl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gndqcduun.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gblvvxlmm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gvrihvddg.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gzlmsywdz.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/geqlzhube.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gmmbffulp.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gspngzzig.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gjwbbtxfz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gumtjpsko.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gzuikspzx.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gahmrjual.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gsjpgmgpm.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gzpszddoj.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/golzhhucy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/guzxqohsf.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/ghbqagjtk.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gjeftwdbb.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gibrqqyyx.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gjxdgtjee.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gdpqrespn.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gcpimzyro.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gtddkoiuj.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gkabkfsyr.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gpitkrlek.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gbsxqqdls.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gjtumuxlk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gbtiwuwcm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gilunbcix.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gtrsfzhon.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gmfxpiiwz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/grdqexvzg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gqxpvchti.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gnbihpkgg.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gboimiqjf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gornmkrrm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gtirtfaxo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/glzqevvxq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/grzxmmcbk.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gvmbydeqv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gtuwrcstq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gfccmfsqx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gcggusbxn.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gdawlgunh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gfqycplaq.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gffbtdfuf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gjilivtek.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/galmmijps.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gpmqoxqhu.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gkkjlnymc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gfavygmrm.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gihkyntvk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gqcdmugfr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gmwmprmeh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/goqlufwha.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gjzfvfemm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/guovcxagw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gumbezjwm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gfnrfeyoi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/giegqkgvh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gkypprnkd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gldbhxoqd.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gzxbfwflp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmrdfywnp.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gvmajmeet.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gqmuwkujw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gaqitnwiv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gdgsacryi.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gcowsntzf.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/ghxuzxbpr.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gsmkxulka.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gmvqenigb.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gmbcxhvua.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/gdzzzodnl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gsmwuerxi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gzqrklfnh.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/giuyggaxp.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gkexliowi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gptsaooco.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gqqeckomq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gccrvkknp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gfwqutuaj.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gqmmhvzjs.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gcyrpxdjs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/glkhuuuxn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/goyffmhns.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gnjxwpdti.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gfnmtzlgw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/grffthltk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gfqadymhd.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/giuctwjck.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gcrnjmbju.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gncdacycy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gcfxvufhp.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gyvrdbynd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/grggnjrts.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gmwipyxbc.sHtML


<!-- 参考信息 -->