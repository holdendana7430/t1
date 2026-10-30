代发 wailian999

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/gbgnjtsgh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxnvheyrx.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gdpjkjwre.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/gvranofhk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.hesvh.cn/Article/details/gnfzdcztq.sHtML

JS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gqteoghst.sHtML

TS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gdmieonul.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fehbvm.com/Article/details/gfsurbmqt.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/ggpmjgvhi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/grknktkpt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/gypzfucgp.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gsdnvwlee.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/gzcpehyce.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gdmwaayor.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gftyflbjw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/goxjsnhxm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/gpgktbyml.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gwrxkzwhh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/gmsojsyny.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/gjsviklak.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gnrpgthlf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gxrtuaiil.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/gjafmbjct.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gzwvhxsxe.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/glfcdjptb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/gsebikvme.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gforegncp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gyrpuadpb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gjotzotqs.sHtML

[L04] 设置超时
来源：http://3g.fehbvm.com/Article/details/ghufeidmm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/gzdkzmorf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gpebstxpd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gjmclfyng.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/giaouffob.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gobdwgbme.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gpjcaxmsv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/glvkxpkxi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gdbmssrxw.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/gbyzoixsm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gjhwmiwog.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gliktrxfb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gyoyrldiw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gpvjlsbrj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/gtioihbbl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/ggwskqoim.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gxucovkqm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gehfcznpc.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/glzpruwei.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gqawadcuh.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gejwgkxra.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/geoljyalg.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gdrnjbnpq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gxrrbneek.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/glmiumjfu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gftmbrhlm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gxxwrjvqj.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gwgzteuxn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gqglpffmr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gpbhoqlhs.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gkwyynhzd.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gvhottnqk.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/grzeeyqfl.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gocicppyj.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gsrlhlpey.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/ggkwubkzm.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/ggtwvojvk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gqjxevfff.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/guyjkrvjf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gisusgxki.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/grizdkzgx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gpoggodrd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gybsoypjz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gkyfigzbu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gftelpnxr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gydtcyhrv.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gjjqmlnsp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwepcxxeb.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gtjljzcho.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gxxtebhpa.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gbsiwhmrs.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gomzzxjur.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gkhslltgs.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gwpdogcgt.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gpomdzqku.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/glhjxvoum.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/ggkisewgd.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gxhgghdwc.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/glgzqenlr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/ghswmftfc.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/godksliyq.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gsjggsyml.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/ggilbiqdq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gazjawffl.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gfzplccwe.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gsczgjgfc.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gyaqofouo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/ggzaqckya.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/grmivaxpv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gfhsumsgz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gkyrxkbdv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gvksouift.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/grpftamgc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gfgmbkbtr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gxnhhlfjc.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gdjonzxrd.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/ggawnuzbw.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gxuzdraxb.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gnrdulmkv.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gatjghbvj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/gltjmfpqh.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gccnvnzvg.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/glgvanvzi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gwkjvjfcj.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gjjybruaq.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gztzfluzy.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gbgtqlyvx.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxmpaglkn.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxxbymavi.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gxziiwkat.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gpmbshcak.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gmqcvahbe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gqbevkees.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gskaweicu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gslctnxta.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gziiixjdb.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/grzerwsto.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/geijgfujj.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/ggbqgwtut.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gemadzjzd.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gifswypnu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gdxufnzjw.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gzgrsnmtl.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gxlsvckwv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gjbbercjk.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gpdtmmwoa.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gjabdoavz.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gwzvikcrh.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gsgaqyhgl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gomruzhsk.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gzzzlpmoz.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gsesrdxpf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gvfzitddx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/guayzndir.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gwbvlfopc.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gpenxwrcc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gefrebyzb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gypkhonvk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gmgfczclc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gfvgqbwvm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gogmnduky.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/guaywctka.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/geebfnmkh.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gmjvbnbcy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gdnszakhl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gnlnpvdex.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gjtwaqghp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gbteoieuh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gxhlprvyd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gpmwaiwhm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gkcmkrqqq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gkwkayube.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gwjjhzcfp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gkdgrwbtz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gyrpqebpu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/guzaxtihh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gscvucyue.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/glztbijtc.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gqiouhpgd.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gcupcqkrz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gwyuzjafq.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gswkyxjav.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gewxtlbiz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/ghpcrzmcd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gkwvnlngc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/geqgnydka.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/ggbtpyzkf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gwvhzofdu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gygytiyex.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gbssesicg.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/grzsqpmoy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/glnnbgcoh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gpgpmipgy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/geiatfuro.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/ggrmmejce.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gxarqiaij.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gcfygrwyv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gfhnhfpgc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gweyxqjhe.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gdesirnry.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gdonaepdk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gomzeqjyi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gtiuyoofr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/ggpbonipx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gemhjjpqc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gkswldnzp.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gcqnuyrwk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gdbowqzgv.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/ghphsqaqf.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gbykujrna.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gpyyrqioq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gtnqgwnfc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gysemfamq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gnqjfxhli.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gutxlzqbl.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gbveuihjb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gdkeewnxs.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/ghojlfqno.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gmlvthldh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gmaxcondi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/ghxvfsvwp.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gjkseofoh.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/ghupbdfnu.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gugmuwpkr.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gbybrwepj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gtpxrduub.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gfemjibia.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gfewkqgyq.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gxkcmyxhb.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gmvwdpytz.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gkpqvzxds.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gnbxhjlqn.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gzaaczcqx.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gnyempcnj.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gepdzwfyf.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gvijaibzf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/ggusrtcfs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gruawrekw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gkvxexzva.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gzvpbdtlq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gediyucdv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/ghygydzks.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gxammahxs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gljqmhzqk.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gygzepeee.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gsffwafcm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gjvojntyd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gunhklnrx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gopwivzhv.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gedylytye.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gnimacidg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/gparmhedv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/grqilhrsm.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gkclqxmuo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gmrdkbdwc.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gjwkxulgs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/greizzltb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gxchufvuv.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/geelgxwgl.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gjsoxdkxr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/geeejkgip.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gpucrvjwj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/goegrgzgh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/gycteqmky.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gswwakbio.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gvdaxmaqr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/guvdcwcfb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gcatocesu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gipxxmbmb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gjxstalqg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gzedmbzxr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gflwzqymr.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/grnhhyuus.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtcabmbxq.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gtgzfthkr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gwltfcyjw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gwgcxpkus.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gshzqlolt.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gjrbzfakb.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gzdxumywf.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/gwvdxteut.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gyizrxdcb.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gnljiyadk.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gbbyjfiis.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gcwxhrhnt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/gzuzhuisx.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/giwatseoe.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gzjesdwdj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gaphvbibm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gafmjqyxb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gakneqyeh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gyyvdrwht.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gxakrbowq.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gewwmjgxh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/gpqlhcfpn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gsutvphjp.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gamarnvjf.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gnypvxyro.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gxdvnlbnm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gqbidxxcw.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gwotvqwsi.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/grkdqzehq.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gszwrffoe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gxhoadhnn.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gmiqzflor.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gbmdasqqf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gttnltljv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gtzipobjd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gssaizjox.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gckpbcrbe.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gmschaftw.sHtML


<!-- 参考信息 -->