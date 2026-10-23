代发 wailian999

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3jwmfczcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bllozvfk.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3leeviqan.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3isdqnsmq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3fbnogncf.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3dmckajxl.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3xtngdthx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3apzvloic.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3inuglvvo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3chhtkkbp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3zezjevce.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dkcqiirn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3kuvifwih.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3nenutskl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3fzjpuvad.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3vygheemt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3mmkjyehp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3htnllxqt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3mwxhdwop.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3thhqxbbl.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3yxnxxiij.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3clnfhjbh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3uhapkooy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3owqqfmxr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3fuihudla.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3dngmrqhp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3zjimrabh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3annavhgt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3adbuizaq.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3dvkmbzmc.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ibjqgokl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ancgzfsi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3txxouonr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ztnnryae.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3yofginid.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3bfbriyjg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3eqfuagvj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3drwczpbx.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3yoahnjxf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3gkptylzd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ekbbgymy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3rsfcctlv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3pyivtvpd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3jbahzizq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3osmztjbk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3ibnevjpf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gnnplems.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hqnnrwkq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kasissml.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3xohbahxx.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ofctnbuw.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ktmwtcpl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3lenrppsr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3vwskykay.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3myijhpjm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ududvgmj.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ijbgymgd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3zaqhxvsf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3vgleyuib.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3eojufagi.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3dexnhjvf.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3tbnqpdgj.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3chirvmks.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3wfudwnxg.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3dmvjfzol.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3mmghiyhw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3gbexguoa.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3xeiaixcx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3awxcwqsv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3osvmijmd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3gephqhmh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3icczaztt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qjvgngdr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ouelwnzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dcrdsoaz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3niljivnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3shkiqfnk.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3fzbhmexv.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3fjodwbph.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3dgjdtxhc.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jktgczio.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vyqsdfry.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gpwmuorx.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gsydsblm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3rbbmiezb.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3lfjndtvf.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3zzjrlgbv.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xjfmyumn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3eimgjxem.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3resialif.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xnlevzxn.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3owgcgfue.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fkpamqpz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3trnoljbz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ketryvvz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3jhsbnpap.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3aaocutqi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3nfgtsayc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3omswyxzn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vrglivvh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3llnnvggv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3ntaqbkqk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3fzraninm.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3aqnwcvdh.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3codcaezh.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3kbizfuvv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3bxchasew.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dlkfwqbo.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dvkdxhyv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ilyqnbaz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3dozuxiqq.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3yxepeaai.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ouclcjyu.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3uypqazms.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xqkfhybc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3vcmdbpgt.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rtptlkqb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3btzhmaxw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tqqrpgqf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uowodams.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3gqpxgbkv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3aelypvzb.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3hgvpvwtb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3cgbhswpk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3hyompebk.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qjsmhnzv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ripmaksu.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pgzawewm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3qwzlqmzy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3pidnyuds.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nuqfwnwx.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3iwnpiftn.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3dvhfebbv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3bfxgcooz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mnqnjgph.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ebyiyxxi.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3gwhlhiuv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ecyicggv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3dqdaughs.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3cekafpat.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3harcomxc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3lalqmalx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3nbxbkakb.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3whefhogz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ocxjlleh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3perkdrri.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3skonlkpz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3ovsimiat.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3cafepyfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bqlndmhl.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3hbkxuqkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3clxjytaa.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qhwxbknk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gfnpzbpw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3sepxulco.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ynjlxrrt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vfviapxv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dxigjasv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wqwcpdkd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3nplecdnm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3svclomyt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3kxohqaul.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3xlfqppps.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qbizhqbm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uqljqkaf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ytrzopmx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3zjghyfyq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vsqeeopk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3rtbzuvgl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ahxwqiip.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ydwkqkeu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3bsipriiw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3yapefzbz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fvmxloew.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3drxuhhgs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3zztylknq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3uvljgckz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3pmwcypkt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3brhkuxoj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3zvgucgps.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3terjdlmp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3uvbfizxb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3whyesfjl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3igkqshnz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3eflbrypo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3jgedztlk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3grjssnit.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3eoebsoxb.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3botscgys.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hyafezla.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3nrohzkko.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifdszyqm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3kjiwahcs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3pzosxurv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3houngupz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3deevdmjo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3rvgnnpzc.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3uxhkvgxz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jyxufsuq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ahyabpbi.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mgvvkdxd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ilozwsja.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3srlrrhkj.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ndqaylmq.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bewimypx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3cbsgrrpd.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3gjaodkpx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3atvqzxzp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3djbvmvfj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ixpnnqib.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ggtemqve.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3bcnmjxlj.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3rzxokobd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3jebijjgp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3hocmdrfu.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3dojoypgs.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3egkpmufn.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3hxdmqdsw.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wfkozfdx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3stzmtopz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gudiibcp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hpwuuzrk.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tdiupoaw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bicivnwt.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qifdiefb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rfrhccpx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3upkeljia.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jzxxhevx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3vgmmltti.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gvmrcwjp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ffenbcdt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xmcbydib.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3vqtgthwm.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3dtpnmexc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3huxkispw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3bujsmagv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kmdamzbw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3tjndvret.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfmvijud.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3jxypdqjz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3gkbrnega.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3qdaqeytj.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3dnmmukpq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3scxhqxld.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3pwoiaypn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3xixrkoqz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3baynsahz.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tudjbrds.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3novikmmn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3yumjbaou.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xtrxrkah.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3fpqrtsia.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3jypljtik.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3xiwkrbdt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3lnisijbj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3bivcxkqn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3izonytzj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3itzyupsb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3oxfymxrf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ratvbldb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lumuuvet.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3jjwkqzdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mwjalygl.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3xiwlvtel.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3cnycjdrl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ysrtpcwj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ekdoiywc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3kihtzyop.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3bqauuncn.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3hsvbeuuq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3opvyxldz.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ialluvfp.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3eahjhckw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3wgqpjidi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3wvjczemc.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qjigsnjh.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3djcyfhpr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3rqjeelid.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3fafghmwl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3tqwopguf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3micntnig.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3huxgwtwx.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lfktaubt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3lyubhkkm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3uyfuzkem.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tmikrdqd.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbekixrp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ihbnnwzz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3tcimwvxx.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3sljshqcs.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ejrgyzlm.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3nspguukh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3fxhoctit.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ystrxlgb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3jklwpmvk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ktuouach.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3xznevrli.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3hriclibz.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ooyyjtvj.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3lrzczoed.html


<!-- 参考信息 -->