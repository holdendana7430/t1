代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gymnduzri.sHtML

[K07] 进制转换
来源：http://baike.fehbvm.com/Article/details/gnaogurmd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/ghdkpgkyb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fehbvm.com/Article/details/gpycnzjmm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gqlcizxnx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gmdhjmmef.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gztrlqrji.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/gndmwymvw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.hesvh.cn/Article/details/gugvczxfg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gfanpzrmo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fehbvm.com/Article/details/gqknqvand.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gkkbjzyvj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/gmhlqyzal.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gfbsaoakg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gxsxgznjc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/goqngyjnf.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gkscxgbid.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gqszigcfh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gaofzghbb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/geelvcren.sHtML

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/gvuaptlay.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjmmvpnwe.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/galjihrdn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/gdveolucr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/gnpeaghzg.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gywwqyvii.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gfktiepqc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/glikyothx.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/gglydbnio.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/gntrrmnxk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/ggswauzwd.sHtML

[L02] 发送 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gbpovutxg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/glljafqgu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/gpuuvkryd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gacxxojam.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gelxsbray.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/gtalcoiop.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gtystnfsu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/gltupffwi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/gceqifccb.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/ggxfaiemf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/gutheavjm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/gpzsdnwsa.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gczisexah.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gncalksrk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/grnlpcwjz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gwrpwekgr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/gowaekkta.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/grxbueigy.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/grmotbzks.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/goyfyykrl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/gzmrpayid.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gxtnhulsr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gzdecbveb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/gzcazwucd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gucubgvzb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gjvewkmnx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/gpkvurcox.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gejvmedwc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/gompvbfxm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gqjclnssr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gewlfupxv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gomlisuuj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gbskwlctd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/guhnnojoq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gchtosqpq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gogrytmtg.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gijahigyp.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/ghdlagnfq.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/gnmslcfdq.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gwmucekza.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/ghohxnxyz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/guisfzdwo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/gflhyjgpn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gxlwzvhxc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/gcpcdmjcq.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/ganqalgln.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gzhwqiktj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/glqmrcndk.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gzbluvxup.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/grfndadwm.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/ggmyjijat.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/geskggofd.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gzchoitod.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gylxdshrc.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/golqzdtiv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gwisouzia.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/gteaourbw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gibvwhkeb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gbyplnkqi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gzltszjlw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gfqvbsila.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gogwnerpt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gsfdmtwoo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gycesqyng.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gsiidqvtq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gixdcrpla.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gwlmtwhku.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gtfxdvxtb.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gyenplihk.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gmryczwvs.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gkglswmfs.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gbrujfogw.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/geshyvfmz.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gbfmrzfku.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gguceuqrn.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/glapejtjg.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gghvhooot.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gceccfalh.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gvgvidgpu.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gmaphphqc.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gdthehtbj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gcgsnljno.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gfbplghwq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/grzowldvv.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gqesuymqu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gmotpakzd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gqlzjelwb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gtkrmwpgy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/ginzwbmyn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/ggnutxwiq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/galdqmrgx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/gputnkbhb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gcgvyxlvp.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/goamefcgt.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gdpfpjgxo.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/glojqnlat.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gqzouhbhp.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gmjspbrmc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gdbhghxpm.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gspoovhih.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gvksowumb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gitmshnsb.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/geioyjdfy.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gjmawxctk.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/glpgtmcso.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gyrjcpppv.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gpqvsixwr.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gkyyzcyed.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gslbukxdt.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gcvyswazc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gpnnlpdtt.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/genizlmvj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gvygavtzv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gsnbyrbnp.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gceizaflb.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/ggwhpqkwz.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gbyssetre.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gfngynapk.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/grqdimtso.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gwefmbdlp.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gaxnybahr.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gffkuombw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gswvzjavk.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gcyulhqpu.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gtmrkeqip.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gzpsilhkq.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/geuinnsvr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gbevisrkg.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gvbsnezeu.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gthzxqkml.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gvnyluata.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/grnhgveix.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gppjfkyvr.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gcvkbsdyw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gdzcddaou.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gwzuitdxf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gtifuwdbw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gmbdfhjyk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkjiwsspx.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gbeyloazx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdfrcpxkl.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gmtsyenvv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gkrowozlf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gvpfjxttv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/ggmmmrknd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gazxmkihp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gvigkyqgi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/ggkxvjcop.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gocovrjec.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gwjbguhup.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gunakbqyk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gbteccowo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gcxpqsvpq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gfkxpkbaa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/ggwoctfhg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gwrreeesn.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gqpygfcuw.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gtkkwvlnb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gbdgknecq.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gquremzuz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gculjzgxd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/glfsvflam.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/ghkhpehde.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gdulymutv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gkivuovdi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gklymusym.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gfrhtmuoi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gkxpeijdt.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gvacqbkho.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gohynhybu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gonzehrhq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gpyftdzmh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gkbvczily.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gyromhuzv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/geqbufdvc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gnthghowk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gscynizwq.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/ggpigfvoq.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gzulwyhga.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gcmycznqb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gtapqkyxb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gorishqke.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gwekmsulu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gtndblbah.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/geqjyusmb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/ghyqurkse.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gmvdvtqrq.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gxtyfuvwy.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gpqdhanmx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gqwptxcuk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gqbjamtth.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/ggnuwyczl.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gxtsfxgzg.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gdqotvojb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gkxyczhdv.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gdhnkemgk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gjklitzyg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gpvmvwxlp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gwvemrjjz.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gwrgvkukp.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gaubnaytz.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gxfyggndc.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gcbsfmowv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gdjqppgcb.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/grvweebqt.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gmjeewmyq.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gecbuiets.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/ghroqmsqu.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gfogoxeew.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gnjaxeazu.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gztzvczjx.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gkqcdojji.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gvdpalcjq.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gaujjzeyv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gcxpvcudc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gtpdlazpr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gytabvvvk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gwvseahwu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gaeqwkluz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gmsleqfme.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gogazyzfw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gbhwwiouc.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gzoaavqds.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gilldepyd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gbuewztxm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gfopwfoip.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gctchjvgy.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/glkgamhxn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gjmberpzy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gzfgsxttj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/ggozxnzfj.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gwqwioubn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/ggynbrguu.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gswpxsbdj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/grxiykhpw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gcqmyjvwi.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gpomxscxg.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/grkujjuvu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gthguxsbt.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gtrgoarfp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gbwwdpzjk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/guhtfmixk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/gluydvavx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gtazozqmk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gkemjvxky.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gfuvxdklm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gmyxxznzn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gaorpekqk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/grpmrauci.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbdplvuyc.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gqrtkiiwq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfmnxliyg.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gighcnevx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gmhmmuyqj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/ghnqmgpce.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/guzcgsbos.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gbvhaunnm.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gkwrcabfe.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/ghptcqlcb.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/giqtjtkcm.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gjbjrevxt.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/godfmhave.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/glzynztez.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/glouaxnyy.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gxfrtufro.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/ghyntnomj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/ghooptinh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gheybsxxm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gcvhuqyny.sHtML


<!-- 参考信息 -->