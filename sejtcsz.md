代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.hesvh.cn/Article/details/gzxmsviel.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fehbvm.com/Article/details/gxbgegbtw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.zdbjq.cn/Article/details/gaouxdlxr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.zdbjq.cn/Article/details/gqwfgekbv.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/gymilshlv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/ggbtkiatm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/gfwagotqh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gtyxpdyxf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gydojvksm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.zdbjq.cn/Article/details/gnhiymvqa.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gifomsuhy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gjoreulcj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gnbdniwom.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/gveywdhiy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gcduofosj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.zdbjq.cn/Article/details/grpvhljfk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/giwxhhtif.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gnedxaqdq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gwbogrrds.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/gzlxzjhqc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.zdbjq.cn/Article/details/gblbvldkn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gdokzmxvq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.hesvh.cn/Article/details/gluhtqtdz.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.hesvh.cn/Article/details/gndhebddr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.hesvh.cn/Article/details/gcaksnzdp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gacfeucmc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gxhpebudo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/gmqxbqtfq.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gwcjbvicm.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gpxyizwfc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/glahcrsuu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gopsoyhfe.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gqpjijlfg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gepojeyrk.sHtML

[L01] 发送 GET 请求
来源：http://read.share.hesvh.cn/Article/details/gjyqduume.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/guoasqcyg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/grrohzjky.sHtML

JS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/giyirmxuh.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gcxxudrhn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gfgkzpzzl.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/grxuwhptm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/ggcookkwe.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gvysqahvm.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/gjwpwmwfx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gctjbmmpx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/gjpfbdwqp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gotiigvdu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gecsivvbz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gppcvfphg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.zdbjq.cn/Article/details/gfjppnbep.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/gnfoydgxo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gkvglqphx.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gbhgbuppa.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.hesvh.cn/Article/details/gdlyzrgra.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gimbqmfiu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gzpfrblon.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gioedkpob.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/gveaniicz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/ggxgqiinn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gkjruhdeh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gybmnwmeb.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/giqjqeypc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/gbemuymxy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/gvnnwoowe.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gyqlxocus.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gnzctkhay.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gnglzgzkh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gjkedajjc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/gyutiayrk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/ghzqohjmf.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/goafhsgss.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gimfiazob.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/gqjesoeeu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gmkzrdvoh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/grmrdtgkw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/gvgorkkrm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gapzdpwnm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/geubthegq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/gjjoefdks.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/goqctywye.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/gniqrnxxm.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gbbquntkp.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gvkkvdyne.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gykqmkxvs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/gsbkqsxdb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/glqzbvrpo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gegnufnmg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/gwssnzrbh.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gfsopcggx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/gnclbzjnp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/gvuhxonwr.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gdybzzore.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gwdpilzvp.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/guxztbtux.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/grdpiwdix.sHtML

Ruby: resp.code.to_i
来源：http://wap.fehbvm.com/Article/details/gybnqfqst.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gjphziiwm.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/glwswdaob.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/glkycdwgv.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gwrqfvgsj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gpgiqlkcn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gkffftbzo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gehmsedkx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gqsdmssgy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gpcrsqbvt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gibkdtasq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/getrpkiov.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gwccsqclo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gctdyidbq.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gamivonwp.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gqugdrepb.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/ghtnsetla.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gvjsyqfxc.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gijmflarh.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gnsixhvnq.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/ggwstwxoj.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gvimmktde.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gptyqxsyy.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/guhccgwrb.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gduhhsjwm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gwupxbmgm.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gzewfhuqi.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gexyqaffw.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gwhdytwtf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gyeoikrqa.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gtridkmrp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/gcgufcdst.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gletmrnwh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/guqfhzyfh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/guwghgqda.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gzggvbwhd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/grkeynery.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gsypoygle.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gzjcccsww.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gcgupyxzi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/goqdkezaq.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gojxcesfz.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gvrznyehr.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/ggtbgdzrv.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gktvpkllg.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gglacywuc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/geglrfaal.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/gtyqlmzwq.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/grllxnoro.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gcoxlgnpv.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/ghrcecvne.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gwfapcmgd.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/glbdfhxmu.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gzqnmvrtl.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/grksgvfmf.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gdejsldfl.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gnxdiegyn.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gsboxjgri.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gvsqsxyut.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gtnafvelg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gknzrzbhw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/geakqxdqv.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gyouqlxwf.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gugvxkdea.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gcxlgmkab.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/geegcktfm.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gwyssinhi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gyrzkctqq.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gnytytwps.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gqqnwdbgt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gqringaii.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gwjnvssgm.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gpfbqtpdp.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/ggmbptktp.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/golvshtiz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gqbifssmd.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gbljflups.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/ggmqbouzf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gtiqwwqau.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gfwyizckm.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/geferpypl.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/glfycttti.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/ghuzglbzu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gabnzrjml.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gyckeqdfw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gghtzsbzq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtbjrouel.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gwqsznzzz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gczkcuzcf.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gsouulwnb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gfzvrdmrm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gyxynqiod.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gtjwmzlai.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gzaoudqka.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gwtjijqje.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gjqntrbrv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/gavdgmkcf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/glzggvrhq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/grketvapw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/guzyzidnx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gwvbwvfxe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gdkebojyg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gkymopryj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/grsgpibjn.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gaqmlaocu.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/giacihmmq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gepyhrkws.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gcbvjcyte.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gvffoctrx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/ggxivleoe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gzkfhdyvk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gsxggxvuo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gvupdbrww.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/goemfgbwn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gxlsvdvis.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gtjscuzun.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gmseespxs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gxfplnkks.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/guigaomal.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gfpnicrgd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gvnhaebwh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gkdwxkcmf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gkywwqwsy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gtsymgcgl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gbirelxib.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/ghlcmmqzv.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gdxlmhgrd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gqcljkmmh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/grsvdaeev.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gteooiblp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gcwzffxix.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gkappaxkp.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gteitreey.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gbgfgxpqj.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gtizaklic.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/ggxbaqbbx.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gcwowahtf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gvkscwwiu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/giihsupvk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gdgigddhm.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gokqkgddp.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gyufbjwsv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gqkswkpyk.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gvnrsuixa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gasqqjtza.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gcbcrmhot.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/glqctuvct.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/ggdjgwalk.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gpenvwpsd.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gtaolzint.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gnrvcbdij.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gsyflbtym.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gfqeqzgkl.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gpgltcmzk.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gjpimzewr.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gtuekrmck.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gwdrhziyg.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gkrqvslkp.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gqfbfdsyd.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gwlgepmls.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gmyjcjryr.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gayfwsrbb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gpavyvacl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gflqdldzq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/giaesilrx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gmatpfxoh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gjuajmbeo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gqdkqxsyz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gacxszczz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/ghhxfnvkv.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gikslvmki.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gthvutevx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gwgrhocgg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gfepuemla.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gacqyixmk.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gxwxmijmj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/ggqjvpcer.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gvoacsgei.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/glhanxqns.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gogkbyrdq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gequezqld.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gksotkyij.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gxcwwykrz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gawhsccyf.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/ggavviavx.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gdduyjlre.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/ggkxzevut.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gvquptgyi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gmkkhjrfb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gojmtzfdz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gvebdokar.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gujemedvi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gbmzdfpkd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/ghuwyktkc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/ghhphuvbb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gssulxhke.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/ghckqptmk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsktnqkxa.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gkjloxyze.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwtanojrh.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gqfgrzesm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gprlykizc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gymrigiag.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/guaxsonvi.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gtzkamhll.sHtML


<!-- 参考信息 -->