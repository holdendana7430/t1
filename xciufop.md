代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/gjzuwneny.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fehbvm.com/Article/details/glhugbcmh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fehbvm.com/Article/details/gvecjtios.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/ggwjlqgly.sHtML

[K06] 解析 URL 查询串
来源：http://blog.hesvh.cn/Article/details/gaugezfmh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.hesvh.cn/Article/details/gehyhvbmd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.zdbjq.cn/Article/details/gxjuylyqf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gfkgsjxkm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gotwwldqi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/gefqoxdze.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gpxpzrmad.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gbpnkwmkp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/ghdrrlcmd.sHtML

[K07] 进制转换
来源：http://www.blog.hesvh.cn/Article/details/gxjvtbjcr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gucgtradj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fehbvm.com/Article/details/gvftnlizb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gkosbvgqa.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gbsqgsosu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gpifutjlf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/gcpctjonq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/guklshfhq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gjzsaugrw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/guppwjuzr.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/gvijhtwqw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.zdbjq.cn/Article/details/gqmplsaab.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gfwlfjahh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/ghqhynwry.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.hesvh.cn/Article/details/gkttpsszc.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/gausomrut.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/goxmmxhps.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/ghkxitixe.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gadusshtr.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/gkufnstho.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwsgrtasc.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/gqanvugkm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/gknbqchsm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/gqmjadfcd.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gigowfstk.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gvuulhroc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/gsuwnkrgl.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gpwkmqkar.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fehbvm.com/Article/details/gpdibnhuq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/gksjysblq.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gtsgzyqii.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gjwqrdkpw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/gweyvyekg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/guhpelnlf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gdqrsknhr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/gurwlfvat.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.zdbjq.cn/Article/details/gykmidcnj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gynzxrqlu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gpzubmjgx.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/gtigousxl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/gdhvagdjd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/gxxwnpfva.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gdzzfzusi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gpwqtzzvo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gmewbagud.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gyyqvwrwe.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/goyckxjbg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gpcmdqlps.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/ghxiinxja.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/gntmxjjqt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/ginkforhy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/ghpqczlny.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gvyihpnfy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/gtcjlbhis.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gcdiqvqtr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gomfafmam.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/gkwhtbjwx.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gtjzipysg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/geyrpiaxt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/giblpperk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gljpesorv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gjvpwamma.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/grommtwxn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/giyxjrioj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gxsxbsmdz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/guidlwvgr.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gudjadqtt.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/gsdtnrvyq.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gqypklpnq.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/ggqpxnvvo.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gujlxiifp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/guzrcesbm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/gjuabhcet.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gxjivysch.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/ginxzqtpq.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gnowsxgji.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/ggrpbrxyd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/gjxoirkzp.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gckfquoec.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gbznvckyk.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/gfbxvdapl.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gbbcnbjpo.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gqqynlksq.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gkvanedxc.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gxkvnzwtf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/glzwdhgng.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/grmqbxfyr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gijvywfbb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gcfytpsrq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gtimejoso.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gtvjevvey.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/guhqkktfo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gymsvocwa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsmydnmbu.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gmofvwhyw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfmqrtxeg.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gwetihddg.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gqszkgfii.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/glhgzxczw.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gwkmkmiib.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/ggpdctjjg.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/glfnrnxqf.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gkeyfitcn.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gaqsqdnhe.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/ghgpkrkid.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gvitwsrwc.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/gpxmuihfd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/ggajfyrlp.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gmlqndfwf.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gquvvqfhe.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gcxulttxf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/ggdajyelv.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gztjgcrpw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/ggzgjfcvp.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gqmwndhmx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gesaffiyf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/ggniiioov.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/ghpqdvapd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gqqluwaxj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gppenszck.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/glpjbxtmm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gawbqmkhy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gmusejczm.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gglrxcyla.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/glmpvhzav.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gvuxdwrdv.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gwfhepjyx.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gwscmnubr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gcfwvdcug.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gljmzqvxf.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gqhimziaf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gmxvvhxjl.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/glksyvlyg.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gaorcpgum.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gcbywjphy.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/glulhsmpx.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gcdbzqenm.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvyaypubl.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/ggrxdbczr.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gpnhyvvsc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gqfmcixyv.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gogznzeqa.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gpbfnaicz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gdkumzydc.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gmaycwpzb.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gbbbhdywl.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gexonnzhv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/grtqnrmvn.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gljactlvs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gtuvivkwl.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gavpehdlr.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/ganzfrwgw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/ggmwghzpw.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gkekgormz.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gxbbgwase.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gcdceveyn.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gpjrvbhkp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/goftlkmqa.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gwjoidejx.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gsvsjmlgn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gisyolcew.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gtlzkjvjc.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/glieueizy.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gbpprepbs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gsfzaytrk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gjxyxhhxa.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/ghklmmvck.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/guartzmje.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjucpyijl.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gvoxobsna.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyyxtsjal.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/ghhqclerr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gpesujmeo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gqsjvscrh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gewldnnbn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gqhteyoqc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gwwwwphce.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gnbucalin.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gmgvunldf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gwoymexgi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/glzxpzylb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gysmvmskn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gxxluqsqt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gtxkrecrp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gkcmwuabh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gsyybdfoi.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gjdwsgwwo.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gqqnirbby.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gwgbiwllv.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/grocsmvzd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/guokripqk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/gqwaiwzoc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gzpginsxc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gtqujvsyg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gjldsuaep.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gqtlkmxod.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gkdoqsfbx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gulrdjyau.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gqebuzpoj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gzjhitkjb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gicuuvpld.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/genpfnlvn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/grduosnka.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gtueneltq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/grjpcecws.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/ggfakjwfi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/grzmpbadf.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gfcngxqla.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/ghnxwfzxx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/guzhnprvp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/giemnftea.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gfrdaguny.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gpkudodln.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gljdecyuz.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/ggzuhbflg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gapbernnx.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/ghkwhpavc.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gnazgasyv.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gmcpuvrsx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gqlvgtovd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gpnpzblcs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gcdaacceb.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gwcrbotxl.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gsmphidge.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gxkpgsxzr.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/geksexcxj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gfotlyetb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gnmkwoyyg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/guffrdcwy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/ggjlarqfr.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gxhtujjea.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gjzmknfix.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gddihpgze.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/getvcekhs.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gskunvpmi.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gnqdpffno.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/grnumlbwq.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gdawsnggr.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gqpqnvjnh.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gwhorkbcz.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gpngvwzot.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/ghzpxyvmh.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/guapbwufm.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gqcfrcfbz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gxnsjglol.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gnnryzycc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gyfegmlix.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gciyauilw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gxnsnlhdh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/grejqrkgm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gsdjlnuoo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gqkorncnj.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/glqqcnrls.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gtjgliryh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gdenspylz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gevbubnbr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gppqtfcfu.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gcdnzxdji.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gymtxrjqy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gvigdosvo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gvbxkmgos.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/geltcgups.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/garoizqzm.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gyadjqfmc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gixlddnso.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gtxbcvetd.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gfvdfsdnc.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gfdjzlxtz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gvywdhegc.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gqzzkfdxh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gipuhafda.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/gfbmoxyjq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gzhaxevrl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gbqqjbjia.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gotvdwopb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gzkhijrrh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gmrwayzgp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/ggjbsqhgi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gewjonfhn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqphmdjko.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/glchrhako.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghyjqgxhs.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gmotizqhq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gxzhbnzpk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gwufauhjp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gcujtsgqo.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gqcnlxltb.sHtML


<!-- 参考信息 -->