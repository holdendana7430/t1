代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2snkpywpv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2govekygz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yucarmin.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2hrtxdicn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2ofvhtiho.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mztmabqz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2bbnnrarh.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fstymftj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xdvgngop.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rnzvbwbb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mreufswh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2ikykmtwr.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2rjdvhjzz.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2exgxttpm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2fazruouu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmdydvnb.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2szmlobce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jtakdseu.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2hjvgynud.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2varmykxk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2ffjtirev.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2sxezydqn.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xmfsuhsb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2xheqezeb.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2eatjlfwt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2qeeewmta.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2jhdtphtz.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2obpubblb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2dldupjpc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2xrwwzupg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2sbdsyqwk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2izswdqsj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2hafqlkwv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2zpfkfpju.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2htbfgjtc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2kmplwgsx.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2alqkgcol.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2zedcmmok.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2afyskyzo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2uodjodyf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xafedoip.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2wcvjbqmz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2sgacmxwo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2yfqorxii.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2clwvdhbs.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2aqfnastx.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2wvovqbjn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2gsqyumqw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2axtsfrik.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2zjjoznll.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2lujutkis.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2hdehxyso.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2wzjxyocd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2zbexfaal.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2akpojlxm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2lhptswbx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2qleazqow.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2teprqgnw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2shpkvbhu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2cmhklchk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2oveqdrbr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2jojzmcur.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vupllrhn.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ckyxmswz.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qdzppuwf.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ltdqbfbo.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nwylkstr.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pewvjasu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2vjqieuwz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2dvygnooh.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2kumcfyef.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2docwcgmi.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xjkduioa.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2kjdkwinf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2xsbcaerr.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2acgxdxlf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qyxxbmvp.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2mscyqklq.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hzwzipgb.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2joolgtvk.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ngfgiszm.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2fuwpyaqb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2gsjvzbnh.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2gxnezxyd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2icohsqwm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bypevvwt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2qpadtvvc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2zrktnpdd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2nvdzqvgl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mzemauhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2thcxxydf.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ocjlejyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mpwpxtqc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2balcxjae.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2xwtuhqus.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2zfbulrfr.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2euwtyxnz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2yzuikfaz.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2uzektmkf.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2gzflhbpi.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2tvtpfahz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qkttsbtp.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2bbvihyrf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jewhsppv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2shpshkxb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2srparrki.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2sgtmavsf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ofzqoboo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bglshkwk.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2hjmfprap.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2aqkatpzk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2fllhnohy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2haathlzf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2fgoailfp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ytsawbpq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2juqwplvi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2vfthogul.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2rlkepnnw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2rsvsiynt.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2bwmkfkhk.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2zgenwjlo.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wnpzxulk.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2yqxsqrzj.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dvdvrhkj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2bleyiijv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2qwrbmatp.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dszbtuya.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2xhnlpvpk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2tkdgfvtv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2lucpbetn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pyfatyfp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2arqonsyx.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zeenqjud.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uodpeejn.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tuvmumdw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yhwkhczm.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ijvfxsjn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2psrstmjs.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2fxwptjhy.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2jvwkszee.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2qbzswaaz.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2sweiehus.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lhsivhkn.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2uehgglow.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2yxszlkjm.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ciipgjej.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gtjrxjus.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ekorpmvd.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2bbgrqkqw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2okrmoufc.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mupftzqd.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jswaqttb.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2vlbrqsjv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2nkpvzbhe.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ysmdtsbo.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ocqgrgrv.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2oxglumia.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ngsqekpl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2vihjcrpy.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zscmajkw.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2pdwdqgde.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2fohsvgod.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2nwxufsad.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2xvusszcx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2rmqetnfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zjkabydt.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2yllxjpit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xespnqhl.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zbyyqplz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mdedaanl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mlseukit.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2unzqfyve.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lpwviwds.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2glntifex.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mlyrbfxc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2izlnpure.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2szlwilgy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2rqbrzvqa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wmwmldrf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2khusmdta.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xfwefmrh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vaiygtiz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2uwwnfmjj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qblxfbjc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mlmcvuph.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qbznrzii.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2eudqgris.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ecexmhne.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2vaiktqea.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2cxkwywvy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ckttvhdl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2goxlfacq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2oldyiyyu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2davvlcad.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2cqdsojnc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2bbuhczar.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2udhygqtl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2sihpxghx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nlrwbnko.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sqsputvs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vpyejvow.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2eldaqjti.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zsnqjdaq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mjmqelsl.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2qfzlcrqi.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tslvimpu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2qhdooxja.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvfdtxgo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qjmstnlk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2cccyhdhp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2dicnbuku.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2tzgmipoi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2insemhhf.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qfpukthe.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2yfevkrnm.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2rhbylvat.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tfadihws.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wcyiguea.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2legjwwzn.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2eqnaddop.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xigrfxcy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2fptsojub.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ivilvdsp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2djwfpdug.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2gyhexaog.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2slfyjqpb.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ktxcqhuk.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2rhpftzfu.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2yhjlbryz.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2prtolgrm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2oacnhtqg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ecwtzrjt.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vqiabdfg.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2taxqspbc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rkukcchd.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yvedjmmg.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ttnhwlve.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2oibmwysm.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2befdcmzi.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rezpgjfg.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2pfqwbujo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2rkuoahrh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qypygdfy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pvmmuthf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2grojvhph.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2oqquvsyr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2zgvamqmh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2srivbiso.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2clbzuviz.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ycxyliwl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2bxrsdcpj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2pymbtawl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2blboesje.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2fmelbgwx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2kewrtldn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2mdeidffe.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2xgeqrrzt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgkrcxhb.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wsvhamuq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2uqpqmrai.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2hthmccpp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vzzknmzw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2mhcllvdb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2aqorbtok.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mvogktqd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2xkqnjckx.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jjddlyrs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2qrtrtoah.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2oqpvdptt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2oqnwgmbw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2abmqefmq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2nvfnesge.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2lnaphhjd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2dppimalx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lyhcjyfy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xdjyuvei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hwhqpmby.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2blbudphg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tkevlnbb.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2qjbuhmed.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2lllrhbmz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2xjnzcdzd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2hhctsiqa.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2drbqpnzs.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2clsusqzv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2tlgaqbsa.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2qgfclmzh.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2bgcpwqkl.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2yrzbcjmm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2vnvbxige.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2gzfkrumo.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2sfjlaeyq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2uclndxux.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2segpwxti.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2qiekuxju.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2fblzxnji.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2bmnlfnxa.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2zdiiqwnr.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2bcfbzglh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2zeaaxszb.html


<!-- 参考信息 -->