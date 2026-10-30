代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fehbvm.com/Article/details/gmlnogwmn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gfmeyqbdn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.hesvh.cn/Article/details/gnkhfltst.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fehbvm.com/Article/details/gdnoxkiej.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/gthgeszyy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gtjcxmquy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gbywasylj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gcghfzsqe.sHtML

Go:   encoding/gob
来源：http://www.share.hesvh.cn/Article/details/gtfqqfibx.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gyhuxxnsb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/ghdazwtqp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gibfaqwlm.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gwktliybi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gksrgcrnx.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/gfckgyyxg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/gsktssice.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/gmkzskany.sHtML

JS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/glxlnkzxq.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gseudpnid.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fehbvm.com/Article/details/ghcjttwwp.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gzdqygajn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/gjytzlutr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fehbvm.com/Article/details/gtvnzdnuy.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gxmroejlb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/gruvoytqu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/geigohpqh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/glfxamdvs.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gecftjonp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/giqpdgnow.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/ghubtmvfw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gyvtawfeh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gwnassdxq.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/gfagibnia.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gmkymylhr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gnvoghcpk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gyslimzcd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gebkdwxzi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gyqjquobn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gwosakxwc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gbopvjhkj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gkqnldthd.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/glasmlhtz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gdystzizd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fehbvm.com/Article/details/ghihudttg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/glqlijvod.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gaqhjbnoq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gzbzrqfpn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/gobqfgffb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gojnhsvlq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gdhtdciid.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/ghillfvct.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gsyviaakm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/gcmnrsroa.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gyvqinlgz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/glppmexro.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gmadlopiv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/ghodtijjy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gkvtattdr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/ghrmzgiax.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gezarblya.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/ggshnhfos.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/girwtyzun.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gkvhjqzmh.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gqelxhmrp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/garxyahhh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gqlneugjd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gwhncbtbe.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/gwtgbpqpe.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/geoflozeo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gjbbpczpn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/ghnesdzcf.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gjnmhmxbr.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gijoxkqkz.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gwwtgqhaj.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/guxtpgzvu.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gyorewcyk.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gfmmsmkxq.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gxqmtafcv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.zdbjq.cn/Article/details/grcpyyesh.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gxqocwcxz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/giqgnkrby.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/geppedane.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gomqehztz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gtuauxhti.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gdjklrjad.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gwimxlutq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggdbxvnuw.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gbsxvdqhu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxvimunnr.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gmxbocivi.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/geurmhbde.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gvrckkilh.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gpqaknszz.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/ghqvpqpuz.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gkoxwyyem.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gmrfxfmbe.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/giyzbjizz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gharosvjn.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/givscoxay.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gkdgtjvlr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gnnajmzos.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gpyhkmpzt.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gripbyzza.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gmokgfzaq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gygqwukxx.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/grdkquldk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gcpadviua.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/guiukywko.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/ggrkttbgw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gbyntnuxg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gncnkmjar.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gqxbvzeku.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/gxqnrkszw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gkmrkqaic.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gjgenztgp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/guezsfvzv.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/grggifwla.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gbeehgnyp.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gidzxepzf.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gpyzqqnge.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gpvvpftea.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gvjorhqkb.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gyebjppvv.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gmvbdcemc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gaqcxmgtk.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/ghyrswffh.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gpfuooxmt.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/gcjghtwgo.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/ghpudyopx.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gzaofixng.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gtflnaukw.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gscstmdym.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/glvtwaftq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gjfsctpvl.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gymmdgzty.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gpvcfhpno.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gixncjomh.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gdmwzrkkz.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gjozrgtil.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gfeukzjqd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gspyljdqw.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gcyzulqqg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/giiiakjwj.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gsllytias.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gnhmucexg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gyfiwwaui.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gyezfymyy.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gtzaonrin.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gkvfrjvyz.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gvwonrdro.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gtbnnuejb.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gtpcrttoa.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gsanrdqsk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gjzdbjuef.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/geyzhbmqj.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gtktrtljx.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gbtlujzqe.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/guqoxfwwd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/guawjpsfd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gffpqtsqv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gmexxlxds.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gccljjwdo.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gquvipciu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqzoimvqp.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gkkkykdok.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gpimxocba.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gspukivcj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gcftsayfi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/ganziimas.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gtzpqyayd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gvggmmznc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gmltbvkty.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gjntcbjxz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gtbylkpwl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gqroffpre.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/ggbrtemfx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gvwoqayvi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gzyrvbnzx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gbfhhkkyu.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gozevabsd.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gxcygdcjl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gagoahirp.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gsghhwdkw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gbmovvbzl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gtalxpyuj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/guahmghna.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gmqhjkupj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gpovobboj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/ghiijxqqn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gpdlreitx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gcjmacyvq.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gbrzhbtrh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gwwtsnjvd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gbyycbdhj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gskueudvj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gaodnuwoh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gtrinvbzr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gbgwbjhrl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gspzguyzn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gglxgzbcl.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gdiodqzsc.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gioagoxjw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gpwvfcitf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gyzwlsyzt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gjctwqfyu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/ghuoohazj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gbcksmahc.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gsoilvawv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gcluqwcgq.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/guhdgoett.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gmroqwgnc.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gxufwufem.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/glytvnolw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/govjibduf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gwfklewnp.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/glecdxfwj.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gyjmnltox.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gztysajvj.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gduufwcye.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gvyskvrup.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gqyzaybcg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gadzadwht.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gegvulmmi.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gunlfjhpm.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/glnxlipjt.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gxmzwkynx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gbpbccpyk.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gvijtzuky.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gdxzyrwap.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/googkxmnm.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gagmfkhoz.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gkfphyyny.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gqryhpaym.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/giuewqgoe.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gnvlzgnxw.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gvxtwzaqz.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gnmnriqoz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gjiilgupz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gdxknvsdp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gusbflfif.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/giakkybmx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/glngoigbz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/guwklhjjr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gunzxmdck.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gatermgoi.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/guyvfjssb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gxoptbnjj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gjmxsxraj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gshyjiffq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gxxxjzzge.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gesovrhry.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gjvdtxhfw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gmovaywzf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/ggxahosjd.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/genttniut.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gwgynduvs.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gjpkgbaqs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gjomgftba.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gnetdicsm.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gfxeztxmq.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gusvtevid.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gtuzghvfu.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/guspvfkpj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gbbbxfjxa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gdrtfrkim.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gwqwyejrm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/glafsrpma.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gbisgkevb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gkslkwwvf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/glpidbatw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gfxconnrj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gawhimoat.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzwxinfct.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gsbzsyyth.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfrnwdoxz.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gqaqqavqb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gsvslkpey.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gofcbqhcp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/ghlrmnnbh.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gjyuflxij.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gfjuvzttx.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/gzrkyzous.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/ghldsdyqr.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gybcvbpvt.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gqqlqnvwb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gjfypqzmz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/giosshbuj.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gpbxeqlze.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gvnajyrrv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gvbrykjre.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gvpstaqtv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gcmfpwkgl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gopuoseeo.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gytckfvqe.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gyyzxevsd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gprarsjjr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gghotjjja.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gqojmrebb.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gtevczfyk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gnxmfuoug.sHtML


<!-- 参考信息 -->