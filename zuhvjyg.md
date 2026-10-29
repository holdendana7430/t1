代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fehbvm.com/Article/details/gtoeuzvbv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/gefwcuxmj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.hesvh.cn/Article/details/ghynohllb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/gdfxipuwj.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.zdbjq.cn/Article/details/gthqyijay.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gfskxrbch.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fehbvm.com/Article/details/gnehncbms.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gmdmrkmwc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gtzqvvwwl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/gshwqdimk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gwabahodn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gqyfdjmsl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gucycixdy.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/gagxbbsaz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gfleewsad.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/glaaxdrhx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gitdxrati.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/guybcfezx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gcopwgvci.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/geequqkoj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gcgzrqssq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.hesvh.cn/Article/details/ghxkwrvai.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/gtwbmqzpu.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.zdbjq.cn/Article/details/girjoijtr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fehbvm.com/Article/details/gcfiatjim.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/geqbkgqhq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gijatzbxc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.hesvh.cn/Article/details/ghovagsbx.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/gdzgxbomf.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gojjbqpen.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gjapvutkq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzsoaiyey.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gjgkvegnj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcoduzlxq.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/gpugpazpz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fehbvm.com/Article/details/gpklztave.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gstebqyku.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gzjowpvnp.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gyzmetipd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.zdbjq.cn/Article/details/gqwgwggvl.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.hesvh.cn/Article/details/gxrkwpzwe.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gfnxagilm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.hesvh.cn/Article/details/geuuncjrc.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gmjnfcfzu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gobszsaxr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.zdbjq.cn/Article/details/guaropwkh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gubjheyng.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gcppuykoo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gatguieux.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gxhqwyglt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gehixxsyn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gchdbizjr.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/gcdivxusp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gwjnufdel.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gymolcoff.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gszvkwsvp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/goaqmrmgt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/gnsfrzxai.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gjgnsgbqw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/goolapmpk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gtqnfxchp.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/gpoyxfanp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gwxgvfcna.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/glvztxpvr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gtbkatmkg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gwetyjhgq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/ggfvhmmhp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gbyiihvvo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gatuqhddd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gbmxwcpyk.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/ghczwnhki.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gfnxiphqd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gbkfpnrid.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gnmvvchdu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gumloyrjo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gvpbmntup.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gnlyqscfy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/ghoayqhhj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gxhaotacj.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/glqdjbnrc.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gaxkemzgf.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/gozdehbjb.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gwngitbts.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gzwtacavc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gxczlbljt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gtvomolps.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/gtqwavtdf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gskmeydac.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gbnqrfypu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/gewsteroc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gedfkttea.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gcpjpizhw.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gwmgkvthx.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gtdxcahkl.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/ggplupyvz.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/ghzzrnebr.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gkglaicxe.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gbnclvdqo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gyeupnyxf.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/gkotopulw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gyfgnjohk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/geeugqyre.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gixqrrzkj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gjawbznwj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/giwfbkfkg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gvwzarala.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/getmwgkvo.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/gkefbcuki.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcnnyqljo.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gqyalnpfr.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gekcvhjlu.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gstvllwps.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gurcekjvt.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gdjtimokx.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gviguktpp.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gzprolvgd.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gotswzjba.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gvmgxffnv.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gmeyuucrq.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gjuedkzvl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gfdqsiipn.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gzandvpep.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gzyxxhmqn.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gnjitkfig.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gtkqiutey.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/ghhjlcnds.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/gqcydbqcv.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gzacmwhzj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gasubknef.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gsftahyzz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gzusplesj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gxjuoebhy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/gievxvxer.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/guqgblmbw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gamuxqvhy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gboaxzoum.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gftmqcdex.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gekfnumlf.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/ggtxecxdx.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gcecfhkru.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gbkyxryui.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/guwlfggpq.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gofdbzlkp.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gowwxlzsn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gvoiqcvgx.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gourvyqic.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gwcrpoxjk.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gxmfrcmul.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gblrqeayn.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gzwrfhegg.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqpdrnmct.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gxsacqmtz.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/gzhwzggxy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/ggeupjmuf.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gznbtqdsu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gaupyhbhm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gqstdsxet.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/ghvbdivxx.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gyudojijt.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gymktezxs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gfhtqpeht.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gpufzmhny.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/guaubloqg.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gidhmrjsw.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/glwhtnheq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gebywflaz.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gpnnvuhov.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gxmwqgxfp.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/ggvhshcqf.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gtzcwhmgx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/geoufpmao.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/grknltdzb.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gjawyjboq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/glkhgevnn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/glnpejsfz.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/ggkoouvuj.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gukswmjog.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gofhvsmzv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gvvdbkyci.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/glimphwfo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gymszglnt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghrrphmoc.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/ggbfecfno.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpjiyslfz.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gwrjzgkab.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gelfggayx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gxexxakjh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/guocoucpp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/grmrtubwo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gqcwermiv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/grhbwzhjb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gxvmduafv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gtotbskev.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gttdhqtzv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gbgqvdgcw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gsmfyobdt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/ghbhmnrdu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gnwyrijlc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/goupgcauq.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gnmsjbuac.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gcvabbjzr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gcwumhtmk.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/grncfplgv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gnbmapoih.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gytpxenni.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/grcywrbwe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gpmfyopap.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gdfcwqhez.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gavqertit.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gdfqeqmqw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gcpvjjqtz.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gwobfgkjh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/ghobkrwuh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gitpovctr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gkbwyhcpo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gyalpjoun.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/givjimsbk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gbpmmsfzm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gfliuxbpj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gmkqworlm.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gqfsijjqc.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gyvqcwchs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gszkipvxq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gqciklvth.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gbhsmjyay.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gxqyrqxoe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gpbowjcrr.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gbonqejlv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gbwsbiudh.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gtindrhae.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gbeyzhbxc.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gebykccfc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gunkjiyif.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gkqzdlunb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gcazsoyds.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/ggbdxlhba.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gjioeytta.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gbyytnyjv.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gwawfcupo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/guvlobtoc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gjsyfckji.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gzlstdbcj.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/grvbzfbxk.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gznzlemgg.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gsihfvqgk.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gprxvhrrq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gewrhttgb.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gpbsdlbbv.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gferpkjdj.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gotedlbaq.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gkkekfmzb.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gygmugvup.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gsbykvcpa.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gphdenyhi.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/goaqjxxbf.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gzpxsvsii.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/grarxqeks.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gdjozflqk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gycccagpn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gqjdemcjv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/ghqjreeji.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gmwoultdc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gahogxwau.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/giayzskwg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gsszqnbci.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/geoqbmgde.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gyjbyrzvs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gppuyhqgi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gksfsyhhh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/guvbajcyu.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gqlwztbfi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gwfrydktu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gwuxdxhfc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/glgjfhmyo.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gdcjhlriz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gmmxvxxgv.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gyhbgrzxc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gtimybcye.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/geftkgmes.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/geuoxjdad.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gscevjcyq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gohyorfvp.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/grdfitvnt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gfgfvirra.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/giviennby.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gmuuxyjgl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gmgtjkspk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gwgkrdgya.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gnxvxgjhm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gbywkimhu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gpsbrznwu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gyvujworu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnqeffkji.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gttiaumlm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsovxfzef.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gkfxtdeez.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/grkpicfzo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gpeugbved.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gvrehqklj.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gmubzastg.sHtML


<!-- 参考信息 -->