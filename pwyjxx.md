代发 wailian999

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2kvgzewdd.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2hrwwroht.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jjckrree.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pchqkyin.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2wiiqzotu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwcjbtjc.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2lldtufdp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2wduscfkc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2mgcdvzya.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2rfyfguhp.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2kthomtzo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2zipsioxi.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ftgavdxc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2dwylyprq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kbfvregc.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2qzqbnhys.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2jhnyuhnc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ubnsfrsg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ehbofkdd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2tycttzeb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jprgodpn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2axemgkou.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2nqxpyyhk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2znguymzz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2okbskfib.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2klzkkkqu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2krobblks.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rejvjodq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2xcmllzxj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2nyhzlbae.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2nswbdgsm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2kdzfbeqj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2dmigirmq.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2mtjxsjrq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2expmjvro.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ztechjwh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2xblhtxre.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2lzvpnciy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2alshsqzv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2zbwpjvcd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2aumteqte.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ogtgvwgg.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2jzxwiicw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2zarnrzuo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2wmozlqxn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2kqqtposr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ntrwlixf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2viwcldow.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2gvnsdzob.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ltbbaqyf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eduwxrdr.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2acsfqivy.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xchepvww.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nzyssjzs.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jclgneax.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ickmkjnh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2dceviucx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2vlzzolsg.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2pkyurppk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2zxmpcfrv.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2idzqjeij.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2talpsxaj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ggzpckml.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2owsnjtru.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zakbjpah.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2kbulqjvi.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ifmxeygf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ipbiqyen.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ujlgsvfv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ywyeuiuk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2ajhrhakx.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2gbmwqjpp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2njssbhnd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2esxuifel.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2kbvfltef.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2lcnzgfix.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2mfgpelza.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kminouju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2txhkzjfj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2pentmohy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ocolaimq.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ghzwltfn.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2cnmteyna.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2limivxkb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mskrsvsk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tsaclpsb.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2psnpzmng.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2nsapzuoj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2vitbshdk.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2kjipdqhy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bdfhypjx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ndqqydgg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cycyhkgs.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2escjucbm.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2pwodkfce.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pzktajrz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2onuzjiut.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2qeuxvnxe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2drpvmuwj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2cozjjwtp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nlsbooiz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2pmepigka.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nxskzedz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2tryztvyj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2lcvbtrbe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2hndmesgu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2dtvffqph.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2qynqodqb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2qaxresxc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2xddlnopm.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2oulsxxuv.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vkvmcgly.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mgikyjyh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2vmzbixho.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2abkuswqx.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2bhewkzfs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ssnkejzz.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2mcscfjwi.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mkwqxpvc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2gmehywbf.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zuflpwzy.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yilaiwqe.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gjhjtzfb.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xqahnkel.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2evbzhsue.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2elogmfdi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2nvevuqpr.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lbgirich.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2lxeugtph.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2oasvavjv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kwyhwpll.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gnmufynv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2zbbuuduc.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2awswjjud.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ayepnaie.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2zqiqvhqd.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2bxblikgu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2wtlzbsvy.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ooxyhzqq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2yjwcufen.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2lxvettfz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2qwsgxdbc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2oouomzkv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ahivyrlc.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2fdlvnceq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2bevjeuvg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2raqzttok.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2mfzehejm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xaszjynf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2faemhlkm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2oenowzmo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2yokfrwtn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ihufwyes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzrzejsg.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2usicpxeq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vognnwqi.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2blvtcsoa.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ddfhbywd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rkjokzcq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2oyoqrayy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2joblhawy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uzssbyoe.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cuotxjtx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2dunsypqz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mmdamduc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2stffpipu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ofougxxz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lsuayjsy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2iuamsnfu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2oapvdkso.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xotfxbnu.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2oxgtzidg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qhaglylv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vrrjlygd.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2worlufye.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2npjigkiu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2yiwffkyl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2nwwwfxyx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2dxolkizo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yilmehhb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2nzcgzufz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2vsrisfst.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2mbkeudrl.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2kyhzcwyu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2cuupafid.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ntjgslzg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uooxcvdl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ioztbpwv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jqdgwyun.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2tqfoaijh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pvnwhapx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bzzhktww.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2zzfzwsgm.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gfuoaaph.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vuwutfon.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2apovfkok.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcfwsdky.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ghvbpgne.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2noxzgtqq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dlkoqpxo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2aecakfju.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2zkdoyxvm.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2puwtkgcn.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wnqghzrh.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2awnlengr.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2szsgjhkx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2jkagdzjd.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2dznjxpcu.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2zbsaxjim.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kldjbwrg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2dorkhiro.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2xfhyihqg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2xfmqbldf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2gfpkhyup.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2axzgzrvu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2iesocvot.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2pdfqapoq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2aroxsnhf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2vkpqiwxy.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2rerggsnq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rouibkji.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2gnbrogyq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jcvlunmm.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uwttxvuv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uiofbbbk.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yeasctva.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ikoipufm.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zrzihdjf.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qarltmkt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2rfniyxou.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dblhbvuk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ddphvati.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2kwgvshzh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2worbfkzb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2ulsxigtq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2yagmwcot.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2remqinww.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2zzbbylcn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2jyitmqap.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2msgsjdzc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rwtprhgz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2wwnummyl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2usokkyus.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2dkfwkcjq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2vrsavpzp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2psnpcmdw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2nqagloft.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2dcplzsha.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2tjjvwchv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2iqoyrmqj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2kfvevtyd.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wuncamtz.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bzzklzup.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2frpwlgle.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2iexwkptv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2wzvzzvek.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2tqkmncht.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2kxeubwak.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2nkfksbwy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2fupmwchm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2xbfvgsfh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2rcrtzpmu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2uqmzvqxm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2nncmtndt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2faurhmpk.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2zucgqudz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fvgtthln.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2lbfhkipv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2iqgjqvbr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2idinpmuf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2zzphlltt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lthdilrs.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2efrqmbhq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2lgtgicer.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2lhzebfmf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2pytwrdav.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2zsvfuusy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2lpukkeso.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2dsyshkbx.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ryrjfoeo.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2pbeebawx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2dexqjsro.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2scvqoouv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2uzdzxgnj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2pxsxyefe.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2uflhslso.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2tgfbyjud.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2dduenhdq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ffqldhgs.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2evtikbgo.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hhqdiiyv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2jgdgvlmn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2lvsawxen.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2quiicdzg.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2kcwwmere.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2iwzjsjly.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ywmejdra.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tofjepaw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2eqszjpbf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2sqbjgmru.html


<!-- 参考信息 -->