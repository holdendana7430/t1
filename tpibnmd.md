代发 wailian999

[K06] 解析 URL 查询串
来源：http://3g.hesvh.cn/Article/details/gbvthmccz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gyravizzt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fehbvm.com/Article/details/gmggngrqn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gtlrcsgbu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/govqaybwi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fehbvm.com/Article/details/gdkjdfluo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gzbopnlyi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gewmzdeab.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gtqilsgve.sHtML

[K07] 进制转换
来源：http://mobile.hesvh.cn/Article/details/gxxocfipl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gjlmquxpb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/glwvuoose.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/ghffpangx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gxewozvso.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/glmjbldmq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gibtbpema.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/gmffygatn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/geooqmnjy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/gcgativqb.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gkjihwsxy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/gvhsewrfo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gkovbeapm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/glaeytmhs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/giomdyxec.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/gyesvnuiy.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gksfjofbp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gecxqtnqr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqidyduob.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/gtffyxuyy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcwglfrxt.sHtML

[L01] 发送 GET 请求
来源：http://read.share.zdbjq.cn/Article/details/gnbmyhind.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gbwzuhqhv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/gitfqkrdr.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gsazrvzub.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gesssnfsd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/gbvzthaif.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.hesvh.cn/Article/details/gbqqzfdhk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gofgdacdv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/gypaigznp.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/geqsgject.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gwfthlklx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/gxsjnuukw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/grvfybany.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gaiwdbppq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/gbinywafh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.zdbjq.cn/Article/details/glnvkxtep.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gaevvgysn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/gzxvlomdd.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/ggajacvyw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.hesvh.cn/Article/details/gxktwawyy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gtfrtjuuz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gkjyhijhg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/ggrxrptev.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/gmmmleczc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gluaacyxo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/gqsrdpyxq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gkcwvivwo.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gpaytyoqx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gnektiepd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/goseibubt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/grstgosbq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gqxxturkc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/gbzamxhsy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/guvyvbsdy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gcaqaixvk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/gbkzsufrr.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gxpodsbki.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gsyprqluo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/gwcqggreh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gxqruqsrf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gkahzeweo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/gaxdjybfa.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/gnvfnoeag.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/goyfyrkea.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gqkfbtokn.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gvepuoyzq.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gmbqxpvtg.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gdnplrzul.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gmvqnrfhu.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gzlnxssbb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gninilgso.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gciuzbdvd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gqlsperno.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/ggtufmwke.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gyjlirhcd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/garucsodl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gbhwxhgtm.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gnbkimakb.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gomzafkpu.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gqcsysitz.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gtbttlzhd.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gprpbmabx.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gdzsmxacz.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gxtopthyl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gmjlsplza.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gnrahrmbh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gtpfnnkzx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gnbguaygy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gfnovtkjg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gjjbgztsn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/ghuyodtlf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/guixthkpn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxyduzfvc.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/guneajgbe.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtvqwfetq.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gfavbfenj.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gzxweqbwh.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/ggdzezlqy.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gktacvutf.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gqzolzjyz.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gnnbafxmp.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gkbedsiwh.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/grmhtmijk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gimpdiufp.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gerputyiq.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gphrqzape.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gylrdfass.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gmdwgnwfi.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gpoitzucb.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gahibfank.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gwixrouii.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gefssputg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/grcqwtnmj.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gxbrnbxrw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gaoihbwtx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/ghdfuikql.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/glsxbieif.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/ggfkrpilc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gxfaaueim.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gwbrgkzln.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gckjitssi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gxvhuajrw.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gedurcnye.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/grirhklfq.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/grarsauyf.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gswiezeul.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/geuqmtooq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gpjfoqbzl.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/ghgoxeerp.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/glgjivzvm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gdmgmaeok.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gyjmnjhvv.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gmokivswb.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gyhqykgwa.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/ggenwzgaa.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gnlivxxsz.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gwvjzdoow.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gcrgeepwx.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gdsvljcue.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/goktauevx.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gxpluggao.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gyukqjizs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gsqpksvgp.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/grxjfsoow.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gzwcvayyr.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/ghikfeaes.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gjyoxaxpo.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/guzuakqfg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gfushgmsm.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gndgqeecp.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gudgezznu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gnwsxvdhe.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gvkzkchfs.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/geztrlwwn.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gvylawamw.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gjgavgpiy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gaosdqnte.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gycyqnnmj.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/grxbgsjij.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/grsqaicdv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gzzpzmvop.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/goleqimuu.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/glbkmtymx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gbzzymyej.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gndjiwghk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/ghqfalwte.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gmqvqhvnk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grgkxvvmd.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gylhxpoai.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvtjonjnd.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gtxqqpqos.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gzgdecsko.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gshbritzo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gdiaekmqm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gcwbfepvu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gbhmntqjq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gpjosjimw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/ghiznvexd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gtpkyreom.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gluyoroez.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gvwvrpske.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/gkmwshtbk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gihhlsfwy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/glplizifi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gyxdbhpyw.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/grwsxokxh.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/ghfgouvkn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gvsmysqki.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gsuoofzmm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gqbhkbexb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gzqztxmwb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gkrxwcdrq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gxoymquqr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gsviprikc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gihuzsopj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gchjjttfi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/guhkafakj.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gostpzvcu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gguzwjtvb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gmpaghrwb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/glovmljij.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/ghctvtlgo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gtcfqdmwq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gcmlxbrwk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/ghupxnntl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gwiqitidk.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gvrqfkbzj.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gsblnjoxl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gwzysosmw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gqcvllnlw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gmowrnjhi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gelirkeau.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gtakamrrs.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gbeknfgge.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gsiogznzh.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gbfscqwdg.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gewgrrzee.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gltlfejvg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gylolhhzg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gcmybipvu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gxviyreru.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gvaaeakfl.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gqsijodnl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gpfhfvaoa.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gyhouesar.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gnukfwwkj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gmnfnkmrf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gaiuvniaz.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/glrypavbu.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gfrsgntij.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gclvjwuwx.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gtxxxmpex.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gtvmwzbye.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gzklurlrl.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/ggetsxvir.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gxexghdui.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gceanxtti.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gwfxqbbgz.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gowsifnqf.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gfweplzlz.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gbevauwyp.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gmfajjzxe.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gpfikmqfu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gflajfxuf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gtftyuuha.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/guzvroosu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gfuzcuyfq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gpllglrbl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gxqrjigvi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gihqcrgph.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gzyfxtfkl.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gryofkmpx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gzrhqrple.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/ghzpateah.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gqyoucqza.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/glxczenjj.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gdoxwsnma.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gebjzdmug.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/ghtmjtrzy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gjvgkthxs.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/glfmwezjl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gsboekfut.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gxodvlrmx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gkreyvqjx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/ggwkvfsiv.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gpbgsytwi.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/ggrxnevlh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/ghqhoxyau.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gujqkdspq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/glomrpenj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/gkpjeyupg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/glrmfbdye.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gnbbjnvot.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gwfgkdbai.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gcqqeelae.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/glgkszrfv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/gllzhujdg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gaxvklpsm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmpipfsus.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gcblpgsii.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwspxtuze.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gnsusynkf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gtwnjvmsl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gxdseeisw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gtrzpcgsu.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gpaxdsysx.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gxoojahym.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gxmjqkkwu.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gkmzqrots.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gkhjkcztg.sHtML


<!-- 参考信息 -->