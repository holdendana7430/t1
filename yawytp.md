代发 wailian999

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3piytcgkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hogplxbq.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3dvjexwnc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3xmitvorc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3djoukjep.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3lgdctfby.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jzqetnqe.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3ufjnsmen.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ooquoppr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3kdoveage.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3gdclkhww.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ifsdkjwa.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3qslvvipj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3fbxphoar.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3viybjhlb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3pefuasqf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3vjhptaoe.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3mnnzmjje.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3odhqgehm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3xgslrvub.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3ufrkkayg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3wllfeorf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ybogxyza.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rmneewrz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3xuocuwtt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ktpkvomi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3didrlcbz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3fevpygad.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3wbtbuadh.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3lsoukzzo.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3fpqmfbif.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3fcvjfpec.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3uuultqtx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3mhvwjebs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ybfixqkw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3srxaltxa.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3lfaosdhq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3wqrlrjrf.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3wqfcuyer.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3oppbwuef.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3kodisink.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3zlfylrsu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kovvcoqn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3eohyeirv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3obgkosvl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3jzbehwbz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xtvzwjum.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3lgivzzud.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3swkygzqh.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3udbueerm.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kahifbez.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wpgjphbe.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3eoqautig.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3zyladoeq.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3sucdarqt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3vbdhsyqc.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ohwwilka.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3usukkldv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3kepgejma.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3bfyzqeao.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3kclizozu.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3otspxyja.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3wydecyyv.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3fxuezsej.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3rkgmtzhr.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3nydbatla.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3yketqmyx.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3gpnzghxl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ttsofeyw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ydovbmub.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3cvafbntw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3hbydrqqi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3kadqmncx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gtktqtwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxfsckxh.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3hhydycuc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fikxvowd.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3iumqmize.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3cnolqhtv.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3odforgxi.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3mhdochbp.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ebcekcji.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3wxcnscxs.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3yuncqzhd.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3bldpudqp.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3pcxsmmmg.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3bwoioeae.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nrlywrjr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3dqanagzu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3lfjnalol.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3kwyadiqd.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yareiokm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hhafawsw.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3eqmbnmpn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mkxcjcdd.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ytttdvux.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3qmfqwrsq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3usvizupy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rjemwjjz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3bazrcuft.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3jmrbqffz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3xccdwbge.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3isguqwhf.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3fbhrfvzm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3stvvfjcw.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3hbfzapqr.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3nhfxzbmc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xcqlaaou.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3udzxuhip.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ypjdzxfp.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3uolbnvyd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3umwazofc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3yedwzkhv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3azllomjw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sxutwmoa.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3nwyqovrf.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lmeymwop.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kunhlhzw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qxblifbx.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yhjeidyb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3rdxwjset.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3spjshyvz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3oshkogkq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3nymdtqpx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zhacaofi.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pvbrosjr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3okibnuaj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3djrzynky.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3dyclajak.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3nzpdzerx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gbjwisno.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3hmdzsgiw.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3lezzfxik.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3whuheydt.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vebaumxs.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wwkmikxy.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3uenqbgow.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3jsmldeod.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3eobxdlij.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xismjaup.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ieqnxiem.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3jwgyvkjv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3gbjtrbmk.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ipckuzmf.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jdzdeati.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3phkubszu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3zcvsuddn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ewtpkcop.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3dkzfwjqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3slshodid.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3lynsstav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hctzrvfo.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3nhauoope.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rhxkqoah.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3iiucchod.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hucelfqb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3aztovhwh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qftmrmag.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hipkkbqa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3zoanmrsb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iidtpihh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3dfhvehtv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ovqgyfgi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3xqkambsi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xlpezuba.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ohgbhhwe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3gzjbcmdg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gkgenerp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ugdsjotm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3fbtjipdl.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3xiyqidrx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3uusbgwma.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3orjnikdt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wjfdzwne.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3hztaypvo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bcstzeky.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3hbbxuisu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3dbiuiqxt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ifefgujn.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3mogzpuxi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wcnhrmas.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3nrwqvkxq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3urruvuno.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wppyxvqj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hoiryhqg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3xrnfqhnt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iozxalqg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rllmnfox.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3kqqnjfed.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lqbgledj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3emnrnzgw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwlvqscv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qhdzocze.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3whpoqfuq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3skqeoega.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jwjnluwg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3qzzyqzwf.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rosyxufm.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3vgvmrgcj.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3cntaygfc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qmyephym.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kiiqiefr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ubimgmnc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3fhqnrcha.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3aqpcyjnq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3tqautrmq.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3cysanvfn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ttzgqtxt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3kwynaqph.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3obdowmmg.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3lkmzitrc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3kruwqefh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3pidfxagr.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ccouuskw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3rldacgsj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3fxpoqmac.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3vewdjcna.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3tvimbqgb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ruyxmsad.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cyziekrz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qechvdyb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3caqmukvw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3geqxinll.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qnvmvjjd.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3isebdmdf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3rekcprpl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lrmmykyn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ucckbbyd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3eqoppqmm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3etydbfez.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3whwkgnmu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qtnhzmgj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3axcxpgfy.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3cspbzrja.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3hpnqqphj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3dttkpzpx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kyfvqjwy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3fscvsnvx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3stwirdkq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3sdkxvzny.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3qsspqczl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3uqsobdek.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wnbffjuu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3pepjftuz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3aomqmiwi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3muwwcgln.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3zdgiziqy.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fylszmxd.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kcatymov.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ipplsmha.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3blwnacxp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3yracdwji.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3zzwymllu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3erilhofv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3bkrxnryg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rqvurfxa.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qdmmiltz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3ttjvfyor.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ylfuclxi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3sycshhhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3urefvziv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3gkjkzrfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jiosedqp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3mcrycdva.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3zjcvqchy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3dysdqkwi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3unkyqmcg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3pzysneqd.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3dmirotup.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3hpfcgicl.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3inkqprcv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3hrivlncr.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3amtysxlg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3dmqyhqwp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3fprivxsf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qfuuczkb.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3aafksxpy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3dlshfkvz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3bcajlctt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ajlzjguv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3qqoqgcec.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3qyycwdob.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3bnyeorbv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3dqmzkndl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3mmijqzts.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3hzfyomcy.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aajncsfc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3fcdelinl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3bphjybsw.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvdgcgbm.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3necobwcl.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ckpjqxvp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3hjdcnavp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3uxglqkqf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3eiwavmdw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3fapsjuti.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3hxzeqvop.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3nnguuues.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3lsfygymm.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3vnlsumem.html


<!-- 参考信息 -->