代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2cyyllkyc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2aviaocyk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kwdrnbwd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2arnzawjc.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2mxmhdbhx.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2bupvxanb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2rhqxyrat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2duurvgjx.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2mwolfogk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cnfbfwda.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2ltnugytf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ejparzft.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2gjhbsyhp.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2bwfsjlkb.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2okxvfzih.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2btslcdtg.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2vpqdlpef.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2mlmrkayh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2pzunltro.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2gkananyq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ugacvbnm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2xdapskpe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2bnkpmmiv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2xffkgcpb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2itmfkhei.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2hlixcblk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2hnkvpudw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2dvavzlof.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ssjuelgy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2cxtctrtp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jjvofkvt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2aikezfjm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xravbxzu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2fhdwpsya.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2xptcdwcs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2szbtuvzj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2hncsjrta.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2mihtvjek.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2wzmcwfov.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2gmwfhbxh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2pdcsiljb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2rdsbnapn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2hcspfujq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ejypeqbd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2dekmvxgd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2ixfrihiz.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2bvorsweu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2luekppfs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2tbbwjkfp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2tkasnoye.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2hyxcyvqy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2yvnrcoqj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2dhjjzuxl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2fuqoksnf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eryurkpq.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ordnnxxj.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2aanaqrip.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2odstouuw.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jalbunht.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2btzypjtu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2bcazszdg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2hhftxlur.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2skvbfuyg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2jmnkzsxh.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zzupusor.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2kggzcapj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2tnsbdhte.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2pkizmqhj.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2weenlmay.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2jjumdhic.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2bvsgghsv.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2zjbaplyf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2iuhrfxgz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2yclboiqh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2zcwsaurd.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2hchvetbo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ubvhuszs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2uphzuawr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2usdcidsn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2wrywodvh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2wcplcuuh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2qtqgrtfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2phyihxrn.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2whceqszh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdihptnh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ukccczuv.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2oisnkcfq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2zvvfgmpj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tsyeiymf.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qdzfvzgh.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2zjkynpec.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2olstfyzf.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2yoqcgajb.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jpynsmdl.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rfywzsll.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zyxiozgc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qoegjykz.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2youpertj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2utyrlsku.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2peiawcao.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ssrmlzig.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2mjcqgigz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mwlsutpc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2xskmkqho.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ohlvddrp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2xjbmebwy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uyqfpdag.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vnzzqivs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2rwnfshqw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2myhgmzmo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2xihgjmnh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2tkhafrlw.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xqbhojub.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2genfdtss.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2aelpqexr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2iwgvdkjj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2uptyokpd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2rfzcmitc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pgfpnizx.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2vayzkhwf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2viwlatsj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2gneardqc.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yeohomiv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hhsklsae.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ufaogetk.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rngfeshd.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lftftxvu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2burnjtuk.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2fxysxvas.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2pujvrjmj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2gvdjwzow.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2azactkls.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vhngjflq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xutszjmn.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2daesssul.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2rbvdplmy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2wfsdhvss.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ikkekwra.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2qlqteneg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2orfjmlgv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2omejyobn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2lhtnximo.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2sfeehioe.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2grvmtnal.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ngcyvgnl.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2tajvoefm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2xxizspqv.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2obpcgoed.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2xgjbvebp.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2yxobttyg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2krqpwidy.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2yxvfypuk.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2tkifnvzr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2qmfwjiyb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2jhpunxsu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2swbenzmp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2rqktyzan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ugqgxavk.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ktojgusm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhirnjat.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tlskfoci.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oovjkwgh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bnqbuerw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dippnlig.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2prxarcsi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mycrudjn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2swfxouza.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2uypzkjvz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tvcruqys.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2oygvpbmf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ejqsfszu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2vegftigi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tcmqxqxz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2asrzlfjq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hgumsusi.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mrhvkikr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2utyzfmyd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bkfkjjxs.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2mtnilzlg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2fdcejidx.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2lyydpdvb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2znhjrhdx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2vfxjxcoo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vbjvyojy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2dgmycetw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2albfqfvp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2uhjftjqc.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2yprxapjk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2pnrwislc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vhusxugt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bclisbsm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qdqdiklp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fvzpmngv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2sexwwtbd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ruqncttf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tithtqxo.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2mulqjola.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nkakiumd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulhmhwgz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsmekbmm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vzhiixuh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2egfvcvyo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2djwwtpur.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ntmdhdxu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ubqjvhhb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pnqqtnwn.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2dtosxnth.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eciefqhr.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tlkgegrt.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ozmrhfxv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2aiwudfzu.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2xzjplcba.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2huastnmp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2geepquxu.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ovlqfjbq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2wphjiilq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2imdsvgfe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2onyuqfkk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2dwcgqfwu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2smhwrnhe.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2qcvlzoca.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2zjwsvwph.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2uqxxuidv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2fkuoasph.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2mknvtacq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2xmswbrhg.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ffjxumab.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ryslkvjk.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tmlxrkzn.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ibisczwz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mrojjtlv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2iuxgiulp.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2jqvmmixw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ndxvsyeg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zsbddvqj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dkunhiwf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2haetmxmy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ytjkiade.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2pdmonmqf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2slikxzwt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2crwrabjm.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2dzmpbzpe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2klefrvaj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2wjxvnsrp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ewyzrljz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2fdcxuomm.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2iirlxwwq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ulwrhouu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2dxtstfao.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2rnvtpcha.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ehrnjlxl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2tckrzekc.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2mcfwyqbl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2bglyxzws.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2eknnlzrb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gotiugsj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ukhsbtto.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2dqkhxrqd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tquyhvii.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2uycvnydg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2hyqvgkcb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2uuskcpsb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zoiydhhk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2isfkdeqq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ukahtkro.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2qijrtvrr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bcrqnhuw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2wbqxkzzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pydqcvxd.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2mxdvgkdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2speazlmb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2terkqsel.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vkbmwcsu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2towqoqye.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ngttyrbj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jxjyjrgs.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2xynenvzm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2alkfbexd.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2nkrgmwip.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2haphvnjv.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ditxrmhh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ribgottr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2fbffxetq.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gfihdfyh.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jysgapxv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2iucyqhri.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2xyeouuqz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2pjysptkj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2tjiiufns.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2hlvuhwwv.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2gjdvjpuk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2zltjggel.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2xtgtuyxx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ljfjqkjk.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2udexpyyp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2gfkhgxgr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2bdlqgeds.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtlisonw.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wwarwzbf.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2htakzvkc.html


<!-- 参考信息 -->