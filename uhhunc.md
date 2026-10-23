代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3xdgpzyun.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ltrnexim.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ktbgbdae.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3npazazcz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3epvuwtvp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3tpwwrbsk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3wgvnflhe.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3znrhzidp.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3zdeicfqd.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3tbqnqboh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3adbbhupt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cygngwcq.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3fefqeqhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3npkraccn.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3pnhhsase.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3fvgsbozq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3iyjxaezd.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ernghctw.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3abiazvbb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3gdyxwjfv.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dhmgkowe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3voxpbxco.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fmewchen.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cynxsdzj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3kejjqnra.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3paglqwls.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3znbqfpdv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3siqeewln.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3eqijnktf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3nkorpfql.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ifjitkww.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3erzyxuav.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3xjnapzcz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3hprmpmbi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jfnnupxl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3lghbxxpy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hwvqymmf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3limgnjgz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3jmcmfftz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3jhyzoabd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3dcutrdqs.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3pieebeam.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3sezprygp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ktvdqael.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3oxsqcuft.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3uxgscfwg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3auhxakut.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3dfraergx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3wvtanwfi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ddsufesy.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3sctdbncl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3yhvutupx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3gweftpzc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3palmyrto.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ntdbjaaj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3jtxasiri.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3geptoeqx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3kerusche.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rmvcwjla.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3efbrupgr.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3cgnwqqfr.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3txeskymc.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bvevyyts.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jurvqmaj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3eyivhpfr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3obcknhow.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3uskxmiub.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3bfjqzvcx.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3uvrkwihk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3lwivtqdq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3vchtamdr.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ikbbgwkm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vjwizzpv.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3dmnqkizm.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3jasbdsfu.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3vioheryz.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ulwuhjle.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3gnlkcbyf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3yeqynmqi.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3hxiyffxf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3purrbrhk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hlsqjjwx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3lyqxacat.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ncqzjqnc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ldcgrdub.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3oqdaqwto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pkeglhwv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3xoexcnlq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3khkqnkhq.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qijzagrv.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3rifxczvu.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3vcznmsyi.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3mangfcsv.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3beargrpl.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ecvclami.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ehqbvymh.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3nugnjail.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3jxmxskyp.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3bcrrhrds.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ltplhkyj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3mttnkmrf.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qgkgciff.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qcjgnvth.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vzhrjhvu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3snfaknyf.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ckncmkfu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3myokmxbi.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3bcfgycek.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3owtcqpuw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3dpqyxscf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qhwujiuc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3moknkywk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3jgygrwtv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3xyxsxqoj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3soircsof.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3vwtxoinq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3lkywefju.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ibxthldb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3qmfvffze.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xgytreoe.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ztczmctg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3tiehpmbe.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xskfrlmm.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3biklqlde.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3wxjccvkq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3yidqrdip.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wfppparn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3hsudrdbz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xrhacowf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3udlxankz.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rjwcwnpe.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bdumuulk.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3izuaabni.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3sdnyajzx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ibanxjvz.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3zvryrtpz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hfeeioje.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tvbidguv.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dunppbvg.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hsizaqgw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3qobsaduy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3fitlsdlq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3senpnvnp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3sjuktedp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3naldrlci.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3tmhefysi.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3pyzfqhpb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3yufpmmyr.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3upnxzdvg.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3smnzhgym.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ptukldrl.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3qlddpnfm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3nwkjflrb.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3rzckvpgy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3hixdogzb.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3vmtzrlqu.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3mvtqitfq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3facliykg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3qcaanxml.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3njknvbzs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3mvzaodop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uwlqtgsz.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ofghmjtz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yooueuoj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3tbdqnanu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ngxyuchh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3sggizotq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3voaxtktr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rtfonkuz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ppfsmzgu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uyxxtuvn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3enjzlxhx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3obredxew.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3nhvebfay.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3nfcxjvjf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3obdzzkvi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3merujkgy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wcrphcjq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3gfncetwm.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hgkhllgu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wxehayul.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ovozzvsm.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3kalgleme.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3qaiodhxx.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3kptngrls.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jhrrplii.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3dmjuungy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3qyhpiesh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3dwaxqzdk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ehvrusoj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3agwlknlf.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3fykzpcgi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ypexytrm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3moxgxbba.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vcuihlyx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kugotlsa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3fcgcnwdz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3wiwtheir.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ropvqjbl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kawfkvwe.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3uguhbaup.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xgxzeysl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3gkyuajxq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhydrbta.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxakdvrt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3mafrgtyj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3zzldetcv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3mmsexdbt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3aexsmzpw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3saxmbgkl.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jcuctshm.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qvoxgxjz.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3axhtsxtm.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3afjwexzp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3vgsahmdj.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3yxkvovcm.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3oxqjekbo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3cpauuqmc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3tdttlkwn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3hbubgnhm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3vcymfeun.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ccttekzp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3eiymwkws.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3rokoqojm.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3wmiaqcnl.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3anvladsz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3htfbeagt.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3vnzxpppa.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tlsgrfjb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ulwjrweq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fibhydbp.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3aybjexzr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yubitmoc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3atxxtkox.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3dvbluaeh.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dedwnibv.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3bjncmpbn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hpehcavb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fbznccqe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mdgmhckg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3aisazrmi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3gimxpvgk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3kizsfvox.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ticcivgt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3bflbmhck.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3jqusyapa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ngcrctid.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxfpzjau.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3cewnvanx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hzgpvxne.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3nphoktky.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3gzbuhqec.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3fmyscyhy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3uiqbybhp.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ksgtgzly.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ahcajyhm.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3nsmbgnyx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ysbjxjoz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3zsnpfzzc.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3iffrmnmp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3daahasgu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3lzzkbfnx.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3chsoflwz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3wcnfnsbt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3kqgbzudd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3wvuvrglf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3cxdosspq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3xkftkveo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3mkchnfoz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3mzowuvgw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3plepxokb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3vexflbxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nnsflwpe.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3rjjiznwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbytrrwj.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3otiodlnm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ewztmpsn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3sisgocun.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3pdthwwym.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3mggwufyb.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ssfzpluf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3jgdbfioc.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3bcbrjkpt.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3vhjandiz.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3drfjdssb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3alfgzcht.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3lwjttman.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3zankmjwy.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3laidyrmj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xgqjapiw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3oesarjax.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3iehxuvcd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3mivsxaoq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3odwfrkot.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3qwtfsetg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3eviwefmw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3mzswbdtz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hpubqzev.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3pxcymvvu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3birxxgow.html


<!-- 参考信息 -->