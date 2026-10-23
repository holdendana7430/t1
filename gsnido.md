代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vdxzunyh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bdcyxgfb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3onbojhvm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3rgqhahaa.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3oxfouvkm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dricsjez.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3lgangrtj.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ixmnzzlu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3pchpuxav.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ozeymhrn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3cevofhdj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3cvaikfrj.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3oxebicqw.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3ndsfdjts.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3kiuezqwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwzigvel.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3llreskts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qxainios.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3asbgexcj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3gfhiqmdd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3lnldcpcw.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3gcxoroab.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ydympuxi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3yukffxss.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3zhuvtafl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3fskqadgr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3wdvctheg.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3tvshzzca.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3bhsujkox.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3dliakecq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3joodqaej.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3vffktgns.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3pbabflgi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3fqlpxktp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3thprsxle.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3aqhtcqbd.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3cswpchol.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3yetzdjpz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3ddfxjoik.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3mkfkvtdr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3rhpyrike.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ipslpcwt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ofpmsmkv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3qlpubuaq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3aqffgcnp.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3lgxbcjcf.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3fssszxkk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jxyzibco.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3tqhshiba.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3gpsifent.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3klszudgl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3psqmhkdl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3vlmofptd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3hxwyyyrd.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3qalekeyh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3qscqyrpp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3kwzzkcxm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jwbhynrb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3usqdbuse.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3qgpyzlgr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3kylzctmm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3rduazopu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gmreanft.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3tyqhttsx.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qwxmwgkw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3xayazqgc.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3atcvhcyn.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dspdgprb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3astlkonj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3meccfsan.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3dkklhtrk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ryemxrsh.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3mzimspya.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3zigrigyl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3zvhiatpy.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3knfxrfri.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3obljucsh.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3wlavtgbx.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3sheqlzee.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3hbyugkam.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3hbqqiyso.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ftnsdfzc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3xwftngwu.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3uppuhvst.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ycxwasrf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3difljlwv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ghuptbng.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3lwedolkn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3tqqawmkp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3qyrbodfh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvvqdcmc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3nzdbflmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yawhfyda.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3turmyeve.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3tiemzjgx.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3npgrqtrv.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hqrtgjcy.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mmryzcmv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3yvlwcdrh.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3lwymfzaz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3occznikj.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3grfseyin.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3kkiuauox.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3comakakx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3yqxboqig.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3galcuscg.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3anxarzlg.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nglpqhyo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qlztwood.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3jrciyttp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dxpvnmnz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ygnghkkw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3owegmojq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3cojqkrbv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3vznfahlt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ndaeoriq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ccgkmmcs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3cujxgwbk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3podymsgb.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3pjfwfnvf.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3sfdgeoyc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3evityqfq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ogebjchd.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nolxsdgp.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tzdqranc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3pbixqedh.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nymtzpbf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3jxiersdx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3cdzemomv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3svggvuom.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mcbdkimg.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3crfehfat.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mwromlmc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kbykxiji.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qiyboegz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kjygtqst.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ozirzsbf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3inobtbhx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3rjrztsck.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3fxgkphii.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3pbuaduhp.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jaxxoijj.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3trlojjtc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3rmdgajsn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3outzelmp.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ybnupytz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3tcjkjfnm.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3plqlhoey.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3tpyhzrhm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3fvyymqfh.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3epczwgjj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ygpvrdvr.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ajmxevgw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ajjqexck.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3yokfqxno.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vinetspb.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ukiqxfls.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3zyryxnwv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3qqdqlcvw.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ieqsuvol.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3rrfonscu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3upfrjyfm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3nunsdrnw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3fnabmhca.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3mloqvcak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elradueh.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3iduezlnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rebzwbzb.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3evnsywyj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fvpdspse.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zvzzkpso.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3abhswpmo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rodjfblj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ebedkniq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rpepkhmm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3oluxwwkd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3usyeuikj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3wvnxfnbt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3tqramtkp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hrgtqzlc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vyhzrggh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3evbszdqz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3zdlldnps.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gvurwakb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jjxtquyv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fcybfoaq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3nkmmjzxz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3qkhvfmvs.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3bgokdhxo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3xeroegzo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3rsvympsw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hwxgyepg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3edvkvmjd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3jbfdtmmz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3xlqawuwu.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ipjfbtgy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dwczuoxf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lqiuuqpe.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fiuzdjjw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jakujqpd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hdnimbjy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3jazfivqu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rsxagqtp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rrcsavgs.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3culrvqsx.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jwienrrr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dywzqevr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3coisuoft.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3olbcrbsc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3roudklze.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3yheiknvp.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3nwhlnbrb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3mhcrjsir.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3jzmapuea.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3eaakkraw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3urvgglum.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vbayjrhq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3viofvhto.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3gzelytaz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3centudqm.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qfvmcqce.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3dvzrznci.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3loivjcvd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3koqcqncz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3dqvqeqfd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3bdibjgqs.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3nfklbjxy.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3xuytiauh.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3bkrkgzfl.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3dgnmwzwr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3qpfokhjz.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3jgqyfdyl.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sglfgphc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3gdpzupyz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3sklfsabt.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rbwdwzui.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yzydxsll.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rmokqzyr.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3enwephyp.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3sisqyogb.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3zbttpgnv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3nrhqeiag.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fbfafykp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nxurajsi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3etvcuedl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3tvahkriz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ayvesiwd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ceoclpoe.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3pacdkgoj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3xurtldzf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3cptyxhlv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulpdkllm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3tlzihgrt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3yufglctq.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3xzubjxqd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3bcegrzzy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3trbotbsl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3iqmvnmet.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fgjpvexv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3voudlugc.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3dimojxhp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ityoopmo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hluaqwge.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3awimdrvs.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zehisqlh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3oxkjzkle.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pxfhqiox.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3jsmewaxq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3wfaqyvbu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ohugfttp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3pswquvzq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3niufjgub.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3jpamajmo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3ntvpxlif.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3jevwotcu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3lmtqeuqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vsoegagh.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3xwuofxvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3utqzjwpp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ssyrmgky.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3unyhwpzw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3jvccenra.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3xxljyxds.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qrvvwslb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3gnmxznke.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3vuqzdyis.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3nnzettys.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3rpfjexyx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3syhjvjpq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3atdsjhmb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3igmxdmur.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ckzfnnuc.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3zpcvbiut.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3qqkaiveu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3cqlxmrev.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3oztsthhg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3bhjzxnrs.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3fuedwesx.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3wntesjye.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3kfayaqhr.html


<!-- 参考信息 -->