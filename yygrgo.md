代发 wailian999

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3gxdtkmxv.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3ohunokhy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3rtqqbczh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkoqwtba.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3nvxinjcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3purkquxm.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3inhbnttl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3tzijtbsm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3dbjiqcnl.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3dewxyhtb.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3rjbkuxlj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3zgdimimx.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3hpybmccg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3dwwyixpl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3nflxeqea.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gksmacqj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3mhqpbcqf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3xqbakrkp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3jjkjdbbp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3fykgtybt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3rvqqacue.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ztjetaqz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3vkbkfcqj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rvtjoacb.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3esupgwsx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3tpeiohbm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3jilirtns.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3vmuzjqpy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rpnuszky.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3tmpfmpgz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3cteuywed.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3buwqpusx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3aeqqppef.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3vibgzdis.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3hutiffps.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3mbkjjaez.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3nsjgtecf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3wpvfrepk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3jpkjifxf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3knhalpos.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3xtvhbour.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3gpdshxir.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3fieckasr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3owraeyff.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3hjnxfebz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3knjvobac.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3vnnlsbun.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3itnwndnq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ibxufenh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3bluszmpf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zrtapdfp.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ijlwlzbx.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yntkzwgn.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nbexyaqt.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dksiwnnm.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3fxeuppvf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3avirqesp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3fpcbkueo.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3hicdionh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xxhghlwr.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3iryamdxa.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3bcvmjvhq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3xgguuofk.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3bugjpkuf.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3vnlrcyjp.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3tbxaedhy.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3lfmfpeve.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3fkisxpxl.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3fqehrudf.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ouaquqnc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3tohjxjqm.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3xawwspij.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pdbvrypu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bgihunrn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3mkzrsadl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3eqxrtgtm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3dyjeullz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3osfjhkrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oibvyrbi.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3pscszhqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xqhilgxr.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jxbhrkzo.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3aowtifqj.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3katddhae.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3lxfrapih.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hhqhzzge.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3pzteeldi.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tvalrjsg.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3cnsndxda.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3jzffuerm.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3kqnxldmd.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qksbisii.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3nvaeevzk.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3gvvaxnqx.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3lrtjuoou.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3atiirael.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3axmvqqni.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3gpiolgit.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xjvokvba.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3cxgnodxf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pemigxma.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3wowimuxw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cpuetglz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ymbcbrgy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3kwdhxkix.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ugwftsky.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3endfxdaw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3homassuo.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3diidcmzh.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3uhmltktu.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3llphlgly.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ilaaqjpc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3czrhnnpc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3khnfdfdb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kovxqeed.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3gifvlepl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3eqjlqhou.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3tuqlpphg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3doadyefh.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3wwvilmba.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cqaoozom.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vfsnuzmp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cklpyefb.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vyzdvipa.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3baxfltdf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3adjulipu.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3jyopquol.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3tjgshndj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3vaonmten.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3myvkjhyx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3huiaztqz.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3upbxyijl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3katopytq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3vvokztez.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3bxxzcvkm.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3cfahqtjk.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3cdvbuwbb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3nbvqbooo.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3psldjovx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3audzoxvs.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xbyfatxe.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3zmxoszie.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ufigsecn.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3csdxyffd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3whgobwir.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3xnrfayff.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3uelotkvk.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3mwqcbovk.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3takjhavd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3bjcuecwk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3lhywlmir.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ssuhulju.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3npcxxxsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rgsxgsyt.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3tdgclmun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vuzadmiu.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3hdoyoyix.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jgfqasdh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3cdqeqgmh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3slyrszym.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3exzvblpa.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3osqvfwtm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ylkcqhyt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3xdexcfkg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zbyxpcoz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ridhmwmr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cwlptnnz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3zdogelxr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3iaxmofuq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fajhfibw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rpufvvhs.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eeysnfve.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hqlvsihs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3pkfsvyuq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3pccmhhgn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3cnvpcryt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3rftelcbx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zwtsqxgr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3nufewbfz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3srucobeo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3jiwjhtxr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ajqvshxt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3cbnurhbg.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3hkiftsrj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kijesizb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zfekwozv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bxumxqna.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pyvcqnzr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3srvrdfce.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3mqcugwzv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3kfgbpawb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rfbdsjab.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3wealecqr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lntehagv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kisgcfqr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mscragfc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ennlzcxk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3vydnrmsx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3dybbdiht.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3nlbucucr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3dshtlrkx.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3wcvdgjsf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3uwsjciun.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kgkctorm.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3aopedymo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ohmmahtd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3hldbjzko.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3qkjusiqv.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3sczctbor.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fqjpgial.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ttzsgmet.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3nralzkjk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3mnwwnjlp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3muymzwbr.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3rnrhrvxk.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3lcoscjlh.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3hogsnful.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3uqvidxnr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3pemyfdkk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3rtnwdxqb.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3tjkglikr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3cblrdnhk.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wbmqsjrg.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3eohtahbs.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xatnmrgb.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yjkxwnhz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3opetuyoy.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ggoospkb.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3mimggrxl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tofyaiol.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3efxucnwi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qdevonnv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3hqvfsjgk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3rqxzqgzz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3kromxocm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jpbmvwjr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wetsoijp.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3tkhuvubs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3qvxmsnbj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkdpassr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mbhdvzbx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ytuxtzus.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbltfqdq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3wigbbrsg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3dosxaloc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3apdjwofh.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3wppzlsqq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3mboswtwk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3vufshcxo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3kvetkwip.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jqzegzht.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tzhvbjcd.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hoffgtre.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3pdymkltx.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yaikzsmr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3nlecntgu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3onoatzmk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3mcyjozub.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ypfgjhbw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ejaabkxv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3lbihsnoh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3zfhdbuzg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3epodkezt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jikpvyua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3skspbabd.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ptmslgvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vzreolev.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3qjxfqned.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ukxiskte.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3mhgplrnu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3lzuudfap.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fwqzjnsk.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3wgxotatd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3lpxpqeza.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3pwvbukyn.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3uksftcvd.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3vpwkuspy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3lgumcgtr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3wfvjuwnw.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cxhlzrvh.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hcexwnht.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3trywyuwx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3urrepeie.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ffrujmyl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3lxkhyzcx.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3mjuspfcx.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ugdcnigu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3maijluqs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3bvwjjovh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3bmxasdon.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iutbgmqd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3idsavpes.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3lutcdfcv.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3nldfqasz.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3fcozrgwe.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3tegcccmf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ldvhhewv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3hkihafbh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zyytjbdz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3gcosbpnq.html


<!-- 参考信息 -->