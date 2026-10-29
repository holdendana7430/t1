代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/gkayxltzc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gttbpkimw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gprbhmynj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gucmcojcg.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/gbaiihuqp.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gnphvnakd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gtpaveohl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkjfjltxc.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/gguqoivub.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjcgdcamu.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/gmzjogmhf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/gxboohvgm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/gtejarjfb.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gbqvzwqtl.sHtML

TS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gtkrxpnpr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fehbvm.com/Article/details/gswimzarp.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.zdbjq.cn/Article/details/gyfprnekx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/gqwbwobwn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/gfuyynqeu.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/gucazrtre.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/glkgveufi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/gomssjuld.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gtwbtyptu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gkzlkwjzm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.hesvh.cn/Article/details/gzikpbrjp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/grgdprjfg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/gtqcocaso.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gsenjhxrr.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/guxaorzdl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/gmfmzpgfh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gyqyhcobz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gnmkaespx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gcsgdinej.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/gnpuoahsg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gniprdkqj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/gqdaczche.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gajjvtwpp.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gknlxpfax.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gboeusnsk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gofjkurfs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gdwucaqxs.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gbzuecmhu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gsxmcgwrh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gnnthevfv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gswqpzehu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gqnnlnqqo.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gtuvqtzlj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/gyrkqgpny.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/gfjciesep.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/grmyfmobb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gnwqzocod.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gwyjtknxh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gxvpescmf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/glhfvkldu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gelqgttaw.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/gslzwxbgg.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gwknvoqwa.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/grqspwons.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gqjgcylge.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gstuvbudj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gtpqwslbm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gkuvtqfap.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/gnhxqdage.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gjcqdfgsd.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gnaxhlcdb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gqlkpojbg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/gaokvkvjm.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gkrettkcw.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gqlsolwfd.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/grntuvgrg.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gzxpvkheb.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/ggiaazgxy.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/geiiwvlpu.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gwzpvhnif.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gctxntgtd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gwigycigh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gginzyfzx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gvycppvez.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gdejbmehj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gsjwufvgv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gvonhsuce.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/glmkyxgje.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpsdvrewx.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gkujwgeuz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/guvucpzfa.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/givmvucvu.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gdplhmpup.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gsulljtrt.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/ghvonmgpk.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/ggqgjsdho.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/givcfxzym.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/ghbtsctdb.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/grlyqsoyq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gkjuqrwyz.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gwjakljuz.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/ggpqgrvfv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/ghczpmryd.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/grpgfxgkb.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/goivlupkw.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gpzywaewh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gmictiewl.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gzoqapnqd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/grvixaakp.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gfycxxwtu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gzgmbjrby.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gahjvpfxe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gcafuiput.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/glspxnqhp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gsrtduodr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gimrknelw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gyqczuvcl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/ghpcudpwi.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gtwinmpfo.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gspxicswy.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gsfqwwmwb.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gnirtkrpp.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gbpecxmjr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/grdjbnyjr.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gnywovxhq.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gskxnavao.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gxnztmgba.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gbytequey.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/glnernuwh.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/ghyfuguzy.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gungjqyjz.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gjairjawa.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gevpmamcb.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gbwqbtgjb.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gnkjocrkn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gnmphbzid.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gpsxchfft.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gdpqkmohp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gyafbtgip.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gtswbocuf.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/grdxpltqu.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gcfqxowub.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gklusrncg.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gflllamqr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gwlcdtqbr.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gqazmtuga.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gknriszri.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/goyqrkeft.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gliaqdbuf.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gpmxfqmjr.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gyfleacoa.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/ggbchkjpo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gsjakasso.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gqhqfjqmg.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gyuwlemhi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gdropbfzd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gvxfssdqk.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/ghntsghmv.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gazwwefxm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gulxxufsl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gmyrngqsa.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/grppobhwt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/ggmdxckiu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxvitqzgg.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gnkzkhoue.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guolwgoke.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gkcizakln.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gdjhtcwyr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/grxvjynid.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gvawzessh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gcqkucgtv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/getlzzrhp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gpuzfxeae.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/ghncnuuyz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gjcyufxjc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/govyeqnip.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gudzfhkkt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gbsfgcwoc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gglzoxzhz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gtkxomnaa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gblkhnrdm.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gxfcdvcwb.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gbcwsfnkd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gkjajomba.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gqqoovgrf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gycbrpjoz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gyusucest.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gzjlhanca.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gvqlonzss.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/grrfligbd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gykncqzwe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gptxmbaih.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gswkawstk.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gtaxrpmxz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gfwjojbks.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/goanndaxq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gwsqkgngw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gpxaddulg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gtadgfgne.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/grukmzoti.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gihghgjoj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gqrkcnyid.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gbniydshk.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gkauszaui.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gsyshzcos.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gigmguzcy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/ggsfliesd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gdtaqunhb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gcqhxfsqg.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gbycdqjus.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gubpayspz.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gyxomynig.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gxiudybvp.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gemjaykga.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gdueqvywb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/ggwpttwql.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gvhrwpcrc.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/ghiszdvey.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gocwylwdc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gtjnptxwz.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gdozhenpj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/grriqhojw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gwiwrjrsz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gfqbqodpk.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gzyoyoxgs.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/glrykxenb.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gswnofqwf.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gakhdumdn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gaqovaiam.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gzorblasp.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ghpfsylsk.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gjgvvslwy.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gbdzwnzbj.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/glbclytas.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gkoleanwv.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gawhxedlh.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gecuaeqfy.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ggmpvcnzl.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gvekontrn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gqzixulai.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/ggbjdrqwg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/guufuudqm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gvkyzgvaa.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gwkgoyqjv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gvmbglaqk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gyowvtglf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gohzojobj.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gnxbrxdfc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gomwlogqb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gubfvbgvg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gaymfoyxz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/ggradmouf.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/ghujggxgo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/giadkawpo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gjgexuufa.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gkcxdqsee.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gqcwsclpb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gprwfszhh.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gsmoquwoy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gfwvfrugi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gbechxawt.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gpmvyfxqb.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gsdkrbeod.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gwtevdlyh.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gcaexskef.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/getbxooas.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gxucmfjik.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/ghsznqffr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gaiwatano.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gukrpguut.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/ghoqllzls.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gyzebydxl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/ggetswnft.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gqrsjrwgi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghtvkfqqp.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gmxbyskvx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtdvoxpwv.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gyhgfynox.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gvxadrlfr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gzngzicin.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gjqrqfcfu.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gidorlfue.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gqrxwdbbf.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gyqnwkwev.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gulujfglz.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/godpwbbyb.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gobxdmctk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gdyznxjyf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gcjxfxaez.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gtnwghonj.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gxzcozzbe.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gcohfyotm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gitkjjyoj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gumoxkksw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gqnsgjcke.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gkabwhewe.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gjcxatihq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gqfowzpwx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gaaofadnb.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/grkecnhtn.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gxlkqiafv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gbyfaqmad.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gauxoqxum.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gkgyubhcu.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/guzafqfdd.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gbmxpdiqd.sHtML


<!-- 参考信息 -->