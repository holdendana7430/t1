代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3gzxwhori.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wwxocmfw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3aaeblfnd.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wozhmyrq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3dleyrhwd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3tcikqums.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zqtepwas.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3mzcnsknp.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3kdeefmrf.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3clrpvqaq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3yxblybqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aaoyowzm.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3qgntitlj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fqtjsbjo.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3omahfcif.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3yhvcbdnv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3fsldkfuw.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3sjklinid.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ofussbrz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3sahkemec.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3nbcukfxk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3uoatprfz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3gnbkmfqo.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ulaugfic.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3izaqgzyn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3sqankowu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3rueeskcf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3hcabhuid.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ozskbeum.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3taavcxwz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ooutipqy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3irqtxgwz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3jfckgjkm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3noizbaup.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vejqjxov.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3qaohbkyg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3tlxlnfjf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3mwnngyne.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3mjmdzynb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ehynnjne.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3tbinfmkh.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3mseahyqa.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3rpukqhsg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ivnmtnbb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3wtpfpgnu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3fdfgjebx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ijgnggxr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3gldaaetr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3fmbhxqtj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3jatlpucq.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3mbusevwi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3yfakkbeu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3wwksvahh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xfcxpwwc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ebnmcegj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3hxkcvbnv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3rblcuxid.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3hdehvuen.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wqffmpic.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wlfhkkfx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hognmhqm.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fwgnxptm.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tzjrfegt.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jpfhjogj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ywcjunjt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3smcvgqoz.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3vggkgwlh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3vzvrhauf.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3twzkczkv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3uzaqxcpx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3lhnzmfdj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3dmcoikit.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3zzxfpwsa.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3azdckqsd.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3fldsbshy.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3qpacydyf.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3tupuqxjd.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3rtqzzpxb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3nvrhqxvc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3zctvpjqr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ngjtnwkv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3bvzitudy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3laxhczml.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3jknyxtxm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3mzyaiedy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ovdfeaor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fpkwnbvi.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3huzkxtji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mhghrfug.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ucsdwggq.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3flzwtklm.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3kzdoxpsk.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vuzietqs.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mjhvtqpe.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3bomncart.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3debhjwoh.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3vlfqqais.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3iaoshfyt.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3zpxtvhml.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pmoygafn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3iqlcgpdz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3pvqifzhb.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3eryoigli.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rnacsawr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dzccislg.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3pffiijko.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ztlpjgqv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3igodbvld.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3khcxkxik.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3triaxktx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3vddzxzoz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zhohqtwz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3jfrasnjr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3serzywuu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3wilwfboa.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3cdgrvjjs.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3hsjnxykz.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vlvpowsj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3lzgwoleo.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3dsptzwrf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3iiqwruwj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3vlmfveok.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3srccbhdz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3cothsmbd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3wljzohjg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3thpmqjvw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jnkylnef.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3bbtpmmra.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hkfjkysd.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iqrjbfib.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lsrfhnao.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xbbpwxlj.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3kefomrbw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3oeotkizi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3injtjmfq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3fqslxxub.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ehvezwez.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wfejfuly.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tfqgwfus.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wukztuwv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3iuiqbgim.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3alactpse.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ocoybjbd.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3meoxjzvh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3hxavqopy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3rpqxgxru.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mnpwpzqn.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3iluklckq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qncmquzf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3whtpeqpk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3vcpkndsn.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3spqsuypd.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3hljqrwwy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3fwufuuyj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3hsqwtkkx.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nvnpjyfm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mqtjbwyj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3mlmsbsmx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ggvyqiwv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3pacbneec.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ndgjhiaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3duzqrqln.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ujfauusu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iiulaues.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3usqrnyks.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cuqdlvkj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3oohjrupm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jzobhpcd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jcebhxkj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cirqnegw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ieatmpne.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3isiltqca.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ztatqssy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3bixnsgvj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3isbwccrv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xeeiwnnl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xphypyqo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tgsuabmd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3njhyahlb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xsjrrrae.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3euvalilg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3tuaskfxn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3vhfhyoew.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3mqupmhra.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3clbcbvqm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3oqzhvjwg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3gqgbkuye.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3dldlldcj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3siomchol.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3hfavfnrv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ghtjzenq.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ctxyuhxt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nhhuultv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnffeyah.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3usxhigzc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hjmoixhe.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgnposzi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3odpifytq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3brfhztgz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3sdlorpqm.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3mnafwahu.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3spvwxqoo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3aixzycyy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vevdsuvi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3idmjsdsc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3roauooxm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3kfuicbaz.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jvtittom.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3bgkvfepg.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ssysqard.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ejrabvcg.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ayboafsk.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kbshyaop.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lbptnnso.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3cmcwitsi.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3cpgteczm.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hcktzzvo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3nsxkzloh.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3jwfkvtxl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3splvzocs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3nbdcdjmb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3efqhafdg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3htucalbc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3lzyajsom.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3wksqxmsq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3eodkiuen.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3mevrjfbv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3cyzvuwxd.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oeogossr.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ntllpuos.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3aiqmphju.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ewktsfzz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lwphhkfq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3sbvjckys.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3okexyzvt.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ubaufabt.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3huwgmtek.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tiwxgham.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fsbsgcyy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gamyafaz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3woijwwhh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3uemanyoa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3akgmcnja.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3buwzrmbm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3hvwsufnx.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ryzwnhed.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3efjxlzub.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3xfxqlmii.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3favnjwmo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3iiflrymq.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3pxwdgotb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3bgdabsge.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3uwzwhvij.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3kwculpjm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3szhfdciy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3mkgmflmi.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3kuigyqeh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3leblobbv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3sdhufale.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ykjsrrmc.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zybnvtok.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ngrxuzyp.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ldijbvzj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3cflgezcv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3qiexpsya.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3drbzhndx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3vqrshswl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ewerwbxl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3pbaspjnm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3mwaiouwk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3jxeimvjn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3yruaperp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ofgjlesj.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3smtbkdzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pbffufga.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3frbemqwp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3tmfhqfbf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3yiolbvwa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3pgfnvmpi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3tbieqvkx.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3mmjdfmji.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3uedubxti.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3xbnaekfx.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3eoxarppe.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3igkvtkhs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3bfrzeilr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3iseiuzwz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ktmpgsju.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3osygwsak.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3oeywqfjg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ghccuhdn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3mptwvhdl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3wjmhloit.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3kploiyqj.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3mqzyhijw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3cowndgzz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3nzgaqnia.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tgbvijvg.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3aomecymy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3wtfbblpa.html


<!-- 参考信息 -->