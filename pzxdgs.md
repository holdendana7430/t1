代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3xbbqvbfw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3rxnmtvdv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3edfbawgh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3srczejjo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3kzicqjrm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3jowshapm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3kayoqice.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3baewkrqg.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3mrdwnmpw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3hzmkmyle.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tikddzse.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3vegbarhq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3zywuoqlh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ylmdfeez.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3morwpawz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3xaurrfpe.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3wmozpxyg.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3pypsfosl.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ljevztvx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3unswczuj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ncqnydxn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3czpivqjd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3xwwctfxz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3zbbuwlue.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3qzyoddtk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3imnosxfu.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3tszircol.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3tjdqawju.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3wexmpwjl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3vgtpakbf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3zjedwruc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ciyzosto.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3fufgfmog.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3fvfgallh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mdpejoxo.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3wvckzvxw.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zkdugnkc.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3xjgcoswm.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3sseifppn.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tuhljazm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3azodsmka.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3axaxysra.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3kgdufbaa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wedkdzoj.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dilftyxq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3caarakua.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3gwzhqtsm.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3tcfnkzcp.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xuykirtg.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3bgazkrvi.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3athlrccb.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3fhdyhvnu.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3gylgqmoj.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3lerximel.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3gzbgcwia.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3vvjtzocs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ocafngvv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nkwjljej.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3dhvcudyk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3llhsvgye.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qmoecdzj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3sffnhyez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fifwpurs.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ilxjvbkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nxaxwvoz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3tmsiiwit.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3tjdlmgwz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3xbqyvhph.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3fhxssntm.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3wjmzhcxp.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3unvziwnl.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ayqhzotm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3kgttvzdv.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hodrdaie.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3acwnihkl.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3aihdmazv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3vsywrxja.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3nljsqpwk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3sfnrvjau.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gjfmbzyr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xwhjyrqt.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3kxjegvsw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3irrdvnmr.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3jaynvfqt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bvkidbcg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ghzlmina.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3gqadzbet.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3uryomjqh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3hradibus.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ltmjwugn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3zikvxfpo.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3mwmfvprm.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3hydbxexf.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ptjncryt.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3xngjwktp.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3bogfmhvc.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3pappbbbz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3oauyuhxj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ezxmhluy.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3giccakrx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3pfnzbvnq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3cfrqmbdg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bacibqrz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3kfsdaanj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xtsddicm.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gqqnpnbf.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xusrbqjm.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kzuuffwi.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3lhixzweq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3qtietqks.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3wklynbcr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ymuaznou.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3foprmahx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hlmunetc.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3bjuoefgq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3nlofhrvi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3simygcye.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3blyzoizq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cegwmref.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3eufkdtae.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3mcuckkrq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3cgvlihdx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3jakkvczd.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3znaqcfyb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3gbetbywu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3hlxgsjkf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3vaeiiixa.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3yzsxkpge.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3nsekiojo.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3vjvntzbf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3zjrufckw.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hdcnpdlb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3tsyyjgwh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3qikhywtv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3izossctc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3poqpxugi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3xbtvyqoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3feqnsynd.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3nborwmun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lrgbzdqx.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3pfsxjtkq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lbqgukdb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hqmrglew.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dqelfocj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dgckyfbv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fddgjius.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bqrweluo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3gqvlhykj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3doqbcwxg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3wgjbfull.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3iuulfwrq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3towkwsjt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3khbhezcp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bjnseshq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3unzjukkj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3shsuseik.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tjrwkyze.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3dvlbdjbd.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3kbiubuzg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3pvugkmrc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3olgmspih.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3xoqinwae.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3xkqxnebm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3xvebxymw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ufasukyp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3uvedmexz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3cfsvqldh.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3rfatgwrl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3tsgygxgc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3pxpztfci.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pwjzygwq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3igszavwl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ivjxocsw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3yayqsotk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3slmwxdyi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kyvyszfd.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3tqrnxvbv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xteojowj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ebquoigl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3mpkkjwkw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3cqcxoxhz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3mmkqfufy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3jxnmvgbs.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jrdzertp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3bkbtrhtb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hlgkbvpo.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3skonqyjk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ncnsxuvi.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wmtepkpp.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kfxdfulf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3wzcdrlum.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3pxabmbec.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cjgjwytj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kqounupm.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3xpsvoqse.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3jggsoyrc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3qnmujjmb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ktegdhxv.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3xdfworjq.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3cjddjilz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3adwhiwcy.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3xfcotmxz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3otogkbbg.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3rrzodwzb.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3weedncka.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3hfajjuct.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wapoiavt.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3puamvbvx.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3anwfykah.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ioqpytxv.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qmcnlost.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lbxzepfz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3hnmtvpzk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3dhmnksyq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kgzzmqth.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lweggnpq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3qjxgoyda.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3afdvhdic.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3wxwgzthz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dnivephb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3clyqqhyo.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3scizdqju.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3mrelcrdq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3zseccnvx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3amwxwzre.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3dmvikwfu.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3sfrnpjxl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3gpnpriai.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3owgrlpcm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlqvdlft.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3dccqxjsw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3jjelkmwc.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3jjjbmavr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3xopbknpu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3muvelusu.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vtvfzwjp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3uopfyekk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3tyqsbdiz.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3emvvuayk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3wkmuuihr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3salxwbgg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3cwfugapr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3xmpygyrl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dvtjvvkf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3lcsbhkxl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3lhheounb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ainzaafl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3knvgozfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fduqpwob.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3wmqskrxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kctftxvg.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3fzvbnqku.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3iqrkicyb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3biyfbkty.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3bfwlrzfb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jpemlcrz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ublusmpn.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3stxyzoxd.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3lonprsof.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3guczintn.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3rjusylii.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3iybaytno.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3jpjuahys.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3guulfcsx.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3fcuzvmja.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3vzcznkgp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ganmiiuc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3ghjadajh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3zylvxjgg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3yhunjgrj.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3xtobduut.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3bguofybh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3utvawgjz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jycilhnk.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3udfgsdke.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3lsfqlxfu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3vomjdfbd.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3puwulehu.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3pdnbvnnq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3legoxodr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3atlgfhml.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3nngbmlvd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3vaqedprh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3hasupwke.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3yzpuaqav.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3imwlhfmr.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3tthfpzdm.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3tycrcrit.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3rnqmunab.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3gvocnhmu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3uxyxtpaw.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bqllaleh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3unadkgpo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3fxuktllq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3quwmkcoa.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3tvawzldy.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3izcpvntd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3odajqwqx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3pyxhnrzg.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3arbyqrmy.html


<!-- 参考信息 -->