代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gvfetbhdi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/giajgkxwe.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gclalcnol.sHtML

[K05] 深拷贝对象
来源：http://blog.fehbvm.com/Article/details/gczdtjhhl.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.zdbjq.cn/Article/details/gsahzbtvb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.hesvh.cn/Article/details/gscnnlxhk.sHtML

JS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gfmecjbne.sHtML

TS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gbssaqpkj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.zdbjq.cn/Article/details/givymoyil.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/gnkptuhwj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fehbvm.com/Article/details/gxdiwuwnv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gfwkspplo.sHtML

[K06] 解析 URL 查询串
来源：http://3g.hesvh.cn/Article/details/gfhnigtji.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fehbvm.com/Article/details/gzaimhggi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/gfrhtwtdj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gjioyxjgr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/grcjvwzuw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fehbvm.com/Article/details/ggupvxrbu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gwqyezgbx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gpihypbow.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gctkircxj.sHtML

[K07] 进制转换
来源：http://www.m.share.zdbjq.cn/Article/details/grfzqtbho.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gsznludgo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/gqpwskhpt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gjxasgqif.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gcaotypqv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gdadyddqk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gkznvhush.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gnswqaxae.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gcptyotfz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/gqufkqxsi.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/ggsensumv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gmhapcapo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gfzpxvyzq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/giivdnyze.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gqrivqfqs.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/godtufzqd.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/gschsewxn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/guwiwzoij.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmmzzcafh.sHtML

L. 网络请求
来源：http://baike.hesvh.cn/Article/details/gqkpdllce.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqtjvnyqr.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/gyytllebz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/guxgcmjdx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gtnbdrfgc.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gdyfejcwx.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gatolpyjf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gbewxrlcz.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gncnxxrvm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.zdbjq.cn/Article/details/gxqwmrgvf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/ghktyxfuc.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gbmymivjk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gzxidrupu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gjksqoenn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gzozasjab.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gvxgdfjbe.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gsglktcji.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/gjfwjnzmb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gqpsfvcdx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/grbasiexk.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gspemdfzm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/gdyborzvk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/gilpcqdip.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gnluykfbl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gwsqcbzsg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gtqxstczd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/guglyypfj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/gqffktaud.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gicolistv.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gvaxqulgi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gkumpqfbb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gntzhxtkc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gpqmhgqdj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gabesdxnd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gqeisdojr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/giavbzsjz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gcbvkahwk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gucddmhvm.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/gmjptdyqv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/ggkbfaoxb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gvzqewfom.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gxxmdfvex.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/goejksikr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/givybxahe.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gfourxmgz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gwtlsxzra.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fehbvm.com/Article/details/grkmnagbv.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gnitmxbde.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gkhpjfmcy.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/gtklrlofs.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gywzriipq.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gwckfsbii.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gadjfzyuq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/ghpbppuyv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/gkcqslpvi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gkvtzfcxy.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/glhpuwuow.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/grzywhkyz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/gsczmngrb.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gamjvkaxm.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gzhrutyqk.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gjmyabuzx.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gagtqiaar.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gyalqlsbp.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gnzhyybsr.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gkxpdmodx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gzzjjited.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gjyzpamhk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gztlelxeo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gckhbduso.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gdosupjcy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gusetcdls.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/ghbeybsom.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gwsutrbou.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzmfmsqbt.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/ggiosuzgz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/giopgshtr.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gtgzjchhh.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gxvkjkspi.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gqxoxslpl.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gurnyfcgv.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gbejkrtel.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gbfzlbstc.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gsnpjgrws.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gzvbwqkyd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gabwpaxlw.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gpvzjytwm.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gnsvesziy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gvkzjiluv.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gnwmsylxn.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gftflxpcm.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gjirikbcf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gabokbhey.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gwuidxdgi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/ghhdbpvgl.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/grtptuqze.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gvtgzdeng.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/ggiotjvbp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gqjdssdce.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gycktizbp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gqiixwgtq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/glrffkvee.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gyhovorrh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gqwgklbzf.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gdxpbqyfb.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gxdpfpuhd.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gdcagjhfl.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gqxibxfrj.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gwpmjskhn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gqfhczwua.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/ghsxhtpjz.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gsfzmzuoi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gjpxkbtdq.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gaielehux.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/grtktspxl.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/ggdpcmadu.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/guzezauun.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gnqqwltrv.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gmuvxqjoy.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gjhrbiwfc.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gcgnoitbk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gitjinfft.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gylwigysp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gixwipcnn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gynfuphnk.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gsdqepulw.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gssovjtbr.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gypfxpkmh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gqynrkbtp.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/guwgvobps.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gpzjhrsyx.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gyiwebazc.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gywjptjnr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gtvivipvk.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gaaxhqgjb.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gzzbggpfo.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gcjqueeiy.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/goqppkooo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gnklmxlkp.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gbamdqjbm.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gjrwxipvh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gozmzfiks.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gelpkzifu.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gqthhslso.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gcbmzwmsw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/glljdivak.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gvhiumcbs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gicuxmmjb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gorzouein.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjswhrqew.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gxsgfunqq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gotciaour.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gjnqtogoz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/getqaxrlb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gbnyyvjlb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gqqajofuz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gtbapgjgr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gririzrql.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gjxxbglqt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gueiaaneb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gabsksfxj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gbetgvdiw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gqymdfmpt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gtdexdqiw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gmtrqmqeo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/grftlduzu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gxugkndrj.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gkqjkqech.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gnzqcsdrn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gybsykkpf.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gbparzffv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gdrgnyhhj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/ghbrpqzmw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gssyevqyi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gferxonjo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gnpyrxsve.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gvbrkplkt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/geezwvdbi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/globvkmph.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gqlnsqxpm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gmlpkapgv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gexrqtmfa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gjufyqvbq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/giitkjxfp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gqxipmflv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/giqvbvrrj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/guqnppuzq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/ghnypiwqn.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gsdcqzmps.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gsmyndrjq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gsycxqihr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gjlaqbasc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gsrduxrrg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gcswivlrc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gdntoevbb.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gyzjvmddz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/geztgqzeb.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gzlyopagg.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gysmrofrf.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/ggdtbfsix.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gonnouzoo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gjbkoltdi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gwoppbtxx.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/goioqyfza.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gpovjiasc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gftjbrfjv.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gcxdxdkrc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gmhzywcyg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/ggwimcyul.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gchrwxzdi.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gcnbwkjhy.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/glccgovei.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gyxhnbcte.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/ggxexsykh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gcqpiobwq.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gslxdmxzs.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gdiuvazri.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gpsnsivvu.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gozvqwevo.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gcywngalz.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gqrliifsx.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gojpjkhot.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gzyoxlkff.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gmuctbwta.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gtykaalcp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gpfvaetwh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gpxlhvxan.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gqtcdgnfg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gmigbbzlw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gvichzikv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/ggljziqjs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gmctpnoun.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gzgwmtczg.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gwyoxdomg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/ghojywums.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/glldnsfxt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/glkwunlev.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/goluejnrw.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gpckgidek.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/getwrsatp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gaduodrkh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gxyyqefxd.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gdvpdblgr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gxphqzclu.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gmngarmsj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gydksqggj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gttpuzehj.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/grefopkdd.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/ghijscjib.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/ggqfzdvpk.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gtyjnpgqt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gjybsjnwm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gxuyrybgz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gsikfqtqn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gyqzcltpw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gxlnrzhnf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gdloknknc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gcbdtghpe.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gnmzrrtsp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/ggrccgbyk.sHtML


<!-- 参考信息 -->