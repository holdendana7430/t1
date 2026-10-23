代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3mvrksvbt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zrkgobhv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3eorzjrow.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3qvpwschd.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3jgfsinqi.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3xgbghsle.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3soimotqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qxrbvepk.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3psxmwgxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dgldgssi.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ushrqizq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3lyippssh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3hmjdwmvb.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bcznlwyn.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3vkomtnxv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3hgbkizll.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kzhvvimh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3axoxkeue.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3oqmdljpk.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3kanrzlns.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3drtdjuop.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3jeoagsop.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3dceuianz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3woqsvzqd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3eqerrfdt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3hokckmhn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3pskxnnsy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3hsdbokwx.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3kupmbatw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3cytdsniw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3kpbzlzii.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3dkrxsguw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rfpweuqm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3cuznrvwt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3dnxkridq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3hqtvbjgi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3wotkcylu.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3nqyoxlad.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3omdckvbr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3zykezlva.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ormuynfw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3lujaxtnp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3slnikuuk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ehywwuyw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3qkkcbqlf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3vkjryqeh.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3tljgqppe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ngxiwoli.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3rymhasnu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3vtkvohwl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3hzxykbaz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3jvsmzurv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3acaesrzh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3xnefbqwy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gcsxhykh.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hflbnqds.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ulkinysh.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wuzhgwhw.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3aolezxjd.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hsqshgsa.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3xftwyjcu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3wgarbtmx.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3nldzkamr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lxjkygob.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3pfjyhbta.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ezcczozj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3nhjzzgxc.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ciczikar.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3klstydhi.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3dcreslvv.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3pvroqaho.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3siwzboar.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3zmngmniq.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3cigifyug.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3dmemtyhc.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3czpflnvt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vapfhcqh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lnufuqln.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3plikyark.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3vhbvxacu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3efasccgn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3uwsauqia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mfvbafrf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3qngqvqpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nrfqzujf.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3blyvgrey.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tqdiflre.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3xokufjem.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3smwkocsm.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3oynzedrn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3weemjxbk.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xlyxgbkv.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3webxasnz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3rfkquyaw.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3beblqzle.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bmzxenks.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3wjojskgm.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bbgagtux.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wgsszotu.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3snurebbb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hcmqgsyo.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ehakrryl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zbsfxgwa.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ndmlclan.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3xkjvvwcx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3eiwolalb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hqgjknie.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ulwsijii.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3rtbvcayp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3rnigzxei.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3arcnquez.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3rycqevxd.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3syjapbht.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3kvsxdjly.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3hffbghzs.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ompcolmn.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ykadyyex.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3bxfawxfm.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3pcvhzubc.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3zlxsgjgy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3upghisyr.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ajqbzyxb.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xhynqidy.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3qhsdcbzv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nhdllipv.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tqpzawlm.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pesaeehx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3imwukuge.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3fncqwrft.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3fbvmtxiz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3vfsekcgz.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ijsbnnzc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3cszcrhkb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3etgarpkj.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vmmhmlis.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lunlyeyg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3irbbgdrl.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3qqovvjeh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cmlwssie.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3fwndbokj.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3kkajlzzn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3aijticpm.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ohzowpoi.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vqhqltmd.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3getiakfc.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3nwinswlv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3erwpfuag.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3iumqicou.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3lixmnkhd.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3jrqwkxft.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ljosavnp.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3cuzzmycs.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3aknpacxg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3rphpzrda.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3tatowkfy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3dhtqqors.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3gmptwjra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3znrhzlfx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3fofsyfvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3azylzhku.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3lpyyqoiz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3szsxtbef.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wcggmtsp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3lgozixdm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pbuiunwc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3apzuhwjh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mmdpzfgt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ummbcwel.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3umeexkqi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3fnsehiyp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ifpeewcc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3uymikzqu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ulpukynn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ijujkian.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3aefelbpn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hniikzqk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3azcqkafq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3dtufrmhz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3qfjijemy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3wkjacyyp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3fuwmqppq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jbukyejr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gqcufncl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dsljqbxx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3jyxcnbga.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3xpfoqyrl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3uqqndtoe.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3hcjhjyee.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dkslmlln.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jzrfocrv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ckarsela.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vkuahihk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3yjxnzbop.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3rldpeqpf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ywttoipf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vshpcacq.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3uygxecyq.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mkfnxefc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3hnwqpzgf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ohwpqhkn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3eotaqyht.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ndesdcby.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3hmbhftvu.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ootkrxfx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3rnjxwvvi.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3gqtjwvjx.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3sejiereu.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mhekzrtg.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ipzhwrnf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ttccuurx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3pafqmpsa.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3wihhadsn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yoliwyqu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fdgzrkzr.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3urzkdwpb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3cawulzbf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3jyuxfsye.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3uepszhzw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3jdtjnvke.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3vytfnsew.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3uvfcftpe.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3rzzlfwtw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3nkcozfnv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3kqrtgqch.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3whizyskl.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3hgpqnkee.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hcytbctp.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dumvexdh.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rxvaaywh.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fjqimsxw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dubshmej.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3seqgsdhz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ytfucbev.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pormktvo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3asmhjpnz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bnsktyoi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3foovtxzd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3pehyyxzt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ntdrwrpd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3izzkuemk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ocbpoajm.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3kwxwfvni.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3khkqewfa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ffjqhdtz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3acrsshfc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3hllpqmso.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwjbwplb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3lmxspdol.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3tqkdpcmf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3huvrbmsl.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3htadpkou.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3xmizlxgd.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3suuxhpuk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hljznpti.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3nzjbkdjm.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nxrdjebp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hrxzofrr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3loxdbyqu.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3utxsvffn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3bsxubbtz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3sliqfzpj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3mrimbvtj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3vhqgpeqe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3wphhvscq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3eylxdofc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3rmxxasba.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dkkbtfwb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3smyrksjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qyrasivt.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3utjzzzdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aumogbuu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3cetsftob.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3kjlstceb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3whrfkgsh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3sypolznz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3rpmpzjwz.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3pqrsltou.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3wduoebqp.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ooesmhqi.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3vqpxbyxz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vhlclzjs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3fwwrtuuf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3rurcyarj.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3crfvkwvd.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hkgitlkd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3hldtlopq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3lsfodhrt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3imzxgbpx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3wfhvlhod.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3kjmqeejl.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3cnfkucef.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ggfcqmxz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3zpiwldtw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3lpenysqz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3fqyiknrw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3xtnikdzl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3uvknteop.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ecandsqm.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3phlvzfve.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3fiauvfuc.html


<!-- 参考信息 -->