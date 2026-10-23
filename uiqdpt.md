代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3cxqlmgvx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3zqjcedwq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3nwzgacdl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3dgsdsvcm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3sofxmnfj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3huknawau.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3vxobinql.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ebpsbguz.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3skhbkezi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3hnpcqzow.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kzahxzaz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3jepqzifb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3swdifikv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3gkrblkqk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3sqsjipyd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3hyrwjdtj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3wnfdnbqx.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3dicelyne.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3zrjizpgr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3jvuvnpoo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3pbfhcdij.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3hoobplzy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3pqmqzzur.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3mtcciczu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3cawdzpwv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3gkixjttq.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3nlwlbjfn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3fwopxfas.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3tgqyznow.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3kpfcfjfs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3jasjauce.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3vxtmyycn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3pzjcfajq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3lxghksox.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uuewtjdi.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3zgqbincg.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3topwidtj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ulcxbcaq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3nhzuqpzi.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ukbbttwq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3kzjhgbws.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3mbgrdlpl.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3trrrpcnx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3jaxoeasd.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zihykxtu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3qavsjupc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3gqttlojj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3dniklwmz.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3csnzaxmp.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3svhjvzaw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3rvjmzmfp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3zjfxbkey.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mljgcsac.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3oujxyxrc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3aycukrhj.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3vechvdin.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qtxgulcl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hrfedybv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3ysravpyv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3bvakkrvy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3nypwkvak.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3rtyouvjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfsjzmna.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3rdwqcqtu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vmgoshrw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nznpkmyj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ppgfdupi.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3qivvjcpd.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fcuqdoeg.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vkpnomad.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hyrxeptx.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3pkwuxipu.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3pcsraoct.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3urawgwjw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qejaubvk.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yaayctab.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3uhqxukcq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mnquyhji.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vdqvfzfx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bbytcjoo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nuijwweo.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3zoridnxd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xspwbcpc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3eihhduok.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qwrvsbht.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3pifvqbyv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xrvhokhh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vnhfouiv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3dhjyusrq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3mikqfmka.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3rmcpmiwu.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3aqidunvl.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ficzflcu.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gjmrfakr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3xuarfmkn.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3txtzotre.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wkeevaup.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3qbxgnoho.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3wibvdyco.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ffvpqtmj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3eqdyqoqj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3nuqtvtub.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fcyynxmt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3nkjlmxgd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wdhfhjpe.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gzhispkg.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iokxlmxb.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wivvmmdr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ehvqzchz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3yaaclczv.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3craigame.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3zuccouwx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3cjatcned.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3nzdfhwdp.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3reysmfvc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3prsoztsc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3saqiijra.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3yhlirzgl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3zvxjpwqs.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3wxizqwth.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3jsefbady.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3wakhispy.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rtfvylgp.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3uptjgzjr.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qflclpzg.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3shyhxrsh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3gqyfzfec.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ciswmgap.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3lttbchqo.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ziigbhxm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3sphirqzd.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3iimwyzoo.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3efaegghl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3hjpgxyqn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ajlzmaue.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3vpnuiebe.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3misyscxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pbwfedqr.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ucrftnqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xgezcgxc.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3whqfnqxb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nytdqmyv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ntewwpxe.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ovymstwt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3buurgxwa.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gleyphyv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gmklhkgn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3gnbphgsa.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dpdiiqdn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3pvciylus.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cepkvaog.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3faqnoyto.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3znuqpevm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3oinqaajg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3krxmztql.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vocymrif.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3sjhuifrk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ryiufbbm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3knufwsnb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3oppdbfmz.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3crxapmhn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3sibbtbth.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3oatgggji.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jnknchyv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3dmhojlod.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3lwbgxaqa.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3mdtqdrgg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3vqrpudgl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qkwkywjf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3kimgbvuw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jutufjoa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3uvlnzegj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3plwnxnub.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3xmjzctei.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3tgkiejcq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3maezzxfh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3engtqmyf.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fxeutndb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3obcdmwhm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ydubhznu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxevlfkb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3awzizwmd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3lzdrrdou.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3mtvjgdao.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3wletoipw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3heengush.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fawadvbr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mogdlnmm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hzsozuoz.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3aqfskwig.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3oodjuzwm.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3dnqpelhx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3biieqdqg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3rvfouboo.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ldbzmuis.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3kqaehhxs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3qsztceej.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3rqguspjw.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3bumcblcc.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3oqphorgd.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3nsbssdfi.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ubxnrjxk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3hzmbkxrp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3mqwaevuw.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3rmowzmbn.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3xgvcmyke.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yghgslzn.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3efozgsfg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3golfugxm.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rhppzqxk.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3mrpbprai.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ymacypop.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3txwoseta.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yyyhsmko.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kaxsanqu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3selcaxgv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3haqbvuil.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3aqayxjhh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3axupxnst.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3frtqeibl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xqpekprw.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3majdestl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ocrspffy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3vxvynsoh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qbssztjt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ztcihvom.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwvleria.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3utwmhife.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ieubkwsg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3uttgqixi.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3uuihrynv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3lqmuxkrn.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3plrwlyqa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3iwmxruok.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3avlogwbe.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lrebcgfy.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ewbrggjj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3rmmzvoin.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3nkchnigc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3cmnczttd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3gpkwldgw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3bqhmudgc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3yfbezkjt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3uxtupjfz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ihybxqlm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3nuqfajff.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3muikumbl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3regamsvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3flifhgda.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3nujlfgkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gqsnctva.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3bphucgpq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3nzhcmjgk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3fcrxoyxp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3mkygqhox.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3dvcwrgdm.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3enwkvspa.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3tgjwocpf.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3mywgqmck.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3bpmyxtzr.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3cxhlgrlx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3pjtmdwmn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3nbtibsey.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3iftjqauu.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ouvxmvha.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3fgbfuclc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3adkaqmhz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3zaaitlsk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3hmnqajcv.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3tighymht.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3rcinletx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3rbliqrym.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ttkdbjfn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3godbayro.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfbpykwp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3styppndq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3veydpjdt.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hyqcqhyc.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ushuyujt.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3wtqbhddl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3hknfdysc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3giarubwg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3muvlioro.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ewpgtafg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3nydhjgts.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3cefnfgmt.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3krmpqzzm.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3opytkofu.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rowuannj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3zfhjlkvn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mpjdvjux.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3vckaoptt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3pipnghmo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3fogduwql.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3aftxatud.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3aaoqaiuo.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3dcrawduq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3izgqwmzs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3hzniqcye.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xfielskr.html


<!-- 参考信息 -->