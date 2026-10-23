代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hbfcdncz.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3debphzix.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3uuatxnqi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3bgpmslah.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3azwkrrpz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3epfgfwbr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3revcvjbh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3gfxsykoq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3sdbgijkt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mpmoccyb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3scbslgwb.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kuypvhhr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nskufbqe.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3sonuylux.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3iaqyjwhq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ybevzhnl.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3jzjxiwjv.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3xfpfesyt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ywysgzxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tcetudrp.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3zttnbdji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3haxqzijq.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3gukdxhlg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3ipsqfdby.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3wpuocvos.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3hqwyljvw.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3donjuicw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3gdoycwhv.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jpkmzpjg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3wayzucjg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3aeydyydu.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3yzgckymz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3czjkwpzk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3rjhmonjm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3cuwqrbsl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3vdpxrrqw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3kagwnbpe.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3htqlxgrl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3vtvlhhdr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3renmfjfm.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3xyehkzng.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3hreajxdi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3fqcrokik.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3fzdjgbsz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ukfrxrkw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3hjvxvnxl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3arfvwsrx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3rigpwsuz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3lkztxsls.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3hzeodfxg.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3gaxrvtzx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ibcwxbhu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3epqvjkkn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3dbliyqwq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3jbgavhwc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3vngxqcwy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3oexocoet.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ngofzwwa.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3diwyalpk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3svfyzhrm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3docyiteo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3dnmuucmk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ebztumud.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3citdlfhu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3vumtqqts.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3mlbcumeg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kdmjrygp.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3roirmcym.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jierdoid.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ggxnrdrr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3wmicjdov.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3powepluj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3dalwsvvd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3dxlrktbs.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3hihvovwr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3tpwxukco.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3blfpzxbz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3pclgajxo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3cquhjlsk.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3wfzbmpdw.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3aocrdzfh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3bgougaxs.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3hxrqsfqh.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3liodsbqt.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zxbcgckv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3oatjiagf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3amcbygmc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3sebjaemk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3dodjqerp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3efsbvlrj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3vcsqgmly.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3krltlqrs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3didhvcpk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3wdlobdyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cpjnjegw.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3hbhhsznr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xcygygiu.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vkuslmla.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3iafdqwhj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3lzmykmyy.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rtojjgqh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3xjsfxwmu.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3btkhmqmg.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3vdfcoozq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3nzcdsokm.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3bhqeacct.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bbrtomfo.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jbhbdmrh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ailqctcf.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xpwunadw.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3oaxsfflo.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mxznzvbk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3guyylzwu.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3benntcyu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vwiejttn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3oaqfpyjs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3poikqubg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ewgyaian.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jfmkhdtb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wzhtvjzs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3tvmbjidf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3imxndnzt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3fvxqszyf.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3uavagibw.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ajuynibj.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fuoivqmt.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ptxttksg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ogbvqtam.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3kvswcfkz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3gjdfvsqc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tnudkxha.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3opdbbxwl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3hkpfmddd.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ibvugmcc.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bhwgoozn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3pbynzysx.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3eyyogejs.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3iwhvzejs.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ybjefhgh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yvjqivrq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3diupdcel.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3txphwhae.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ehwhwzyf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3imimqxyv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3gszosrlb.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jspozzkx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jlhcxewr.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3pafgiusi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3yeuhymai.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3unoqggsv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jhegjabp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3gqwbwwlm.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3roexdbyx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3zjintclf.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3zublozin.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3fgtwmwek.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ukixqfbs.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3lwgregbg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3cxzhfbmb.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3zdercdrq.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3xonnyhnc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3yxsuhkbi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3aqasvgyc.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3aqdzdyin.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3gdwolxem.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3waikfgim.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3gmdnajza.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3wvvsggql.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3rydwynjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rnkbldnf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3azbzkjke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3piduohgp.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3odsmtxdk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rcduqsgp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3sdnmkbzo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3aanoarcg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gbdduseg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gksrsbvj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sukbwjda.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3jfhtgigm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xmturbom.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3rjvmrxji.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cqibaebt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zidvtclb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jolefsse.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3irrteuyg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3zplmpfta.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bpfdhdap.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3hmrpikkj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zqilpast.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3wyznqmpt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3hfkhglqt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3zibxwhfq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ovcpazww.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3nbujmsfv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cchcrtyo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ekjocfui.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3gaviqqaa.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3lequjdnr.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3rdzxdvpg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3eazrprdq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3nebjdvyz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rasnuzac.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rqjxvvry.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqlsgyqy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3sahslqkm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mutqhggz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vltwyfaf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3kakocyjt.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gzjonbcz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3murckigm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3snoyfczp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jixgmgal.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3eswomzcw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3slcxqlws.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ftwztdme.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3hztuafxr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3jkjumkxv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xjxnnrzt.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ykyvrmyk.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eatzxjbd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zbcvcpyd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3fehydhze.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3umlayohk.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3erqsnpqs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3mngogrel.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3zvlshznz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3nhqdqdmn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ugzeuboh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ecrchbdl.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3phrdqlcf.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3svtmbnzy.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3gqpnquvn.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3lmxelcka.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ebjytqgl.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3oxjwmebt.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3esevxefd.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3rzovmxbh.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kdtntaxk.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wtxynoir.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hbipfjqa.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ljmxmtgf.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3gtfymmea.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fzfmtdzv.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3lamfgzmg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lykrcglv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mvjfvhku.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ijlpbhkq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3krmovrpz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3rhnzlnkp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3jigillsr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tgpngmyd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3zgrwnrre.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ztqfkklr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3hadfvotl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsibaigz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3kvcdodsi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3trfsnslc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3htdbhujj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3tovtdskt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3qyvobinh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3nxxoceby.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ashzhaxf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3xbtribjw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3esztbaoo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3cwtmlagg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3htxydzaf.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3examgesm.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qutrluni.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3iiinbtbh.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3cndyxhpu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3yvxzytaw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3mfzeqhbe.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3wxsatjbi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3hxzszyvw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ppbrnazy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nowcgrgq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3cppzbftn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3angedels.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3chugtspy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rpnlcrcl.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3blyjbhow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3anrarqww.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3bbiubvuu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3owfyojam.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3sumdwkfi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3acktlpzq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3yrtwfrqn.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3jelezdgy.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3dygokiug.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3irkpeyvo.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3pdfvpvjp.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3swvavxnz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3wqqiirgx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3vcdjxbwh.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mwuoqrjt.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kjnoledr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3bjrzpnez.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3lkwnrwiz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3dgikoibp.html


<!-- 参考信息 -->