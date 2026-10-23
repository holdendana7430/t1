代发 wailian999

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3odtpkoqs.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3szcgpmzh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3uekrpkui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hzhewhvm.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3jxucezxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yangybxc.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3vjqvqxts.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3sughielq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3eklyfttb.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3okzxxagb.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3arzxfyms.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3hdqiyvid.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vllhxfir.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3qsdvptse.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wkmdurrd.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3teljhdtw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3bztalldm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3gczkwxnb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ihyojnfn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3usbjfxdy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3odzffueb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3slshmudv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3mcijexgl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3mbuogtnc.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3wnfkyvnk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3gkbvbwrf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3wyprfoyl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rusbiuuz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3lgpluwov.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3lcdjwxpn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3hxaxupqy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3vsvxiias.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3cjmkppip.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3pbfuafxe.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3gdjqsjqt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jcuellbf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3nujwtaxc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3joswjduy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3tchtdwnr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3zjfgwbwx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3ckirxmfa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3lkjegvxg.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ybfkaypt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3pjmpirnp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3kujdeoqk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dneuexkd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3uedcwabd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3iaugilqr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3tmxrbkxb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3kdmrphvl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dmwplqlv.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ulbgtyax.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3mwhesymj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jvqzqmxl.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nlpcxors.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3szlwcmhh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3sdenekfl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3zndzxbvo.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3tesnbyhp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wediqppe.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jjofroqp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3hzmzbzls.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3jgzfxcbi.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3jgfeojnd.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3pwnujefp.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3skkwahlw.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wdygldga.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3wfsvrwss.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3grkgback.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3nrdktatu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3hngtecyz.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3cepbvewj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wkypkvis.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tggiireq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ftjriehu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3hjcrmzxw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3kntvymhi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3duebhdsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3imfmvnax.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ixtcupce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wlukadzd.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3aywalzua.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lsumpkhm.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3mbnnewxv.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3gzcdmerb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3kbamewhw.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xnietzyr.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3zdwgqspa.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ibhnbtca.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3aggmluqn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3fykazxue.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3leoclrdx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3knvbclva.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3isznxgfr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3krhyokyl.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vypstfnx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3spywpuho.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ezsufozj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hsregvcp.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3xckrvfhg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3xkpmdztb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3lsyesoef.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cjwozoou.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qvcpoyyq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ligwtsvq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3wpnkakza.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3dtozxpmy.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3wiurxrco.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ebqzpnrr.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3aacvlebl.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3bacchjjc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ijklczvb.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3imozlfww.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ypaogmuu.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3eytdazqd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3vpewfxmo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3xqvifbeq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3muwtpaiz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ypvsrmle.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3loduqxfg.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zpbyzrat.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pyjfpvzf.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ktdjrgpr.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wblsrmks.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3asawhrum.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3bfyccpiu.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3geferkez.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3qteboogh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3szvmdqld.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3exskctml.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ptzvphzi.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wfhutmmp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3przmxmew.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3mbqrvwvk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dsmucpij.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3smjqhxnn.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3tfdvsuvn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3csprntyd.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3kegjdbhk.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qiucgthc.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3cbnhxxmi.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3fnnwwvde.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3dvgqakng.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3lkhjpgxj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3muklatfc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3fdelqeek.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3veoczmei.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wffwoxvq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3rpyywubh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3aapcuivy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3gjoqdtam.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3wanhgnjx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3jyxfkrgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tevlcxfs.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3bhcptozk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3syykvlhr.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ijcxzbne.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tdfdmfdz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xckxhubj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rtcflozm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3lqnzfkfj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3shadsedx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uzgwdikk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3cnugpetv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nxvoyeoi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3pvldagro.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vlybtmxs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3bknmnkah.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bpamxasb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3iugzztqk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3lzipitfd.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gobhwyud.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3eisoorek.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3midjgphj.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3gsmptlvc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3qgtmijvm.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3zztzdwzf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gvwwasae.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vnfdaarc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jajgxtyt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3efpscvbm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3cxjefahv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3lephwzxf.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3vzameakf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wpblymlf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3fplmtbpu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3havxhmrq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cqdpccoz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xlbtghpb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3borlskws.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3efokmsvv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zzwplotc.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3wsvopjmm.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3awzqjwoe.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcmndlmr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhndbcuk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqkijlif.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3gcjmuyec.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ftfnusfw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ckeksbla.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3knxxlfjv.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3xwnepjlw.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3agmcglxs.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3teebteme.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ychngaxd.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rluzwcch.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3beidocmi.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3qwpveohh.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3whvpigsq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3idpwtfma.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3bsltinbj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3qkxmheao.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ipmfdgez.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3xkzktmix.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3hacajzpa.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3sifjlwod.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3aioleumf.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3iuxblmhx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3foqiyppk.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3vegwwuff.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3hkbeglcg.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3sgufwtgc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3affgxcdy.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gwihmaim.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3aigtqkib.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tydtcsdr.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ckwznrza.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lyzecjhq.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3snqnoush.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3iutzlpfd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kuzlblyj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fbgzdveo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ffwmygyf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ntqmfqpn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3rijpjeko.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3igadwixd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3smumjdbp.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3bstnlnln.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3tiaheadk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3vhfixlty.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3blhcsahh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3jnbzxeht.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3gewuwdty.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3asofpkpn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3pgmjjmxe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxqtumlc.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3slfdzyvk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3buqhrygd.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3inimgupn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3dflmqwjd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3oaqvpzmi.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wurgjyhx.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3guurpqhk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3zdwtoxmm.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ntmcypzo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3uebhrtex.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ebwuoqqm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3zxfmtxuo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rcewamsd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3wgeiorbs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rdxdaxyo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3nyvpjyfs.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bqoeyfhs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ppzbyxpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rurvswhl.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3gyybnmro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lhmnilym.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3wyysgnhc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rxfdiqgj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3copnjlcd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3lmhbmqvy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jshdbkrb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3gtfoswdy.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3vvcidams.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3vgrfqcex.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3upxswtul.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3azxuxybb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3uhnffmjo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3abxcyzhg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qezvewsx.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3sdpszidr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3cixidmpx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3nweipfsc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3kcigzfdh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3spxslvrx.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3jeynpyts.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3huvsjalv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3wowjypav.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ondofldh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3gclllrsp.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3rvzdotzy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3wpqdgxyg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3ftwcffnm.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3gygsyatp.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3rwmqszfp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3kxypjkax.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3mfyewdhz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqvcnjtp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3uprknxjx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3lesjqhrr.html


<!-- 参考信息 -->