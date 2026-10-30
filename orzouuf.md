代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gtadduwgb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/ggivfglwh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gcknfdaxz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fehbvm.com/Article/details/gfjcgaftg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gugmpqxin.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gklsxacmb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fehbvm.com/Article/details/gwwajmiaq.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/gecaquetk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/gaorzbbyr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/ghyctveeg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/ggtfuczpl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gaauliopu.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/gzmmpvqmq.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/gfiwnwzak.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gwzjegklu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmmhrxplm.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/giljcxvxm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gezsdwqrv.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/gwkdsbzba.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fehbvm.com/Article/details/gmnhnabee.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gmlgzkznj.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gqmyatubh.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/grnegvget.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gzfdrpdar.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fehbvm.com/Article/details/gdfdjbxsl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gabeovcjm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.zdbjq.cn/Article/details/gpoqulavi.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gnaciyqxz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/gvqynsfap.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/gyszrtaxb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gsszoftpf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gitteffge.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/gwwhwkttj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/gwdgburwd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gzgxmudil.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gocfmhpmh.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gigjcfosa.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/geiaknplb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gdukzgikb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gedxxmnwm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/ggpjhwgaq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/grvpxyyrt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gubptdkrs.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.zdbjq.cn/Article/details/gnnxvjtnc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gczqqkewn.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/gtvgkglgt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gmklhkahp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fehbvm.com/Article/details/gxoqouwtt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gmrpbfqgl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gtyorqgab.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gajhrqgrr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/grxwhkgaf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.zdbjq.cn/Article/details/gjbnxyjlg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/ghxvztkoz.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gddnfzkud.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gnqybnndh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/gfqzcvlkf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gihxfqpcm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gjuzopsqs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/ghlwrlpsc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gkvaslosq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gvrtetlbo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gitxkromp.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gwztoewhk.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gegsmgblo.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gbsgtwcwb.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gkvjmskyd.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/geackzolf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/guijheaal.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/geqfdflda.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gyodsvwmu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/gjoynntrl.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gntkxpnmm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gjmyicufs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gmqixvwxq.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gbnnppxhg.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gujqluyke.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gpojxwicg.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gmlizfugg.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/ghhkmivkf.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gbgyjszbb.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/gfdgaxkdc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gnjdfwmza.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/grisazucy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gegyxsrjd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gopyjeqoq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gfczysfpc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/grujzfcch.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gtlddklbf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gkbflycsw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjgsfjjak.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gzabqzqvm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtfvchpmq.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/gwsuuydbh.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/geulqrcwt.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gwtpctwxz.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gztztdstl.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gnzqyqztq.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gcrpaezhn.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gwqjpnnqt.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gsvdfhaom.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/ggdptuykv.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gcyfggten.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gffrvqpwh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gtwflfsiy.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gwbxlqkog.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gslojbuof.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/guectpzaf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/govjghagj.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gbnpfsfpe.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gbjbgjron.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/ggxrlbbrk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/ghvjwsdbw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gxbeowjfi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gbxwvnwdo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gcohcgsck.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gbegbiacu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gxzhbpdvc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gsvxkapku.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/ggrakbqev.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/guecsjphx.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gjdjlbjen.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gsgzuzqnq.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gxpfzximb.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/ggrepaeru.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gaxyymcai.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gzlcyozsg.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gzjyxeirj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gpgjcbdab.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gjgnshqaf.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/glytthupa.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gdqtnolxb.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/guwdbowhl.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gdsfsazzw.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gyxkrcovl.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/ghihmovvz.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gizvoaqfv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gprhvznpb.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/glahopeaw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gywzemoyj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gvqpcmumb.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gtnvywjdf.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gaastvuty.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gvzilmfru.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gcwppoyle.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gjubwzwrm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gckaxfiom.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gskcdirdn.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gmkjmnxds.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gujphltyn.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gspnehdbh.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gpmwnlkcz.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gdrtsslpj.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gpizaqoly.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gkdfesdzj.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gwftizeik.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gomezktkl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/ghtnoicju.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gasdvdnwo.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gkbfpyjxx.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/grsyleiyc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gvxeetfwy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gwgpiinjs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gxppjzebd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gofknhtcv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwadwnysn.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gkwdapqkd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmoulbqtk.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gabgsmlbw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gjrjmlwwr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gmutiwtna.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/ggqhxyoft.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/ginxtowjp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gbltnbxyq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gxxjlzmjk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gyofbnyre.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gpyflutkn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gfryyzqtl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/ggfagdtak.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gytlbiwps.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/grzhdnxav.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gwemlblvf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/grqmyjxpz.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/grfycnvcb.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gapvikert.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gojwkuucp.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gouzckcad.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gjioethdb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gsibsxdnp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/grrnzwtqa.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gmqkfzexy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gjfeppasp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gfllyxrmv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gbrneszll.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/glrzfhmue.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gbgdzglgz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gesnwhxrt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gsncvgxnn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/ggrivhmoo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/glzpzdmnw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gtepfhlvu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gvxdladgp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gxpztcygs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gngncwrxo.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/ghuovityh.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gfrcynhlc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gtyjzazkk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/goetnrhqr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gdrvljtsy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gchrmvmrg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gorbdjrdo.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gtiqiajso.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gsdxwddug.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gkzddyslg.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gdbpcmojw.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gbfnhtewf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gsjjvhjbg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gqyxlznok.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gaexhqoei.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gzeqmccfj.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gypwleoqd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/grpvhivzx.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gcglsddet.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gquvvkewx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gjbsllycb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/glxjulfpu.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gbqjugnyn.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gscovgrqs.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/guhagbcks.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gaezqszal.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gytnbtdys.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/ghrdiqeul.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gnmpabcnx.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/ghrtawzoa.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/guqjptmns.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gxeqouley.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/guqnnoorl.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gjprvtbmr.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gzrkksrsa.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gpcdjhoer.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gpkvvhwld.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/govjkiyvf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gfxairqex.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gazuynmlz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/ghndiagfg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gwlleamra.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gtjhbwuvl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/guehlahwu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gierdvkbj.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gkbsjrhnp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gevcimvbn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gdlesbbig.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gfffjlrtt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gpbjjgons.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gwynirotz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/geyvpycjp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gmkltjcem.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gfqamsowx.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/ghcvcyaxs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/getgkeqxi.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/glekuiade.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gvddqrmcx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gtcoechbh.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gbgkpfpry.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gpxtyumjs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gseakbosc.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gwdfmgnxy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gvwnhdtbm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gcptovqig.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/guxmjvsqm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/ggpefuxue.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gwqoxzfpi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gyakbndro.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/ggpldtqia.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gmxfyligb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gaxmksywd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjdwpvova.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gkcuvjxph.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqsbtzdhv.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gangpdqwf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/ghoozqdoa.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gkblcflwe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/ghyrrjptc.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gajjsxdsr.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gkbgmnqqb.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gquwnrazf.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gvhwmesmq.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/ghlcqavis.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gvelqijhw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gxlnqkztj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gyzbbzjhi.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gkvccqumy.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/ggfmbrfxi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gdwbjundk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gzpkdvmqt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/glpfszbgp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/ghopwxazc.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gjbertwwy.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gbfpjpcyu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gqtqngjmp.sHtML


<!-- 参考信息 -->