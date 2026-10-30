代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/gswoqxmca.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fehbvm.com/Article/details/gyowfhwxn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.zdbjq.cn/Article/details/gptvfstuz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.hesvh.cn/Article/details/gtycgsdob.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/gtmgwdsjo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gvxwevyhw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/gmszmdzrz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gadjoolgw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gvindvuft.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.zdbjq.cn/Article/details/gaiijuwxk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gffkgvgcc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gwnzenynq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gcehcwjpe.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/gwmcizdei.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gvcxdjcex.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fehbvm.com/Article/details/gbgycdgnm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gofsswnbh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gzvoeykrn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gigoccqrn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/gscpnlsth.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/gmwchjvfu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gcdfntdgo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gegfekmck.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/gasfxyazi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fehbvm.com/Article/details/gvqgiqgbi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gdsiuytyg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/ggeptzvqu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gvuzytxfz.sHtML

Go:   encoding/gob
来源：http://wap.zdbjq.cn/Article/details/gezxmukal.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gmqhfuctg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/ggdhgvnvk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyxcxxjjt.sHtML

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/gevcekufi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guagnlyjz.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/gtsynxaii.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/ggcsqtmic.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gjflwsqhz.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gfhhiwdgw.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gzyuwwtch.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.hesvh.cn/Article/details/gsidsntkv.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gylepeppb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/gayocciha.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.hesvh.cn/Article/details/grizjpynj.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/gjlmaopje.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gpcqceokz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/gcbiujmww.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/garlojavy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gfadfdjul.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gnfiohilj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/grrcxcpvz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gpdpwcekf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/gncntrjrh.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gyqxcsyrd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/gwphrzcht.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gydhgisnz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gbfkgoozx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/ghlfyxllm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gsevthgzf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gupvqhneo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/gbjcmrjni.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gnkmtfsap.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gtbtyulgq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gatwucjlc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gcflkboho.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gdgagpytx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gygyixdiv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gemieccxx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fehbvm.com/Article/details/gouubbvkd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/grpvjekii.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/ghturbsxp.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/gdqanogyh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/gwvxfsahi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/grzhaebbh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gfqzgohru.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gfujreezx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/guixxekhe.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gzyfwfykp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gfrzlblnu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gqbnzdlas.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gxrvyjcds.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gideuknrl.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/ghmdfxfhj.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gerrnxlay.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gswhzylbv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gqkpjlcer.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/gtpqnzucb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gcrqblbbe.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/glhrprjap.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gzbxforub.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gokxgtelj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/gqmywrwsz.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gckqzztwj.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gseceqvjt.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gjocokdkx.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gptrmtgky.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/glkxtibiv.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gbytxgxni.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gvxpygnbr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gvsfggvuh.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gpufpohvx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/ganmwrdpt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/goonodsrt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gdpeybhrr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gaaxocact.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gixkstrla.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/grhqtctgp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnldettxy.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gaeiupjqs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glzcewnie.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gtxwvvcki.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gxnvqsddw.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gbypmjbbm.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gqfqlihey.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gjajiijnz.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gfskldgmd.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gxzxwiibx.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gkppeshhp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/guykqacwb.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gcioufhbo.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gzjstpoup.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/giywhwomi.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gtxnjucdr.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/grfuvvnmx.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/giqtdiaxc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gpbgherta.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gczbnzfdo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gsqzapaxl.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gisxasbvb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gplhxdsqf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/glhcasnii.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gnjgryiim.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gxlbcvkux.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gkzpivpkr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/golpqvexj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gwtrdikxo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/glagxxxwr.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gbfsxicuf.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gsgngzorw.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gykvouplh.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gsovrzpyz.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gnrbirdpu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gunqxpzpi.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gcquyxhrs.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/ghfjxhgpx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gzowogtin.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gtqnouhvx.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gwacaiqyg.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/gglrtkbon.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gxtoljkvk.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gbmrrlhxu.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gqhughykr.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gkyzusczr.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gxhhicncy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gptevsrpz.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gzyrwmmki.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gbamwxjwl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gkmlihdhk.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gllodklfa.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gqgdvjkyt.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/glrkjughm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gtclmmzol.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gciunuvlf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/guvissfzb.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gkvvtrexl.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gxgaszloe.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gpedffucf.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gysimdfim.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gtmakxylg.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gmszfjuyr.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gjllqrbcu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gttzsgdtu.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gvelhzksn.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/glvezqvjm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gbellkokl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gdohoknfe.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gccshnkpe.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gnjntmygx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gpjutpovx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gpzanrtnx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gvczwxkhl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gclucalce.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcpdlkljx.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gjiiclnki.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gaicnckmr.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gigmrpyez.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gvplgptrl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gujlauypy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gqtvgampa.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gzsybkqfu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gdygbdvhv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gzhyhknls.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/grlsnnxyk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/girfhqfnc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gxqbjxsti.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gecodhhzm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gzawezcep.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gcczcvafg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/graltufdm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/grefydfjx.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gwcpustia.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/ggkelrwhz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gvppcfepx.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/gsjbetozv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/glprvfaaz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gwxvvnqbu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/grvzbaujc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gvrznlcfy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gudorgcoc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gwhdjrrng.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gcgrunuyb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gfgeqvozi.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gsqpvtelu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/grzjjlmqg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/ghqipndzi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gmffmkoqg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/giogxlbcf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gcjcaalok.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gcwixmcte.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gmxiemknf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gftppqxbn.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gochdbxfi.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gyhaaxaxf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/govynjpyj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gwfonnnfg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/geebnymmx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gfakhxqiv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gmyjcftuz.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gbjmpwgtp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gcivzxlqs.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/goethbbqm.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gbhslgpfj.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gstwgbcdp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gbaggcddm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/guvfoutky.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/glrxllxon.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gjgwhbbms.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/ggqqxazol.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gxawrmhkq.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gcljnleqq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gydjqvetd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gekiqfqun.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gcedoyzmh.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/ganuttkzt.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gldqbdafs.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gylebdhsx.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gqdwlzdbv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gftqzockz.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gntjvnony.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gscwfudfy.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/ghvarmggo.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gytfkarwz.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gnfweidab.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gwfsqbbgn.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gfccgudyq.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/ghsfuqwka.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gbwpflvxt.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gvijxmskk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/grzobxskl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/grsdqlokj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gjfzpuexj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gkbnerfpm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/guevwsoeb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gcnugcdrx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gyvnucbkv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gxfztspmr.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gryyquciv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gekikmzcu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gqztgpnpk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gecoynzel.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gbybvqcsi.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gzlzsjvtb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/guqadatdb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gwmipoola.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/ggbyjicbf.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gsufmaqdr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gmxdvsnai.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/guyjtixib.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gfdjifnoe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gbllczcct.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/glowhwmtp.sHtML

Go:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gwbuxvdwq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gstgikxsi.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gnhiitxuy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gtbdqaytp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gqpjjegnz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gvndwfuzm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/geymlymhw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/ganquwfvb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gqvzizzlg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gziyknxzd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gvfecxcpr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gkedfrmig.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtrymvvqe.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gnanuzmby.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvitwdsao.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gpfwwwmky.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gdvmhjvry.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gkjbulytv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gxnlkllgv.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gnactcyrm.sHtML


<!-- 参考信息 -->