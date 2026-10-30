代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gjqwdxulr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gxzqivtkq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gzaiewkxv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/gzmhilxwb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fehbvm.com/Article/details/gmqarbsze.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gcvqnubef.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/gmpthmfme.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fehbvm.com/Article/details/gdbzubzbw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/gwnvosqoh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gmvfjamfl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gloocplgf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.hesvh.cn/Article/details/gxovpwzpq.sHtML

Go:   encoding/gob
来源：http://baike.zdbjq.cn/Article/details/geiuirhcx.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gekcmujfh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/grnlrfiot.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqvcvfhvv.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/gpudzdyio.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guqrulbmn.sHtML

[L01] 发送 GET 请求
来源：http://read.share.hesvh.cn/Article/details/gwchjndms.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/glgruodvs.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/grhpgzgqu.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gkgkwscfc.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gczxvattc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/gwavgwzkj.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gdfutaget.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fehbvm.com/Article/details/gmgbidwlb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/gfesyawhm.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gojldtcsr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gxsuqdbxp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/gkvylgpwo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gtczludsg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gjqsjilup.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/grludvxub.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/ghdslhaxb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gwbasiviq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.zdbjq.cn/Article/details/gtiedjvkd.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/gkssgncab.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/gldncxvkv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fehbvm.com/Article/details/gkoylnjxt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gyzjuimyr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gvzctkqsl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gryrxnbgz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gizsgslqf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gowmrvfzj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gsiedcbhy.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/gzlsynxhm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gtfaoeyph.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/grjnpgrud.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gosyevrey.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gkunaivet.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/grrwvudkm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/gzshbqypp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/guhvfjqgm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/gfybgyhvj.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/gadepfvyt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gqowcfncm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gzczqdynn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gcobiypdj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gomtqbkni.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/grylqpmqk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gwjeumqsg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gbudcpguz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/gpwiiazer.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/ghdpmthft.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gjoeuqxll.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.hesvh.cn/Article/details/gekecdtyq.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gsvsyqzww.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gnzztabij.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gbwvdxfva.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gtfuvvrnn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gbttbxzpr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gdbhiyqyg.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gxrjqjdic.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gmjgyodbp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.hesvh.cn/Article/details/gmauqktpl.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/girfrghgi.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gjiwxgsjy.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/gdgrpdada.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gbbfxherx.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gdpjenkvo.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gshhossjb.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gilldlnzw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gpfpiihec.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gmwgedjjb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/ghrvmpzgv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gkwqepnyt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gutivmrap.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/guzubhbfv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/grjshmhms.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/ghdmdjkvg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gicorlmqa.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gilzdloow.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gayjjbaai.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/giisdfstg.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gcynegqxr.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/ghkkqodro.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gxqcyycfr.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gdojuermo.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/guxuavrwn.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gsycdwgjw.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/grudlulmj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gpobcsvuq.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gfacdolic.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gilkwtofb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gawrvntrq.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gmlwktfiz.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gizgqqfxm.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/glnvqjwnc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gksgowmhc.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gkjfqjlwc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gcgyhtaxn.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/gyubqzfjg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/ggdfqraqf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gikbydzgk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gtznenjwt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gnzhcqbkz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gvzodenlt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gywridgci.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gihwffcbw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gkgzgknsy.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gbxxtouyy.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gsdwzuinv.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gpbglrnju.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/glcsaxand.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gklcqxghn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gxlwcttyq.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gwzwbttot.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gqhsxenxn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/ggtsjklla.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gpvvqgbvu.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gumcvyxaz.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gervyoopw.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gtzbbyvms.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gggrlxnim.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gbhfmxytp.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gtggoissx.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gfosiwiuk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gqisvfsxj.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gyvzjllzm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gsngxiyfg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gcqsbksff.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gmhvlnvqr.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gbuazamjx.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/geocstwsc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gcisnsvao.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gwcqxmdlz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gyilqkbvc.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/ggcqkpnfl.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gfrpndtxp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gvpgqgozb.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gskukbpqa.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gwkklzfnp.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gemqdbhqv.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gntlwpphs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gkfiewpzr.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/goioeuodw.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gmvboxabr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gtmdjdmjq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gtwzvsdjd.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gyizobmud.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gxcomxgau.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gkdhahgcp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gfwbclzqr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gdquvnbgv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/geotnkvwi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcatetyia.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gywkaqudq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gopcooyjd.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/grmltgbao.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gcxznjmrg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gzkyqfoak.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gwwosqulm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/ggtenjurm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gwjxhjnll.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gamviavte.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gmybuqbgj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gxsgctibg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gopbqiwep.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gppwddena.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gfwijocmx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gmkdnslrq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gyocjmeoe.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gtfzutpoe.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gmgqipqup.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gbejytjyz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/givpacrei.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gwifimeug.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gjtjgnjyq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/grsbilrmp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gdaocnmzc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gbwbfdsnz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gngewboue.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gkdkjvrnr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gaczwzwfp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/guzhuayxq.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gwrkfzggb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gjsxfpnns.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gvrhvegse.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gymffphfy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gbjklxdsq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/glztlwjci.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gkudszfqw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gvliqjeae.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gbjlpqiqv.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gsytnkrng.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/grxezwcth.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/grmujljmb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gnaqjzieh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/glyiqrwyg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gdsusclrh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/ghgylyuyu.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gipdqwbpd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gvhxpxfnm.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gcbtokgov.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/goiqfjtya.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/goucyavgt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/geeskyvtj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gkqmmajcy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/guwrmqiar.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gtrjtnlhc.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/goemultgx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gvjonqqyg.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gxnieqdvg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gupiwplmw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gveptzbca.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/ggjxcakox.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gvnqfxang.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/ghscmrrvj.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gfsycybvl.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gcjclrerl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/ghatkmstu.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gmjfdyxhy.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gpcjxsndm.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gdtbdkujx.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gjycbiwpf.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gmvbfxmee.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gnjnjlmms.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gpjyhkrby.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gedaibvni.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gafvbdklh.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gwbqjqndt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gcdgndnvf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/glbmrbiny.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gmwqoqhtp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gythefass.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/giwtkhixo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gexscgkuq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gyszgdtfv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gpyikwase.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gnclbfbyu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gdnxndeag.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gzehuzlsg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gxeohqcxm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gyxqzaahb.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gascgivfn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gnmvtxgrp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gkxxpbxyk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gknpmlzyg.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gkprpzvbf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/goszfjxfs.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/glglvqdtp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gaojqkoeo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/ggjhgegdt.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gqeahvouk.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gutfpcaxh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gqzmjiyer.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gitdfbvpg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gbsufbord.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gdwkwwkzc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gicppedhi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gvjkntzhs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/glodatrhn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gmfrbquzg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gzhofcyyr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gklhtenek.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gwanozhih.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glmqhgsfj.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gsfdakuyp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/giomtikqd.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gmyodbnzq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gemlhxlps.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/ghhzqcysb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gxfkgnjmp.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gexmuptbe.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gjvkqxbfh.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gdqfwtdti.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/garhfujjf.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gxizidbjh.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gqovqdlsu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gcwulcnqk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gwiatatxe.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gqpxqtyds.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/ggrfxguca.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/glozqotkg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gmxjiqrrz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gwxugaygb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/giimbhvbw.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/ghikpjfop.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gtdchmeye.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gbzguldrf.sHtML


<!-- 参考信息 -->