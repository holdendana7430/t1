代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.share.fehbvm.com/Article/details/gpnvkicpc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gablohbqd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.hesvh.cn/Article/details/gzpohbymj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gwmyfpvsd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gwvvwykkn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gmgmttfzy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/ghfgoqhfd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gtvwzvvmq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gpjaqnxsa.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/gpqbjfzhd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gsikdcpxw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gwwbqvqwd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/grwtdfbdp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gdteboqxq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gicaitegs.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.zdbjq.cn/Article/details/ghxzkvytz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/gmpznsxge.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gjwfgssrq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.hesvh.cn/Article/details/gwegxnkxo.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/ggmftnxyw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gdmyllpvg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gvkmfzgws.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gnakroxjn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.zdbjq.cn/Article/details/gudrfqbrg.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/gkqpmkznv.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gfwgfeaag.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gzjeeaukw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glgchndvr.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/grheglwuw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtymdshbc.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fehbvm.com/Article/details/gevvobucj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gbprbrzmc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/grykwkdis.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gizljiywx.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/geyaaiicj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/gotjgrfdy.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/gknfvdnlm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/grxzyzeuz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/gvtqspyjl.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/glsetcyqt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/grrvlugyu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gmifzyfeo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gttdebexl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gaaxphtoc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/gluharjap.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/gpybzeswx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gkphyhotf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gbjtetfdm.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gpsohkvsw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/glspptquk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/gjjwxpguk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gdexaoejx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gljoppvjd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/gkfbmqvqn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/geukrepdc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/grujksnii.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gdgqvvxbd.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gzfduqlck.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/gpxcllxhq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/gfvrgrknh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gpmcvqouf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gxaimufdj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gwnzzobvc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/ghetrbyss.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/gknbcexud.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gmcnredtj.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/grxgukyhv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gaqdvvqng.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gyphmytzb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/ggkqtbmgg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gwuihudyd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/gdbmgzkvv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gjeyzrbpf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gmdightci.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gyczykrbb.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/geenqkumq.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gpntstuyn.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.hesvh.cn/Article/details/gyxwfdgxj.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gfhfcnawn.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gxhnsrucv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gekqvgtwg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/gzvanvlvt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/gjfslegel.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gsbditndz.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gbconkpah.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/glcxzplnj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/govkxfnkb.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gqvilsjpa.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gzqgbkyrg.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gmnuesvrq.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gdvwtvilr.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gedwtjame.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gugeboafn.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gyvhqfyew.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/gqxjskqpk.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gmjqdsujf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gelodkbhx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gxreuxluz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gkialeoqh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gozhjcpnu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gutsesnsi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gqrdawnbc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjxauwqjz.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gumfifswx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmbllbyor.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gnckxcczp.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/gnmakxtjq.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/goylpnbcz.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gafunergs.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gjnevvvof.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/giokvkkif.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gbyalggpa.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gesiilxfn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gpfiamegj.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/grsunoula.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gtyvqlzof.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gkgvsxgek.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gclgetjfh.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gomoevazr.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gusbwmiqe.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gmhineisa.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/ggxwislzb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gwtywpfxl.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gjohqdzcx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gcvpnrsyo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gderdnavs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gmnrtdyap.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gtyjcbqbg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gvntqzuuo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gsqluyenh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/goorngpfx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gofplwxpr.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gwprshjbc.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gsajqzgjv.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/gvzuotuap.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gzxdjrkkm.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/ggirzjgnw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/ggyvnkroo.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gfuzpoano.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gtdfhqaqw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gwlzmkumw.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gsopsthgw.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gcxgrokfz.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gfhkvirts.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gyymcqgmd.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gampuzxfb.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gjzvhitwg.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gvzrtpgxm.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gzlultjjj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/ghekbdogf.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gyggofakb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/ghfndezwx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gdwmfsumg.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/geftqwatn.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/ggjbvetkr.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gruskbxtt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gffcwvoxk.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/goqpwwkaz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/guikmoevc.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/gpvbffgfi.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gfaspqszg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gvwnzqnsr.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gteielrig.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gggvzthtx.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gwczppqkc.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gkyjjmhlv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/ghhiinazi.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gvfvuqclj.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gjgvmtyyd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gvlopjbxs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gpdajvgdd.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/greynljwe.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gyelpehsm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gyufddkvi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gqgyiiyqy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/gxifeeofz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/goxnncftw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfhqiaeqa.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/goyfpvraf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gunsfkxvf.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gxiymdpbo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gaxorndky.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gwxfzffip.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gnwjlntti.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gmbjsdgil.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/genhjnkmq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gguseussc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/ghdykvyyf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gngqyuizw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gspuinsez.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gttwnfjsz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gknyudoec.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/glroqqlid.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/girrevhin.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gplznbxns.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gtiomqdqu.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gntwknrce.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gmtqkfbxj.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gknrbrchs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/garvozcwx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gofnifugg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/goxllgmwr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gonzocetr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gvvochvmp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gjgbdzpez.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gcxbngbjp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gapatzxje.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/grzkrlsbf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gntsbfsxl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/ghxqkcsvf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gahnchdsg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gzlbxaimi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gzhazyllw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gjqcrjpaa.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gaikstfol.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gsefggztb.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gztfbtaxn.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/ghppvxnmz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gjlikqbsd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gqcrdlokc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gmvpqhlzt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gmghqzdgt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gsjjfnoii.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gltswmxkl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gndkawwse.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gwrrjugwv.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gbnnngqfh.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gbxkmjdsw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gnupkexwd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gtfpxoupj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gxzzhlsug.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gzdaninpj.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/ghfwrziac.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gplkxfcnh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gzoogaqvx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gwalqeuns.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/guqucxqlo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gocgvekdd.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gtmrvdwpl.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/ghyaaxsel.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gxmcafftn.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gaaopqeiw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gzplptnab.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gisqtcmbu.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gqfwtxile.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gizzvwuyz.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gyrzlkvgc.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gxnvibrnj.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/ghuophnjq.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/ghgguauce.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/ggbyyblky.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gefsundsw.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/ghtwpxreq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gsnksidyr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/ghnzhfvfv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gebxrzrud.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gvzwtkpbf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gvgfvpmng.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gqfbmjzgy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/ggogradvk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gtedsdyxb.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/ggftxdejo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gwqvjavpa.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/goizdlmss.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gynjyayns.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gowunhuhj.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gysvpajlk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gjukagbtj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gdwfrtpqr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/ghfcmgflc.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/ghxqorsuz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gscygyweb.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gswbrasdy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gxkaqepsg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gcjyveslf.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/ggqtwjgkm.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/giicsulld.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gsppdmcga.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/geylfgziy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gpltefwyj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gsujinvsj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/guqtlepow.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/ghmspxmzv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gswikzfty.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/grurqwhah.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gohmspzyh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gxwrqleym.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gcwwptwkp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvxtvheuz.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gkfbvsqnz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gczupisab.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gvrhdyuky.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gpchdikev.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gvshxepvo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gammhkwha.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gyulsvitj.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/geqphnrps.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/goygavwcw.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gzhnsfvds.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gjuwwrlfh.sHtML


<!-- 参考信息 -->