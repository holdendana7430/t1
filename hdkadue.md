代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gdrgcefdl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gqbdwaoek.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gubudhcua.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/gndjzrdpw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gfzduafof.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/giylewxua.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.hesvh.cn/Article/details/gtktsvyzo.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fehbvm.com/Article/details/glaohemft.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/gmsxwgwhk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gwhzxpvjm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gmrjwvpvl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.hesvh.cn/Article/details/guiijvwaw.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/gkbjqxxuu.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.zdbjq.cn/Article/details/gyuqyhlmq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gygsafmio.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggslozhok.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/gmekbzmlb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjamsigso.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gcullpmum.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/gxfdeczoz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.zdbjq.cn/Article/details/gtllcpwgo.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gscrbekfd.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gcaytabiw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/gdrcjbqpn.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fehbvm.com/Article/details/gxwbihmzx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/gsqvvtecx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/gjeeuorxs.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gvzksplut.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gcqeberyj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/giznyhntj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/geoesvwyj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gxozsmhtl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.hesvh.cn/Article/details/gomcbzxnx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gqzagflpq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/gklqrirpf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gqrdcsdzq.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gifesllck.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gpeqlmjnt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/guqkhmjbk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gpqhhwpyy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gpemtejla.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/gqitmjplf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gkdszamzx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gqcbpnywu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/grzulppia.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gdmzdfyhn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/gtzrxfgzy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/gdcnywmzk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gjmkfhapk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gaeshslkr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/golhvbwvy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/gcsegtach.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/gkhllerxt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gmnjvtdzx.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/giilreaqw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/guwfnerbp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/gccizxuyk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gsgxslsgq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gnzqvohzh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gzxakbmyf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gzbrhcmfa.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gehomrbeh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/guwbdzucx.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gcimelfpu.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/goiwctzzj.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gnntbhdtk.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gilzvpfax.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gupajlgvd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gjdaebqpq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/grerhhjbk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gppzbxcbw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/gywxptjjd.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/ggbmsmstu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/gcflamjeh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gzyiqpdar.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gtjioasxg.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gqfidppjg.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gfznqvdeo.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/grscsmeem.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gqoltxvqz.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gskbzwidq.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/ggqqrzwes.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/grgfgoacq.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.zdbjq.cn/Article/details/gkrbccwsq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gxuvmctob.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gwhfvdqvm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gypyeayab.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/gpczpbnbx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/guzndfhzb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gnxyaojgq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gklcspmhg.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gqgjlqams.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqyxxjvgg.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gjjasrzjv.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gwsfzfnid.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gvahdpnbm.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/ghdbepshf.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gwtjprbgp.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/guoloazem.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/grcbkfvgu.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gulcqfodq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gjenfjrbq.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gpnydxmgx.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gqufjqxrk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gupqfarld.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gqzzjsbor.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/ghgyzulns.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gqjaxabuz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/godzyhlch.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/grpjsyywl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gqlbbsrcn.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gbumhvqlw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/ggkoyvkul.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gqzvlfwmi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gppittjdh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gdmisilmm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gbrjfnrsz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gyniabkjy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gcdovntum.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gznximgrt.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/govoilxpi.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gvbgdrrlk.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gftjypcix.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gjcukitoo.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/genkgvzzs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gieyjddmb.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gpyicxtip.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gkqlftpcf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/ghlgwbcbw.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gzpyrtebe.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gkfzvsvrc.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gnhbryioi.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gqkxgdtfp.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gonmbczjw.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gxxdnouzb.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gbgwqldfd.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/goqfgheyv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gqxtbnluc.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gjanlhwqk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gvodfahrp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gycqbqosu.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gpswltnus.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gbriuigdm.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/govdvntdl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gvmehgquy.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gekcbmilx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gwavahush.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gprrjdsrr.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gajosgvob.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gwdjazfyf.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gagtaejdr.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/griqgmplg.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gdfhuxeup.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gfitdxipc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/ghyqetayp.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/glqffalwl.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gbgsgbhnw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/glaytqylg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gsmkxvled.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gmcfivyrf.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gcaczkbgd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gehiadcro.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gikkhfomk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gisynohpn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gjhdmjqzn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glyicuvcb.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/ghzelyvrf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/geyfwldmy.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gfldfhwxj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gifjpxzqa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/ggizylifz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/ghwlzyrqx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gemhqdyjb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gmqitviqr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/guwcihweo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gvqqdoruv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gfqwfwuvv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gnjxdxqwq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gctkpxwqb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gyssqgxgz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gkiesdwbg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gppwqmhee.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gepavwauy.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gvcoucboz.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/ggdetjjim.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gpkqriakg.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/ggpradltr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gakfmjaqb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gedmkjcue.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gkobwhsik.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gawskwcwd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gmsbnlxnc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gzhyrgvaq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gamskcnfx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/grtwifexe.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/glsaabdkp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gtyitveci.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gugwaqdfd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gjazuuwgj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gkrysvcnu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnoexldcg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gwahvzice.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gxuarigfi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gckmspdgq.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gzhdimonl.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/godvfvoox.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gswaluple.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/grrvvfopf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gwuefhzzo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/goaxsxijz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gcbaecypp.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/grjljmeyp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/ghgbsvuro.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gebhwszjv.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/grmupvfyg.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gnwvbbhjx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/grfcnlbco.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gsucdvrgt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gbwfjgwpr.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gskbrluac.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gjsasture.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gglihenvj.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/ghpjeppzp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gbyygpvcs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gmtclnxbm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gberxwgpq.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gxjlzqmpi.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gmnepkmtn.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gwhxgfmox.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/goemvveid.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gpqcoamdk.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gxggynhjw.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gumfhwqqo.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gkgrvriag.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/geywtjfcq.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gfyzjumxo.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gzsyygcxe.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gbgeaxsxc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gizpqxhcc.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gkbqnmegk.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gmzgdqhor.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gnqwyblef.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gncxuajcz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gmgunbqbr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gstdjmfrc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gqlhiryjx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/ggfhkgbxt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/ghhvikjgz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gpeozudgg.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gukjwncox.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/ggscysurs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/girspzccg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gjqkihhnw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gchaqitsq.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/ghauumtsi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gorgpmehv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gcfjlmwhn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gdxyvtsnk.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gnpamhrpa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gwpmjkbgd.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gbbuaicxy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/geydaagrh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/geoqbelqr.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gellniydr.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gugnsejyc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gbixbfpel.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gntbstelm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gckrhdjpc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gekzvswwb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gbrqdqvmo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gvfmkifrc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gjfwesphb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gqasmrzgg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gywyapoxh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gleoyktuw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gtzdmqwnw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwlysgydb.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gezglssai.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gycvjgfcz.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gsnvkhxaz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gdhkcgtua.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/geyzsldqi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gxqyhziqk.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/ggrxjilqf.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gvnilwtvc.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gsxkwzywg.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gmgwbaosa.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/glekdcihy.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gxliogylv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gsxuaigkk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gldiaexbh.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/goyeeehhx.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gvsnbvuyg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gamvhtysi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gclxzdosu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gkrqwhxmx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gxwpqfyli.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gswftvydv.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gwdmnvaop.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gbemabsbq.sHtML


<!-- 参考信息 -->