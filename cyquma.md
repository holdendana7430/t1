代发 wailian999

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3jbvuipxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dfwvxbfy.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ddubtwsd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3jmtwhvts.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3voegoukm.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ynoihcxh.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3nueqjqpv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3wcrwalnt.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zftydjkh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3rnsdzure.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fssnvcka.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3aspdlaca.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3zaflfocn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3embxszub.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3dcaqqvpp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3yprsgkgt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3kvisscjs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3qwtkxeqg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3aohxzhxz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3hjewyqas.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3qmmjxtzk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3kzciqdlh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nktvqrcv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3alvismde.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3tizjmalt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3fvhqtixs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3zrisydum.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3zfrqownf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3oqjzxhfa.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ynkewgyn.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3hkodhucc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ygejgioy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3agmchxhi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3cmkecpet.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3dkolipvo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3dswmvwns.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3gpqthnza.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ojohfxfs.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3gnkwrgie.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3sdqprbyr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3pmkznsqe.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3fvzhykxp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3escgmmzj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ijybrxho.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3bdknrfoa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3hruraokl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3keunfndi.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3sxdaomwb.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jbtthnqc.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3hlxinrwr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3epecnyqs.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3blbuunry.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3gwjedtad.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3syselqih.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3yhvdzzfs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3batetvye.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3menbjwts.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3czbwtjax.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3owtqrkpp.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3tjhsbnzz.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vumdxpwe.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3egkmwzkp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3odiftydc.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3rftrnrwp.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3esjbyrei.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3tghbsahr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3tgmihzns.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3mjqwibdh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3niahznzt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3eciruphg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3njdqabjh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3haluukxj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ecevcnzl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lqldwhrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cuqbbzpg.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3whrpixwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ofhdojge.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3seubebcr.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3zazwawha.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3zyrfmyds.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vhxvflgi.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3usuhsrmf.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3gbcvzlkc.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3djtyhgrs.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3gexlbdov.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3yqcvcbbk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3jrhpokip.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kvuqbkvn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3baqizmry.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3adqqdeeq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3blksizbe.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jpsfzvbl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3exqageho.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3acxfnyze.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sptrsdpr.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3smzdfkop.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ktocyceb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3zzvcxwfy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jixgiuzc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3hvfuzttx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3legbpjal.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3hdsotede.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3pitdyvgl.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3mqjibetl.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3gvejmzag.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tkhiimtf.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3yexsqwkx.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ypuqcgrq.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hdiassgw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3yuczpfes.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3sdviefta.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ozhiholv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3rapjqvmz.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3vacbmdcs.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lonqpsts.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3cpxrdjks.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nklhhraf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zuqvalrq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tdtgykyx.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sdsncaaz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3luancxop.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3aruyxwlm.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3sqklzwyc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zutrayhq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3cfmcormt.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ncgxmfkh.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3olppflib.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bymworxr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ditnejru.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3rssqznhq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3yxhleaot.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3bztczwfj.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3oaplejjr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3yjwyvwfx.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3vzukgbvx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3aguyseir.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3osrrfghq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3apwkfxit.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3topheehn.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zspzzbnx.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3lpfanmgy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3zkazmxgt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3igdaolbp.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ufndhvyy.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3qkfbaygg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3jhjwjral.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3zxglzsqh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3czhqtnny.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3zcuuupvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3niydrljy.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3aiodngzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jsgimkxo.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ylvnmmzu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oifgsrwn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kioknozn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3oohhxlyt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3djkphqsp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3inluccmm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3msitnopr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3byfhtpzr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3feucjtwi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3htovepqx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rnlscboy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ekzbvwqk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nfvacehl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3cqstdsos.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3wajjfqbg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eziehhbu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ctpykwvx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nuyawexi.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3lwevyxgk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3mqwktruj.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3wkuvqwbo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3uwvldvdc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jsgprtvx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3berjfraq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3wycuqogn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3fnrsuikq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3icjinrqd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3rznlnhgq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ofbgakkm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3fcdgatbc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cunwthfq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kgtggygu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfaspbkm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3aynssikd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3cynsenni.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kknfwyou.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3xkrxqfxp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3uiyricbo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqpnrehj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3daarddja.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3nlooflmi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3qkrrojfc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3qhussqlw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ehvmcprh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3nkobylyb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qlunwfoz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3spqgtrrb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pdunghwd.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wpqaaeeb.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hbuqidvi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3drmlxixo.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3liwugrnt.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xcwcknpr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3wmimlsxu.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3kkevhlgb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3qnsiiwqq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3pjpfkyvk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3qamigwvl.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3pjceuymn.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3lnmgdclz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3atxrdbsm.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3liqqpevz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3zqocbfkb.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3wqgvpjpr.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lnfoacxb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3bvqbhqqj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xseawbmp.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rsyiovzv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fifignub.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mxoozxcc.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3znsgryhv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3odwkvgce.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3kzwurctd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3luaxjoia.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rvudrkej.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vceowxlz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3hdcgjrbc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3oxiifmxq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3mmrlpohz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kelsbirp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jdtozmde.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3kaolkeqc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3vezgfhjr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxnffmbj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3kkcrwyxv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xheyidbh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3rpufxapy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ikxjldrp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3zoyfxxai.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsuqxgee.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3otdaqrgv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3pqfdvuti.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3krkvcact.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3kiagauja.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3pjfosxjp.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dolevrsr.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3eqacbfkf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3jimsqntg.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hhjrqyxw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3vfztdbpg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3smoqboye.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ljipmbek.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3hbztopmi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3uqtdmmtj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xnwcxdfb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3seufoibe.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lrnbbrqh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3asphdpxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqigdfvu.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ncwrbtci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qthtqhcq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ixicfvyu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3yrxemclj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3zqndvalf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3pynqqbdr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3oqlpgywb.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3xyypppzl.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3hsfqggtk.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3vihsodmb.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3garpbsxb.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bnfbjwfx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3dukohdyx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3wytybwak.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3vuxbdzsu.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dezyhkwk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3vhnixyhq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3abkgnvcc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3dzmptrra.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3lloqnaei.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ozrtooqu.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3tzaudbcj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3vvcphxyp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3jqznvpto.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3tllvqvfm.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvephyxo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3mfwozhgx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3bpvxpreo.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3dqdlvlzr.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3stwwxowa.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ucrhbzky.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3xytdteos.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3muwmsdcw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3jxujrohl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3jctdibcg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3plhmbfrg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3pkaeyzlw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wosejorf.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3rjywgjlx.html


<!-- 参考信息 -->