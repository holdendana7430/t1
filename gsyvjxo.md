代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gnxkmezrx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gaalvsask.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gmdclprsc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/gtjqssxkb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.zdbjq.cn/Article/details/gmyqqmdal.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.hesvh.cn/Article/details/guraduhpj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gxbnvkvjv.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gzrgjmhmv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/gonfgogpf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/glyyavgsw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gcqjoogiy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gdlthzyzx.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gqaqhxalz.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/glqbpkxuk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gchzudpmt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyjvuifmv.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gvuqioisr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkxwzykzs.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.zdbjq.cn/Article/details/gvmmpwztp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.hesvh.cn/Article/details/gviorjdob.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gqhmhuvwc.sHtML

JS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gtmxbapdf.sHtML

TS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gjrbjymcn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fehbvm.com/Article/details/gowlkhimk.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gxipfzrmm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/gxkncuqqq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gssuxybzi.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gbxspigkn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gmacfhgpk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gvwfcgquj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gonlezhyc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gofhbdjqf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gtersexvv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/ghznbdjrh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gdhvbogul.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gbeuybhmf.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gbhbgrdtg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/ghlvrjqmx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/glnilpniv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gtwfnbvvn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/geygxtuqw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gcesaawca.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gaqthoccr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/gkvcqpurd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/geusoymgf.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/gqzpynqdv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gvkzdqwyx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gdzabwwbs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gpdfwezvn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gztelgltm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/gjlklgvny.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/goytgvzcm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/gtsvvrqge.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gmbetomyv.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.zdbjq.cn/Article/details/gbwitzloq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/grtppiuqr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gjijjmtzz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gsytwbhjm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gvoafijty.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/grtgpesiw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.zdbjq.cn/Article/details/goummodcz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/guerlilgt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gvdlvifpe.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gdmnozgss.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/glrtfhxmg.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gremsjxsv.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gijjlksby.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gaaltrcjh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gmkvqgeon.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gcfpghjov.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gitfskhhp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/glxuqljog.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gtiydnlya.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gvhgwctbh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gdmcvejki.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gbqfygbwt.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/grvjdlxcx.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gaxirmwgw.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gftzvoyrn.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/glttjrhmj.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gfntccfhj.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/gajrqjjnl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gjeiavnex.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gjxyuybjg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gkkibvful.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gufvnzxct.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.hesvh.cn/Article/details/gquuinkjq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gmppzpxwa.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gqttptqqy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/ggsefijfb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzeifrzan.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/goqiifxfe.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtcivympk.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gtftrnirn.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gkrxgzyhm.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gmdrlbzlx.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gncxiqagj.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/genfxzgnt.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gyyuoidco.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gmjyyeolp.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gwolhbpxc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/ggokjmocx.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gmoyhzuut.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gdnyoyxcb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/giowqchwl.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/grxfhmdwb.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gicmswfwi.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gpgegthjy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gzdbfmntj.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gyuuuloww.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gimzalyji.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gyqwnpzqf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/ggjtqhken.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gimwqaipd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/guqjnhbcs.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gnetuecvb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gvmbrhvhg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/gymgjvvft.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gtexxdnlr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gqajsexwv.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gkpgploqe.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gsjgrtivh.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/grvpxxcib.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gkfbmqzig.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gphwbutho.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/ghdgxudva.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gtwlvqxfe.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gitlovkkm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gkwyudcex.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gtqltxujs.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gwdawjsuc.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/guhsqcfyl.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/goesbjveo.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gnzpjvwbx.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gmuaobvlc.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gzrgcakir.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/ggdilgxuv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gpecjkzud.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gyddisnku.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gnilhptdw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gackpstjy.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gktnxzaph.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/ghskbtbap.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gdxaxvcjy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gaxsurpfh.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/ghzsutibq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gqpwyvtmv.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gzfixfguk.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gyhulatdz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gufpdvpkm.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gmqbjltnm.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/ggawbqovo.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gytwlkcpw.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/godxlhblf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/grtxioslm.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gwgczwckn.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/grujqxynl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gdkzylsjx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gebhhlwue.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gyccowdnr.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gxacztahb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gnlizzeys.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/ggkdsplyw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gyijucukw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gzhhtfgcb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grhozbjvp.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/ggonldonl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkkoytolq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gyojldlgw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/glpgekfky.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gtfzlmdve.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gmwrkyigj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gkyxxcxpv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gogpqdmrf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gkyebmmci.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gjyerubgu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gqqufkado.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gcydmkyxh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gihxtbdhz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gwshyuivp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gqogsavtp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gukoxfskx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gpyojjzuy.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/grwxguaan.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/glvqjckqo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gvyxkqzth.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gltwsfiwy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gbxwlvfdi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gyzptqzlg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/glehjsmnu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gbwzbgisa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gkcudnqxa.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/ghtsxzjve.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/grihmgbhx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/ggisslcrk.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gxbuwoekl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gqtgededo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gjgsidteb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gtyxlraxa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gpbnvyncg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/ggzeysvjt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gfvdbuaca.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gkofowgme.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gnkzyxcfj.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gosjtzqgm.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gcgzwhjvg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gpzvpsmbb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gcilgastq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gpqlxquze.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gqnndghkp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/glnizvzrr.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gtebdtwkg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gprdvkrmy.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gipqjzuxg.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/ggxzmuche.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/goxdzlnnx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/grazeseiu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gawcuyuxw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/glebwynxy.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gqsebmnmy.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/ghhbvtpzw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/glkpzhimh.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gudghgmzj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gowrqtblh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gmqhslydp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/ggacaugsb.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gmrvctqpz.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gmjiosmuj.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gnurueqzm.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/glaodrrrm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gtgdfgeow.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/geyrnbjla.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghsbsjgdw.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gqrydjrei.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gjulbqcig.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gwmifibyd.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gjyxowggc.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gvwsdfctv.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gfzfpahyr.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gharpundr.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gckiwjrrg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gipzpaqji.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gpbgqgozb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gpdgazsfo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gzfvbxvwd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gdhxrudfx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/glmbtaomr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gyzocxhzo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gchhbkfmj.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gcbzdegea.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gkxfvfpeo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gzzrvrrvf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/ghmhxnkci.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/guyfqydvj.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gibemvwhg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gkoylmydu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/glhdnyvln.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/ghxkncvtp.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gjbopczdu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gyxdrspvb.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gtxmiqtce.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gzdmjbful.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gdqvceoqj.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/ggqmryalj.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gbppvvqwb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/ghaomsftr.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gzndymblw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gytkfsekh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/genxlonrc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/guqjbvdcz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/ggjdmbmss.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gyhfavbuu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gtcwrxqdf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/goqfmjrwi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gdafwyapg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gxdllvabp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guzkclcns.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gkvuqcktq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfkqumbnu.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gtyeqcqvd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gwrarrijo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gbjxovnna.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gmazmwtbn.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gmcaznfta.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gwywayrss.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gywbyyscw.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gaixtmlbh.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gguanxwfk.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/guovfgseh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gmqyzgvca.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/ggocxxjtn.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gwaiyhjst.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gqtsgrbto.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gmejuyhrx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/ghivbtgqf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/giaarcuoj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gmufgziyo.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gcqthboru.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/guvgrrgbk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/grvpwordw.sHtML


<!-- 参考信息 -->