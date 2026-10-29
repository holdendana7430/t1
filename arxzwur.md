代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gxqxjeozb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gvlmglxav.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gywhxgsgn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.hesvh.cn/Article/details/gpkwptjpt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gvaypqphk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gahavounl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.hesvh.cn/Article/details/galimfyyo.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/gycfvlnzx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/gogjkrdsm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gkrrcfcjt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gotjfpzyu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gjtxlkurw.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gefhkwbbp.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/gmpoevwkd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/glltlqmsd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmsmqhrjr.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gfiputnhg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqbawxjhh.sHtML

[L01] 发送 GET 请求
来源：http://3g.hesvh.cn/Article/details/gmqzeydxu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.hesvh.cn/Article/details/gdpowmrfz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/geoqzxnew.sHtML

JS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gyjyqyess.sHtML

TS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gupikqoui.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.hesvh.cn/Article/details/ghbtnewqa.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gummxxhxu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gyizlxtga.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gsscmlqns.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/guxatumzg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gzuoaqcdt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fehbvm.com/Article/details/geyasuotj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/grsqsjtlp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gziuningm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/gxeahvflq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gczsjzudg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/gwxhachvj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/gghbmrlmi.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gfhawieaq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gcekmwdfj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/guntmnnwj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gatnujjnc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gfpnvxnnx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/ggrknorlq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/ggjuicshb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/gjmrhyxvm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gkciyrldc.sHtML

[L04] 设置超时
来源：http://3g.fehbvm.com/Article/details/gxbpwdyxq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gzioypltt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fehbvm.com/Article/details/gyrognwmb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gouxnrzjp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/ghamcwrhv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gnjrjruys.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/gnelgbkex.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gfczatcwb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gjvrziwdh.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/gwuvcllwc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/gltmytyqa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gwuicwhce.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/giksxnzyy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gfifxmrwq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gmawblumh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/gilwuvnju.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/gppnmtpjr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/gwuxqohws.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gqdrddqsi.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/gzitcvgvf.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/giiwedlxj.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gkqunduye.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gnutkgjhl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/ghxiyrsxu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/getbdgplz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/gjxvxocjl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gewtbqcgl.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gznaqvbno.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gdhvoapll.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gjkrqmxhx.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gbuvxycsf.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gloappxaj.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/ggpxmhqza.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gxucdxvks.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gunrwrkhm.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gwlzgzjrd.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/ggtucfjiu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gbxjpmlyu.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gbgtwtrhz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gvyfkvyfp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gjlddvswo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gsygwiapd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gqjhrojne.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gpwatrhdb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gixmjjjsd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzytoralf.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gpxftjdkx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbiqpxzkn.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gfsyutrro.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gyvdjzecl.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/grpwfvqru.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/geqlowtre.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/giegnzdbv.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gvmiwulrn.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gvujfsuxv.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gejraripp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gyyqraivw.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gnniywpos.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gsvuayqge.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gxgzpzvav.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gnzpvzwgn.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gaxtwtoww.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gfcfyrbqt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gobcfolji.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gbqxbrthg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gqqlwfegb.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gzjaxmsns.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gznrpiqyu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/grqbfdcdr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gcqvobxmo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/ganbhoaqk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gsavkipct.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gikjhihpf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/gvlyzhdun.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/grtclaibi.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gfhnxycax.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gryhuiote.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gipdaddze.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gcbpurjdg.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gymvtjzmn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gymoaxxiu.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/gzjpktwmi.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gfwsguyzi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gxxqckonk.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/ggjqaiezr.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gnsxnxsmy.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gbztsakej.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gwnkmjahx.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gdjmzulyd.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gaucmgrzf.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gamczbqjr.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/grqipxgeu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gteecjcfv.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/giizqftey.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gudaogsvo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/geilrhwjm.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/ghmeqtanf.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gdrmdcgef.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gzugtpmbj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/grgwlnkkj.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gqaujmrfb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gayfolwwb.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gqsisstxr.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gnymwsadk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gdbkjfitu.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gtkvtfifv.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gqltlhawi.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/ggcawhomb.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gshtiytkn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gtckoyhcv.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/goliwrkkh.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gkxsmzhne.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gjctibbml.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gqbcvtbai.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gmhdzaibc.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/goecawpbg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gnoybvxpy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/ggritliuk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gvhylxfzw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gmllnurlm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvbezncyn.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gqabvevmx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gazzaaqwt.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gptvrsxig.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/ghkpjvcds.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gxulayfye.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gzlsemwmi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gudrxicqv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gipzqbkty.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gnsucryzc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gzsrktghy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/geehdpcor.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gkebqrdde.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gmnedxtxi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gsldjhjoq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gwgxopkdd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gmwtrsrov.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gxmjgqxzk.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gpckgfbbp.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gwbumncxz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gypoupbqm.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gazsosxrd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gipbxpcao.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/guxoaevgp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gmqssxyao.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gimyspblv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gknrgxmfp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gssjpimur.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gorbjtzct.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gxnwtgkdd.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gdmkiljhg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gdqcxncrc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/grkpyiinh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gtbkjyehv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/ginqzajob.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/ghmgxsabs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/grqfmwauh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gdsixfamd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gcopcqqdl.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/ggdsomcaw.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gjzhbtfnd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gefhlfbfv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gqdgaopzt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gyygjkghv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gqredhsoz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gbvtcejqo.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gbbvqhhqb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gikseelgz.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gywquzuxd.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gwifhlhge.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/grfrbdumu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gdxcaqoxa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/giwcoerhh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gghochmkk.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gcahnujek.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gkaoonjpj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gbxgnkgos.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/glmanfffv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/ghxcoxsok.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/glmuuhsdp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gtdqqemcv.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/gndvofnuy.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gfsmkooyh.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gdvqbnfhz.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gbhvdlavg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gmsfowtty.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/girqczqup.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gezdtqldc.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gklrolzwi.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gcxoayflx.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gnyjzbbch.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/grhozperj.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gdyrhrpjq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gwktvjayc.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gbndfvnmm.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gmhsbvgdf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gpnooctxg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/geptpdolc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gbymrbqrv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gbygloure.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gnaxwbjol.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gorzosqaa.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gthixwrmh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gpuprwzut.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gsbchrkzb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gfomytrcp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/gaigcevgg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/geyqcmtjs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gfozyyqxp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gvdmrcrzd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/giwtflbzp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/grerewklo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gacplcvsg.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gqoybfbor.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gppdurowu.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gzkmmyips.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gossgkoau.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gfrjxbqyv.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/ggbuepeoz.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gtgngjovf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gsrjzmvzk.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gktbctfgw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gwialsbrk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gcmbirglo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gysvhsdsm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gductcviz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gzhcxoqxn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gtcwfbswg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gpuntbypc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/ggkhakrhq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gmgxmptcw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpgbxgffn.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gnjgmebvp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvzmahisx.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/glcsthtkj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gzzxllcuw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gzwttvxoq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gxliggppd.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gbakacapp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gevkfxitd.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/ghsxwuvdm.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gbbgkterj.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gjschszfc.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gzaabsria.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gdudmvexm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gbeojockz.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/ggjyfeqso.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/geazhvumq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gvvjlzqlw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gnxisintq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gtmkmknae.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gbstzoago.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gxsdvakqg.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gkatjlmou.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gnxgfqfaq.sHtML


<!-- 参考信息 -->