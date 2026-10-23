代发 wailian999

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3hgmtbpoe.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3plzgwxyo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3wtauofuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ymodmuvg.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3gjrwrvyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbknaeyk.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3afdbogma.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3rhfjoyry.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3ecaspies.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3apwcbqhq.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3perzjayr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3bgehkdws.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3qhklszny.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3rofxmjob.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3oguocino.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3hzywaqwt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3tclbmvdg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3zvtxrcal.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3vgrfykqq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3jaggmjvt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3menbpoov.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3bphevhda.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3buezvngg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dwoefmmz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3czcxlgvs.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3qhaplwdr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ziltusmf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3wiorupqj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3xbfpdkwx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3keygjamn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ftabzkng.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3oxscaqgu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3zggahdni.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ucidrxkh.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3gdcdyphd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3zequnjny.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3lnjtidfn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3agxbnoht.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3slaaofaa.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3sxxlllnd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3huioliiy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ipecdgyb.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3vgnwhruz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3axesgwog.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3xxtdobvx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xguhzzbi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3xbjmgqgz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3tctwvjaq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3clftmoop.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3sgdkvqwg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hfzdwitz.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3npfvwlrh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ysyvlmes.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xasttjka.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xkczscuh.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ftpmfngg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3gldhfkxj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3dfektjex.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3gdhktvwp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3gsjoiibo.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3cschdadx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3hrddhxxi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3lrjoltfh.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3jtmcqlcl.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xiypbjdc.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ucobpvpf.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3jakqhvzl.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3cpmuuawv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3vnlpqffu.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3qsuwmsgr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3uadncrmp.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3zxlmkxjd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ezpjtgdt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wukpifah.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3uumkgibi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3gvhsrerj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3vsgfevzq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3zlrfujan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3onvmgllf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3nwlufjwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eeqcdutm.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ymyulinz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3aaylygix.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3djfmicvv.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3lvtrchbo.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3nfphdojv.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3bwwazgjr.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tcqyegve.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3iyghkppe.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hacztqlx.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ndburzur.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3retakhoz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3llwxksyh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3cwudwtbk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3bdxpxaeh.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lfitnges.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3glepiqsu.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3bghhvrol.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pmvbubmm.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3bmoxkhao.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xwnlzxdl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3gfphfvkq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ihrsiojb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3drcktnoh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ioyizluw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3zeiqjtsf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3nfvvifju.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3hsrbqthf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3rdkvheli.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wravhfkg.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3xndbkkab.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ldpvnznj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3gxuzcqxj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3szdctktk.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3uvzmoizc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3whgzadfp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3qymshogn.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3mwnccplk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sahvwhgz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3fzcjknho.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gaxpfdbl.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vtgfgomx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kfkawwuo.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3azbdncwc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3tapolwje.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3zqfifbys.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3vaajjccy.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3vmcqtnlh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3nnrxpzsm.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3deetadpk.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vhnbwseo.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3hfmkzbwp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3qbdxglwt.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3yjrxtkhd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ecamnvka.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3uufifibi.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3hqlnqifr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3cbeoikub.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gssyhmxd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wevdjddz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3gmiylasv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3nrkhdgei.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3wpfdijbd.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3oqbfytil.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3wxrnrhnt.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3aivfvtcv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3mmvxhjah.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zxoipdca.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zivwwnpv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3jkyimndg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3auivpzuq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3kylfgwur.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3bysbhyfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cfwujxan.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3jwstxvlf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jimzdpwd.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qdbszzhr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kapnqtnf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3agucfdrb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bssbswof.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nszrpmyq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3adqwoyds.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3krqjufft.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3vjlehbhd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tscashys.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3fywnxyuh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rqcrjdgy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3lurmioeh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qhrfqban.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nzflucob.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3pqmgtdvh.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3uvaycrqd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3flvvvevr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3vicustyn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3nseuqrol.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3pxbdrdvu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3nmzdewog.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jwfntstz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3nlhmcqev.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3zypmnauy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3stbsmnip.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3pzxakhgo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3piumkgeh.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3qihoyoto.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3zbagzqrk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ejqpvjfk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3njolffol.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wzdmnabb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jvlfcaef.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3kitgsdgh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3afytewqw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yktoufqj.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3sdrhtdhn.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ecuhfkre.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3squfuskk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqdhxfln.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhvmacrs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ptqxxgfv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3jrjkdpvj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ojhbhzee.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3nijkdxsj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3difflrko.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3kyrddvqd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3guksyivz.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3imvrqzfu.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3linpawrc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3qxgpsjty.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3hjsjrxkz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xqoqbjtt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3zlagbrgd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3kfskhebk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3bwpiwtdz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3jajztbnp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3qgkhjhno.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3scubzheb.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3lafslqyf.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3fzmjdihw.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3zyewcqnc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3vohhcwpm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3usmuxyte.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3wrwhnphx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3dwtwsfpu.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zupvvapx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3weksvmdk.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ocmtvclq.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nkypdijj.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3wptmnwaw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nbaseuef.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ewnegzpr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3yupqdgdd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wzoqnrcf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3melwlerq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3xjshnlcx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3yioujuxn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3orolhpvt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3krxcvaxz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3jtaogkus.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3xvlkqnpt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3zosqrnmq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3iigrgzsa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3luncjjxr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3cgkfejhe.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysgockns.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ntibuoyo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3fhtqhoul.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3nbcsgdsd.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ipjjntuq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3iyxrutdg.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3sktdaddt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3zltyvaix.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3hmcqebju.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3flygazpn.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fhofvhaz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3uvmytiik.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ysvqltbd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3fcankbdo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3fefcjjvd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ruzllqzd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ahyjyklu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ffxguwqd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3gebgjxll.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3wjqklyba.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3czlnmbrk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3cfbmkxrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bfheyswb.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3bhnahfts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ovylinat.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3pviezvws.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3emxqawoa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3zhrtfxuu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3drrahvlc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vpssawnv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qtsighal.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3uqndvfnc.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ypnugauu.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3kpimlxxm.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3siyjlogp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3frzunogf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3xwsutezt.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3xucrwbtn.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3afkgwcmc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3woyroaic.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3yxojiffk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3vlqlbwxn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3sgkhazjx.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3fqctwffz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3sluxxqqu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3wkhpsxjh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3rswqepip.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mjfvdubr.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zasloqks.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3dstbogdf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3cztqadyh.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3hwwuczjv.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3gezymkcc.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3spxlxqih.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3eaxyqawt.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3waavihub.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zuvnfrdv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ptcexjrd.html


<!-- 参考信息 -->