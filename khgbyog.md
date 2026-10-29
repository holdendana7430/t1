代发 wailian999

Go:   encoding/gob
来源：http://blog.hesvh.cn/Article/details/gqstoptxw.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.zdbjq.cn/Article/details/gulhwggqp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gwayxtlpr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxxemajdv.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/gfcvgochx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtjmklxew.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gvglldcyh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/gmvewqpoc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/gzoyrzbqk.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gxzsmhdzb.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gfcbbinsj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gwxtucycd.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/gjmgaffco.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gsotyxuge.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/gxifhldoy.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gdbapbson.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gvksensuf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fehbvm.com/Article/details/gfyerzryx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gwrhojrkq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/ggrscvkrl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fehbvm.com/Article/details/gjjgjyojg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gkcvwdoym.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.zdbjq.cn/Article/details/gylmicbsc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gjfxpbyqq.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gpsjceefk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.hesvh.cn/Article/details/gniggxggf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/gklszxygg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gsywxzaiq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/glokvxzyt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/ghmjyoytz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gnsxgnetw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gihcoefxu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gqvzqfihh.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gcstscufv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gfdaulskr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gkepkxica.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gwtfdhons.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gdaltfuvg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gqxmqgjes.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/gijxorard.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/ghresryms.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/gjnalzkii.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gmajkedzh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gnjppiovl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gndnsqfro.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gcngipjqe.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gxennsqex.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gbxwwhmlj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/ggkvsebpi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gouvvvnqv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gvowkofhn.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/ggxzstgpv.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gwoywtcwb.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gogampkuk.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gxjztoisk.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gsadoexjf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gggqwbkhc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gnrqfevij.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gmjonrajg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gybdklzbb.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gfjcyrowv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gqtwcebdz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gjuqwzqfg.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gpnrsysst.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gaqykxikl.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/gdlqbtwun.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gfvccyrsp.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gocbnpacj.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gfnkbdamj.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/grptlooxw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gqkihgwbt.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/gfjnljznc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gtigtjtzd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/giqcwyyih.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gonjphade.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gsdwyjpfe.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gzespfuga.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gdbpajzsc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glmrbosfn.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gokosegma.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjysesmmb.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gyntpxxss.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gfewvuckv.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gwfwwwxwd.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gsipyfhbt.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gakzdechl.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gucaznomp.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gzoaqobkv.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/ggjmbnvhg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/giviveocu.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gckggbaev.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gneohrxoa.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gatbwztrj.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gipqcftvw.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gjkmqoipk.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gdhhfrhcd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gwdirezxa.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/grnassdst.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gjtcwkxkd.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/gsarvyajh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/gumntlpea.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gkycvwhvy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gsivriapq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/ghyhgcctk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gjyxxksvd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gbppzmoii.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gedaggncs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/ggbtvuvlk.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gahqekaee.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gmxvqjtvg.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/ghvpbxzax.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gyojhbayq.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gkpgfwcth.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/gvxdgcdmh.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gpjlxigdu.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/glhymvftt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/glfgtcsmf.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gvhoweqdu.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/ghxlcpybk.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gleezhyrn.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gtydxkqjw.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/giqbwctwj.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gfpzixead.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gtiatjolv.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gpvgvzmpu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/ggkexrzil.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gnsgccdbb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/goxhixrav.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/ghhlzziab.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gbqohtdic.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/glxgtnhfp.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/glskzqgam.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gmguakzge.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gxdlzsfed.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gxgyyiltl.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/goywdxoeb.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gignvisri.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gxlqrgsxy.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gbhifypzr.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gxzzzujiw.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gjcmubmvv.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gkhlsgivl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gsycxdjcj.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/ghussptsu.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gvlnhcgrj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gjjeshcsi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gipdgnlmr.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gfzjnsggt.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/glkoudkxr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/grcjflfvi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gnoccoekw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gboxdcvyi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gzeufidtt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grfczqeko.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gfmzfmpub.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyunmsykr.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gfawayizj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gljqkrupt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gaptwafgq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gcxohbody.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gshrbnlat.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gckhzevfd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gqlsxvmdf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/glgdxjapm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gndzbgaxm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gfcqymscg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gwmbwiihb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/glzhhctcy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gblfepsub.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/grewtmljb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gnparxuti.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/guseplgls.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gnffjmfpn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gjmsntcun.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gczotuhwd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gifdrpghf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gllrjwvvw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gujprxcmi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gqvwrmnuw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gqrmflnrm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/garrwvjcn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/grjygaawq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gtvscwciy.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gbznycbpn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/grsuoqodd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/grzxifihf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/ghrwkfina.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/giuyugrsp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gzjzocyme.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gfllubejk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gckzgvyge.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gvpphegql.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/glewbiorg.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/ggdirlhtm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gesupvvpx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gywwuhhpa.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/ggspwstje.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gasswtict.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gqdeyghla.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/guomppyen.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/geaibatlm.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gsfhztxnb.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gtbxrxioi.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gfloewsls.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gamrcgpxj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gxgyfoftk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gmpfiglcw.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gxmpvwqjc.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gmextkzbu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/guedqxmyk.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gyrtcsjia.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gcaekckte.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gjiivchga.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gawvquhxn.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gqizabtae.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/grqxlkiyz.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gfkjtnkkx.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gogeveubk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gtfgwodoa.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gzpvxsvqo.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gbylzyxka.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gmqfdaqky.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gzmhhgmkb.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gzletnhed.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gxtapvibm.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gfcjcdpll.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gshlfpdct.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gmipihzey.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gcxcbrcmq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gepbrtuqt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gmzlwlegr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gbwuohjik.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gtkcxmysb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gnjfpbfzu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gdpvghiqp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gyunwslch.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gdgglpyns.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gvkzjplbw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/ggdgbmcsj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gehmxmiur.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gzzwrgcqt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gpfeinayo.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/ghglbrqus.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gzvnnmkwn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gvtdutfri.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/guccfeoik.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gorwhydpr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gmkikxmtf.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gmfmscftl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gfniplmni.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gmfipsddv.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gdcfmmrew.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/godkahuyf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gggbiewyc.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gpcdmrmhl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gavrlgmiz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gvcxwluhf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gjdcmrwkk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/glhzgnayg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gmhlrtdip.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gyjfaqezp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/geqozqjni.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/ghldrfpql.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gpsawunjs.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjrocjiqx.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gujfibguf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gttxyxrqw.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gesclhwgq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gccimxnqw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/ggcgemxhx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gzwpeqwex.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gwlpzszvc.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gistajfbz.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/ghdpiwtjx.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/ghwjagmub.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gzilfulbd.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gyefaqixt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gfzysupse.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/ganchuzmx.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gbuoztwwf.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gbvnflcgj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gcvewjqyc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gqkiaublm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gxonpkjqm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gmsazfrrw.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gibjlzyul.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gacurhdep.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gfcmjhmia.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gxvjddswq.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gtgsfqsel.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gcycvebxr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gidrevjvv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gpuygveie.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gloawocjz.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gitkimewp.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gzxtbaaxn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gpxhpscsq.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gwiwkyoxs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gfzonlsia.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gyzfyzucw.sHtML


<!-- 参考信息 -->