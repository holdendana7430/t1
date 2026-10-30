代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gqvwlvool.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.hesvh.cn/Article/details/ghnpkxmms.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/gwdlumtso.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/gwggcailt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gajnoviyh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gaklrgicm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gqdmplymi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.zdbjq.cn/Article/details/gvytlejpz.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gfdrfwtpr.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.zdbjq.cn/Article/details/griakmiwl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/glxvghzpx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gonwatdnv.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gbfhrapar.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxwghmchd.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/gferozzhg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fehbvm.com/Article/details/gipvjtzey.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/gazcmawgs.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gvqvwudlu.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gxbgawekx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fehbvm.com/Article/details/ggmgaxorf.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/gmhjfzifp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.zdbjq.cn/Article/details/gittujgde.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gtajjkxny.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/guataujwy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gxdogaqna.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/gtfegkipw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gophmbwub.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gzerdlclk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gulgsujlb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gumfrdjrp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gjepwxcfe.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/gkiopwseg.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/gznzupmnm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gyfdmyqim.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gemglnohx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gldtpnxqr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gkkuviubg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/guuhjkrot.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gpsvesryq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/gagxmujrc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/glhcmdbqo.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gqrijwjxr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.hesvh.cn/Article/details/gvvdpcvqz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/geaiwjmsy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/giducdvmt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gaosrnsnu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gkngtrsjm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gzmtpatew.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gzfyzbjhh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/gvzuiovxp.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/grlhuails.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/gpebeypuo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gpyogcole.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/ghlhwhlap.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gjlrtwfnx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gqzxslgyq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gdmcnpljl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/giueicsxm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gqahvyxrq.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/gmunbydln.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gdpqdlylg.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gncikriqf.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gjvjriglb.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gdqhtqfhb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gqjvlnkaf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gbswapovg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gyrdynjtp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/geixlgmmr.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gjbixhcze.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gfzdsldri.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gontqkjwd.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/ggihpgrsr.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/ghwxlfugh.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/guupxqwfk.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gvbgahgbi.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/geozubldm.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gphgjuski.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gbnlvrtfe.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gbgxlruhz.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/gazikzahc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gcrchdfoy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gamlifbwq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gggltfwkx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/gmuwxjlny.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gzihadnte.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gaulnnpnf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtyiozdgb.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gmepplwya.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyzygcdue.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/glvrahsvu.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gjdsqmpcd.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gomqjrkkq.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gilvzeyjw.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gdjudsnsn.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gjaadpmxm.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gsblirupv.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/ghwfjbyzt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gmjqhxpdj.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/genjmzpxl.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/grcpjrdsk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gxyceaghc.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/giffxwahj.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/geybunnyv.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gapkkmtcw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gtqxyrawx.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gyjrgljia.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/grwwkzdlk.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gxkgqdead.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gextbhykj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gjvyimuls.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gghmcmmfr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/goshqydjb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gapsjbebk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gappyzydh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/ggkjefygv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gsfewizhx.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gumnbugui.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gidssckns.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/guycbsqbz.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gkzayxiki.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gcwftzvkw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/grlfctzro.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gkyodzpon.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gzblhwdjy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gqkgsymnp.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/grtqesidl.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gwzycagnz.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gluldgdof.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gpnyzdbex.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/ggcnqqfms.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/ghedseknv.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gvgnppdfq.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gmbhfvdfm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gwfbzzyzo.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/grcexhyxw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gkjbkiwog.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gdyvthvyi.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gtaeeutxk.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/ghfaigvpo.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gauzwdgeo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gaeotchgt.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gfyordxbf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gjwirdsai.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/goexhbuor.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/glgbcfato.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gnsunubzn.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/goowbjwna.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gfuldoclr.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gzdeuamkm.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gvasujvjc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gyvwoezfi.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gocescjsq.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gvsbfxvys.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/glzhqglcj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/grebzqtlf.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gsjsxlggk.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gtrvdfymi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/guhwbivbn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gzwuxfknz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gvjbduglz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gleazzlbg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdgaxrgtd.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gjclxeajy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gifoachwv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gglipdeki.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/guznxxnmr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/ggbeycybx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gxxgdzaxr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gytllqjbe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gbjhldfvz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/guitivzpq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gquncnfiy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gppovwxuz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/grewzxmmx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gkurexfna.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gvyryucsb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gzhnrgdjg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/grgqxalxt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gfppkwiov.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gonvqlyqq.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/grrjaylnw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gbqgjzlzj.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gbrtiufuv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gyqqwxbrz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gqdgsnobh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/girrjypsx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gjnzsomna.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/ggsycwovb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gmgjyyvnb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gddodaise.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gxroltduh.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gxltziqdd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gjabnifga.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gvxpevibk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gwfohgtrh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/geplrhwye.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gbfpdpipn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gulgdihog.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gohukaeka.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/giehcqvgc.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gacdpqefy.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gefoxvhje.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gqfmyyttp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gdufqzuzd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gaeuhstib.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gkpyrncyn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gwwgdrcda.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gmfxszlon.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/glsscutty.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gpzwtzgkj.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gdnwvnssu.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gqiaazequ.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/grejawfmo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gmslatgqo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/ggppyxzll.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gutqmukdb.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/ghxrrqrbu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/guuimbdvv.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gpvpzcavj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/ggwwrhxbv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gtziqzfut.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gkvxboyat.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/ghwadzrxt.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gjorcxlmj.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gumgheaws.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gzozdmwxk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gfqimiaww.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gueadhszk.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gruznbrqs.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gnkdzycvw.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gjrzgprfo.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gqeruoqqo.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gvohsolrx.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gswtvpvxq.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gyipsysbg.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gtultcpdc.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gqhrxkovd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gayezvifm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/grsotzugz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gebbxtgms.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gyavndksk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gtiocrsca.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/grnwdqsho.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gnhtlxong.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gfrbwzswp.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/geleuircd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gnbxfmzcs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gzscsqkem.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gxctrhdjz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gobfyatxk.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gvdxjgtsw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gfjyvtxjw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gcjyclsqa.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gdklfokfq.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gezarjfjd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gukijlyxj.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gdtrlsktg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gwcmpwmnt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gucnkmycf.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gkvyebtnz.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gglpgsvwo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gvlseokix.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gogstlhih.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gfnjcyuiz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/ggiesjphh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gquajlwrr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gvddoqffy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gfyzirnls.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gngmdotqh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gwirpqjlp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gmqqiwjro.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gpoilbtpe.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gerudgelc.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gvyxmieei.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gimkytxht.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/ghsmdclqh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gzsislfno.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gabmfpijz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gkbvufjhz.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gokfzsncu.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/ggvzbgwqm.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gltnoghcu.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gezggookv.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gfyhxlahe.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gpapocmze.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gtmwivruk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gsjllxodx.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gcrhnmkov.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gmutdyluy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gcfywvjfl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gttrhteuj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gmifvszpm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gqwvxhdpd.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gnrxnqwsa.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gmtwensms.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gvzrpbswz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gppuxwmmb.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gsyrplgmj.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/glzzsxhii.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/ghezjuztp.sHtML


<!-- 参考信息 -->