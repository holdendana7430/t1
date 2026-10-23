代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3zhevvtbo.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3rbmlvmya.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qaylkajf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3sixmhlce.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ifemwqou.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ljvewsol.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3jlxwgmvl.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rjxduisf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3wtpaanyq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3hlirfffh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ygldbrhr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3qcrmfarh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3dpcdkdho.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3lfscrixl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3zfzhbtzl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3gqulhyup.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3lnhduzow.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3mhhxgcff.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3gtbmocvh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3drmjmzkb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3wxrveism.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3tlfvglem.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3pnwcibvb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3pqwembqy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3iizdaxqf.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3cewakihm.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3jyjkgqkn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jnoqlcuz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3wlekgpve.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3jpgkxhxd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3upisfljg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3uxzmvuxf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3ufaifznb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3iiedaoip.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3bkbiomnk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3clnpguvw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3lxcajpdq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3hsqifnuz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3csjwtmuf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3eyqebutw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3qbwfloax.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3gzwouflm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rmbjkkex.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3edaayfyw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wttnaxom.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3zrgxztld.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3uhmpwmmp.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tigxtnod.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3hzbhpsmi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3zljuaxpq.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3pegenuac.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3rvbomcln.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jsjblruq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ouvjeeqk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3xakmostb.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3aowmvuhk.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3sljwesvz.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3diezdsvu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3lrfqkupi.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ocqfpjxk.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3qgjwqksv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ztyswlro.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3sthxnlij.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3szndeabv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3agzaxaij.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xvmzfrmp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3dftbxvyu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3aekorevm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qjakgeib.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3rgayvszm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fkjbfopq.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3czweecyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wkedooxe.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3mqyjicdc.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3krdkrpci.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3jvgsuwzw.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rmddzinn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rdxtipnx.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jfhasbmy.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3igbbzlvr.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3jasfgmsy.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3bhbnzohw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3tcwmvqmc.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fotvyhcr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3fnorvbch.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hydioobj.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vylzivmk.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tlarycub.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3uswtytvw.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ofotjkvt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zvpxexfq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3cgvyvhpk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3koiicfob.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3slhwjsns.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jsvxvqpm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fpcemnri.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3yonbayud.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3cugsshbn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3shpdxrja.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3uvegulng.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3kpvdqzdb.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ibskkygw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3uauyfxnu.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3buchwsme.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3egivbkpt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3qjengpmq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3rmobwytd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3hswuembr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3bapktdhb.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3icvpnzca.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wdlavlau.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3fpfrbxwa.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3oykhdhud.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lckucxjd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uhltythf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uhfjtlag.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3bjdtnfsx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3timmbddf.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3bsrrgeqk.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3muxrybzx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3uvzwumjo.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dgkmsvxn.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3btodgyzh.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kgqjtiyy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3hdnivova.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3rtfwkqzs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3xrphyeti.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3habcxmwp.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3obuxlkap.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3jtwaqdns.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xdakzwbq.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qepvsyqc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3gcnmsswa.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3hrpmcnlt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3cdynztkd.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3lmajwblf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3edwtcqrf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3cfobqrfo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3jcqgemmg.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3vamkedwa.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3fwwvgjqz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3nabafygw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3hiwgoyua.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3xnboekgx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3vbuxwfnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3veizsjsr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3mcibvaof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ypdacgok.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3aefwlajy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3svnlzcsf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xdojpnxq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ehryokcw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fqwvhocy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nsmcvwni.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gbzxenpe.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3msjnbgyd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qsqencqb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ypttbist.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3akrdykha.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3hgixnrgd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tlcbthmv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ywngewiy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fwkxmfow.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ztjgalgo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3hsysawyr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3eyivrrin.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3gygnqidc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3trzzynml.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3pdqcwlua.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3cuziaupb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3xnrmdelh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ronlvsaf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3dqrtsbgr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3xkxefuhh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3rmakppyk.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3hfjgvuil.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jfuextjx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ngvlnfqt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ygcqjmuc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3npixyjpi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3nxtdllaz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3orqseeif.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3njronmjf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ggxzachz.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ouhydcfe.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hwwoohla.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3atzobhkt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zratpzxr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3mnyfzars.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3tqcuoggn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3bqkxjrso.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3wwqfohqd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3gpnnuoqa.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3syfenmcr.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ozvetqqe.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3njzxhtmr.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rreyyrcz.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cgmgryqr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3otccvsnp.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3kibsbecq.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hwvckxdu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3oajfowsl.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3paydhxay.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3obykquux.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3udipkkvy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3nacakydo.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3hkykrjph.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3sjwvqtvg.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ovrrhzan.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3retwgbgu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ljrmrhit.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3qxyqjelo.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3fpzstpdk.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3wnmjkpvc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3twnxsocf.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3shullaab.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fveelrdk.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zvxhnfor.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qowfraik.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ioxjhhkw.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3tcssllmp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sixteohm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3djqukwxv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qpzjwebj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3gvcoobjr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3nvftujvh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3niomirwx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rrzghuch.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3wjbkszyx.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3zhuhqgav.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ocvwelxa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhlbawmo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vskcuczy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3tcabcwbe.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3recudkdp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3yuxbhebw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ombnfyjt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdfbyukt.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oemfnmpp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3stjvzspo.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3slebaiui.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3quyubsvv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3vbldwjii.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3uzjolkol.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3eonumzoe.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3bhccrvdk.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cwmgwnmy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3bfjzlkad.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3hntdrxdm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3oizakemb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3jfvcjgja.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rebpmbmq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jnnueccx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3opmmqeku.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3opdcnahk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ehqhezeh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eddkvngs.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3qrczesfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jomewqeu.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3vuvrhywg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3qkerwauy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ymfpgtvn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3rikintxp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3sizxpctl.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3msitjbql.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3mwpxjroq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3uxqnhlrf.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3bprjewwx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3djljkfcx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3vpkxsdom.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3cfgxewul.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tymgfnmz.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3juxulzky.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lancebme.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3cjpytbhi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3hjicllnz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3gxnpwwbc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3puzzklqf.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3vxdedxhk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3kabnmxzj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3vqatqito.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3oazejege.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qpnldhop.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3hlwhevmo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3squhdqvx.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvbfkmoo.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3qeivizmk.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3xnulxxcz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3zfqxalkf.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rpngdeit.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mqrfxlfr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3evggumog.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3fpzpisnf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3stwhrxnu.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3mmkwzknc.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3elmrgdkg.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3hkxxxden.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3mkzzumlq.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3kzxxeqwa.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3cemdwacq.html


<!-- 参考信息 -->