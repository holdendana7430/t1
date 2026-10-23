代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3kbbftnsa.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3xdjroajs.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3imwzoxfx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3mshvciiw.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3lyynvwkp.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3ppyyyafe.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ybmvmdfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xbftfdub.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3nnjzpcji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3isohbxyk.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3uyrglsvr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3zazeojha.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3uqhqiawo.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3nbwuouzb.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xfclhtsc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3ozjmdguv.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ykxztmbi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3xfwyprya.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vfnmqyos.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kgmgmlnl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3gzlcfpdy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3iosryjbu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ugnygeoh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3kngencxu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3xpsblgfs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3kdaksatq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ifzvutkv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qvrqichw.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3rzjvnmth.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3nznfjbyl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3pzmepoqt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3krbjlexq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3hwmjsdpt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3xdgtvbkq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3hglhtrvf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3mjnojpdm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3rlsgpakw.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3dnnpppzu.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3pqpduqje.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3aoqjodme.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3aulbsjuh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3furisuho.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3lwgyyekd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ljrjzqnq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3gpmfbtsv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3esgpxyku.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3gvjxvdyd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3bvbqcsgq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3fizaqzny.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3enshypbl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kbgmmucs.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3yztvwfww.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ihblqijn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3dmtuhajb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zjgflmoy.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ztfkqztf.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3nvtezrvv.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vqkwvafw.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3byzgjysp.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bppjelxo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3gfrmwzdh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3xuevzusq.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ylukvccw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3hwplfdxc.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kwtzdfrl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3pngbmvad.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3iqjqcjqv.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3jeczjhyt.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3kncajdtc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3srlnfkpn.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ielakaqw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3iavrdpqn.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3femwgwki.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ddhfzafz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ygnpajic.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3rxsvlzpf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3uxbarbwg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3cyadmxus.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3zzjnzvuj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3yrldkoag.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3uckswktk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3krqguodq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3djgaqdxr.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3lkfmgjlo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rcwweqoj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3piwlichj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3cjnfsrmu.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3kuhgbdtn.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ukapjpzf.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vdcmgvnf.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3mbvzqtwd.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3atqkjvrr.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3sxoixwwa.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ytsoqwqn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3tlonajwn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uzpjvalp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3atvwfmrx.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qnoaabbw.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ehkybjmi.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3oisntnno.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pcvfbdao.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3niewazrp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vfqjplqd.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3dukwhrki.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3apxetlkm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3inntubnh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mfjeqkyl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3snkodbrq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3jvrtosga.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3ihmryqww.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3yxswoywv.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3yjuibvxl.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3uyeggiez.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rrkbavnd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3uwpdyprk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3awwswiny.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nvtqkhrs.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3yvhbzwou.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3jbnwlqxi.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3budeikzv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3uwfgyfhi.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3iyczfzau.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qdntveng.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3pfpaiyzn.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qaiyqfjn.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nysryhhq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jkrxwaxi.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wnihfyyo.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3kysukkgt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3wgsrszde.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3epuqikpn.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3tbwetztl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ywgwayws.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zsctuoeb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3srihpnnm.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hmbpimlp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3knncnokj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3mjajzgay.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ftxrodnt.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3cqbjocqn.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3izvgylqa.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3lncznxzr.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ivliyvwm.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tiobktre.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3vnuedxsj.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3njqkqtxs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3rycstpdq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hvhgtzly.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3imglduog.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3giwdrnfl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3iqqeazma.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3aovbueyo.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3fdrxijdd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3pcdclpkc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ndtylcdo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3rxzdsiqw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3wlcexjny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kivmdewl.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3erfzbieg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bmqqqyhz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wbwpxhxb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iafesepe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3gejnfiwz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3woygxgwz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xqsvoyty.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3obqwemty.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lxeynole.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3amneagty.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kmxmxphp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ykeblrke.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zajepqtc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3stpgzvky.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qzgidisk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mmgfcvyr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3nzhoczbc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zocgkbjf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3drmbeckm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ugjffthb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3sggfyivg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3mcmlmjle.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3fgsdtqlv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3rxwkoitt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3imnoqxcz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3jvpqsbfe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3xptqupuc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3cdealgod.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3drjqthhc.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3giujgjig.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mfbzmvnv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3egpdbcfn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zplvbzic.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rmannpja.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3phovlcuw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3napvyuxe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3rzyytwkk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zwbuzygb.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3lhuydbgj.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3avomuhja.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3qjalnzcl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vrxowvww.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihgfvsxa.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3zlrjcycu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3jxqoakic.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pwdirchz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ermtttim.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3pyscmvih.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3yrytlyoy.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3shfcfhet.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tvaenejm.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3skrfyxvk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3bdfqmtsq.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3uqddmicx.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rpnsxtvl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zcwiqbsy.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3kfumhboj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3axposfvs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3cvfrnzjs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3hxpiaimg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3qcjzszjw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3jstdkuzf.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3pyytmfxc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3dnjuaxvn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3nxlfnmsd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3viiuurhf.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3mqzanvro.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3jmbzdmry.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qyfhpfmv.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vdynngib.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gizvkuug.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ycecwhml.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nyqcsoss.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rhqlejlg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3trdxmkdf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3mfwlmfms.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tfoohztt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dgozhsmi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3dpzarvpj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3yfuhmiyg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3nvmcgmdp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lfzdxbsf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3vcfanuyv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ntkeujfg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3hlnvdzyf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3debmoilo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3rcbalfkx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zigmjfrh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3fekogsen.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3gazwdtye.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3pwhuvgzu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkwjtdlw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3uragpfvg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3rvrdinbo.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3oeckwdkh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3yngjvhmz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3tfbybbyx.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ijspahsa.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3imnqprtb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3qojcylwd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wncubtdf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3zpapjmkv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3phtzfvpl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3kwoyuzwp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3mqrqkylp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3mxmidnjo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3bedtpown.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3nzqyrfus.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3hujnooug.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3zxmbdigb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fbmeinqi.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3tujfyleb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3judwfoia.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3odckuldm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3dthgkcwy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3npiwolcv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3bbgxepvx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ddodvqun.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3znyddifr.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3bjabqedd.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3rvdcemhq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3jkklrano.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3siqjpgje.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3uyvglmqv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ebsuwmvq.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ofiujcyi.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3oycmswgi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3wtrepsyx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3jqtpztln.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3knpenbgq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3oypzkjai.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ebgcdlzs.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3oxmcsqaw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3gubbibam.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3aqpvwlad.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mjcmirvp.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3gvkjkdck.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3fvakwahh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ouxwcint.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrhnkkef.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3kmvvsvcw.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3jriwjhos.html


<!-- 参考信息 -->