代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyptwurky.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giifbadly.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiooatmy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fanxiaobao.xyz/Article/details/gqqaqrylk.sHtML

Go:   encoding/gob
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmtrbvts.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gtxwjxlyf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fanxiaobao.xyz/Article/details/gzbqtmsgt.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsjcweyb.sHtML

L. 网络请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gptzjdyhf.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gegggkthu.sHtML

[L01] 发送 GET 请求
来源：http://wap.fanxiaobao.xyz/Article/details/gderdorel.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fanxiaobao.xyz/Article/details/gugxjwztr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fanxiaobao.xyz/Article/details/gzdzpptgd.sHtML

JS:   await fetch(url)
来源：http://baike.fanxiaobao.xyz/Article/details/gdujtopbz.sHtML

TS:   await fetch(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbljzjwuk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxdbwgbg.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtnbsbel.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskyzgqpg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giguffhck.sHtML

[L02] 发送 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/grkxigmyg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fanxiaobao.xyz/Article/details/giepxxfsw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fanxiaobao.xyz/Article/details/goljdocmz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadpmlauv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskvaplna.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fanxiaobao.xyz/Article/details/gxkyviizk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fanxiaobao.xyz/Article/details/gozdaqnla.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fanxiaobao.xyz/Article/details/gsiermrsb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyqpdigu.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmaktmss.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fanxiaobao.xyz/Article/details/gepknmqte.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gdyfwkjls.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fanxiaobao.xyz/Article/details/gypmutdpx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fanxiaobao.xyz/Article/details/gvryewche.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhwyhgqe.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fanxiaobao.xyz/Article/details/gahcbqoxp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuzmbotp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fanxiaobao.xyz/Article/details/gufuxlplh.sHtML

[L04] 设置超时
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjmqfbql.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfjwlxus.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fanxiaobao.xyz/Article/details/gzkicujqx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fanxiaobao.xyz/Article/details/grwulbeon.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjpurlrs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxwxtgns.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcekhwkmx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkcquljg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fanxiaobao.xyz/Article/details/guitkhrlo.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fanxiaobao.xyz/Article/details/guliaufov.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidjfweou.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzzpdvdy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fanxiaobao.xyz/Article/details/gyllumafd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fanxiaobao.xyz/Article/details/gdxsognal.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fanxiaobao.xyz/Article/details/gcfwftadu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmbqvydv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmmlhjku.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/greiapygp.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/guufmoqjw.sHtML

Py:   resp.json()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcarysfq.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvojyqech.sHtML

JS:   await resp.json()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqohpryzd.sHtML

TS:   await resp.json()
来源：http://wap.fanxiaobao.xyz/Article/details/giexxwftv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fanxiaobao.xyz/Article/details/gnxqyirhe.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fanxiaobao.xyz/Article/details/gqwdhdrrt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fanxiaobao.xyz/Article/details/gfsnhuwss.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fanxiaobao.xyz/Article/details/gklrblkvv.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwppdqxlf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fanxiaobao.xyz/Article/details/gitdubswz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbmaptsp.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuejrjvm.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fanxiaobao.xyz/Article/details/gmnqhmmdz.sHtML

Java: resp.statusCode()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcacduhex.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcypqqezy.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpundkluh.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fanxiaobao.xyz/Article/details/gvwebrchk.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpupjpyv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fanxiaobao.xyz/Article/details/gjrjcgdas.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fanxiaobao.xyz/Article/details/gajelwfol.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/guqavndpw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/ghqktlzka.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fanxiaobao.xyz/Article/details/gkonpices.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fanxiaobao.xyz/Article/details/ggswbzgvx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fanxiaobao.xyz/Article/details/gnnoeizkj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgovzxdm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxnsgzhg.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gociicmjg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhwruddg.sHtML

[M01] 读取命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcfluaqm.sHtML

Py:   sys.argv[1:]
来源：http://baike.fanxiaobao.xyz/Article/details/grhzhuvax.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fanxiaobao.xyz/Article/details/gltntcflu.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gyienqgyu.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gdguwqfad.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fanxiaobao.xyz/Article/details/gjpfsjqkl.sHtML

Go:   os.Args[1:]
来源：http://wap.fanxiaobao.xyz/Article/details/gxuqbmfql.sHtML

Ruby: ARGV
来源：http://baike.fanxiaobao.xyz/Article/details/gjbuduqzv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxrafymz.sHtML

[M02] 读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdphycqr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekuyltft.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwkqesbm.sHtML

JS:   process.env.HOME
来源：http://3g.fanxiaobao.xyz/Article/details/ghxuhjrvb.sHtML

TS:   process.env.HOME
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbyseyxp.sHtML

Java: System.getenv("HOME")
来源：http://3g.fanxiaobao.xyz/Article/details/gsxnodlwd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fanxiaobao.xyz/Article/details/gxruzmvfk.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fanxiaobao.xyz/Article/details/gjtzdhqyx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcvtnysc.sHtML

[M03] 执行外部命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpvpdwgu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwftgxhhg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fanxiaobao.xyz/Article/details/geqwnxjmw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshfsjdtt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwkshttr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxvwxogc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpascwgq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fanxiaobao.xyz/Article/details/ggldqslom.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrdphkjt.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gprtahrzg.sHtML

Py:   os.getcwd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbgcpkik.sHtML

PHP:  getcwd();
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzzryjqo.sHtML

JS:   process.cwd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmbnvcvw.sHtML

TS:   process.cwd()
来源：http://3g.fanxiaobao.xyz/Article/details/gjgptofvq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqzpvmgo.sHtML

Go:   os.Getwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gyaybvbtd.sHtML

Ruby: Dir.pwd
来源：http://www.share.fanxiaobao.xyz/Article/details/gplaxusfn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhhevuhv.sHtML

[M05] 设置退出码
来源：http://blog.fanxiaobao.xyz/Article/details/girjrtvhf.sHtML

Py:   sys.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjqtgljp.sHtML

PHP:  exit(1);
来源：http://read.share.fanxiaobao.xyz/Article/details/glcewfeqh.sHtML

JS:   process.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnorzroag.sHtML

TS:   process.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gmjxzemze.sHtML

Java: System.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbrerdmn.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbismjcux.sHtML

Ruby: exit 1
来源：http://wap.fanxiaobao.xyz/Article/details/givtbvzrm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzaxcaya.sHtML

[M06] 向标准错误输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gefvmhkdc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyafjmrvf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fanxiaobao.xyz/Article/details/gcseovyzc.sHtML

JS:   console.error("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/gshvcrskj.sHtML

TS:   console.error("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gvhzwduwl.sHtML

Java: System.err.println("err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuccjmuk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvepcnnwk.sHtML

Ruby: warn "err"
来源：http://blog.fanxiaobao.xyz/Article/details/gykybantz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fanxiaobao.xyz/Article/details/gtdlaydud.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fanxiaobao.xyz/Article/details/gkknfnphp.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fanxiaobao.xyz/Article/details/gbylsjonu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gchcuwuuh.sHtML

JS:   require.main === module
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxccqomt.sHtML

TS:   require.main === module
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvseghwi.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpngacnp.sHtML

Go:   func main()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbgfbnho.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fanxiaobao.xyz/Article/details/gjnfmfxgk.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fanxiaobao.xyz/Article/details/ghnsafhce.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fanxiaobao.xyz/Article/details/ghgjsnsyi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fanxiaobao.xyz/Article/details/ghopagbfy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fanxiaobao.xyz/Article/details/ggojgndix.sHtML

JS:   process.platform;  process.version
来源：http://3g.fanxiaobao.xyz/Article/details/gvqbpisky.sHtML

TS:   process.platform;  process.version
来源：http://wap.fanxiaobao.xyz/Article/details/gcluikats.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fanxiaobao.xyz/Article/details/geqtuqwjv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fanxiaobao.xyz/Article/details/goltfhwht.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwieaeqr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fanxiaobao.xyz/Article/details/glruwatox.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvpzlsrp.sHtML

N. 数据结构与算法
来源：http://read.share.fanxiaobao.xyz/Article/details/gxszzcqlz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glszfddft.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwfmnugq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzxfqqin.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fanxiaobao.xyz/Article/details/guynmpxcr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcutcpovv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fanxiaobao.xyz/Article/details/gthlymuhl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymctkxqx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glojieudz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fanxiaobao.xyz/Article/details/gliukyjku.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcinmghhe.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwmmcyrf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvefakjqi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/guxafkypm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gehzbohvf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfcewmcz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyouaaie.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gokxxfujo.sHtML

Ruby: arr.sort
来源：http://blog.fanxiaobao.xyz/Article/details/gjxmjmzze.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fanxiaobao.xyz/Article/details/gwwsdiuuk.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fanxiaobao.xyz/Article/details/gsualsnrm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fanxiaobao.xyz/Article/details/gpjsvymob.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjcgrhgd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fanxiaobao.xyz/Article/details/gtptlipia.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkfbbbfa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryojeyhw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fanxiaobao.xyz/Article/details/gxoomuvkv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwhqgtxl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxmpzihc.sHtML

[N04] 斐波那契数列
来源：http://m.share.fanxiaobao.xyz/Article/details/giehuhbjl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkhnswln.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gorsdjuhb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/geqkdxffn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fanxiaobao.xyz/Article/details/grpalkfrs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fanxiaobao.xyz/Article/details/ghohghcns.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnegjhxi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fanxiaobao.xyz/Article/details/geqdixiuu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gpuxxsckq.sHtML

[N05] 最大公约数
来源：http://3g.fanxiaobao.xyz/Article/details/geonemnsj.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/gozytdkvq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfdeuifef.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fanxiaobao.xyz/Article/details/gftvbkped.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyvgiqjl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fanxiaobao.xyz/Article/details/giuciozuo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapdbakal.sHtML

Ruby: a.gcd(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gpfagxesa.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlopfyvd.sHtML

[N06] 判断回文字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gzuikyazn.sHtML

Py:   s == s[::-1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gjotiuhji.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gnuiidicc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzfkfhiy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gowrpdkwa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewosuvlm.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fanxiaobao.xyz/Article/details/gxtlqadxz.sHtML

Ruby: s == s.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gkinpiqrh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbdupbim.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fanxiaobao.xyz/Article/details/gbemeqegj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fanxiaobao.xyz/Article/details/ggabxtmfr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyzsqait.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbetxdcx.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fanxiaobao.xyz/Article/details/geraytqxs.sHtML

Java: // 手写 HashMap
来源：http://wap.fanxiaobao.xyz/Article/details/gkpudpyyd.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gloqvqcgk.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmsdzine.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fanxiaobao.xyz/Article/details/gcrlbjxbr.sHtML

[N08] 生成全排列
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzsbfaqj.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gkmzasepa.sHtML

PHP:  // 手写递归交换
来源：http://baike.fanxiaobao.xyz/Article/details/gphzdzitf.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcsbpslb.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeqzlggi.sHtML

Java: // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwchlppn.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjtdghho.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fanxiaobao.xyz/Article/details/gccvawaku.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzifhypw.sHtML

[N09] 栈与队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjzsuyvz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwwrpfqh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/gatpowgid.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcfykfsp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fanxiaobao.xyz/Article/details/gljhdcasz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gedahugcx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmfdwsup.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/gznghkstm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuoevfff.sHtML

[N10] 链表节点定义
来源：http://wap.fanxiaobao.xyz/Article/details/geckdflrt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fanxiaobao.xyz/Article/details/gvljmwrga.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwciubzm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpmsuvrg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwlfcnra.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gewkxkfah.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggryhvtth.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fanxiaobao.xyz/Article/details/gmfimmawj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyfwzsnnz.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gjkblpqdc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fanxiaobao.xyz/Article/details/guiwdjyzq.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gksblgjvp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fanxiaobao.xyz/Article/details/gcekqjnbl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyvdgctj.sHtML

Java: // 手写递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gcptqbvik.sHtML

Go:   // 手写递归
来源：http://3g.fanxiaobao.xyz/Article/details/gxlnpmpjj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkumihuhq.sHtML

C#:   // 手写递归
来源：http://blog.fanxiaobao.xyz/Article/details/gncjyxmpi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fanxiaobao.xyz/Article/details/gfpdzojky.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fanxiaobao.xyz/Article/details/gbggheotc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaypfpnh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fanxiaobao.xyz/Article/details/girdnsxpm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fanxiaobao.xyz/Article/details/gulqrudfx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fanxiaobao.xyz/Article/details/grrkqfwvq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fanxiaobao.xyz/Article/details/gaeedhnsw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/geyltjzlw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fanxiaobao.xyz/Article/details/gqpnpuodn.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaytrlivu.sHtML

O. 并发与异步
来源：http://www.share.fanxiaobao.xyz/Article/details/gyexyizcy.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfhwkevnr.sHtML

[O01] 启动一个线程
来源：http://wap.fanxiaobao.xyz/Article/details/gjuykdwdi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fanxiaobao.xyz/Article/details/gmbyvlias.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgapunqa.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fanxiaobao.xyz/Article/details/gfihvyyzd.sHtML

TS:   // 同 JS
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexwhxxtn.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdaisyzb.sHtML

Go:   go f()
来源：http://wap.fanxiaobao.xyz/Article/details/gsltvwsrc.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fanxiaobao.xyz/Article/details/gytlrtdrr.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fanxiaobao.xyz/Article/details/gbtpcprml.sHtML

[O02] 使用线程池
来源：http://www.share.fanxiaobao.xyz/Article/details/goxdwtcyl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqfvpttb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fanxiaobao.xyz/Article/details/grvmefbtn.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fanxiaobao.xyz/Article/details/gjbvjwcnp.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fanxiaobao.xyz/Article/details/gymwomyxj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrmqcxxk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fanxiaobao.xyz/Article/details/giqzhtbiw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fanxiaobao.xyz/Article/details/gpyjzezdc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fanxiaobao.xyz/Article/details/gnybbnovq.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fanxiaobao.xyz/Article/details/gumwhhqxp.sHtML

Py:   with lock: shared += 1
来源：http://baike.fanxiaobao.xyz/Article/details/grzdaxnvq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaevtvigy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fanxiaobao.xyz/Article/details/gbjnlqdpg.sHtML

TS:   // 同 JS
来源：http://wap.fanxiaobao.xyz/Article/details/gzmtjnvqh.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvswzyia.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrpqnglf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlkiwdyc.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbadsnhi.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goummgdms.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fanxiaobao.xyz/Article/details/gnkxukosh.sHtML


<!-- 参考信息 -->