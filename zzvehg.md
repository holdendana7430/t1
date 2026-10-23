代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vbrmkzex.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3sijekhlh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3dcxthedn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3lqxudqew.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3attqjyjo.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3rezlyewy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3fzjkpbqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dqguigme.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3ieuxkizw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lmfveqfp.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3xwnnkefg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3setobvsa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3vdbgagrr.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3vztvjacn.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3bkhsvile.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3sgywlvgp.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3jvxdafhp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ffemcgso.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pqmbzjmm.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3lpwxfndu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ujuhhyeh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3brbgypcs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3lnifiywh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3cbgubbbh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3rxdlzdhh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3illvlmql.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ngeeeqpv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3surrlqwj.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3vzgfbokt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ljwvueaf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3mpnyebwy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3mpdiclgs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3tqsieioq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3btekvwpp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3cpsvlshw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3dlpjwalj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3czzzviya.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ajqeipax.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3dvgirutl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3pbpvpttx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3rxrasyuh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hqdpkprb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3jkkfzpkl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3agswnhqn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3ibyyhxqo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3rwfltpic.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3etxeuntb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3fyhmjffg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3eymvagdy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xwepttok.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3tyvvlmcv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3pkmeixgr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3pmrpqyvd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3uujnuvek.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jaohhloc.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3bkgzozqm.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fhfhkvgc.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3xlbewmrw.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xwdfobwq.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ldvxphci.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3hilmbxlq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3qkdfgnur.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3hxonjabz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3cvtumbnq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3mzoecqsi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3mnjvrgus.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3kyodmwqj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3mdpecryn.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qtcisrzf.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ioegoila.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3hmedvjvj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3oxhlkiux.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mulankeu.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3tmabdjww.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3kxixjuay.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3uzbuecft.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3uheirffx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hsobtuot.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3voccavjd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3zjwmwdto.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wfknbnvz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3crtgkdro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cudcrwbg.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3xxjiqwxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dqtzzuxh.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ucdengav.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3zxtfdwdo.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3pxirssrg.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xlbburcc.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jbvlsqag.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xpeumuia.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3uoaptgbs.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3rfhcczbe.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3jjyedrkc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3dqnfegjn.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yknrcwqo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3mhppjxyi.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3eeeewxfv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xiawjnrc.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wqfivfjy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3krlfdfxh.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3spxeltwh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wgtoewyc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3nwodnmeo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qdoxtltx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ieznisqt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yzrhmryf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fsxvcfks.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3pbjlvhgh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3vohzqsgz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ytxbcpdw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3sxinfmnt.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3tjgvjbsa.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3worwswwu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3dwwrjrfy.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ihwzzzom.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tyjbnysb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ifoevyce.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3dcprokqn.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3alslqtgu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3yfnucneg.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3oitdhcgn.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vzqlnlma.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3esihllhh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3opjjpewh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gmucpsfj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qcjhazhr.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3udcyeqgr.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3arfeudgh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3sdqikkqq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3oaidrbuq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3tbljqkny.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3cwzebkge.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rlxhmimq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mvicoxgo.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3licykjqn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3roqjbnra.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3lpjjvhrz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3njygypio.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3kmandgmj.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3sejacuzm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3djtzmkyn.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ifihqser.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3agxmygmd.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3uyousmxq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3jmssvihb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ayizgbbo.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3rpoircwk.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3iumdyrnk.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3adfjffmz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ljougzte.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wdpgcwjk.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3tcbvwgwe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3zeawobrf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3eprmnuqk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3yjyoycpe.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3uopfpenv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mjqttmag.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3moijdpyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ukwoibdq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3nhtigctn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lmhfoulu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mniyqznw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ottooowc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zmsjgxao.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sbsaamhh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oaswzmrn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3rzfeajen.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3syajxjij.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3flkqagmj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wumpemlj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pjlrofpu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rbkotycb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3laxwdptr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3jpcbpjoc.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3oziwfgsf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vrimtrxa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3laxpdxyv.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3eflsajza.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3izoswvna.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3lnjfdtul.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jpfgpwfb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3uuvpzqwh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gpkwsxkd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3mwakujdr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3nztuusii.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3melxuusk.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3dgmbsnzs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rtnxsxji.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3raqmbczu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dbmnpzmt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rsbpxsrc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3lbjakqhs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3dhgtglrm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bvwugqkr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3klzpoaul.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3pxwstyxb.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pvmmlizw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogijpqhc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwrafgqc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3rojpdehw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3eyotbtwq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3buvwdpnf.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3qscrhxja.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3oooasknu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3etuwbnwc.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xtyadutb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dybswpci.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ssadeson.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ijfnvqhb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3qapdvhcw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3bsbwvqep.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3wucqkskv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ajozierh.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3tcbrssfl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ysxxxszc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3gkbhprew.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3axfzxzkq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3xjzjrfox.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3bjwyeqgy.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3mcyhjswd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3xcdkczuz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3dhadsqmu.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3pmceuvsg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3hiktbrgy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3serzdcex.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3eeveikdc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nglfollz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ovoyucwr.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lrmoeklu.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3jsoonuvr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xvlkrpxt.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3kxnrtlwn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3rphwdbhm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gtdowthk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ftakdhrg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3vugqwbqg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xspncegy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3yzqjxdln.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nbokcuce.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3axxgnnsp.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3wciicpjv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3mjiejgef.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtwjczbc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3dyaqcjuv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3wvfjztao.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3dlyqtmcl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ljgejifc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3rcyswrbx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3djbtbsbq.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3idjhncjm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3yuveqvhh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3kilsluci.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3wuqueyha.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3osqpvacb.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pghiuuwj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xjxlxzbm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3yxqlidol.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3idoweoff.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3uvrdfldp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ierjxsid.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3iwqrddkf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3scizzkwl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ukkalooc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3sylttxpp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3dlpmqmpw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fnxqnmqn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3isvtorht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3moevgymg.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3edjgodac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqgkbqbb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3lnkfqxgg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3pugsznzq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3szfcksdv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3unaabjua.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3flzsdmfi.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3mbiqkqxb.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3atzicqqg.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3mpbwbdto.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ryxbocsr.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3xejgjqkg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3feumlsmm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3wsqompvq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3gxunrqmh.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3boiskhcf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3rourzukm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3otrknoxf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3vnaauebz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3arjdpugl.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3huhxvsfx.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3gnzzevju.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3lovrdlpm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3iiegshdj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hlatyrxt.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zogpizzf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3mnjwqmda.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mzjqimfm.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3tbhiekgu.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3fwqhufvy.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3afkwdvqz.html


<!-- 参考信息 -->