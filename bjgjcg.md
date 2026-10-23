代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3htzpfgpz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vyghyydv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3qurdaink.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3itqlciin.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3ubymynfk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3uzawkrea.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ujqxtwlm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3lmzaqwbb.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3fbbghzir.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ejaqbtpx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3eiwrjcuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xyvsibfb.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3jbowojps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3apsprokf.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3yytyqflz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3odxawdar.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3ezcnzjdr.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3wqdqfnrd.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kfdsfqpx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3pqlbzfkr.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3jfzlroxo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3aiyogyzk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3rvghakor.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3nklmcdhj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3aylssijd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3wgfheiwk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3iojsmguv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3wybunldj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3qstlzalb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3eifvlwmg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3lkxkrola.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3bejnyklm.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3jcpbbeha.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3irvizgqk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3miaionnr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3mvrzlbvp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3cvwbqirj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3xlghgvjl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3pbzprbdh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3uyhwcqlx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3qgyhiymh.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3hprjiaan.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3rivsrqxb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3oplngbtx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3myzwovtx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3sskhclak.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3rpwwcwah.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3tducdmro.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3pvmwenli.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3zicxyppn.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3rudmdjnf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3juowmjtv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3xqodkpqe.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3mylsynoo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3izkqyjwn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3zcxokkcc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3cqotypcd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3aapftmty.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wfrnrdop.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ujandojp.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ijcrwlds.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nkdcbaon.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3gauqobsv.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3iukbsiyl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3cckribge.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3hhovauqp.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3nlzqfuuo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3cxymzwmi.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3jjhziqfm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3kflhugve.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hshynzou.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ngxgijdu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wjtbjfyz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3illjhfru.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ermiyhaf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3rcnyhesk.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3dnplucqn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3mdyoedig.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3nholuyse.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3xgwavevs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3sbrgdndp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3aipvdlnl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3bsplkkcn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3wtbirrhf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3okldgpah.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hhtbelun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aivgizrw.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3lyrvarvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjtszzfy.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jsxqnnyk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tnndgbpo.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3zflfxpzy.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vkiauyae.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3xtratqfe.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3norutydt.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3vzyuwgfx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3suytifqv.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3tnvjmrin.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3hnovnyuj.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bxwprwmt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3wyuqylva.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3excpiqfz.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3fqqmjsfp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fihzwcdk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vzmgvwvg.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3yuiyvbcd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ifjkunai.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3gjyvtsnk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mqepoqgo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3jgrhomge.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3bwkjucqc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hgnwtigh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3okotegps.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ntsjwjwl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3yahmkjns.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3gqrkoueq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3mgzqpzqk.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3xphmhpgd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3clseliqf.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vdcjmgyx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3nyzytvzk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3myxpwuhe.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nivogbfu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3upnafnoi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3gnrkslam.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3jieygqzp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bxgmhxci.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3efppzsgr.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pxrxyrrq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jktftooa.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xtapzaro.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yrpeojuf.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3qwlznoyh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ifprufzr.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3nzutjqrc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3cxqwkuau.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3nbwoxgwo.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fvqydxql.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bmizdqws.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3leghocna.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3zetsqucb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3yyfcjkwe.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3dvyrhdfe.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3kbuygoku.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3habevcvb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3kshrvxqm.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qlcbnucd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3botnujpf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tzndvael.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3zufpikte.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3snobdbfg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3suzfduva.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3akbhqrtp.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3hxqftwcg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3gjhgdile.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3psgpsmkj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3xpyengyc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ljejzuro.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3smajadnn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3iiorrtxn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3wbonpima.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lsmogtao.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3uwhjcjql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfdpyzig.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jqastiks.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qcrznvmz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kaoqibcr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rbexuzcb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3prfgdwke.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tcndsknw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kijcwvlw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3stnauwhf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dpfprfvt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3tkjxvyum.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rxtpfpec.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3lubzsmfj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xeadnqau.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kwcehxrq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zzwiummj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3knuxhuse.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zxpogygs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ncnuyvcz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3vsejvgcz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3eaofdubw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3xrtmclqy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3pdniucom.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3nnmwcdxa.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gtqsbncd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3oadluyop.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3omsdtjtx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3swenpnrz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3gqcfvxwq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xvjsoeke.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3nqwvwgth.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rrubxepb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wlmpdcge.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwhpnzla.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3dejslgqe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cfjlbwvb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ptsevymr.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3xxwutqlg.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kihkyrrb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3qluoinaz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsxfzmrv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjklapfu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3sqeojlvc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ooinrbkn.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3tnoqrxrm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3csxmjdjs.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ggqibrfp.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ocudekeg.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hlasdkai.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wwertpwm.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uxgkomap.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3pibsudtx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3nljhfymk.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rwdqkdur.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3pytrqcip.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3cfwjnjwp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3cuucfcvr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3lxtyambd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3nnzwvhul.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ucayzzlv.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ubaclkvd.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3mvnyywqx.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3faatbqzc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3baqqqpzb.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3rqcmxzcy.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3enmjcwka.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3prewwkch.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3snryrfkw.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qjpafvwa.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qxbedgkx.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wbhrhpkd.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tlkobesa.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rfcuefjj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3kydkrmws.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ukalormk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xlfahzwo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ralukpvi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3treeqapd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ijfvmjdg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ybiavxme.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3elachdti.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3bmuchxhi.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3qauhtijj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3cvuswmst.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3tmosswfk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3grfxfgmc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3odjieaqd.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3loitjrxc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3xspmftah.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3fhkrswoz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3qrpuqrpb.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ookczjdb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3tbwgraoj.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3lhoozutn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fyhemidx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jidsizfj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wwkxiewe.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zdagngey.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3yayxfntf.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hkprfrfb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3eewosvxo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3izulxjpd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3vsermieg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3skdgroyw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3extksjjg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3mtlsiquo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3nzufufab.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pldwfvrh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3pkrajnhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjvbahin.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3idkwmzwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vriauxvj.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3evarevzc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3tazwkeia.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3hgzgbnwm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3mtsklzfa.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3dfizlwhv.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3snmwxscg.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3nqpxhzua.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3zltxjmbe.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3lnjzkrxb.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pykbelwe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3kwkmfhpx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3sahnvkjg.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3epdpgspw.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3uapyxknt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3kogzmmry.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3uzywddcg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3pvmpamad.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3krmmlxph.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3sxukhaas.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3xocsuziy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3jllxlnkw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3txsgrtot.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3uixilhur.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3sskkkqgo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ttkvmxwk.html


<!-- 参考信息 -->