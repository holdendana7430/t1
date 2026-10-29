代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/ggwbnxums.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.hesvh.cn/Article/details/gkmmenqni.sHtML

JS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gilebrgkx.sHtML

TS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gthykbczb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.hesvh.cn/Article/details/gjokcupdu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fehbvm.com/Article/details/gzkmxmwqq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.zdbjq.cn/Article/details/gdvahyuob.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gbzvyruoi.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.hesvh.cn/Article/details/gtxrvesnv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gmskkgwdg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/ggdpgromg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/glvclmeqb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gwipdnqaj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/gjdjeiwgq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gtyhooass.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/ggvdbqqvd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/ghxvmeoxl.sHtML

[K07] 进制转换
来源：http://www.m.share.hesvh.cn/Article/details/ghosxwfao.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gmziyvpyq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fehbvm.com/Article/details/gmutqsrxf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/grbllqgyi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gdcwrmgcx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gsijkpvca.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.hesvh.cn/Article/details/gcadlcxlr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.hesvh.cn/Article/details/ggsmmsolf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gzmvpeooy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.zdbjq.cn/Article/details/gkaknmgiu.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/gwezrqysf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/gxhkywbze.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/ghxqmjasw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/glivgjfzt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.zdbjq.cn/Article/details/giljmgczh.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gkqyvqyay.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gvsmagwvh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gyomjnwpc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbradueih.sHtML

L. 网络请求
来源：http://mobile.zdbjq.cn/Article/details/grafbndxv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfuzyppzs.sHtML

[L01] 发送 GET 请求
来源：http://3g.fehbvm.com/Article/details/gpuutprft.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fehbvm.com/Article/details/gqqckoepl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/gtbfforcq.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gqkdlnldz.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gzlcbwjln.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gsdallhwy.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/gppdyivgq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gghiuakjy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.zdbjq.cn/Article/details/guoasdnhp.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gggkscxtg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/gdohommaw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/ghiwkttbw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gmhbrkwbn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/geonjuyms.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/gjhquxaik.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gaggywojf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/gvucslgpq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gzcaaujvc.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gykyiojmx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gjhlbclju.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/gzreizzhg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gfthvtzcx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gulrxvjkh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/gyghzisax.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gfjexvfev.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gpvhjngjf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gxogsqrpd.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gvyohaafe.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gmdsvxwmf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gjmjicexx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gcknrmsom.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gbinjelyl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/gqquigpds.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gherxnasc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/gulpbdavu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/gbqmqclne.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gnrwqrftx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/gudiflawe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gjaxpohco.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/goavnzbvp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gucrzrgmb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/groplbgry.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/geqsoaqzq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/ggxtlsmmv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/goaoemykk.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/gvbismbnw.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gzncwmuhx.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gejdbumxa.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gmidlelfy.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gvafkensk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gccervudz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/ggfudvymx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gkpoqayzd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/gazruariz.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gbvuketqp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gkixeourp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/getexyepq.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/ghiimuozm.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gxbjwoeco.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gxtooskit.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gohkedfgz.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gclqgprga.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/grnhxnzkk.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gngzjwyie.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.zdbjq.cn/Article/details/gbwgzrlai.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/gdwlxdjve.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gdvnjavqr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gkcwyqlup.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/girweaasb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gspxqhnkb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gyhazkecu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gjroiauad.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjkiyxpwo.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/grdvduate.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsmfhylpm.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gviugqejb.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/glufepqbc.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gvhwbgkda.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gaxdgcnbv.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/ggeeqqkfd.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gqewsreww.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gubfdmbjp.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gilkvcvdd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gwunuhsnw.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gkbuvbxdt.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gdhrmfbrw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/geblfsyor.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gsbsimhbk.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gwcsmxqbs.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gfkoxpksa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gvnzpuqjr.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gllbpyfzk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gecowesye.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gpvpdoxsd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gqyyuldaz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/ggbaqxlto.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gtdqyjhqu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gzyilcwcf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gfcsxfrfx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gipsthrhc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gvnzvtxwv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gyxfnlikv.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/galktkted.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gkgjwxstm.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gqqvsvpxv.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gzafggjqy.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gacloaghu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gippnahvb.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gvjbzyhid.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gecstllqk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/ghaiupsqh.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gtpjrqtvm.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/goqicfody.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gjqyxivay.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gioethaac.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/guyzyjadj.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gnvgnwuvy.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/glwunczqd.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gmqdomgfg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gzmoraadv.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gpqfmxzyg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gjyyiwajf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gbwgpabbu.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gtjizgsvt.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gvqdbsqiq.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gijwepsec.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gnzgvigdb.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gwruswili.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gpbszrlkm.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gtnakkues.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gpgonjdvc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gjvkebrjh.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gwdbfvlci.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/grddyevno.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/gcfwsjebq.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gnbmvbfth.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gzuyqhltr.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gcpsmwzph.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gppuvmndu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gxxajbydg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gjmvaldkr.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gizyrmzmz.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/grapgbrkq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gltzmwabz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gansxvoci.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gbltvmjyb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/goewcnksb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdywluiau.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gzjwujrhu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxxiqzxpk.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gvsoyvmqt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/guquadjsr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/ggylwykmy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/glufxgdpj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/glndndvzf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gouudfhxb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gddjjajuw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gyadjlaqw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gcvhenxku.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gygtzlvot.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gixqicsxw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gghdhycuk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gbwoztbne.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/glgczyoft.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gdmsmclsm.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gveqokeyo.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/goiqcsllg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/grkweoizv.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/golnwhpkb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/ggylitsvl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/ggnmzyyky.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gkydkfjfu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gtpumorwi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gfxtzrnrq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gvjapnezp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/ghijoopsg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gjdhwchpz.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gfjdgymxa.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gyizwlfpq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gndkyfpcg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gbcgvewcc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gvzrzljhf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gahfprysy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gfqnlbabk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/grdzhzkkq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gjkfvdmnm.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/gidjkxwjs.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gftgbxgdi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gqjicryld.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gtlsejloo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gptwgobbl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gklvuzqyw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gmncqpktu.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/geafnawye.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gawyfmkzv.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gcriryyqq.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gragvjpqb.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gvltdvwau.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gfkqslaqz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gufudvfxe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gfivmkgqd.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gwgvjhsls.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gkxxrplky.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gqqbwsstp.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gvvrfztwq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gsbaevjbv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gaskhbwwp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gfdhftyaz.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gyarjffpw.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gcexecbpc.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gzntqbqcs.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gbyskxmjk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gbxdkensn.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gyedivbrt.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gdkqcuoys.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/ghbutllht.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gijbrprqa.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gzibjubxj.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gwhnibnsj.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gnzinwgiq.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gcwozpfcw.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gtystqzlk.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gnbpfymja.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/grarpfixn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gutdjierm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gkarlszdv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/glizaumqt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gxlnarpie.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gcuidjokf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gbpncdpax.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gvihfmljy.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/ggiziyivv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gcdzzqpjv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gxmnmqdkk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/ghzcdjljq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gdbxemwxa.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gcfueinny.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/geisdmqke.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gugqnizni.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/ggqkvtmsg.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gjgbvmzlm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gtjuegmze.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gwgbekrnh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gvoexoxvw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gkuizufez.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gyvuzuaed.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gluhhoeib.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gaskoznvx.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gtyzphbwt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/ganiugbnn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gqebfzhjc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gomklrsiz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gqyeebctc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gebbaebeh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gmyigkjij.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gakdcbexc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gcwohxbuu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/ggrhfjmed.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gloojfdjb.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/geelnopfp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfjqcworn.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gsxrysdwd.sHtML


<!-- 参考信息 -->