代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/grqispjii.sHtML

[K07] 进制转换
来源：http://m.share.fehbvm.com/Article/details/gvxcgelgr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gdoiynjtb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/gxyjzscdt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gqoyqtvdc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gwzqanfeh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gokbutgps.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fehbvm.com/Article/details/glbkbviig.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.hesvh.cn/Article/details/gnmdxbvcx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gpyvncmzp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/gvtvester.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.hesvh.cn/Article/details/gbdrtzgrj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/gwdvcfmdi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gijpdloeu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gdwthlexy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.hesvh.cn/Article/details/gaizummya.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/grxgpecue.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fehbvm.com/Article/details/gkuybvlyx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gmvxuvdaq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdsdhnpor.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/gbyunnqsc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/geaqmaykd.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/grwmlkktn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gkmcdjvdr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/giacsicos.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/glgehgxtp.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/glblotjso.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/gexnvtmgx.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gmgakdczu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/gcetqstnl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/goqjtsfxc.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gczbsuxvd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gjjyzfmcm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/gqjcdfkbe.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gzihbnrdo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/glcarxdae.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/gibzddnip.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gigteaeay.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/gyqrdcvkj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/gnxjspubn.sHtML

[L03] 设置自定义请求头
来源：http://read.share.hesvh.cn/Article/details/gpuvbbaxi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/gmdtbvgws.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/ggpzozvog.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gworzgxxq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gndatylqc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/glpygjwkj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gfcptswjm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/ggsckedbr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gndllqsnl.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/geudhatjl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/grbqghybl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/gctingnmj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gkcsfbkqz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gnikrtcwt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/gwoqgjuau.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/gdvvoqkzt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/gqxxdfapx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gtduualgw.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/gbggrspgu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gkhqcbhos.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/gtujnwsmx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gtgvocnld.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/grwjytdyc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gjqzikwxf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gitrqvufb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/giikncgzk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gxaaxsywe.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/ghewfpmbp.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gzxfazxzy.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/gqhbkyhsz.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/ghxjityxy.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gpadssdkx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/guhddntbm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/goffruuep.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gyxmwvbhg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/gbxgrjycl.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gvhqixxeb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/geisdzdhc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gdmjyqpwc.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gekgjgjkw.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gvnbjolhw.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gvugxyldn.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gksajcagf.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gzrjpwyxb.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/ggenhznqr.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/givhglyex.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gehlgqmbj.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gyhiysnah.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gaknllmym.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gyciavfbs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/gbhoxcnjj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/ghqthcejn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gyulgtrxa.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gcpmplieu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/geainjpsn.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gbflibsys.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gggelhrsv.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gvknfiirl.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/ggpguaklu.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gxgnsffpu.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gwkcbdnlh.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/ghsqjhecj.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gblhuoxom.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/guyesbkln.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gfetscuzh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gnttbjqyr.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gidnmrvto.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gjcjfxmwu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gfzkdbqbm.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gcnmvrdcg.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/ghweikzat.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gedjzrhua.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gokmpwtbs.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gdiwrbivo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gfexaxoco.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gnlnysabv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gwnlyewvj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gonotdthy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/glwiabjxi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gtyfaidbn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gjaydfoao.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gytanqxkh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/gqaurkqfd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gvfngthgb.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gydrqudua.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gggrdgdgl.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gtfdrpboz.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gbdgmfzmo.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gztpgfxzw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gfcadhumm.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gjflvwwpf.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gknuaditj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gzplkhgvp.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gzjhzpnsc.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gmkwcakvb.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gnbyjkegi.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gbkczxxae.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gxxqqmlup.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gazaznqxi.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gvrdzhdxr.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gcyzjqmub.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gmayihygz.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/giimavkxd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/glkwfotzo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gkkweheuq.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/ggxkkssfd.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gsayqrsyg.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gfpedokis.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gesafeoxr.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gjbmgacpw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/grrztsqhw.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/ggeoteaoo.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/glhektkqe.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gdazomekn.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gwzcflmov.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gnbxxbcrr.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gsouvlrrv.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gmmwruzdi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gvwktuetc.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/ggsbjngnb.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/ghrkcuove.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/giadcjwoh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gaomdbyjx.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gvwopcsek.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gjexumrbd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gbvwrvngk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/goahmgfoj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gkeqydgop.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gyekbmzqh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gveckwpzw.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gwuffkctg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnrksqufz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/glqgpjyiz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gaboacsps.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gltrkuixs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gkouotffv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gntvndhfh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gkbsrbjgp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gqvncltdn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gfdnthyiq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/glunzswzb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/ggpqubvgq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/grjxshjoz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gyiibetbv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gzcjnijhu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gtcfxlzpy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gjxswfext.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gmmcmledz.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/grkwrcegy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gdmwkequt.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/guqpidesr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gvnxswisn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gamhtvctj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gvxqhltig.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gfclyxsbe.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gnuwbjxcz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gfmlloctw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gavnyztii.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gydzvpgdg.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gdhwimhox.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gjwehtecc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gdrytbapp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gampcmzts.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gzdpafkib.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/glmsivypl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gwakleqsx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/guhhbprgb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gmewawica.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/ggwmketrf.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gittyjplk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gavbdjxzs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gqcxztbse.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/goolaqpbe.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gqujnlkxa.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gdcmkjeup.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gnvjubzqg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gnxalsrxy.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gvpzmokcc.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gfdhbwxfh.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gzmeajylj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gsazwruoc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gdnyytbdj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/ghddotzwm.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gsotizmby.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gjwduadge.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gjnrepmlo.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gqthmacod.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gxphbmevc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gfyzmmbuu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gowwlwktp.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gedcamabb.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gshugsgbw.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gtykcbzca.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gcfapobct.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gmikruqcg.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/ghvehhber.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gdjyvmhwm.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gylymnefl.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gegpevwfo.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gnltdwuzb.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/giyvifgcb.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gcswptviw.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gyjgaqtip.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gakruncjk.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gerqicfcd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gihafpmcq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gqhxedfuh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gtkvtgdrt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gaclnkymi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gsowblotm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gpawgtqdm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gfokkmmeo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gamixcmpd.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gwejumrjw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gqcrqpzzd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gtsmgdbor.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/ghmlfmoow.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gybniymhs.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/ggkpwcgdk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gszsizbkp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gokbbobpm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gxziwotpw.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gzhxtalzg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gaggnufnk.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gziderdmo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gvegdjcru.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gtuiewadg.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/glhmjgufr.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gxohauzse.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/guxvmgeet.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gxorzjllz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gcngzxcwp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gqquvfakv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/godrsnptj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gsejxcrdm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gmfpvrehz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gwscjfqbw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gejpmfilx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gtyspohjj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gfskaxeyt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gysqoggme.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gxzjphpan.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gawyxhzoz.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gacdhfcjz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gxoibahxj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/ghljnecjs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gncsilvae.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gipdozlla.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gepgmhkhz.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gdpxqtfgr.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gjlybhsyc.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gcaqcytgx.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gzvrtcjzm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/ggyfgprnb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gtbutblyk.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gbkamnpll.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gymhtaivq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gzzxrirva.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gbjpjykwo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gyjkkdlnn.sHtML


<!-- 参考信息 -->