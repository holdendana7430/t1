代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/ghbmtoacx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gnvkiwuui.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gpyyxxfuu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fehbvm.com/Article/details/gfrsxzrmo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gjkrhlyoq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gujlgaeyi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.hesvh.cn/Article/details/gtncdsfce.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/gcfrbqdwt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gcyowdkpw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gtbzdxsga.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gkxbdblzu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fehbvm.com/Article/details/gmanchhzw.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/grptlvvxz.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/gohzudqkv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gtrjljqaz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gaennagys.sHtML

L. 网络请求
来源：http://m.share.fehbvm.com/Article/details/gfrffaxxf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gypenhoqc.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gueaqrtdv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gldblchzy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/gomelxhuj.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/ghrmchfvf.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gfqfdigga.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/gsovmqhwn.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/ggyeqezjd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/glwfiylve.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gagakdumf.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/gdzvaapdw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gsghhluyo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gxrxmjqzo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gxxwpeghb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gytkksagc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gxdldudhj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/gxzhbbahx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/grpedmbsk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/gfifldmwz.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gwcfrdpqv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gpwsoijqs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gspbdnlir.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gdqcdipgo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gjzwssnln.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/ggogoshdr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gtmvzunbt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gergoyqfw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gwdzhxtrc.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gtwliecqu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/gpymktzkf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gcvfkvpzt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gevjwsyhx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gogiizbsj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.zdbjq.cn/Article/details/gnmsfrbki.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gxcvxzknt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gpobvstxy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gkhnibnqo.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/gdfgfwvmf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gyqayvong.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gzcqybovp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gtsyhncya.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gyckxpjsh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/gtwrgretd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gekdzujlc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gvkwzvfkr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/gadtixfcv.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gwkdmwbdp.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gautjdyrx.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/ghlotbjxh.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gjgnbslyd.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gxnootzts.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gkahpdlro.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/glgpfdmue.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gqwvzyolo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gpphuundt.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/ggxxfbmhl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/grfctgngl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/ggtybbkmg.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gpmwslfcj.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gowglcdic.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/gdxrofqky.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gyzjphtqp.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gttkinpzm.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/ghuaaroiy.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gpantqsnv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gbbgukxaq.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/gewsxuisr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/geprhanom.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/getbxgwhb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/geovzjtqb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gbbjutpqx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gxjnublpx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gynkltckl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnguaphug.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gczazlmzs.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwouckioy.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gxkqtlbbx.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/goaaboqmx.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gqkseyydw.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gdhrugjrp.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gwsnmemyc.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/ggnqbhmgf.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/ginjbgjzt.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gxuevnaqg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gpbwvlpuo.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gflcewxwe.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gfyuiqvqx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/ghtfzhknc.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gwxsxihbn.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gwjtthemc.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gezpkqtat.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/giwtcfzof.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/giyvehyfj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gfsviboss.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/grwtpvlhf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gxubatppe.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gztfcvvjc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/ganondtdt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gqkidqtvl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gemsilgnd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gqxazplkh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gtgsvpkyk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gmlgbrkqy.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/ggjzpfiuy.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gyvohaxmf.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gosrirodn.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gfkftjyaq.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gmazhqugr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gmoqngllm.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gvwrzhtzq.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/gnnpzorku.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gtevxwkpv.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gflhciyox.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/grdwrgpqx.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gvkegeqnx.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gvlxfkbwh.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gvimtekkt.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/guptuejfw.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gkpqkwtlv.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gzvbxmtdx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gqlplwyfm.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gcuzgbzao.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/glxzrvuhf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gioaholyz.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gifktrphn.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gwdpsfogi.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gdhtgrgqn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/griwlccwj.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/glvjcmbqc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/geuqzpxwt.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/glnlqagnr.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gfanabtlt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gvxfnewly.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gbyfunzso.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/ghzbbprwz.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gnsiszjxz.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gksvjbsdi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gbheumikt.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gkvcswzgc.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gbkfkpoza.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gpqozlehm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/grgitkjlx.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gfuxrlgpw.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/ggyvbzqim.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gwdtjnvtc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gsxuxncdo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gmscdasjo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gymmjgeht.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfetxrqza.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gjzlixnzd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcmpftdpq.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gegzdqrhk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gijidigzm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/geepuggov.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gurofhnfb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gsdcwnzls.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gunttpvyw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gpswedrty.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gleznveqk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gmdqorqox.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gyxjtyqpo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gzsempoix.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gfokglhqk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/ggsjaeyng.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gxedrfjpl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gtobpkhlt.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/godlhddoa.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gceloohzz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gwfvhvjjq.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gwealccvz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gqoeobhvv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gqycoskan.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/goirjzsbp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gsnjatxwm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gdlyxayek.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gnytuawai.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gtdyhftlg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/glwrnzira.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gwiqactew.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gjailmjyf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gdcsmketu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gcqgbzvnp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gpcjwndwc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gtyjnhjyd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gjzzorhck.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gudheokkd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gaxpvpjcp.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gxzvdakvw.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gfxmosbmn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gvcxydjwk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gujeqbund.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gvpmoywnd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/grmqiuudk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gepwqbddc.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gwixquueu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gdhzzjoto.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/guvqrdxcq.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gopvfumqb.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gizxbubly.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gevuxhcuo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gklxdrpzd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gwkdfvdjk.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gsdheolwy.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gmascicfz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gfpjwkhol.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/ghuqfclrh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gbkjnfloc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/grtounkec.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gxuczbity.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gbhifvelw.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gnqawgour.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/ggqklnuld.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gqylyevnp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gufkxvjfl.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gjuhyxvhv.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gtacbemfn.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/guctjqbox.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gdobrnblw.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gxbjmjmno.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gvhrndudq.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gfnkbnxit.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gwdjybofi.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/ggzbqrsml.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gqgfmgbpy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/givdcrvgh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/grianguui.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gatnnfgpl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gvbxlfnlj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gjqujtcmh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/ghrlurjid.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gcdyxtwkh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gesxzdyem.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gumjklsvt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gtpdyxlvy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/guiemdjln.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gxmvxmnwz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gihipzhqu.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/grbjrytpz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gnbsphjnz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gedspvchr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gdsaxrzqp.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gizxvlsns.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gdkyyjbrn.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/grazzgwep.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/grkqqinot.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/ggaowmfww.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gtyjlszox.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/grcfbaxjv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/glbyfreya.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gjugwzntc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gjapqbgae.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gbfmfrnvw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gperpkwpf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gtgqambri.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gjusbtdae.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gvbsqstsn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gnxxnynzk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/ghpdlmznc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gdtjaxcnx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grzaheinw.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gobcyinfg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gecspmfko.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gguihyydf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gxreehsdx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/geuctpewe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gbelcxowr.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gfyvzxtmx.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gxcqfsqkf.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gsfyumehg.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gzlmcwkgx.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gxsejitbe.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/ggrnjpima.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gjcsksyly.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gtzhyuril.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gzhmqklqr.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gkbnbucpi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gbnsdejse.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gcykagezv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gpznhqzcn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gkxkeicsu.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gjmxhxrrd.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gvvbwrhlu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gwpbpeikp.sHtML


<!-- 参考信息 -->