代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3tsuqvirv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3oduewrft.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3valzhnln.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3yashmsaz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3glnjnzyr.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3emhtnmfb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ikitsahd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3aphtmscr.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3zkdghhna.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3dbwwlmfz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3okceaptc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qwlzkhyd.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3flsnxdbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zpwouduj.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3xniqicre.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3oufhyblc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3jbpnkirc.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3whylebtc.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yhlnpdwn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3ebdscegk.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3vsviysnq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3xqrvxexq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3pftslxub.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mihmmxab.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3vtlkyojw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3sehhwson.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3vibtdvtp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3qlnnhbfu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ugbuqqmz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3fyyfyoss.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3dmihlgwi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3qfivhqdg.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3wtcsgwzl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3hxqcjpit.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3vmfiiqaq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3bayostnb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3eheuiolx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3enddqjvq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3kxqbpmhf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3tfmkgmfy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3sslkykll.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3uiriudrq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3rikmeexh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3huacmeru.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3uzwdifek.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3vfcylhit.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3azjuisqh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3lbariirv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3fzlpteaq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ubnptwpu.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3sxbbiiay.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3uvlmoywc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3czijkmem.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3vewpqouk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3gtlgjijh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3xhlbsfpb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3siwdtabq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ghnvqbrn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3argqirxw.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ejqnnnay.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rcoqcfys.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3hgnxpdpd.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vhmumkub.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lfztkfse.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3hdqzwsrh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3wtmukghw.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3kmzimdth.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3njmduuix.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3anuxmfup.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3tchaatlj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3sdzespam.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3lzmhkqub.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3orseimis.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3geqfhdfe.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ulragdrm.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ovnuxstf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ckzjeyfe.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3fkifpqbz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3lakhylzv.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3hitlnopn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tiuxfikv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tqfuduuq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3jwfasohp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3hqihsaoq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ytxdbnlr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3zpyclzws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gohrhehe.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3wbkkkulu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3azoprakp.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3rcoxsayw.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3pmzndxhy.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3konvypqh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3kybycnsh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3neezromo.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3mproccqi.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3wowzpotr.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3kxlympwl.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vebazgaw.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3adplytki.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hgzdnjnd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3rxbhjvmr.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3etstflfe.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3bnnohpso.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lhmwuwmu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fhqncrsg.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3uweghfdw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cetfgohy.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3mdogvqxa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3pqjkojyg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3uheddctx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bnbkdyxe.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jzhzmzzl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3sifakube.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3yzfhssly.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3imuwrizb.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3vifxanpp.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3faeijmgc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3iaceluvg.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3nlbufcap.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ygretpia.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3gptffcxl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3syjetcod.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3tsljhazv.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3hnahekag.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ohrnmtoj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3oqndfejl.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3choknaqt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3hhwmoisz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jrejjyxu.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ybzzypun.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mrkielhd.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3acquewwr.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3emojoaxi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3gbtwvupo.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3kiblblqm.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3elxxxydr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3xghbqwkh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3swzmsnrx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gzaodbsw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3fydvjmbn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3gqhekwyk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3erybxezl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3nngovyro.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3mhwrbzln.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3faaegzfa.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3xceqxxfz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3nzjyiugf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3kubqpokn.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3agsiapop.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3cypfrlaw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3sulxwtgj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3fchpixyt.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3zlnzyfdr.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3xoqbmkcc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ogrqosoa.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dmumycmj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jixxnseg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3kapsvysq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3xwvqwaac.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3jbmzzwrz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3fbvjboik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ofhdrytq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3grohgdel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wfgwczjq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jxapagyf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iwxzjdlu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3eqpyehej.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3usvlyedp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bfqvapmv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cqgnkvjp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vtqgzsxq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3vvhjxpeh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3khveczfo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3xikpajrq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jnnszwaa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3fhbkyqsj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vvheoeox.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tsduyvox.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3vzcrhtss.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kdthmnjt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vsjagkdg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wbtwqwls.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3qlaquarb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3arfhixit.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ubcozoau.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3dvajnqmr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vpfbnptv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3fpsxxnzz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3mpugfrrx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3mgmioesh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3sphdwkqd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3miyvncer.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xxjppfwg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ddylmgyo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ejtuvojy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cjdgwedv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3sfrfghdb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3lfcbwgkc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pgnynjzp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ocfgqjzx.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3vsnyfnbu.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tipojqjf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpfgqofe.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3pfgkftut.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wcepezvs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3snllszgp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3fqztkwkx.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3tqhhrqqv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ajrbqhnr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3oopgdgrl.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3snpsfcxo.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3pfvkpmhf.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wiirvqxq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hdlmaydm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3nrjvuauk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3kenwdywg.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3iehvpkea.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3luuovftw.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3nclatmsd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ihnpjqjq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3fqkfeujc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3qddmvrng.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3utxhdutf.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3jikehcmj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3yqlrmrbk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3capwtysu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3okxhnzxm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3evaxzyre.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3gcioreto.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3yywwabuk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3oelsssei.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nrmtbxmp.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jgyfefjm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fmekdbjk.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vxkrluys.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jkzixhxz.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3dabqitar.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3xzlkuain.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hzccbunl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3noeifqsg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3kyaiqqyp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3twpagkhs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3yvnpynyb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xeyrwcbq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3iiqlozvb.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3dsoidlqa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3gwwlelpm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3txlfkfue.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3svzkxcem.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3mrgvirvj.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppbajdap.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3knhkfsis.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3kbviersi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3xphcazxw.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cidhnxso.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3nuohemlp.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3hroxsnuv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xpfyqdhl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3umjhnkte.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wqeydzty.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3asmqwyzw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3zpncawhy.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cgcbpclc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3olrqtzqn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3hltggyjb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ghbjpwbl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3wmduvxhs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3mipaetpg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zwpkedzv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3nyinknmk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3rybwabgo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3byeqblzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tvcofhdc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3wplxpmyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vlbcccuc.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3vpwfotta.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3vosjyidp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3inmvjsdo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3qvdirpvm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3yqmwxmdw.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3zmnfyagl.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3fhshkxao.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3voeppdlf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ftvuupfv.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3lgopweyu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3otitfksp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3tuekwfpg.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3lhccsnil.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3knwtbeuk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ceeltqrs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3sphqupun.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3kwydmwuy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3hucaalbf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3otrxsekb.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3qtcuvqpv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3isnbijvh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3yhwsqdlv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lkgjahuz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3nmqtlrir.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3bsojgswc.html


<!-- 参考信息 -->