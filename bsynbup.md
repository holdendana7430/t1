代发 wailian999

[K06] 解析 URL 查询串
来源：http://m.share.fehbvm.com/Article/details/ggspmkttl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.hesvh.cn/Article/details/gspixiuko.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fehbvm.com/Article/details/gmawnllxg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gklpixdhn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/geyspkfgl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/gcptndkhi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gxzrnkpab.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gtmzputta.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gkmzecilg.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/gemljvdwq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/goapygkna.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.zdbjq.cn/Article/details/ghnyfbdhv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gtbyrqffl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gmjikavhf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gzizxeszt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fehbvm.com/Article/details/gnnffimca.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/geiltywvw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gkpojcekk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gfkwhgmmw.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fehbvm.com/Article/details/gfyrjidpq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gbgsseqdf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/glhmpjpxl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gxvqpauhx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/gvydtobsn.sHtML

Go:   encoding/gob
来源：http://wap.zdbjq.cn/Article/details/ghefrwluz.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fehbvm.com/Article/details/gatsjpwmk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gxouwzxqc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkbrbyokj.sHtML

L. 网络请求
来源：http://baike.hesvh.cn/Article/details/gvheivehb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gckqlwypm.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/gbfvqdjbb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gmsfdnuai.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/graleeshm.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gardiiocz.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gsuufmjwk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gnpdtwtfs.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/ginthfibz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/gtycopdak.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/garypezqt.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gvahhvxyy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/gwobtkcko.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gevplqwoy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/ggsiffavc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gyfcdunjm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/gokipkyqo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/gbborkyjh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gvrkcyorx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/gvgfnibhn.sHtML

[L03] 设置自定义请求头
来源：http://blog.hesvh.cn/Article/details/gupqkyzrm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/gvhrzsndc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gmzbpwjnp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/goiasujpt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gkobpnnxq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gxdduaoli.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gjhvlhcwj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/gcgdcprwi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/geqtrztpg.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/gstguwccm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/gkzpvmszo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/gsznvloyk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gyrlzvxcv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gutjxtusm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gjqiyuwri.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/goxutvaio.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/grcchylht.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/ghmioeulq.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gtpimtjds.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/gthedrkdi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gqunwghiz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/ggtltfobz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gqeqthpxw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/gfbaxunig.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/gomhybryl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gzhktzxmt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gubvmqviq.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/gdclzyvxm.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gzdhvyijy.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gsszezggz.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gtseqewkj.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gzwxtptzu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gayblncko.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gkyqxlare.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/gjpwoxebw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/grsticbkl.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gaxsimizv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gwbcbibcq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/gbkcztqjj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gmzrrlgrc.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/grhlpdgdp.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gsvweftfx.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gqsduyzph.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/gktfybjtj.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gcqkqrtgk.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/gkwyfurrw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/gqmlgufka.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gybndoedf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gynaophoj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gxpksfoqy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gfshvovbb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/govlepjoo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gffawonuq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gmqcpejtb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggyesjack.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/gabqlrvyw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gextiewlo.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gaugvhjbc.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gedoyhgmt.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gzqyalrii.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gvolkensg.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/glkhhildj.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gawpddxfh.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gddahttqk.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gvmjpjrhx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gtokzfnrr.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gduowxdfz.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gebflfend.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gmywmflva.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/ggxrxaycf.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/geysduwco.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gfsekyzex.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gxcujtydg.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/geztiojpb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gxopplozt.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/ggctlqifc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/ghflkxnpd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gdfecntyw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gakziaxij.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gnzmpjldb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gfxiyltyv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/gshswwkyg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gatvxckbh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gsiwafglk.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gupiifblx.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/ggbjbebkp.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gibdbecbk.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gyeukmvpm.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gwsqybqzr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gqvmeezdp.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/grmkdacje.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gcjxvrcqb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gctzecycp.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gdntaozwi.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gdyqfruhy.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gpocwmbrz.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/greedmmka.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gznkxrovf.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gyojpzpup.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/ggwpieeqo.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gandigzjg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gkwgfuzfi.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/ggrrylthl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gwchoqmrh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gkwfsklua.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gftgiyqyr.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/ggjtasgze.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gcwbexdoz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gfyjtzakw.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gmkhuskgp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gizvournl.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gmwiihyzj.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gblvukvkr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gacsqrujn.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gbalmashv.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gzzxoteux.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gbtduinfg.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gikezvaac.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/grmxbmkza.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gogxfiknp.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gthvsjqyc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gbribwqir.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gwositjeu.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gtoivpwqi.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/geryarcwm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/guchcwtce.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gskqwacnr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gredddxkj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gsqxadqaw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtmnsgbzw.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gqjqytvrv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxdeqdihj.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/goqsfsvhv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gpzubyovv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gcxbeugrh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gaexufzdy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gjtyqmyac.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gzqfxwznn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/grskobmpm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gstmgduhi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gcaknbbmk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gdikvywqq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gvjmbdbqj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gqqfiujau.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/grfpwuhwe.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/golmafsml.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gadujgzwu.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/guiojxkqz.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gsxdwulao.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gsmsoespo.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/grcgmlxkh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gcjhlnzrv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gxwgdoejn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gfjwksmxu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gktmltlgp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gbxnpcvix.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gjiccedre.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gomvjljcj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gjzsytpsn.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gfvfdmaxb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gmtwxdpgy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gtjzfmzim.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gaputbikd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/glbobotou.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gqlhdtyky.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/grmxqjkmn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gaujmbjmv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gdrjtodwp.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gdxrzzrmy.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gzthfxxhx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gutxqdcti.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gntaovwwx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gkvnlhvgu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gevfhshzl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gjbyhuflz.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gorsnerrn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gqdghtqwu.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/geesakucn.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gissmuqre.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/ggkgobkfx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gmzdqgxio.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gzsjafnuv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/grsizhwna.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gkcefeavq.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gwgufxjxf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/ghnqywsfq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gqxxwiwyx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/grsxjkemw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gusqdoiqk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gufehawra.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/glqsmppxj.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gedozvlsx.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gqvvxpzti.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gngoduovz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gxkxinhns.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gzwozqpvf.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gkiutgjoz.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gvymbyhek.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gclicnbhf.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gljnzvftb.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gbkgyddbq.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gozdemezd.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gownzxadi.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gdzhjewfw.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gytfayjze.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/glmxuiawz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gumhkinfd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gavslavpy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gjgfkkcmy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gsltnnqsj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gwsskhife.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gmkzrarep.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gjzooruiz.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/ghybhqfok.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gfwqfydzp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/ghqnltmjy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gotibbhwd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/givpxeakw.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gxjwtuvag.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gmojtnyjh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gwzbsutgg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gnmzjjncc.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gbupkkvur.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gwvcdjwlv.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gtwqqdcst.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gyrnxhcxt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gawqwrhpk.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gsdxtcyfp.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gwxgsancr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/ggtudnkas.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gbwceocyu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gockvsapz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gndqrjxnb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gpzxabecp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gwafmoais.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/grquzssqd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gpjxpjloo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/goskhfmiy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gbhyfjcjx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gstfejgwy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxcftqaqt.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/galanbhvd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkgtbdcou.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gklbarbzo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gusqmciir.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/grswdasku.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gwypujxwc.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/ghsutbidf.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gxahnifxu.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gfanqocmp.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gtappcqma.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gzqzlekqt.sHtML


<!-- 参考信息 -->