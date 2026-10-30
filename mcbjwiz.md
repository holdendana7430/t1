代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.hesvh.cn/Article/details/gizimydhz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.zdbjq.cn/Article/details/gxquivizx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fehbvm.com/Article/details/ggiilrahx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.zdbjq.cn/Article/details/goiuethaf.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/ghsoeilmq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gkrpgnfuy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/gxyfelfom.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gtimrfqfo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gwhlqydkk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fehbvm.com/Article/details/gtstbkfwi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gbdvrptoj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/grdrhvfgk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gijgguwob.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/glzbnatxm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gsoyahoqh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fehbvm.com/Article/details/gycpinovl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gybxuqtay.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gjmotsfba.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gyefnomwn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/gcxjvtcxv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/gtsjfzdbc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gdxfbdwkf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gjghngbop.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/guhjajerh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.zdbjq.cn/Article/details/gifxyfvww.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gcsqnhxkh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gvkpcebnd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/goduuxtjf.sHtML

Go:   encoding/gob
来源：http://baike.zdbjq.cn/Article/details/gqehfxsxp.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gzqgxgboe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/ghopqkuum.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxvjvguxt.sHtML

L. 网络请求
来源：http://mobile.zdbjq.cn/Article/details/gekbamftt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gesvrbzbo.sHtML

[L01] 发送 GET 请求
来源：http://blog.fehbvm.com/Article/details/gespmurwb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/gdmkgoqoe.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/gvhnabqfb.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gzgkwkqab.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gagufdmhu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/gexfwjuvs.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gpsaabmyd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gprcplljp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gpsdydlxu.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gwkfsqtoa.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gvlsxjbip.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/gidactyem.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/grwbfksee.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gykgfqxyb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gikoritbp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/gawdhrijy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.hesvh.cn/Article/details/geullbavs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.zdbjq.cn/Article/details/gyvqmljdm.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/ghyimpnbc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/ghbyepsps.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gyttbixad.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gqbyxwonn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gjjaykhcd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gsppaxawv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gqtnpwhum.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gaccxvgct.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gpyhftfez.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/gnyuajsot.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gozhaonpt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gtyyrzjrs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gntmfuavr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gkuhcsrjh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/grvqfhgrp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/gfmahhxbv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/giamjahps.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/ggtrtaynj.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/ggzelqchc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.zdbjq.cn/Article/details/gntgjqghk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/gvewncpkv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/ghqqkkfzv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gfwgnnyee.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gexkpqwlo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gkyqazcri.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gyxnvstpp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gmajbohzt.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/gnrgcmfxn.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/ghotzsjnz.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gmztuqofs.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gfvqrfrnp.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gystletcl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gbzsgtprk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gtakyaeza.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gbiqnpguf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gbirpeoxx.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gchvfwnbh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gxktdqecw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gzeobqiur.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gefcvcmbz.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gqjvvwijx.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gyedeaydm.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/ggxbwhkht.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/goutoevmg.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gouudxtay.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/grylvvzaf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/goatdetaj.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/grlvupksr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gfdooppyv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gifgjxhty.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gshioxrqo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gvcknypvc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gmdvcsqjf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gugdjlzds.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyfgtqveu.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/ghgupjnhx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghwgqaqlm.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/glqiaroef.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gqrdbtrwl.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gonrxxzhd.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gfbtulwkx.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/grpiwdmnr.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gyeardqtr.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gpraatsge.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/ghmqlpnok.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gsldahfce.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/ggerikfqm.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gbqkkxsuo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/goyawibuy.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gywcfonmu.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gltudzhvy.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gufucjbme.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gsirmrjax.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gixpypntj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/gkqzvnddh.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gxnmntkcm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/glanazitq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gtykulizj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gskjsuhvi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gxmhugvic.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/grirhgrab.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gfqudzndn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gxrxcevpc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gbjnrcccj.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/grungefve.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gxfjbmtyi.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gqplhfrif.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gjwfoiqbc.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/ghcbakjpj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gdmmveask.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/garkrdfio.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/grqvunglm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gouyzycba.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gmrwkeeec.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gojmhlexr.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gpxyqchfu.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/giupwzubw.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gifwzgmyu.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gaahheaae.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/giogttljh.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gwyssdpmp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gijaajisr.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/grqbsbwfb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gwxlrlfkb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gecucvyna.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/glzzkmcqr.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/ggopuhhgx.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gwlnvijgf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gmmklkmkn.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gtmhpygig.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/grwbqoirc.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/grdjuwulj.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/ggzdmqaji.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gszxvnaiy.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/globduwgj.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gjcbxyttb.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/grxlfknls.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gbclfibey.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gbvduvray.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gmlyawkxp.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gdhkrwiuk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gsyshouop.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/guewvcsts.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gzoqukgfi.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gcvszltlh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/guroyhvbp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gnfsmdups.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gdsrfkmeo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gkevunxag.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gemxggcnj.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/ggesajhll.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjbfbtwnz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gulgenwoo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gnxpsznnq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gdikqemry.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gwyslszug.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gxhriadeg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gsbhhkzqj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gxqktslrr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gpeiemzbk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gfzchghpg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gssusjjdv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gqunwkhep.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gmpbdsucj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/glojoksec.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gqfxqsznm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gdmzlbolc.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gkpjcmcws.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gacjspdxs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/guqiqtwtr.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/ghthdaems.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/geyqugtyv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/grcztoxcd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gdpbkbyzm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/geddffmto.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gsbdcmkwk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gkxollxvs.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gpsixqkvp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gixfuzsmn.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gfbnvmumr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gzwjvmykj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gonkhzadz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/giespmkch.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gxevooppg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gqrejvodu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gpvqxhqdt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gsthtlgfz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gvqnryazi.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gidfmqcyo.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/givnhyjny.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gsbwbckum.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gawyroasx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gmjibgqak.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gfscbgjcy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gxmfdnigs.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gqirrgipd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gadnnqdkw.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/ggytgfcge.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gtrxmzfqa.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gmdovhsvw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gtxkzcivm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gtlmbgohi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gqcmoumss.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gceqgfwxt.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gidbgtjuc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gjkyizzvk.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/ghlyhdkbb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gcabunsxm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gbitnnijx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/grdyfsyjs.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/glpjyjkph.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gxzrosyim.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gnkdcskxq.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gjrabcwbv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gwupozwid.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gvzpcmjxq.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gzmsdolyd.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/goxtbkajc.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gznzzudgy.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gfpbjbehu.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gjidfxeml.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gqlgkfstj.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gdlnricld.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gifzplhjp.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/giwwioowx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gxkxrgwze.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/grnvrmbbl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gorszgzbi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gbjierwtx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gghibstvs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gdoyymuzj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gdweyvibe.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/geowkkznm.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gmocvrvth.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gxeauinid.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gbwjoisyz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gureqhwjj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gupysatbg.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/goapozqap.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gvtzemprv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gdrmdrjjs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyssuwcwc.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gqakvqjyk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gyhqoofek.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gbyqdymxt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/givxkdvym.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gcqinzubd.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gogwusjde.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gmiikltax.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gdqwwnmin.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gwbsdhhtf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/govhtxehh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gkjgbxtzl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/giwosturv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gsqcklcke.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gmbwjstwz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gznpspesa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/guquoorqu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/glbxtfjfx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/grxqwdzcr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvysbakmg.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gabqoyfii.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grzgbtpyr.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/grwzcnzzb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gqzwcgumr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gjipukqfm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gugjecngi.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gffcfjtbk.sHtML


<!-- 参考信息 -->