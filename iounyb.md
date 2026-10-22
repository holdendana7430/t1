代发 wailian999

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2qlamvlfi.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2kstzkedk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2nyatszma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sksqygtj.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2rsylvxky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2frwsnzrh.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2gsllsjkg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2rlqyddvh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2dcarwymp.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2jmrkjhfw.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2htvfepqq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2fbyljgbd.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jftvfhwx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2wqcqwgsz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hcldgnkd.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2efcekihc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2nflnbkjd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2mtiwyjce.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2zchonkus.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2onklyqwq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2hjoxeulj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2elmwzcmy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2wvoeryxy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2lbzzuntr.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2ilptonoe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2hcgtqlop.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tsyhsqir.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2nrfbtrxu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2bwfswbrc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2ikrycdys.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2toirzzmz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2kothvzza.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2zupunvdb.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2nkplozvw.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2ssfeagso.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2dlvizbca.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2mqqhvefq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2izqnfqsq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2uvcwmlds.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2uglofyup.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2bhcfphqq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2uyktdhed.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2skgjzjoh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2hejbourp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2tajqmqkx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2efzfcwun.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2szwdzmeb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2mgpfzvar.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2pbhjodvv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2eefgueco.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pyshldut.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ejuelswx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ydzcekol.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kjkiqcgm.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jvperlwk.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2viouvhde.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2jeqlyouc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2bzkihjei.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2jbzsojkh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2tsmdqyht.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zhrpsylg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2bbcnkadf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2krekqbbh.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2aouijyhq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2dxjzwkcy.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ljgshwgl.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2srhvtjte.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2zjxnqegs.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qdiqqzaf.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2mhzqwgcb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2tlqvkxng.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2qwtmofgy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wethnlcq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2goweuzdk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ceymvglr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2gbyydkwp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xcfmxdib.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2aqsuottc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ouffmbyv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2bjsnhjti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lxnbtbvz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gcbqidme.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yscvmtbk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2azgoiuwn.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xbukvlpe.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2czicfiab.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2uvmgasah.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xvvbpxxh.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2noguxgji.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2bvnmbdyz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yjjnyqgh.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hirheicn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ntyyyrgo.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2lwgglaam.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ysreabpx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dkoaxqil.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2umblshmf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2zevvpyra.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yxfgmxjy.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2liwbcpax.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2hwqnmotd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2elkbrwbc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2tmddbbmj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uxpgxmbg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ijohmsae.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2hokgdsvw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2kybycjig.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2npeeoflt.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2pejbxczi.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2doagiprq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2czsstqvu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2epcktcdj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2sfldvkxy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2nkadzpkt.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2wagxfwpw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2kbprzwqf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2vcyvumdo.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2evagixkh.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oefzfrqw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gzyuvjur.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mraxxsen.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iqzgkrjs.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qgtmqpfl.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2eeedghik.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2rqrygdxj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2nviaaamu.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2rjzcvatu.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2cxvyctac.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xxabswwn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jcolbvkd.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nkuamwbv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xjbijcib.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2jiksqvib.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2kfebybyk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2xejfsgsz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2mbangner.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2dsfvzhqj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2twcugmdu.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ziewxaxf.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fykvnrpo.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2uqtjgnsk.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2fqtzqtap.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2fhhrwmbr.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2krfzlagx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2rbblbibj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2cxdgknwo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2uabvsnma.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rbvyqaio.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2qfmixxrr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ioibstja.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2bhdbbxri.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2iwdundyd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2wbtfqkqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qxwtmaxk.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2cdvoamdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ulcptsma.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2lmdheews.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tbmfedyw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wquommrn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jxzbpxps.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jzkvyhoy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eklwuyhe.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dutpmdub.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2dtrxvpde.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lcnlsghr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2dmxjwphg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2fdabktdn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rfsxkidq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mgpzawkf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2puzjuinw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2eruharns.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2alktwtox.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tbnqhuvg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2kjkdhalq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2lqxpcrkb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2jutikmtm.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2jeiijvze.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dworjvqz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2onivdryq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2hyjjvzva.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2tdgbyhwi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ntexpmtl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2dozwifmu.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2yudcyuur.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2huusqnpp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2kzacbejh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2niicztxn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2umhugveg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2pwtdjplj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ktgfydkn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2njokozsi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pxlpkcbo.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2dybwpyxh.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ijmkqbzi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2vittqrzb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsqntpec.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2uipnchck.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2xjkgigzm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ihfyxfje.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2loozvoor.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2thipdnof.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2kaxnrgzm.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2fakarotx.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bxbyyiol.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xyovccoc.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jnshixsa.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ffoujqmv.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ordumart.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kafnozzb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2obijsdpe.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2lebwtitz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2tntytzsw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ueexfinr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2cmgdzygk.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2knlzjgks.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2mtkcxofm.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2nrxfldcm.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2colxeumr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2iwnwhyxz.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2gmoessci.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cvijvirw.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2eiiexixr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2okufxdhl.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2oxbwbsdw.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lykygcpg.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mdiuufks.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2yhndtotc.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tbgfqqhh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2pwujjvju.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2levxkuxe.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qcgpdouc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2iijuoxkh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2mbfuaqol.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2twdthwdg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2dqcdkgqy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uvgnefiv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2mxnolbka.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ddxctjee.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ndxjdfzd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2awxgpmpw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nqjtsirb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2tctvjjed.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2tljurjqm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2bkznvaaq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2yrevfles.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2qqafxmot.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sdjpwbxa.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2qoxaajxb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2epuobjly.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2sdtbmgvb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qlgvnyrl.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nkiiphxt.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bfgsbswv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2gofarayf.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zgdmclxc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2mdjzjltf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2xrumbkai.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2boxacloe.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cvnavbeo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xefmqgxm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2vvzkxson.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2wuleshrx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2wzfkzfya.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2xqfuoflc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vuqpjrgl.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2qfohzxcd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gockcypq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2mboxgrbg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2asxkhgkl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2dtofszgl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2tsnvqbmb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2vvpeujvt.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2nhdtdtvt.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2qzqxmnxj.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2bburbxla.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2tlgthkgy.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rrzsnhxk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2wejxmdhm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2qgkikdys.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2cwobqwol.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2vbboysmq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2qeqkcyqw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2opekxxqm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2fwlaajet.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2qwqoshpu.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2mraihdqc.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2snmumslv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2wibgqsbd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2exxujucs.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dvdigwju.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2guzfbrjx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2sccjdcpq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2iqsoggqq.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpuukply.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2zpbbydfs.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ieofozzz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2bzyetosu.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2tnulcayk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2aligwshg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2mhatgnte.html


<!-- 参考信息 -->