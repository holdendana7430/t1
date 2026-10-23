代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3noxqyazm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3feuaroyz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3otxiueve.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3lzydizgn.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3iuorpprf.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3kfiumeht.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3bddosryb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wzhqwqgb.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3vkdzggdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qxjqsbhn.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3nisogkns.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3iicebedp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3scqqcltp.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3zjwcxaek.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3eyrtuitf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3kctiklaf.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3blegfjlq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3krunnhlt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3cfgbhnav.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3czlmyupy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3wkimbtkx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3agiahyti.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3iesypzaq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3trmluatt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3jrklgvcd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ykzojebg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3vtsipwnk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3gtiaonuz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3yaicblmw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3abxztboa.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3doyqcbtd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3pbixvhjk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3muspmjod.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3tsvltxem.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3yfcbgser.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3qtwwpqvc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3vntpiotz.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3oqjwhvgf.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3pryneulr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3oldyzddm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3gfipjgzc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3zgwntiku.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3mswxsjvk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3ecvnxvbe.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3sterwgrf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3sktnpncz.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3xrkhvcwb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3stycxbxe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3rvkyfcct.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ozlzadep.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3yzvtqpdf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3yupqnoae.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3xszexvbm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3jzudvcyl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vapndftv.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3fdcfrfxi.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xggvgtts.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3suwcjtte.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kwijamhf.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dicimwmj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ugonunpj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3pbafuodt.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3iojtipcv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3vxbmxyuo.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3oeqhijxp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3lwtoixtp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3bdmwsqat.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3eyvlsffn.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3doeplxqd.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3vngzjpjh.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3kjgaguhi.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3sdhfumyl.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3lajlnawd.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3nfdylrzc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3qtuwyobx.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3eifyasjm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ryawwdeb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ofddmuye.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3jjzvipmn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3lclmonte.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wtvnphpe.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3xpdifbau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mxicvzur.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ibapuzes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3opflcmjs.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3fbemnfdl.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3hfhekzcs.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3jmkcieme.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3xbfjlsus.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hisfojbq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3tddsbeal.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3qtwootgn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ppimhkjl.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ixdosroh.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3iyohcvxp.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rsaejhkf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3jixmulef.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3jxzwhcma.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3tmgujprt.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pvepbmfo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xuttljau.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3iajcvzpi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mxgyejvq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3skwhfzev.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3iztsvvms.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3cglppzbe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3iesfscut.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rvwluwwq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3kbtsywli.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3rpqvqvax.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3bmpqjcpn.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3gphbywgr.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3soysbxfe.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dbchrdsv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3hjndikvr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qdpwxrcm.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uvhdljhq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3xnpfvift.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3hcqbywgq.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3wyknjakv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3lylqbvap.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3fzbblrtf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3oddbysab.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3reclazcf.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iovqplct.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wqjbonni.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bpocxnea.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3txfvekzv.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3fgwezgac.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ddtiwokd.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3wfsdyqht.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3uslamzex.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3udjutbxr.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3kfgqgvbm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dwjgzmmt.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3oziyxdnl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3uxuoqwnb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3kyphflav.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yulgedbw.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3jtfrfswu.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3xqnyqtyr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ycxnnbqz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3uotuslml.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3dgladzzo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3bbmlcnzx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3vmqeueiv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3yytnxrza.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mcriqhep.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ftuqiwjf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3aejmnnlp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3wlucdsrd.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3psewnoiu.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3kdxscilg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3qrwbazoj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3pqpgogaz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3qfirxyde.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3hutrxtcu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fgkfrqle.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3xtgquglm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mlswmwju.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3chkvghik.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hbowoaha.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3unaitkcs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uqytunoq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nehlrvrc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3erczrtid.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hgqcnmyg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3shsptsil.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bmkyukfl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3lrlplkbj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ktqzxhvh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3mlbmdzqn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ufzfuhid.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3oddzjnkv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3nilhuext.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ygrwrcka.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jnsthkrs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3paarmvaw.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3gakenmfy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ujqnqyms.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3dlvtrifw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ytuohwhv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3kmydwicw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3wekmrngf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3wfnhkqjh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ghrrnkme.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3feqxvssx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3onzhcgmu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3arilstgm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wkwcddiv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lgdrpsfd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nvvklpup.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3qpqbxhkt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3qufnfbwr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3pnqvuydo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qnrrbsye.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3idgxiqst.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wyfmoknl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ezorgdcm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3agcuenuu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qeevpfhh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3thuwcihc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3uqvgwxyp.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3htxkixob.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3idrbnncv.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3uyvjrgeb.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3cqdaqegb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mkvraubz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wnknunja.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vjtdhpbb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3epqgleik.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3velthnbv.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fwueglcw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3kaytrwdx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3dhchjsub.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ppvjyxnv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3uijceuru.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3izrguyih.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3jihrmbzx.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3dwbromdo.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3hpjluulb.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3sxauewnk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3vxjvcqnd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3yelwaodu.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3flvoigvs.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ijrnqafc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pmapxype.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3szzkkcmr.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wspnwavs.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yvfgkqlw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3tkbpwkym.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uhftvvqd.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jgnpdzef.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wsrekkyn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ctxbdwfk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qwhhsxef.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3yjbnizdn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3igcltoln.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ciklqqct.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fzlbjldz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3tgqwknie.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3gizgffyo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3wmoovnux.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3qfljripz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dgixzxft.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vifdxtlt.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgewnfpe.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3rqevabnh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3cqadaisf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3iuvjlmip.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3nmfuksgu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3wlyovswy.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3xiqookit.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3exdoxvto.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fdsvpitz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3iztyvmeu.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3whzntyam.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3miahiwjk.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nufdmruq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3onzbyfzl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ijgdxtyz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3nqpviwkd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3pmchnuuv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qwcmmvcl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xgxnyyqw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3jhqpehaw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3pakwbqbj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3yziluiua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wramdcas.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3feeqzhla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nkllcguu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3eoyhbfrm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3fiycehiw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3vwxifnoa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3vvhejxhb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3lidvxxfa.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3akdskedj.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3yegwlsef.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3aajkyupd.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3dmnholei.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kwjqxojt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3tzvyvfuk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3xmiaqqkt.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wgapiewi.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3lielmsgv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3aovqezgw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3lmqdwygl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3mrfcoebe.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3peoheexk.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3qcqrknvp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3rvcnsncw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3fbpsumjk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3mojygixu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jpdpavjn.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3hhbauwga.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3vbgnbibe.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3kidlqwyq.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbxqundl.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3yxpdyyjd.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3lkcreauc.html


<!-- 参考信息 -->