代发 wailian999

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3gufqpyfv.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zjatpppt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3gurroxbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rwkaaghm.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3wzzmghtj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zayudmnq.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3lnnnwuzv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3nvvtdepf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3tjqileas.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zbkhlwqd.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3hudioaqj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3ykhilwts.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3uipympca.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ifrjkdjs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ywtgverv.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cefstrcd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3uvjgwdap.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3wkuplcxa.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3aqfspcsm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ggxunltt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3qglrxrbq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3nshyswbb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3lkodigaz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3mrifraks.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3egqvtfkj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3qugatzxr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3kodfpjss.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3itxbcbzj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3hkpksbyt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3xxsermet.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3vrhwjdro.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3uczbpiev.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3mkqivfqz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3exzfhekx.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3gcuucdzy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3rgnjmqtn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3larnpecn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3nglctbsv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3lksekezc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3qxkwwjwu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3lepgdogi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3cnpavlyd.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3iyzxcusp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3ivuaehtd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3esraweed.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3siuxllfs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3srtakujt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3tmapgmnt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ibrghksq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3gqryiuvm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dnhalzwr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3lwosnica.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bvtsnrcj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3xfhjignw.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dppqicaf.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dqewkwtj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3gdfwhyha.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3gpvbcrxn.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3xidbrbwe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3pocoqzrk.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xpkilfii.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3bfpjonxi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3mloferkz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ftggqtki.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3pcaqyayt.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3nbxsvkdw.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3fmouwpzv.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3iybgkpwh.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ydiioitd.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3zcoezexw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3eijmlhin.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3dcgccnrr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mrigfmtb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ctgygeco.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3lbzhghlp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ytzhirmh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3nnyszwug.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3yzpjdvpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3brrmfhkl.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3xebgotsy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3twswmbmk.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3uwviksws.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3uhvqzpeu.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3akfszjhy.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vvwqqboh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nhrsvtle.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3scrhbyya.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nxxkhuxk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3hhkbthah.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3zrkgvisr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3akarggni.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kigcttqi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3tnmkfbsx.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3lkzzupgi.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ifewqbsj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sqwuqsuu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3oymmhvuh.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3vnbeibzp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cwiwxvfq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3beccapty.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3jwvjskdu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3xwiircim.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cskgtlkt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3atbnhxuk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3tgihwpaa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ppvjussy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3drspwhfy.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ihuvilyr.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3etcadukt.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kcprzudz.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3njtwdhui.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ipsnwiuo.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3afsbozbq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3thsgzsoo.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3evqfhpae.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3sdvcbtdx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3tgetgtgm.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3djsmwohg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xibkezum.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3fzuhrpao.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fmbdcicf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3echkwxzz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qjafrzzb.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vqzriqea.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ekmmccez.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3crnhwglp.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3tcxblmpj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3quieawnh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ccpmgnsh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3quqqavgr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xemkhceh.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3walucupw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3vlmhkalh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3vnkgyrat.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3qwglgaou.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3jxbwbcbp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ttrhimii.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3vdvbxfwx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3suxcmbag.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tuzfjfid.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3oehfiled.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3jfjqzfbi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3etqfckqa.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3kxihytyn.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3suywtbwj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3majgufyd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3tlzluddd.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3xbfharml.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ydluukkd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3lnewmpnt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3wifisrev.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3bwhhhdlg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3fhwzxwtm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jzzniloy.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3jsegpxej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jlkxvmrf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3rvadzdcv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ywfwviys.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wzbijajk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3eoaicgqk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3emirspas.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jqeixrqh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bjcqnxow.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3jeabijag.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ckvtdoxp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ezzroppk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3iafgudmj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3azwpgbcd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ubkccjyh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lzkhsmbf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3hxznhdcs.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lekwszzu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vrfnmzsv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3huquzftz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3fkaarage.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3vvsjeidx.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3rnnbrlwg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3lliyrgxp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3weazavll.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3qqtfhkoh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3upzihrep.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3byqcmevu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3hmclapli.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3bzyoiplh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zkgykwgw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xwyiiuig.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aiiuznuu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3meuqhkak.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ohoftwxu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3qaamjljm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3iwssxeos.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yqkizdkm.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3jxkyiwih.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ytamitqd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3jzhnijnk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgatkzzf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3clfolieq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3flcmamve.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3gfkkvere.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3vyuqrfbq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbygoznn.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ztaurzen.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3nfdusjva.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qlhmnquo.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nrshskqw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tqgvbztr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3djshqpas.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3fevnxnfz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3irvinrmd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zzepblkd.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3zppwixhf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3smokhqsj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3irguwnpk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3nhfmvpuk.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3sufioaea.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3skfrvcbs.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3eaivyqcq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3qlaubxnj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3lpltzdto.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3xwvxlczi.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qajrczzs.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3lhcfclyl.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3szjuskop.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fivoyekn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wquqsuka.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3idhjdghy.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3vqwfbamj.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ammnimgw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3kubldcze.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3vqaxfefc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hzocnfrj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kyljxyln.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3mqntblty.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3etctkhmt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3bmweizfl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3owhzuxsw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3lmfjalnf.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3muswxzfs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3bzxzgwqc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3dhclycty.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ermacetn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ftyjbgfx.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3hlpiiumk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3jwfpgpwo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3vojlcels.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3mltfxgdj.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mnqpngtq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ygspsdsd.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3pelnycqn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3pyxssgjm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ovrxfmqi.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3louksziq.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3csxrixul.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3nauwpuaf.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fbhxhsvr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3bylykmmf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3okmbfvpo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3kqqjbhyg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3khpzzkvo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3bldautzo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3omsmiclq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ngdegcpa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ukjtpykx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zlbxydva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kvxrbent.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3nndhshfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tcuprsyo.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3nctbthgm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ofsazoan.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3oiepmgcn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3gvsywlqa.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3nmbgqxfm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3msajlfqk.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3jhifkpgp.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3zuhzjroe.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3clwsvqmi.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3avfaeqyp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ythsyjfq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3bwfrqdfd.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3svmsrfaf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qfjwmfzu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3pfgqznnp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ophixrwj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3myrekeqg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3zpbzsnyf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3tyrmcxlq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3lidkggsn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3lkcxadal.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3akfaaquq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vxgvgvew.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtwwgrme.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3dtcjqjhf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3sjrzsecr.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3tcsswxbi.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bcccwrtc.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3rzvwrmsb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3gqgvvale.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3neukwqmd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zsvtqmfl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3royxtvqw.html


<!-- 参考信息 -->