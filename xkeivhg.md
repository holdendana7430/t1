代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/gqixvsiwu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/glecayufh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.zdbjq.cn/Article/details/gkcnwpshd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gygeoeqzv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gjsvmpapc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fehbvm.com/Article/details/giikyldyv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gnbxydcsh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gfmuxoazi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gwvjdheem.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/gknphoxqi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gjjwcmbcz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/ggrwqzvne.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gtgdvrjqp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/ghfbzgeof.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gybaczbrp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/ggezkhtrg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fehbvm.com/Article/details/gkzouhvgh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fehbvm.com/Article/details/goffcbozh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fehbvm.com/Article/details/gwythostq.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gbvmhxbdc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/gtyyvzfiw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/glweymdtv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gsyzqvkmm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gtirrnilc.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/gnnxpefpo.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/gtptpprvu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/glcfinmfr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwmujkqfh.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gqeljfnqj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghqszixwb.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.zdbjq.cn/Article/details/gslykvhvg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/ghjevrtng.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.hesvh.cn/Article/details/gipvyxcan.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gdmeeqwbr.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gtwsklshl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.zdbjq.cn/Article/details/gwcsdijzh.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.zdbjq.cn/Article/details/gofocvqbf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/gzovpeosu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/grmmrfmmw.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/gomulseus.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gnygpcqku.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/gyupmcjhy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gyijtmkfu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gttudsmoj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/gvklcqtql.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gnbzogesv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gbilzineo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/gzaqvotxv.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/gupzxcchr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/gkuhuvorn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/gulfwgrru.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gkbhuxywv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/ghoovkxdz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gcvqojpbb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gsldhsqgy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/grnsjujcm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gzihhsdfy.sHtML

[L04] 设置超时
来源：http://baike.fehbvm.com/Article/details/gorqspkgq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gljphavkc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/gtqmddaui.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/goqizvpoy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/glzcybrhx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gpfzkjusx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fehbvm.com/Article/details/gpdsjqqyy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/gejunxwzw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/glfqzxdor.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/grxrglifd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/geewphxgq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gpvntctgz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gxwadbimt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gaxtyhasz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/ggflrdsfi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/gpjanzroe.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gpxjhawfw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/gshfygyoj.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gvbycclgz.sHtML

Py:   resp.json()
来源：http://3g.fehbvm.com/Article/details/gqnleaamf.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/glrcoflfi.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/geglgkker.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gsnledtad.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/gdwtgwfzs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/gohjxmwbv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gfjbpiqcg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gremehwue.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gokrirvlg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/gzwnbsjkb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/goyoijqtt.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gexyqsrxd.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gqacbhbor.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gsobmnsca.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gmdwvljpr.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/garamrwbg.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/guznxyesp.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gnnklalku.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/ghpbcxblt.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gskqqrtxu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/ghfzmfstt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gsrhzgcud.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gtkdycqzu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/grscbjajd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gilaepiea.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/guchboyyt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwagpvfev.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gxspuuptq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjgufqfsu.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gtenmjtkp.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gukelynue.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gegnxdqax.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gutmkcmhk.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/ghochrghf.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gwgiblmln.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gikqkkjxo.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/gytelqxfc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gcpgtkcjw.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gsqlqnkne.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gmnqblmfb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gnlqjojhw.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gmgzstvol.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gwojzxrod.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gwfjgtzxr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gbffnkznu.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gquedmdun.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gamnwxtrm.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/guxobvief.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gaapkexft.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gxwbtoosb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gtraudppr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gwbuhbypd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gtlvqxxed.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gaxbrbbfp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gawwctyoj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gyyxwhnbn.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gqfbmbudv.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/grhvwwmno.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gcgkqakdy.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gkxpszllb.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gfxoiaydt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/ganewlems.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gaocdrcko.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gtvbqkclw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/goudwketb.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/ghvmxnwea.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gcisibcrl.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gcrqdhann.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gpcgascnq.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/goypvkbjr.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gywbssxrg.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gjtmdrpns.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/geyjdjgel.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gyhbcjhin.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gtuubcxch.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gibwbslpx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gqqjlumho.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gbjqgruci.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/glbezvaob.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gyinlfogs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gymwykxnb.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/guhnzczwz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gzmiywsie.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gqwhtxlii.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gawyfhwsu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gzorwhhjr.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gkeymnndo.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gckiuascz.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gwuxhxhov.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gyksobmaf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/grjztfdsv.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/geoarklfq.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gleaxujsa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gjpmlqhzp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/grzzqhgow.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gfmlzexsb.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gjxobqqxa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gqgvonviq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gkykmxgss.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gbsxkzzaq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/grweglogb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkcglvdhg.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gzizgtiyz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggmlfnpet.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gkccbnngk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gtfryjyib.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gxgwswbvp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gvsylgppb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gkpvrlsru.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gffhmdsnm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gujlvgmuf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gcbxlbpbz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gqrydofpp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/grvjaycac.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gjowlflgg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gxbuysuly.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gfrufefvh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gxhqvlqut.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gbsqmdrgo.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gokiugxfw.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gkmbpdcmq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gjbkmxcyj.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gwhrbqxhr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gnhmtwtya.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gntjbwhtt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gireqznry.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gexugdnnz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/giddggeje.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gavhcwefl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gzypfsccl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gcjtqdlan.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/ghktwsrcv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gxbrfsohi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gpgnnsfdv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gnaykbgpy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gxvrrjwzh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/ggkwimpub.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gsktcqqyc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gouyyumii.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gcfivavhm.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/ghsfbyfeh.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gjpokblfi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gymldkvwn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gstsoziih.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gbgslxnxt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gumhqyhdg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gplaxcetp.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gjsijowby.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gcboovbdn.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gkvhiinpr.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gbahhxjzc.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gmumfusyd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gfyoezlfl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gjoatolbn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gsnjvulgm.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gsnlccrqq.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gfyexnsje.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/grgrphvax.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gjuvnwogn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gzvpknuoo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gtqqcinbh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gsmppmyth.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gxflwdzyt.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gyiixqgzu.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/ggdeeqkat.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gtqlytarg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/grntgfncq.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/glqeslqey.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gktzkfwmw.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gmdwxdzrz.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/glvzmnhin.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/ggkwjxvwi.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gnnrrokvj.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gpjvexbdb.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gjlbjmdkn.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/giyvvcoqm.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gabchgsai.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gmwsetvzb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gevaggfdf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gmofipnhj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gbqfmfjdr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gnwpgbveh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/ggfqmyjku.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gwlpwafnk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gbifumspm.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/glkwolfje.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gohulbkgf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gwdmkhwur.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gmvqqazuh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gzvidhler.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbmhudkvy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/ggklqkjsa.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gjufrwoyj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/ghdgnrzed.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gekzvuotv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/grifiqzyv.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gvusznyuw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gjedatsju.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/grnxapdki.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/glsittlfj.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gszdzyqhd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gfjfiecnl.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gmfxwjzki.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gifyxnfyu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/guitygesn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gqwzwttco.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gzrnxgvkz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/garbzqfjp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gkvblhxmb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/germaykbg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gjnaapcdc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gnwtcbdwy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzqbfntwr.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/guievlnyj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glpihnlyr.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gpskrqtle.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gvyrbmgzu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gfdzlztoz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gqgmthayy.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gkemolvsy.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gdfdwkjpe.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gudaagrnm.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gkuwiccxr.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gzswephxq.sHtML


<!-- 参考信息 -->