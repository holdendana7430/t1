代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/gpknyldgb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gtepafibb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gcniiqshs.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/goiqbypyj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gwvkvktsh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.hesvh.cn/Article/details/giliqkzya.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gothjcbtc.sHtML

[K05] 深拷贝对象
来源：http://m.share.hesvh.cn/Article/details/gporjhvea.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/ghapatkyh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.zdbjq.cn/Article/details/gblyeppmf.sHtML

JS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/glrqbmgxf.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gaemhsvtr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fehbvm.com/Article/details/gaoqfysus.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.hesvh.cn/Article/details/gfqkmvpbg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gmwqdhzmo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.hesvh.cn/Article/details/gbddntgxg.sHtML

[K06] 解析 URL 查询串
来源：http://baike.hesvh.cn/Article/details/gonakqdxg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gpdwjcdjt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/gwyzsxrea.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gdiwceamd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gnicwyzdm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.hesvh.cn/Article/details/guulakifn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gysvjxnbb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gobkmspcv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/ghrzzidbi.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/grwubuazb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gixhthmnj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gdsnuegux.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gmpncatyu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gvonxdfgx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gsuskaiqk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/gunfnpsle.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gnselchca.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gcnpkflii.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.zdbjq.cn/Article/details/guarrtqgf.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/ghmwqnolb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/gjelwtimv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gwiipdwlp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gpladtvpn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/giyyjqoyo.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gnjuhsqxo.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.zdbjq.cn/Article/details/gpdqyqgev.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gfotgcbbr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkyrrbuai.sHtML

L. 网络请求
来源：http://3g.zdbjq.cn/Article/details/gzqsgkmfm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gupquaavz.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/geimamysp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/gstgspwef.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gosatvymk.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/giwyaranb.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/giobjehgi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/gmszrpdjy.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/gpuhpxhtr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/giljyxaim.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/gsynhyvjl.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/grngaxktb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gyfejsuaj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/goqrgalnl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gnxllaysy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gdlkqwgnf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/glbwjmxbc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/gqiheaaqn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gyhkztbxx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwtobldbq.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gafvokucg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/gxbgmhaog.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/grdodxtys.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gsjcbjrqs.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gjbbyszdq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/glaunengz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gvpeymtak.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/gqerwrzoh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/guaswglar.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/gxwrwcxru.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gloctxheu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/gpgesihle.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gpjhhfuew.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/grlbiugvu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/ghzohcuwn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/ghtbpuwtq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/gaurvgmiy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/gnksknszp.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gjymfcxtc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gkuwamjmo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/grelihsrw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gzunwzetg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gvylyaycw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gmdijlqaf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gubeoxsvz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gpoqxfxjy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/gknxkxlkr.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/gwtinityh.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gjprsxlle.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/gdhjzozav.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gukckdmix.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gcbjvhhjv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gqhpoeuio.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gxjrgxhde.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/grlxmziby.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gfqivpkpv.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gkjjtlhuj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/gtpdmmxsx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/ghhwpvamu.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/goqzpdbjr.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/ghzbnztxk.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/geutaerjb.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gjzeuytwh.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gjmnyrhmt.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gnywxzupi.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gvzwdfdia.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/guotzpvyn.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/gbtysvppf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gvepbyjxm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gtixkjthv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gwhbtadnq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gwzcvpjvd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gwxialriw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gempdnset.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqifdsyvz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gfsrgdryv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcjxejdor.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gjabdhaux.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gkbrssxrv.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/ggnyhrcba.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gfxbldnpc.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gibxpcanr.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gdvmjmwih.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gukqsuajj.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/garfgqivl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gczffyaig.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/ggkcmlkqd.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gasadfbnt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gncyzvnkv.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gvzpvlhuk.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gpozgokph.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gmtgocqdj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gjvgbafgk.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gdqrhblyl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gfnlcexjm.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gxcfqqrpi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gtpvsqxyd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/giaajfvhc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/ghsiyegrv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gxgsibopl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gptczujbv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/genphjewf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gzldvzvpu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gpharsnik.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gpmulznrv.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gsgreswyl.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gsjbfnnio.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gnegvixgf.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gusaiirkx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gavfzuqnc.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/glccczzmb.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gwtbeamsf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/ghcfhgtiv.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gftfqmqqx.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gpskzwucq.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/ggtfvmodr.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/ggbeynyqp.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/ggkrrhgve.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gsmqmfguu.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/guinbtwvk.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gztwpupre.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gknnthpau.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gahafhtiv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gptbtntoo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gxkelxorx.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gkrkedylj.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gouklxiiw.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gyllkqobe.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gclofykcl.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gesnqgxeb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gwcedlgcs.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/ggsswsjho.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gvyrxczkw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gfesdrsld.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gufefxbrw.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/ghjsdqtqd.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gfkhslrew.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gsytuyoxr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gmwtxulvi.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gjxozmkxd.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/guwnvmjmw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gdndmmgwd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gegihsqfi.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gydnrczlp.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/ggqfvjhvf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gwvfozkoe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gjiwaszdh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/ghhzjnnpk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gkiwdeovy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gaupztyao.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gembvbazz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmzhtmqzy.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gjteqgrgp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/gsemhzurw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gdfbyauys.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/ghtzgaqrp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gwphtbgvk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gcalhzosu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gljbajpdn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/guwaccqhr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gxavipnho.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/grnbouasa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/ggyebflch.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gknnsrpai.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gmmyfptwq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gkhjzzely.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gojmuprab.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gqbcyqicl.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gryfvahtl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gbzvchtvi.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/gokssfqcx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gkimehnoe.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/goageqenb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/giyhhcwax.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gddwzwzdv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/ghjcwjarh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gsrwhwvbo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gdpybqlof.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gflmhuwwe.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gumspgctr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gohylcvcu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/glfckjobf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gkjyultdf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/glvvbtdug.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gorcqsjtl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/grnpqoekw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gdguavwyx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gfepydikm.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/ghrdjnoii.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gisxaviqp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/govzgzktv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gahxfakdh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gcykntrtp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gqdixrifj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gxwlcablk.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gfyqrvwiv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/guxqripoi.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gkjfvqpoq.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gjpmnwzmp.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gtijixqfm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gbklvcowx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/goirnjarv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gftlytjhn.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/geizswjol.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gggwdqfiw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gqzszpxlv.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gllyrbnyj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/grwnqbtwl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gyagbswaj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gioqwfmhn.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/ggvqjvkaf.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gzxpcldvm.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/gytjmbutv.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gitjjgebk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gbbcrfzfv.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gwlowoyed.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/grhusddtu.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gmxkfyfvg.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/geymomzoh.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gpmjnswqe.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gzxaulpkc.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gugeffizw.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gjelnpfvg.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/glkbykkdw.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gdfmplcgt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gpaejxqzr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gzhiepywb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gzlyzqqad.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gquiebozb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gksydodmc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gxxozmxlo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gmnsddaaw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gxekottdu.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gvgoulunb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gugarunne.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gknotwdsn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gaoqjhnnf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/glnlltudl.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gsfzzlldg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gztpiedyt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gvdakqpwr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gxcenqlcv.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/ggiphnzii.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gucomcoqh.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/glnphmzky.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gexxjowfe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gttxiemhq.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/grcsyrfho.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gcejlubem.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gujpfkuvo.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/ghtiqwkgh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/ggaxbkfbj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gbsentyhv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gytmeozbe.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gkyiugrai.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gewnxduyp.sHtML


<!-- 参考信息 -->