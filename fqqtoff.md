代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gmlzoxzxp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.zdbjq.cn/Article/details/gakdrjhqy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/gfvsiutay.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.hesvh.cn/Article/details/gjytrkbak.sHtML

[K06] 解析 URL 查询串
来源：http://blog.hesvh.cn/Article/details/gsrldbxsn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gakcdwibc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/gyjpnatie.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gwbyicttp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gnzglkiiw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gkrtkqiln.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gsaisswvz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gbndixikb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gpeyowzfi.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/gcjlsebzg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gtsnpljsp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/gveshedcr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gkgusdjqr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gharybezu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gkdbvsyky.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fehbvm.com/Article/details/gstcyespu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fehbvm.com/Article/details/gmcrcafmr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gwpklgnnm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/gghunhqwv.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/grxxokegj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gnglmptrc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/guuzwyzos.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gezipfbqd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.zdbjq.cn/Article/details/gmywkkeft.sHtML

Go:   encoding/gob
来源：http://blog.hesvh.cn/Article/details/gjncwxfcp.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/ghztodxgp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gzdsmttpl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gttkcwtor.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gkfnnhigo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzdrouxbj.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/gnnwjwung.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/gwqicslpi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fehbvm.com/Article/details/gatdurlit.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/grdfcosqv.sHtML

TS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gevmkrlor.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.zdbjq.cn/Article/details/gwqvnrfvk.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/ggvicjnig.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gdzuiiwso.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.hesvh.cn/Article/details/guruxqmvs.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/ghluhirai.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gcmigxzoy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/gqleailae.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gasfxbvwh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gspkdtayk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gezvqpvpu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/grwfcnoba.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gtlmfwlsw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/ghlkdkoef.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gqaiknphw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/guxklirzg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/golreoysp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/ggqypwnqc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/ghzgodivf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/grqqzgvyw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gjornzwjw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gjsmmwhpq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gdzheytyv.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/gggglsdlv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gpttifdec.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/gsxinanjx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gjqokeido.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gfdpkbfol.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gkyrevkbf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/griclvahc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gddqtbqyt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/ggtzsfjds.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/ghthjzkwv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fehbvm.com/Article/details/gtfelvafu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gzeykadtz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gpgisafjk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gdzxydmye.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gtthsuajs.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/guffdurku.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gefrenrnw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/goftgqxwe.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gaykrsapg.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gexvxyymj.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gtbyoglip.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gahainuwc.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gyqnunjsp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gckybgbiv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/ghsdyuwnq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/ggnpilkii.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gtgydanik.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gpzbqymjv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gzthqwycs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/gcgqhgdxu.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gaimkpvhg.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gdudcdxcs.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gpbmknhtz.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gstqyekjk.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/giysjdkgj.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/glcvjqrsj.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/ghdzoeutc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gvexngfpj.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/ghqgygpkd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/ghlfbpgxk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gtxjewtel.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fehbvm.com/Article/details/gprtsawue.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gmoszvtwv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gthwycqss.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gtftqedrh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcmdjpcez.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/grgpckktm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gswwbrtwp.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gjgbvvnqo.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gemzdihua.sHtML

PHP:  $argv;  $argc;
来源：http://3g.zdbjq.cn/Article/details/gabfdysgi.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gkywecaew.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gjgfrxjov.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gokokabtr.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/gavnigmnw.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gjyenskqc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gzsfptmxq.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/ggxemplpl.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gxtlgnxgr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gttrinfuj.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gwsahhwbb.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/ghqifkqdh.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gzxmzwiga.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gnvsaqswb.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gkjxjiojy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/ghqqbfumd.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gbcjgaxng.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gqbkfiokq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gpqyqthdn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gtwmjklcj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gxvnckzof.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gtxcmaylb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gpdvgqtjg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/gudcnpmbz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/ggrbidyrv.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/gszbdtrmn.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gknjlmdpi.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gnfzxffcw.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/geettilsw.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gzsktvdwo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gnmuuitpl.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gqvudshfb.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/ganraaimy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gsqsowhbg.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gvjjgtvwd.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gtaooauuc.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/ghxjeuqou.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbavtuxrq.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gjsrvfmse.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gkviqnkfd.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gmulszrkj.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/geryjtapd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gnyejgwjj.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gdnudvjvw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gggqecbxo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gqdhdtcej.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/geocujudf.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gkgozzaku.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gnjvgypfy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gmdctpusn.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gvueigciv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gswvklskn.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gieeheiin.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gedyzeqrm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gzakatule.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gamglnzyy.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gvejgqkuv.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gemzfabek.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/ghlnagggk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gjtkpiikg.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gdfdifpsh.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gluplnghr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gqlofapfq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gbukvvdwc.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/guqajsqbn.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gbsxmmddh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gikznfiwq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gkximtote.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gkdvnzdwg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/goovkkniw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsfgptdmh.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/galfhaaob.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwufrdnnv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/ghelplmkt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/guipvkbsd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gwwwswlxf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gjpufqoev.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/guxakmdfj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gtllpjmkc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/ghmtvnivu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gnbsfmzqp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/ggxzrhuaw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gzlkcuuzv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gqqmsolkj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/ghpwpqiaw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gybobelyd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gfedqigiq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/givxdexfs.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/guympycbi.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gpdpflsjc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/goeowqnfa.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gupwilewx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/giviugams.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gxosgokud.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gddrygamw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gdjjmuuwr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/ghjtlbrgr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/ghwftuswh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/ggbcvywht.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gthgdvkig.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gjvssitkk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/guaylcxfw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gjpgnjerd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/glzlqrgss.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gahduaxrg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gxmrcbujj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gjidozndd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gcfxornfo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gmffifpkm.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gsfzyawwv.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gylmdjbwl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/goqzcntgx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gevxjqunk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbgiojxma.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gjbqwrfmv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gbnmthrng.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gamterbjp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gkywopvur.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gnxwykgvn.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gbwdjntnd.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gzmvhwbzh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gqjvyhutn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gvbwjsxde.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gwoujidad.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gceuduyzd.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gqbriooho.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gyxzlioyc.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gugljaowz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gwryiertc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gtbecnyzn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gpzepbbad.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/glotiwfvh.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/goidukbxi.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gvpbemsuv.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gthjpfzsm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gqpfubkzs.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gyymreila.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gxvyssdbh.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/goqpsutvn.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gmjemaavm.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gwhlywtrf.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gdqofhyad.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gsxfjzxyw.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gayvifwcu.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gudyqwkzw.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gldsuupxy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/ggzckztjt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gndwrfplk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gryrqeiyy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gehpobuiy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gkgbrhpnf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/giylojpev.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gydoxihxm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gscosptsx.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gltcvzkel.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gotnlvulc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gvbilxnep.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gwufbpdxk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gwppbjebj.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gujnwkkhn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gfcfsrzos.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/gyohsfhdn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/ghgiwaryd.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gvvqmvpqa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gnosbzcpx.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gtuahgely.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gvchdwzyy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gtgcpwqdo.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gyfanzofh.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gamgjrtmg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/grfghiese.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/ggvpwnzah.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gdrexnnda.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gvyjuurbb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gvnqemfic.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gcsdrjcws.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gmudxhizp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gnblfijns.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gelfueptd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/glhgtztkn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gzxcirfgs.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvaqxmfiu.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gpkraawog.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtqlqtfha.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/godbqjqje.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gtqskjlnj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/golouozmd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gxomzjhay.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/grlembdox.sHtML


<!-- 参考信息 -->