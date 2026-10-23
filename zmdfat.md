代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3rldohlxt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3ucvabyqe.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3snozjktr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3beemnerc.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3qdutlyhu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3uuuaxdzy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3ovelmekc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3kkxopjcn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3vfteceyn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3pbinqwjr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jrzsmwag.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3dslrsqje.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3otayljuf.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3hysyhybq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zsauejem.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3wxfceezz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wxojasmn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dauxzqgx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qoffvcmu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3jinqysfv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3bigqekig.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rtocussw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3wasbgpjw.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3jkvxugqo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3almysjnu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3knpnxnof.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3wwzhkvqq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3iuywonio.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3lrpeexrq.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3oqeqmomn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3rqdwwlnm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3djvozuxh.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3scjbvqyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xcecqodv.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3gubqijew.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3gllzfvhv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3ftpgmyou.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wjgnqzch.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3estaolcf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3dmotednq.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3vdzvwvem.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3qbitevip.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3akpzqptg.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3hvfgqpxg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3vtgxyibo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3ysumnfjq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3hatrxrxw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xvubgjwy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ihhxhfvp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3cceogaqk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3pczzbfqm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3cmfbakfy.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3jdixkbnc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ydisvrcb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ukygoifa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3cyexgivp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3fihglvkf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3kshcxffu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3lacpoafu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3bfexshfw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3fdvvzcku.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3kufkifir.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3szvdcmyx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3wewvlkec.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ppgllbig.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3oeiptwew.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3blwvlkbw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ybwxbpss.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3yfooqsiv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3yeozpbkl.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3jhdhsnrm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3fobcbmjl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3xewnqfzg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3pbvqdtmc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3xufymogf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3uebpseop.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3nrvhzdmy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3mhyczbnx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qvrstjup.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ewsilfga.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rfhiodgp.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ipwaikiz.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vyjqeiky.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bvyuhfuq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qervesbm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3jwxrmzrj.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3xuozlmld.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3clsmsabw.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ikgrzgiz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3dsyvkzhd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3nzqvxaep.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3kuimtzuo.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3sbfnybni.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3gxrtsopg.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3eppesuaz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3vxjlmehs.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3lisurhqr.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3adatrrsr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3rjmpfjru.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3rlmmzaud.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3sdqbggnb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ocgfijag.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3yvvpdono.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3uejpcord.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3uoncebwf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3tmagnvou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxcfkoge.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ncfhlcap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fenvzykj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3hgdtognw.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xnwbttoh.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3rdcgjwqs.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hmcxrlbj.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3enhpyycf.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3kamggyyy.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3uyrlqjan.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ueezywfe.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3odvhlmoo.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bnqvdjqu.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3euwveagz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3kpfgaxpt.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3oylezlmi.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ufmacwwu.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cciihrqo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3itieajbu.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3kcmemhwf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gxiuyrfx.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3soygaodr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3osfxekek.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3bqpynxsa.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3venyvhzb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vrlakqyy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3vezcmqrt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3fmhxossd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3spviiwjs.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3rodavrnm.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3zxmxgojz.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qregtbis.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3olnpedpa.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wlrhlvek.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3twdzeyxp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3pdcpzlpy.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xjtmiush.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3hvwvjnrk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3gbeitobw.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3shxwyfqo.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wprplohp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3imoxoizz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tzdmxzuf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bihznwtn.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bhiaopyh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yqmylzfc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3cpldgxwk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3rjdknxkj.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3onooaxzu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xvbroqry.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3fbsreqxf.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zrtbdalx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xttvbovb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3tqdfuiot.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3jsszxunj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ngvjkvnk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3llfdhnir.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3tkehkskk.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3qgsrilew.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3cumleffq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3uuinmfed.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wjacaquz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3deavyfqn.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3srvpqniw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ffhnbdlk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3uhhdjqpr.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3jgbhoznx.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3skmuoiio.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3kqucgzmr.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nvenxkzz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3tuopmxsj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3kzpxiudc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3njfabcmb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ydwtyuvl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ptleymhf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wlnmlcvc.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3rynqnxzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wmknipga.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3pouidrsx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qvdifqdv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3krcmpfwv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xioktveo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3oduytymn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pcgrwykr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yicfhize.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3latghixe.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pgbtafme.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3apobvfhh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3doisjnzq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3zwaurczd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3aksntqlq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rovvzyuc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3peollgjc.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ronwksnm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jxcycaue.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3zdjplzax.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3plmkiugy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3hpysbyaj.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3paktlxvd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3wvexakwh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3roeulxhz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3vipgnjzw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3hxxlolcy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3kxzhhmzp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3dtybuoql.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3uvppzgyk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3cjcigwoq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3aklrwnve.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gylqvwna.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pbnzsdpb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3cjhhkxzl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3qhgamull.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xazjmulu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pnnxyitm.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3vwlgkmqp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vntzrtrb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvdjwfzx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3cubvknrc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gooxkwgo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3kfncnzud.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3uflaufex.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rhadasvs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3xdzbzcma.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3uimexudn.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ohtfbzia.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eksklyhu.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zjdweexl.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qxsdeezl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3lpnxhqfz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3dwjbvthd.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3camopqkc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3clhxyfwv.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3vcqrtsei.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3jdbnkluz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3nxjanwiu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ykujvgfg.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ibpuxyct.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3dhifoaff.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3cbcjepme.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3mapiqwhh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3bdwbmaba.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3cxnyiohr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3tbqhxpoj.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3hrdldzec.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3laogcljp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3klasybrw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gqyoutln.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ngzgttmm.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xomwmrpo.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3svgnzslv.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3kjptxokl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3iffwymvi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3audkrndz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xkvibfxm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3yzymspot.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3hpztswkh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3oqrmpbqh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mhvguaed.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3sjsnoihs.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3awfrwtsb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3vunnvasu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3piffbngy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3utavfcqu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3cvcpuldd.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwjnjlvl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3oswfyoaq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3gjokzbvn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdsltsft.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kkhhrnwi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3hbdijqho.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3diedrhwt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3lasvttvm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3uisnagac.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3syirrqmy.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mudsnqdu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ockkxfgx.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jehoxnfs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3xppqzevr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3stbosbqf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3qynzjcby.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3antoaref.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3xheugofs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qztnpdgg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3kquzjnue.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3cbdawgzc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3kluhsscp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nwexdyxj.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3mzaouoov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vfvxeumd.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3wtusacwb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3wcfrjbcs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3jrpkgokl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3gfqjzfgb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3nnpjyduh.html


<!-- 参考信息 -->