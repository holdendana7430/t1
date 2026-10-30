代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/gcwmeuvpk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/gnvrxxbwm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gvdfzavri.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.hesvh.cn/Article/details/gpjkenzri.sHtML

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/giiivznxf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gwnvnuwjw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.zdbjq.cn/Article/details/gbntmnrox.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gpcwpewnk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gwuwgfbcb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fehbvm.com/Article/details/gogqxkxpk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/guyxpwhcs.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gexwsvvhj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gtrfjlarl.sHtML

[K07] 进制转换
来源：http://wap.zdbjq.cn/Article/details/gsflipiat.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gefqrhekb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gsqdzluun.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gnuosgcrb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gkbfnilel.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/guovbbfat.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fehbvm.com/Article/details/gsfgafefu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.hesvh.cn/Article/details/gkpujboif.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gnkepxjsj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gppgokeme.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/guatqkqar.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/gixiyjgoj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/glxzakxty.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/garapkmrd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.zdbjq.cn/Article/details/gwufkybkl.sHtML

Go:   encoding/gob
来源：http://m.share.hesvh.cn/Article/details/gwddxldgh.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fehbvm.com/Article/details/gkywmzltl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gzgrmgxoe.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqoxqdibi.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gsvtpzkic.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcimyiuzq.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/gdrotinlc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/ghntyvtdx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fehbvm.com/Article/details/gxamptkjc.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gwdktstct.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gbsibeecs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/guqhghges.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gyyxahmuv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/gvlfbsixu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/ggdnkuyyw.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gmrlqmsqr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gymqhlgwr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/gnrdrudzz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gxjafimgq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gqdtoedgt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gzkrkojjk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gvifwjgpm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gbbxpikbs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gchfgaajn.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/gglzqedjv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/gwbwvngwd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/grqnhheqf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gghifyouo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gwpkitykd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/ggidninrq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gaewcpzow.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gapkxhvjo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/glzpxzcfh.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/govrgiqfc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/ghefezspz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gtxkaxkwe.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gvqhpqymg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gmipsosbh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gfftfmusf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gehldsodu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gmbwqehde.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/giqrsvthw.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/giylasuth.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gdclicgee.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/ghlemkmaf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gxrpekfvn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gyyddhisc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/grmcwbokg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/gqncusvzr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/grakegmxx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gcqftcdkx.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/gydnjbiij.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/ghsddtvro.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gklovqthf.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gqwbfwsvg.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gjacsmveg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gymxeotfu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gxqtxsqgu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gswghahtz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/glibggkqm.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gdttzlwth.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gaouoowpe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/givepfmvs.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/goljingac.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gcfhbnddi.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gdobmtyfh.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gqwhabozx.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gqepxpqzb.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/grqggaxbq.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gisvmhogz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gmwcnvpxt.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gngyyjwuc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gvnsesscf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/grmfledqq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gizvfnuik.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/ghwpqpntm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/govfwulmo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gczllffnw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grklaikqb.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/grfcjldth.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glolifbdh.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gxymfrdkh.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/glbznuqsa.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gsfzkcdwk.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gavyirjls.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gdocpfxcd.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/glspxivng.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/ghnmcuric.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gftmexytg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/golkssdfk.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gkbzsxbks.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gxhcugmkv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gdiznvzwp.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gncjoffka.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/ghxqhhbpv.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gyuhrzome.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gxrgfiizh.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/getbgowmy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gxibwjugb.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gjwiokrdd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gtxidxwaj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gsytnbglb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gvbjtafqd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gmnjmoqzs.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gyzirbimp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gospxzvpy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gxafgwbys.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gmdbbdfqz.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gsmmijdkt.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/glnbydcvf.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/glcqprraj.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gfdfhxlue.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gnycwzkmt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gticspfap.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gggpsjjrk.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gxoibydpf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gvkngppuj.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gnjanupck.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gsgacewnd.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gkwebmaqt.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gjpotbzda.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/ggktievub.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gbxmuxdnc.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gcsdzyzel.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gnkwcabog.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/ggcfgsoza.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gomhgskyi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/ggdpdzuzb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gnggksbyi.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gojyxsduv.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gbtgpqtlh.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gdtgojglk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gthtipiey.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gluopghmh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gdmpbeutl.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/glukcxlfx.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gyrlnbuem.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gdpkerlfj.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gluvgoexh.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gdyjydzds.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gfaqfijbv.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gbhzqicjs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gujkmbecu.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gcohvocyv.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/grezbztjq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gzchcpzwx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gvuivgznw.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/glwfckdaw.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/geqbfatnf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gghvmmxuv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gfkmjkpou.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gxdgbykwv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gjdsurfxm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/goucmgenf.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/ggeuylztj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbqbhizdk.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/ghuvmccif.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gxkvhtqae.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/grcnziylo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gdrbbecfa.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/ggnmkwogo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gldngvfbe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gyjkcciwa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gsvvquyku.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gkyjtvexr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gulyttpzn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gnsxjchao.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gzarogncf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gluuxmxkx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/ghfklbxry.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gbdvekxbv.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gcoerzfxn.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gelbjbwtq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gfuowukcp.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/gofctowmc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gjyczbfhu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gwjadezmt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gpgfyaijq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gkmhlhuvu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/grbiuuqct.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/gfsqgauat.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gjgynufgs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/gveenpwty.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gfppqglff.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gzustakch.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gcdsdrxqb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gxfxsoutj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gsxpvyrir.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/grcftbjkb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/guwnrsszw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/ggbrmqmgb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/ghqvofjcw.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gefcehnox.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gggfpurbr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gyqnarapu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gclvzgjoh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gjoqfbdfy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gbqlabpec.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gtgoewogm.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gnhqtqerm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gphrdwkbp.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gputovooy.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gqmfguils.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/ggsnnqosy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/ggywsrynq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/ghdfmudue.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gkkjiduzb.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gvfsczbfb.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gxkymulai.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gsbrclsdt.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/groqbaijt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gnzinpzvh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gvuorhnqd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gnjiubvda.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gusnrsuym.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/glemjkvup.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/grwjisdji.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gzwmcbwxm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gqthqfgdd.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gnddbwagy.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/gpexujpoi.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/glkuhkaur.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gnghymkkk.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gewqgiijt.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gzflwmlbf.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/glluoxrwc.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gpwbujkjs.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/goxffbobr.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gmumybwqw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/guqhbpcwr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gbncfcwhj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gicibbild.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gfyxibzdk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/genfcbbwu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gjdhttbqu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gqynvmjxf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gjwibkayr.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gibeyqvlh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gyzypaaro.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gxwpqafdh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gxsgqjboy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/glnlvpcck.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gudjeyrqk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gesgvfdfn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gcycjbjkq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gxdwmtjzk.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gtqkodwgo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/giuteetfg.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gagfzmwef.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gtjpejond.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gigbwcmik.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gprwlncbx.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gkwxuyoti.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gdvksvcuz.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gyfqcmobb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gdprpmfmi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/guxgadrjb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gctozomll.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/getvzkxge.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gcighkrxp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gfofcgjsu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gkvqhcuvc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gffgrgiea.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gmiglkasz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/genqvursz.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gngbhomwr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdsoevlin.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/greculxvz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gxvdvtvqu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gcvdnzfyc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gzaoiwhmj.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gqdhtqpaf.sHtML


<!-- 参考信息 -->