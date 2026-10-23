代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ludtiwoo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3cgtqelkg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3pgzrnlos.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qpyxkdin.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3hiacygwy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3pjxvbwrp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ubtffshk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hhxlwbjy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3opoemyta.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3moslboep.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ooprwjmq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3tpkynzko.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ypvkccfb.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ygchmwsp.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3qllssygd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3xcgjuqhd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3mgccujam.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3cunyrtqp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3fikrdthf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3naycqmvg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3gzzmhgpu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3gwppqdan.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3zmpzzwpf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3odistgry.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3kkxnqvye.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3clrjvpew.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3idbyaqol.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3tjdwsqwq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3aoefpkyg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3yuqpouqn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pgorrldo.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3eauaofhg.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ipfjkjck.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3lthbafyv.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lryzaqvr.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3diypyjso.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wzwgaqzs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3mkxeagco.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3iwanskdw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3afoueuxo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vbhcrltl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3oajopkaw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3tlqxudiw.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3cftgjavz.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ftcnwipx.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ebkotabv.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3knezjlew.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3msyzpkqt.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3dtxjjzck.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3qexdinvo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3qmtovrvt.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ueqhvgmk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3dynssurx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jaxrtzvf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3lzrvcucq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3hyygrvok.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rcwcabwf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3aaohaozj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sayfmggv.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ejnpsqui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qfcdcdpy.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jzsyxlfj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jfkqkpte.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3jawwxnhg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3gmqllihn.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3bsiisgqo.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ewvgsmtz.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lsvxalaf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ufpfbdbh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vkeioazd.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pdtsrxzq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ototvuze.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qjpovdbj.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3tevpucrd.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3rdgucbip.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ixuwsfig.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jthcqboo.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3eoaoygmp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ubwakirt.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3qvbprpvo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3huqnnicp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3boyaeajh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qffqddoo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ztcsawep.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3oudjvpxj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3fkynnogw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3bsexrnbd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3othkwdpi.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3lrlluint.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3yfuskuxf.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3nuinnfbu.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ziprrbgk.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bgmadhwa.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3bxqsyofx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3bvvocwzf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3zjbqrszj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3cvunkshp.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3cjxtwbhw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3oquaqwlo.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3hkcvmxee.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vkyfkurr.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dxmfirud.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lqqsfsly.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3aspyrnhm.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3bquivapd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ljvclzfj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3hjvhbsev.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3odzzzwcf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ktnhjxui.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gdwnzhns.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dxzmazrg.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ubpwnuwk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3oqiackic.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ejtbfedb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3uousfaln.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3uzxzngev.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3zblumdbi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3rsasvpdv.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3pdbcqajo.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ctmjxkxc.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ecavvcns.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3qxvjjzrl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3zvvdniuf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3kwhkgztt.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ugfcwfrh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3rhmfvfma.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3vhljpsdd.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3lfyrnqmx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3pphjgglp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3hdwyffav.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ttdjpybr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3dgiyrngl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3cbapeurq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bcxcudbs.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3gyciznbf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eyxrwfey.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3fiqbsmuk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dyvsrmlz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wmgciywj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fcxxvtiu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ydivmbkq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lwzyajlx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qlbtglma.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ppcpldrw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ihkbhxkq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3drzwdvcn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tqzwmkop.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pkhsirig.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3sleehmer.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3penplbof.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qbalwusg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zomykjir.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3njgzagsy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3rxutbnms.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3bihdwwcm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3mkniwwbb.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3cjgilapn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zfjqmfgo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bowvtulr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3yiieykkz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3liufmqyy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3qcjffolq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3iowgvclu.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3khmrozcx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qkpbpzae.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3whqnvokq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rhxrjnpw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3edouknpj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vayjvdia.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ltrpycjy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3mfosuqqn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vpixxjzo.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3vcrpsbnw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3imlxnqjk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkjqcddq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3llakcksc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3txmcyrtk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3zuxiqvgz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3keihtbzz.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ascyrgid.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3icgusidr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3cglydjob.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3psjjsafo.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3nfamurom.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3awjllcue.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qzibfnow.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3zsnolmzr.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3uzauhlwx.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3grndcfhs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3fwzpcsfw.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3yesmzetc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3obhndrju.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3wmjbglvs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3dqnqbfsw.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3rytiiqzu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3kgopfwab.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3lnupheld.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3gqxqoaov.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3wmnsodxt.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ojizzzvq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ckdotsoc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3prieodep.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ucswqpjk.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sqaqahbg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ohztyylt.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3onbbduxn.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fsnkkfnj.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yjoezxtn.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3fsghyzlw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3rvgguhxw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3demuweqo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qjjftbkq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3lygfmrvw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3dgxtzxcd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3eqdwdgsu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lqlfukvt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3qmksgbvf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3lndmqaxo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3dburzncy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovgpdjkr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bqgdolgh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3heuaojyr.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3kihcanip.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3uuugjqlz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3vvuiqbmu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3eoqjpsyx.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ebqwuaok.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3bfwlfawz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3gorcptvf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bfosxggo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hsmvzqeo.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gsvhvsjy.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rtspgcik.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3dzhjdplj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qqwukotf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3rkxoflve.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3uedceton.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3qaegmrxp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3bdgtwdto.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3xyotdzpd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jhfmrxff.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3yljcuykt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wfewqnhs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3obqpcfif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3racjkyot.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3tlkhmiwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3usjbpouy.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ikymbqxw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3eooahszc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3apxaqmcb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3skntwzsf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3dgmnaqxw.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3itcfgndi.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3mwbjatvt.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3tqlvbpzv.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3eghwdvra.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yrmfhkkj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3youbgzfb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3qkejvorv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3hhyttkqy.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bysqggue.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3vixdkgla.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ptncazpj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3oktjqkem.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3shugwuqk.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3hbocxxsh.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3rymsrbig.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3crfpuhks.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3qayvwxne.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3apmtbzjq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjlcxnfm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3oyffeuje.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3qwcbuebv.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbhljfsu.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3xtlywixr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ampniedr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3phkmjvuu.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ogktgzok.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ircgysym.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3jflrwopj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3apmiolnq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3bbehnozg.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3zgkazyhi.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3gkqmtrxs.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pyciejkr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3tafzdheu.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3zdesscce.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3efpsadxs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3wfhyvzoz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3mgoitijk.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3latmbfew.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3akanfrap.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ejghcepf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3qwmgkuvo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3jtblmnxu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3aqrwesuu.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3gcoljkdv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ygskkisa.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3aytuuxep.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ztehjtim.html


<!-- 参考信息 -->