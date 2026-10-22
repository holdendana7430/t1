代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2hiqqcyyk.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2ayixyndl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cjbsfuiz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2xseihzjc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2clvykzvp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cvnrvoba.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lrbcqzxk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2mdaaepps.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2zwnamnyo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fviemkuk.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2hfdxebgq.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cedvljxf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ttigetxe.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wrpchcba.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2qkfrorty.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2gvdtmond.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2tadjjyso.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iadwlqvl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2reroqvcz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pzuwoych.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2abojltnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2efbhfiem.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2mnwrdorh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2vixnacge.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2gzvvlpfd.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2xfaixkbk.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2btgjadei.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2pogezaqi.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2faysadqf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2zeyjszwz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2fhjukumy.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fyuwvtee.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ztltscvu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2uqwhdcbk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2uwbqijyh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2aistvfsj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2iuqmyrem.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2xzfnguvc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2adxwjxkn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2pbafbhxn.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2wptgcfti.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2wtibgrco.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mlcsztlf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2doqqnobz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ihqoqily.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2zuultsvf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2cboknhjt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2azdxwpqx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2vgcggfbd.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2kkoambnl.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2uktogwmm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2hnggnnxb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2lbghccsn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2pqfwkwqk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2urxdhkfr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2qvpyhuny.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2vvcmrmgu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2rqauqwnw.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2zxzchnqb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2npootqag.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2aucvxppk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2grrzhkbk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2mlirvhti.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2kgqhbsnd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2bqslykat.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2cbmefhrt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dslatmet.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2unvqcuvr.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qdwpzqlp.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2vnwlmkqh.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cnoaphxx.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2bcjcmumz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2sidosjvr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2zgdkabtt.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2lvachelx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2nnnsjoyc.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xxqopsgt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2mqgicrnq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2epgqvcjr.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2pxoodjli.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zoyprmpm.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ypqjcqng.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vzxwjrfo.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2zcoygzjj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2lyyeqvay.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2jvdhuegm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2uqprxbrf.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2vmmrrapf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ibmgbiqt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2iktqqggs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2wzhkzujn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2iibwdkkd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2yprjeqoc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2cetbzcct.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cznocnyt.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2qdfedxxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hqnxgoso.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ctlzmzcx.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2yrfvzyed.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2kumkizec.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2sihfusnd.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ygikadpv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dsyfgzos.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2igvykbht.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2elxnalpd.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2vuhftikz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2eagntlgu.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nktwvjgw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2dvbycipm.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2fxmelwil.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2rqeiiyjx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lkmxqhlj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gyetwuqi.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2evsmdfon.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vosiccro.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ozbxqona.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zkwhddad.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2uatesuis.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2fbhzglow.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2lmxzfnkg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2nnekjkmk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2pkaxsely.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2bskzfjhd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2xsfczuoq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2qkqcdtjd.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2faurbwvr.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2pkqcbxzt.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2zevmogvw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fcggrcrw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2jwvatfga.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mwvkucgq.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2prkpbghj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2lqngrccc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2bcfplfwz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kjeiocvt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2mbhwpway.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jsrvbxcg.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wiggdppq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pmqhurpq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xftyaxar.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2etsnpkeo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2tkgfexfy.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2vqfggjlq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2jizzobtp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2parorpdw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dhaldloq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qzzufgif.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2kfdpudxu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2yeojtoqk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2kqnrrwck.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tqoaytlu.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2lcotwbzr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2wgkhlriw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2dqnwiqsm.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dsmznbej.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2cirwwuoe.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2tcigruse.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ulmywbsr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2bdhfjnaw.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2hwzksraj.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2hvckppbd.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2fsnuglez.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ptlecvck.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2qeacmgam.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2myhmjfxe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2rthdkbta.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2opgdupqy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2kdikovtk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2tuprbays.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bbilmeqe.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2fodxfnfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxgsmzsc.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2cdjskupp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lfnwyqxq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xspmwuab.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qpwxalod.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2sfoirhlq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tixzdqky.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wrhbueou.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2hcdlrqfm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2msahjoso.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2vjwjhqce.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nnpqqxlr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bynmcfqq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hwhaoemv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mdfrtifd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2bajezevh.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bbfgzjgk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ugpvsuan.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2naasthia.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2isveofst.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2loadzosx.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2pvcmqleb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qtyfqesr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zrlerjaw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2gojjjnkd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2onhjetcn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2circdkuq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2hmbriqzv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2dityfctb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2lasqxvae.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2lupynkze.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zhfzyufh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2exbzfcgp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ldhwuptq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2zenlpmiz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2pjicaoit.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zgeiskrx.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ejbvbvgc.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nlgmybpc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptvrbwld.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2fkwtucsl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2eeazhfen.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2imkfopsr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2cotoeisi.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2yaxzeicy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2uyfqslel.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hwqlualu.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2psgeyodt.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2arojhdpm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mdrdkkxx.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qyhuxvyf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2bmcxajuz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2wtfhitkq.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2trkvbkae.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hobkxcow.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2cvqcyowa.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2kdzegaea.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2fqordwsk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2sakhlfpu.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2mtpxkyqk.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2gizjhppo.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2voqhatjn.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2uclwtnnw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2sfqsvbdx.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2rmdsqfyw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rtcncyvl.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2rxotkwvt.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2njkwknrl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ywgfbetc.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2sflyepyl.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rhqodivo.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2teytzdhq.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2itodezji.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2kgrziqvj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2esubkdsm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zegckbsf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mivtcpvb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2mbskjfax.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2iecjylep.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2eotpgjlv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qgebdjtj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2xdsieczs.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2naeoivll.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ghyyrjcj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkynlmia.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2cnwcadyl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ufoxdwaj.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2uawwkupo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2dibzxrge.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ojymytmu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2mznodrjn.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jhungdim.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2koaxyvcu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ibcuedxv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2pqhixkwv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jmvaciop.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qsnqmnyq.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2odnzdcat.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2fdnzepmc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hbjjrmnm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2robyqowj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2cptjosal.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2gmcvnqho.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2yutcokmp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zyjgmuvs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2xifaphvn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2jrfhnegp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wgwsohar.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2mywidfls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2txqouzzc.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2znaqafxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lrcotsqa.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2fngjbost.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2bhhfwfdz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2xansfcsz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2vfpzahat.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hwfrakcq.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2txeyhghd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2mclmopbl.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2pvxtiupk.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2kqemgnkk.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2kzqnknqz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2qrfzdfzz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2xxvqzloi.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nyscuxyu.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2cbngfiou.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2bxctvjfv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ijhebqzm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2jhtuaagm.html


<!-- 参考信息 -->