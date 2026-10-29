代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://blog.fehbvm.com/Article/details/gqbcknaxe.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.hesvh.cn/Article/details/ggglkxmbw.sHtML

JS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gtsjrgnxw.sHtML

TS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gdhbtnnyn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.hesvh.cn/Article/details/gbmsjobnb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fehbvm.com/Article/details/ggofnotzx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/gquodbstm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gorpiepei.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gmjayjmwv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gtfvildgg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.zdbjq.cn/Article/details/gnehxjzpy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gyumptnjm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/grzsjutkv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fehbvm.com/Article/details/gewwgaupc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gexagcfbm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/ggkzazndb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gpxfjnwcl.sHtML

[K07] 进制转换
来源：http://baike.zdbjq.cn/Article/details/ghwqoqwyq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gbgqaynxe.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/glmofwsma.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gybonpdgh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/ghrlthnzh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gnrcepdpy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gxgxqknxw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/gpjvwxaly.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gcurdbhgb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/gjtvmmkup.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gjqkecxba.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/gyhglxphl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gydxloajp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/grjqzicjy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.hesvh.cn/Article/details/gxyfinmkm.sHtML

Go:   encoding/gob
来源：http://mobile.fehbvm.com/Article/details/gwmjardca.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gljtfgzrq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gmkbtzxrt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwejrakqj.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/glsezcktm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glfcoznqw.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fehbvm.com/Article/details/gqubalhdw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gcxnkbjne.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/gfciusrqi.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/guiybakly.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gjwxonyrg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gemiteaej.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.hesvh.cn/Article/details/gxcxeiauw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.zdbjq.cn/Article/details/ggvfrarod.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/guhtmyhwt.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/givluskwj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/grdkapuzf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gxgrsxovx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gfztnunil.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gpyxrydcc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/ghgggscum.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gpovsxqxa.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gwruhdvqc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/gqlwyhqqa.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gisvoreaq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gkjyswunb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gzvydykbt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gprtzfuvf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gwnujhwlx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/gfqacessv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/glonteess.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gewufpmev.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/guoxwrqaj.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/ggeylwzvy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/gjvxtdqxu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gxbsgbclq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/ggpmaqwsn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gdeyiexxm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.zdbjq.cn/Article/details/gfysrwbda.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gakswpihw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gbyoebzgi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gwojlcklq.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/gzngfcphx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gqkueddkn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/gnrlzftow.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/giqsiptrk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gjzjthwoz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/ghilhhypz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gpyfeyaow.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/gklpuvtwy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gahhrxjbl.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gcwgkcaql.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gxktfbyso.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/gahnggxls.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gbnompdmm.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gjruexcjl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/grcwucwcz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gupcmyxug.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gfqlbuoxq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/ghurlqjdl.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gsxsxvlii.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gdjakihnn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/grnxhwrjt.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gzxvgeqyi.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gdsbtdmno.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gnyfwuicn.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gbmutgbue.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/guttchnep.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gqjqnukho.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gnukrkkfc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gdmifacta.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gpiccswkp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/geulikwxb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gkkfcvtcz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gdlxnbonk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/gjusgpzap.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gsdmwuifd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gpfqgjhon.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxithbpqk.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/ggfthykrp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxtnqzecx.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gvracbiaw.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gcyqibtng.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gjqzubanr.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gwffeztnd.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/giasjhxlb.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gisnvwkld.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/ghkoouvfk.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gwhvheefz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/ggscsmwbq.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gbqelefhf.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gbwmlemmb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gmjrowvtf.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gxfldjtpb.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/ggpgvzpef.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gosieuguw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gmwmzzesn.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/goinyfxvv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gtsjchmew.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/geolqmhap.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gkrozdjkx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/glzztkvwb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gmlzginca.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gtvtywhcd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gevtimbae.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gybcegnto.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/gfaeqwpkh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gzedrphqh.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gfztmnrlt.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gxzdggtqo.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gralypwes.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gsvpkkxyp.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gejvmiusz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/guxvvcibf.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gmnkgvcbf.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/glbspkydb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gwakaytds.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gfikabzec.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/giozcczsj.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gorvtxddr.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/grmimdatv.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjihyhndy.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gyusgakes.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/geeyyoakp.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gruwctvcs.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gepjwqbcc.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gihxlmkdi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gexzdqfuq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gckfikzvu.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gloihpqns.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gwdzpwbux.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gxgutqkvj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gocxreppw.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gqliboyko.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gfoouswqq.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gqsyquxtq.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gypokieim.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/glrxfmojf.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gkfmfhzvu.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gpzzardyx.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gyxatramd.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/geaiwyskm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gmnfinuez.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gnvwrooja.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gijxbkxll.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gkwgdzgct.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gobdwchso.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gpkdjutat.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gkfjqlzkv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gqkxfqwcw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gbunlbjry.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gjellhabw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gaxzjwcfu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gypgvigzb.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gpiwbwpaq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gshgpglqi.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gcerwxqie.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gzrslvees.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gledmrkdr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gycjpinqm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gapmroxrg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gvtcmfapn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gxtlwmkca.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/ghyecalsy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gnkriwier.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gztfxiahy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gzvsljati.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gacswrnli.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gtessdzsi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gylrvvhjz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gqbpscuxq.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gdnuypzwd.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gwsjeigse.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gltjleoll.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/gokzffsam.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gyjxmxcga.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gsgpubwyg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gdsxklksx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/glgprhhtg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gqeivinqq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gukkyfluj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gicrtylrb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gmpegxsep.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/ghtxachmw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gfptkxnjz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gziaskmbh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gxlupliml.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gzbpjfykg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gfyubmhif.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/goitwpppo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gudrkrsgn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gqvfyzcqc.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/ghccoujlr.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/ggcywxrer.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/ggkqdkfgp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gomgawidu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gzevdpmke.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gpppwxcsp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gqkwdqnfw.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gwtrisapl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gspvwtbza.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gamoobgwy.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/galiqtqtv.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gfciztxru.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gyujvetuh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gfoxybpmj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gxtkkipmn.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gykqpkzpi.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gycgpfonj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gdfpmuzko.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gcemtngnn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gbgauuyvq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/ggdamdlva.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/grqbgikuo.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gxzeetwxs.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gbgtykpxf.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gbwhgbnps.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gnfcvojdu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/grnluolyl.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/glimjlbrb.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/grirvjkfl.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gwfbdcian.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gtsxampzv.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gfshdzdxm.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gaghuwgxz.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/ggroqpula.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/grnuskhzl.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gkwjfhbke.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/geckspcek.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/goqikqfdj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gtujuetlz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gywapyhki.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gcfghoxuo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gecttjgpm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gsgflwgtb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gtmfhyxep.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gipppeajp.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gihoekkkh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gbvsxntwg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/guqnmcbhq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gkdwgpbzh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gommegkbb.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gdiodteqd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gyavbudhz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gmcmqwbsj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/golerdugd.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/giemvadcr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/glnhsfprb.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gnndjeotd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/ggqveeqfy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gwdduqgbv.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gkjartqma.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gdyectxoy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gmqikuaat.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/glklayvoi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gynhcuurc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gcbbrfnlt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gphlwbbgr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/ggrrkbxwr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gjofqjyrk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gatgxrpzr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gtrkgbtcf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/giqqqgkvd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gsbzniexu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzsmyswci.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/goxederih.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glddyfrpd.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gkcvqajdu.sHtML


<!-- 参考信息 -->