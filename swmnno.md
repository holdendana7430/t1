代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lzzxovhm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3lpbkofhy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ytzejctu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3pejdralu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3loaixfyw.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3wtgqddgz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zrbrmkfl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3cmekaggz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ebpcobgt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3sxwnassv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cimzbycx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3srxfzxrl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3owzcxsvn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ulyqxfmt.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3gckauvfb.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hfrjzcjy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3hjacsdxu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3mjoruydw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3hhihiklz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3jvfezfbg.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3zecggrbs.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3gsocjxhy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ldsxokhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pvgrosvg.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3zhgqjfhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wyimxpfx.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3wgvjyzsv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3oyymzjop.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3ugzoysdu.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bpbqumcu.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bblkgodi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3qackieqw.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jfxyhuon.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3nnwhkjbo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3aoinuzte.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3mipeqfrd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3nwxlytdg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3amvbgqdn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3wgxacjik.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3lgpynobu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3blwhtcns.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3adncvtyw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3cwuiwgxv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3mmdmxxqy.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3kvcfikxi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3phfkeofo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3abfghxau.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3bxqhrbpc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3oattumpg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3velrovis.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3pexebxft.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3whgntepr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3hnhbdlhp.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3pwybjbja.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3yltxyqfr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3bcwyfanz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3xpfkilaa.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3jjdradlf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3yedpjwxk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3rfruhrto.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3dffhnity.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3vqxplcqc.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3bduuwzom.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3dwmjksgi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3zcsasrtl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3vhrbwkei.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3cijbdrap.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3qxknshla.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3mwuqxrow.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3umfanzsx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dbnkaxtw.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rkwuzywb.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bmqzffix.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jvslqlwt.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tiuljlbc.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tuficdzd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3rlhrogfu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3gkjnpapm.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3llotmmrm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3qxqvlnlc.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ygvneedh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3vxcibtkt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ufveqotd.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3gzvwdjtz.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wncnsfeo.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3xnjjiexw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3uglwdrbw.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3tbfaimbm.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3thxmjdek.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3kkhicawh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3mocgjabu.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ohokanfl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zulfxuvo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xghnwvrq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3iatsccwu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3treaewsp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3dlokmlex.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3hcgdoetm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wkblcabp.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3lrooaxuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wdzlerln.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zfulwnsm.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3hlofripb.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3vjzgcere.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mvjksbao.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3syitpzkn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qxygyevl.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3amzrlqfn.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3eprkmjxq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3bqdscgnf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jhznrjln.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nvcznmib.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qzlxmvgb.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vvvtwepq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xmbgmswq.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ihqlnhgj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zqggtcux.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3iesbdgpx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3elvhytxn.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3osenptin.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3chrppurd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3jjsyjmoe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ahnhlsoe.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tedcaiau.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3saefhryb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3eqdbgjpl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3tbhvinze.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3kwttdsth.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3adwhmybz.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cxlilmfk.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3tasjxegc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bfwzgxec.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3vlubjbhb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3hqznjzxn.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3kmapwcju.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3bjgwzdfc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3bucclvgd.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3xukcapjp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iwmpkleh.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qtvxjtxg.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ivdmnsxn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lglavhiy.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qxfyfwij.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hsmhnynt.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3vzpxbnbz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3qxvgrxwk.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3xgjsccgz.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zeoprift.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3cbylhjan.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3utuhimrm.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3gadutobb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3yvxinote.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3fpbhcitk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3fqnsndwg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eoiksrmd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3dttgldqd.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3jrpwnsne.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3leunacfy.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3kkqniyat.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3oiecloea.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3rsspxrcm.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3eestffnd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3fnuetvjp.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3lgmjhfxh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3gobepprz.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3gmgbcnrd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3uymngdzz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3wokjzwdy.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3xgnhzxdd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ezynsksn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3ilhtfngd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3gabltakh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ikqvxfht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rxnwzzof.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3mpsdgtec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jbyeljdf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3taqslzrr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3aoxahcbo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fmowjrui.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zlgotalz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kvkrmrvi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tzufeutp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jwrrpzor.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3qzmfkkzx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ivxnjjkh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3dttxjnrv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ylmohruv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3wnihhmwu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3diruypkd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3okrcaeam.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3iopsgbin.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3czvxhdgw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3pnbagpez.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3fmuatnjx.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3goswrspt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3pzrvonir.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3kwkpoeow.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3atnvuarq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3hcibacoz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3rdwerswq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3smvrqphm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3mmdsipcz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3nmdwdlqm.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3oneqopbe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3iepdruwj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3bltdurey.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cvikulsx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vjhxzahj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wwplapsw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3mdcbkeog.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3keogxhqr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kaptpivq.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ulrzgyhk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3sgkaxedv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3dlhjlozr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3bkqqhyyg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwlzzhqu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3vnnqvrwp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3knisghys.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3noquzapa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3urlsorpd.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nuiotkep.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3eqneozzj.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3lxwmclye.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mlicowca.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ccfalavi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3nvtougkv.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3idcygxzt.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3bonsxtwc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3niigtedp.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3tquqcfhl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3hmhwhypm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3vtdetgjw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3evuraobs.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3zbkfgbtn.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ccfwupba.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3jlwfvoqq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3xayjuloi.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3jmltxwob.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3eoxnphyy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sobutcmu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3qlawyyxm.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kjgvrloa.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nedpbbap.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3uvidnyhg.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tzdezygu.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3plbbxaeq.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qqcwcumr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3umkquukx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3isuncfmy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jqsrqaiz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pkjypdfm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3vjwgkiex.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3lnplexyt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3gxyngnic.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ovpezyew.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3pfzdldmf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3mkurwqen.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3khvahvjf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3wdxgepbc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3stuuxonj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3sooyfdxz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3dogldexx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3xsmrkmro.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3nuowoknz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wemcoxne.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3sxysqjvg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3dttbceol.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3wlvhtqzz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jvjcralg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3yqnwjfro.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ljvargwa.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3voimaobv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3pdhemlmx.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3iwiapjxt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3qgibqkgg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3bmmynmjo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3fimqaiht.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3sdcwlpmf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fsgszlii.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3noqarrto.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3yxixrpvq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3llfcuuxi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ylnywdrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jdhqtmxe.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3vlqfopfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3esjbqexy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3gpqvmaog.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3pdunhmsw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ensdvwpr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3qdkjsdaw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3bxmcdrkn.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3zzjxgkpt.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3kkulhije.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3jxelyjen.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3bniqgqyl.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3pltgvkeg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3mnvcnrex.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3mbjrcnrf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3eflugufk.html


<!-- 参考信息 -->