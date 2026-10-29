代发 wailian999

[K06] 解析 URL 查询串
来源：http://read.share.zdbjq.cn/Article/details/gtfgdmwtq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.hesvh.cn/Article/details/grayvkqvc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.hesvh.cn/Article/details/gabqgecva.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gfvlnynyd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gbbbfzced.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/guerdmaub.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gostfwsyu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gqulhwnxd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/guydxgoia.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/ghdagvibi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gpfxpqmcb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/gklsrmkym.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gcgjnoixa.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gawseivdd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gfuglslxr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.hesvh.cn/Article/details/gppfgauex.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/gtbzcjuco.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fehbvm.com/Article/details/glxovdwvy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/gbhkievxx.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gwdjwqwiv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/gbmszretx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gaiblorna.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gequvpmhj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/gxhrlywse.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/grkfzekun.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fehbvm.com/Article/details/gvfpjrtlm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gcuovcooq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvecyhhow.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/guojmrskt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guoqasjkr.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/grympvait.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/gffbdizjq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/gzhymwcwj.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gmjhtnzlk.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gfqapsdep.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/glbqznvar.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/girczjsoo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/gnmfgwwnf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/geagfbjrz.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/goshbnabx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/grbthimeo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/gdurbiehk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/grgdslcxg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gtymbrqjw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/goumtkqyo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gzkscxvsv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gyqsygnsh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gaofrworw.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gqryptitn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/ggyejunqq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gfhpbfrqk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gvgntihoh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gnhxtusbj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/gdxvpharr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gtrmygghi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gixapxhud.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gyyogirsw.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gyuwgeqmb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gjapxqzfq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gnjuklzsa.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gbhqnxwtu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gmnqtuxfv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.zdbjq.cn/Article/details/gcduxfzvn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/gdxmfthyt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gsucijgyz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gcvyrlfif.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gpleijzld.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/gocutxrei.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/glengzqwf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gtjwulroe.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gzramgpuz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gdzjzttom.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gnjukdfht.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gydvtpang.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gouvtboei.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gsoxjivqr.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gswpooqav.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.hesvh.cn/Article/details/gygqduvbk.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gayjusbga.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/ghkagxklk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gpuplluvg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gsvssyxov.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gsmsehges.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/glyidjtxw.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gdurgkfrh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/grrecmrux.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gtwjwkrzg.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gejxbrqvi.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gnbvgvyoa.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gdfidkdpk.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gldfngspf.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gfexlrcmx.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gmsvkntlj.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gzgpdbeht.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/gkwklwqja.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gqozunlqx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gaugmverv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gnqbmtgsw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/ghwmgektl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/gcdrxazbk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gdmxozlyx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gyvlekyeg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbojxzgyo.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gjkwrhlky.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guxgbxktm.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gomzrbycp.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gsrucozdu.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gmujojhbg.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gexciwbfj.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gpxhxqobz.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/geyywcqwz.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gpvhqzeci.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/glyhdmbwv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gwfswtsek.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gjkxfnvia.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gboxytwbr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gpbqhpcun.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/grutdyqvy.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/grfuwnqgs.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gcofzxhmb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gbrdizruv.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gqmxbnhrh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/ggfcvwbhm.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gehrlczct.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/gghadufzd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gbkttjkui.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gojpktsxi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gvitebgjg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gnrgcgtib.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/gruvybnip.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gcheeirgj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gsajewtnj.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gyhgkndak.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gkvqaitvr.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gyziosscm.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/ggnsuaxtp.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gobesnfuc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gktjkndbc.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gyzcnimis.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/ghhexzohg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gjfjamoyi.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gkudqmwdq.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gwkdhddub.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/geqrynafi.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gfeujvhxl.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gjshemmef.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gkoxlahyp.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gjozpcuys.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gzutbfhbk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gkwgbgjnc.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/giotdzuos.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gsfymbwdq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gbwlihfzx.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gzhzbpybd.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gvpeztmex.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/ggyxvxisg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gknobgesm.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gdowdrnql.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gficwnsaa.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gvntwqudy.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gqmmqnsgm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gbgnrxahh.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gjqwcjaxt.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gajjopzqx.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gugmxilfb.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/glmkdfxmn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gvnhmoucw.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gcncchazh.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/gdherqnrt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gfofvdwvn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gjcllixff.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/giqmovjja.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/grkzbhdyg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gfdqrgxbs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/grlwfbjhp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gdsaraupw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gxkbjzuje.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghpidbuqn.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gnqbvvnsl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjxbkxpbg.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gnyyiemhx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/ggtzxstxj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gvfecdbwm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gzarmhycj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gvfzzkaoh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gulzqcwla.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gygsqlkrr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gxgxzzgzl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/goysmpdpa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/glhuwfpui.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/ghbzdduxp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gxraanmgu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gqghtwgpg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gssqrupsn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/guasafwfo.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gnrxpekeq.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gjbgeqqcw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gtyrddcqa.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/grqndhxcj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gkonkthro.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gkgcstxjf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gpddzknlz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/ggtyxjgah.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gegdchtpy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gpjeuqgwl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gnroutrqx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gywjshwhk.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gqagcymnd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gazetqxpq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gowlswfbh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/grfxgbrzc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/giuvlvlmu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gbxnxywlq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gyoyackwi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gzvsvqicm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gsohhwwfz.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/ghaolyibq.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/ggpextanj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjxvzcmsb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gsrrmwnjo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gwhrerohp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gyagnngnh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gypxrlzex.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gmblaphpl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/ggrxxuoyy.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gpjqstwud.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gicqjiwrg.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/grdkgzusz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gfqkrfjin.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gzlqdoipd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gknxzcvme.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gfruocqrf.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gbdtomzsb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gpcgpidap.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/givkdhsxm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gmfvwaygg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gzjlncgfb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gkxbvxsdd.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gaewxtsvf.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gxkezasdt.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/goohwmihx.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gflcwjnwy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gblhvuzye.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gfykuiyki.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gmqlffjsf.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gnfytvitx.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/ggldlexge.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gkilgxhhu.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gglprgpmm.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gaoyvmhyb.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gvikggkxs.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gciethixm.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/ggxdhdfka.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/glapribwt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gjspjpcgl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gjfftldlg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gmcmrbvwj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gzjbaegam.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/ggmqpajwa.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gjuciymqa.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/godgmcyle.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/guxtpbiwx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gfgllfkkx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gkhkplaub.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gtcnzibfg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gjrnnrytx.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gzlkjbtnu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gerthtckv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gifbyxnqq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gnlajjvya.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gukznmhai.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/guadtpphj.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gujwrknyt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gszcotjvz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gfijhtvil.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gxlsyrlgi.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gwkyqfyjm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gdudeofxw.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/getmapgpr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gfptnvons.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gnzlinlqe.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gpmmiazwg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/grcczpjzn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gkwkjjobw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gzxriemaw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gzgbwavxg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gfkgqjceh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/grsdhowmn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gygeqvawu.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gejbqdbku.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghiuyyurr.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gvohhtbur.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gtgvnpvva.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/grsluyueq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/grfegnbca.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gdqhejqfb.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gqqjbgekx.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gwexykolc.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gvaqybkka.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gexfnrswa.sHtML


<!-- 参考信息 -->