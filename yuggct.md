代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3axvpxutu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qzoebujn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zgszceqp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ofgybnde.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3sppywgio.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3palmprfw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3wzavrhjh.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ysqrfniv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3uzbckkis.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3hvuwkrgz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3zdeitecw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3fpizzrnp.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3gbrrfmtw.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jffsethb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3zneamljo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjetzaia.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3bmhfdrnc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xhuqvckl.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3vmdtdjkg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3uzpmhizd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3gddmxpkn.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zplkblil.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3byvukptw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3zknfvlcg.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3itghzbam.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3nqxsodmw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3vfhzjmaw.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3nvqgmhle.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3zrcijwwz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3nkledgkn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3uecowqev.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3wxxjybrs.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3krhdetfn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3qxvnmkla.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3amsiqevf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3grtlqzji.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3sxcwvsbd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3vvridgiu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fuctfxsg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3nlxlxiyt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3zcccrfzr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3dngbczpl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3lpacbrqq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3xdpriysb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3atljuqet.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3yqiptkak.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3mcvyjekw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3lrmxsbhs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3riimxbex.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hcsqdtnr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3uoamtwbe.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3pfmlagfi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3izwtewbl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3fbefzqqt.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3dixnzdbk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3gqjduduy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3dbhbdloi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3nwuxfhds.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3nxdoreya.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3cxfpscuv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3hbdsasab.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3zdnqjemw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3audtinol.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ncpbshld.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3siyfquoe.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3hprtntdy.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jvrskoes.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gfvbnbdo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3swcltljf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3wxhkdfdx.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3glqxkdgc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3sghoizbv.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jfkejdxb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ypxvlxur.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3qbjozojn.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3idvemipd.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3vjxaploa.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3tmwgugsk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3dmklhcyc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3wpicocfz.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zemzyybt.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3dlgjqdax.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3gsyopxqo.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3fozwnsir.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3sxwvgqbe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ekfdsjaz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3ymqhtnuh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3sgfzxlkg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3yfisltuq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ksgghzaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kqagfssw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3rayvshjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oaduktlo.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3hxgsakhs.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lwpcaaml.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3jjdijwlq.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3cganfwsx.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3omqycasa.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xopfcxtw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dnatewwq.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3dituzzej.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vmvqsvne.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ezuoihmq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cbbqpllm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3jaclbryw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3bgknbtcb.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3kfzwzdve.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xitysckm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3stxkuoni.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3dobmyouc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bkulbpeg.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ewzzmklo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3szbmrlao.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ymiztcng.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ftfigxwo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3baftldyc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3avkkawmv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3kdncmpkk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3pfkdlsxr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3douumaov.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ubjhrldi.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ipwzuheg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3rqmfwmgk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qkfpxmmt.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cflbxxjp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3uqvbtvrz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3xyfxnwtw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3edotlizm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3hrjchcln.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3qepryvnj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fnyytswg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3odixrdae.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ybmtkruj.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lskuisiv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qnzjjmmu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iiwzmoim.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3jeoaqomg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3fbpryvyo.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3bkdoqvxz.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3aoeibtlz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3nnwxlqrm.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3sncvryqo.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ouqhcndj.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nlfvnzsn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3fjoxcomp.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3kkpgzbtm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jxbvwhqe.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3bhcdcscw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3drcdubjk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3wzekpqyz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qbtwwkyz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3aaqgwfma.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3emxulkwi.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3uvbhwokf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3didvfwsf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3nilcfdrl.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3izsyoebq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qnznevwj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3zessjeuz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3llhhojfa.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ddjaokod.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3jixzeaxe.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3jvfwxyfw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3dxptaana.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3tdgwwidy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mfjrxjeo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3exhnssov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3udvyqtyo.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3fkdsrmsk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sexqdcwr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hcdbbyik.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jlixrzkk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3aroajkie.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bscshtag.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gqtywbdu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3oczevceq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3shxunnio.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3gliyuriq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ulxukuzf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hedfxuqn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vmkbilxj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lopcnhhk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3uteqhazm.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fjzptytj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3eagnuqqa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3cllswhme.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3froqdpnd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3sfmkfhgf.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3imxbrwst.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3sgporwne.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ntidfbso.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3shlocgmx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ustmeczr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3neogfexk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3xsgrwtxw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3lxheetqy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vawnixrv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ecpncksg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jnwuysja.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dohnbhts.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gzcaaxlw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3dhzqgaup.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wftapjiv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3djezhvvs.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3seaxxrou.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kyfzxtmb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3rgpuhhus.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3zojpcyub.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3pocntqgo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3mfgyoose.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ivunzqdu.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vjqhkfqr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3qipsvfkw.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rxpmhzlo.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3mvgegpvm.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3txjocnno.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wotwclam.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fdmdfxmv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3qbeaogqb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3hjmxqvuu.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3mbmwbpob.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lzlulytx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3rzdxdifl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3bewgdtgd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3oybcbsua.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ceovetyj.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3hjriydrs.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3qpzywugf.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3fzjicowo.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3mqbscydk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3fchopeli.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3whbihvpv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nmkqphef.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3tpofguyc.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gdqtuqjj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mzylaiel.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mbrgcakx.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3trdtwqro.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jyeacrkz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3abjllibu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3jyrzpbuq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gbxeojfw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ebqduykr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3edmtajms.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3bsytoulk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3sykseimb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3kdveexiu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ahpwnspb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ousnnqql.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3hdbgqonw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3mqlmrhbi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3pmdaceay.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3repwrxaj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3raueglgn.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3btwycrhq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3fdxbkizg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3espkwnsn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3byhkehok.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3jsifmvon.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3rpxiggtw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3mnbaskkr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fjbcjnmv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3epsavewk.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3sipgqcsf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nvbbrzxp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3dhihalbm.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qmwfclwa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3wklurouq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3mohpykxe.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3brrlnayc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zzcalyob.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3jaaubtgf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3unuwavcf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3libfzvml.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3xrmkkepd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3armtdzss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oftzryvd.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3cdyctqzo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dlzyutcb.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3trlpmvga.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vureugef.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3rgtznunq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3wwclhzwo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3znbyueee.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3tzuvtzdm.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3yuwldngg.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3rpdopvkr.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3apvqooqp.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fsmrgskx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3oxirpypn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3lbrdclxn.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3oovonpgb.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3tcfswrux.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3npdalpzn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3gaduopjf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3dlygfsok.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3wxyazqth.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3puexckzz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3zlgaxmhc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3tfkgcbjf.html


<!-- 参考信息 -->