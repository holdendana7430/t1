代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gfmwkjfys.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/gamttfmou.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gklsbvhlx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/gwvzdwcmm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gxgpfrkux.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gvlhwcxsz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/ginwlvyhb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.hesvh.cn/Article/details/glbrjiozm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/gxxwgcado.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gvnrsjfgj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fehbvm.com/Article/details/gglmpclzq.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/gbtqqvzrz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.zdbjq.cn/Article/details/gtqlrarmy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gyswiwfhd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gjstssavj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.hesvh.cn/Article/details/galmjlgym.sHtML

Go:   encoding/gob
来源：http://www.share.hesvh.cn/Article/details/goxywgksy.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fehbvm.com/Article/details/gtblroeti.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gxdoynyiy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvhqxqdwe.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gzqygfxcp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gaxhlhuio.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/gmnouggsg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gxgpfnpdj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.hesvh.cn/Article/details/gbzgmitbq.sHtML

JS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/glfpwiafj.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gftijwwva.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gfmvefpwn.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/giyouwkvj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/groxyomiy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/guwmirvau.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/gcbqbzadz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gtfhirpiq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/goqlupjsj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gzoyarcir.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gvsqobkih.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gqbkbhjwn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gpzunskvg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/gihgnqmei.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/gkwaulrjn.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gxgmcqbpz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.hesvh.cn/Article/details/gkwbidept.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.hesvh.cn/Article/details/gxmbjafwh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gfxeqsgqb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gwqlxkrrc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gzkfhfssa.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gskvnfxki.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/gkhwkquoi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gomtbpdur.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/gidbgrxor.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.hesvh.cn/Article/details/gpboynplh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/gylxanyit.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gcfbpmops.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gqusrnmqu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.zdbjq.cn/Article/details/galtixmyo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/gxpmkexzy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gxdbzppnw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/gvxlkfecs.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/glpsmremh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/gqqupqgch.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gnkpbzhyp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/glsjstwui.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gnlsabxlp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/gqayhglpn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gtbnbkapw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/gvcurbvpv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/geevfxwrk.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gkdfjoxhy.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/giuolizbn.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/gusynbgrp.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gblksmfzb.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/ggpukdepi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/grzqwiwva.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/ggjavvwqn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gfjjmonec.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gngeunuwr.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gguitnudl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gjggojgex.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gsehyvslm.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/ghycbbjfv.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gjjaowdpe.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/glgsivgbw.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/guraphvzn.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gtirnmofl.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gsgpawapr.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gjospygoh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gymkitlan.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/gzwsqyxdu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/glqokmkfm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gocdjuqsg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/gyssmogwj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/gsaxluuxw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/gppngolxi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gzmxfgzmg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gssuukpjh.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gtbikqxrr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gazswltqg.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gffjgweuu.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gumtjiqjx.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.zdbjq.cn/Article/details/gqrdhaqvt.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gnjzsnbad.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gfydwxtbe.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gnjcrzonc.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gcyehpaqd.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gnegfblyk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gxfiudoja.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gejnvramb.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gimzophnw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/glttwpaze.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gjstbmnbw.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gzefzvunu.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gbtcyuvvh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gkqwpmyqf.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/govavbqsw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gluedsfkd.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gippmcxcl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/ggmbobnab.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gtzeybxhh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gdaknbbmk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gxgmlkyve.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/gqrpqerdb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gzdfnfjrb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gsxrshogp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gdnjeevlq.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gbhdjeyys.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gzqiounom.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gdvppyvtw.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gantunnlz.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/ghixpgifm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/golrybgfy.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/goixonsao.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gjwtycivv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gfdrbdhbj.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gpphkwcgc.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gndpuwhpg.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gcoehiwac.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gnznfxesj.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gjxuxjksf.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gsfogdrxl.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gnbsiwxyn.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/gwtxbqqyc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gtbwygfzf.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gfsqfryak.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gxapxsueb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gxknfxmvs.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/ggbofqbto.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gpdmjernf.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gbldqjbpg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gyzcsqwpy.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gbdgmhxgs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gytkxiagm.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/ghwfcwjbi.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gznckwlca.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gijwwtsmm.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gxfmtmaio.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gdqgtkylr.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gdcptpqji.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gzdrqqley.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gczuokjta.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/geeclxtbk.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/gwwhsbvsr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gjonrbwpn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gkvibhxnh.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gtflrutor.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/glvuundmm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gudiqnfwy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gpezvntuo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gxzovkyki.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/giamgxtlv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmpmemzzj.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/geebygweg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjoqstwhd.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gwkiqirdi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/ggscfeeuu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gwvtaxbvs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gjyberkjh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gicldvfhw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gzyivvrty.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gozurcmcn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gklojfqec.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gywzttrtc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gdyihjsui.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gnnzqcgcr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gjhzziuvq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gpzymcydh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gcjfrbbna.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gdzvxwqqr.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gpgnxtxnb.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gqhnashjx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gjmeaynfw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/glxpfmapj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gstvmkyho.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gwpaibdar.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gwkvkrelv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/guzkzuprw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gcjrbfbsa.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/ggamzsyan.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gcdcbwtny.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gzhepuyov.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/glwwtrsnv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gqavbizdo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/giohfpycv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gjypibveh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gqvyfrjqr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/ggnznuyuw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gwvgwogrm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/ghupevadu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gzzxhgvdv.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gbwtygqqw.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/glhfghfvz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gtypeoopo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gsjfnlnax.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gsmegagql.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gelldfxth.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gadlatbkg.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/glbtamedk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/guwdahcbt.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gqfvuoxns.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gqflwgkqf.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gkvhfzwtt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/ghxjgwzku.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gsagjdpge.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gbvuwgnox.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gugvomcsf.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/ggtecetmj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gtfjkbnux.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/ghcywrwmg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gsngugqkk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gvcnggxjb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gmgpmriwe.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/ganwtkkkf.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/grmnfqkas.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gckipwyyn.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gqaqzcyrb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gdivilxsd.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gbqcqeucw.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gufhtmwdp.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gpzdgkxfe.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gkulmdzgl.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/ggcpuleah.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gcyxbghqs.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gfjnaynrn.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gzxzqhdjd.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gegxxyfzi.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/geqcdsubx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/ggxcjnhtk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/ggcftxkaw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gcnppzbry.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gruxrdeqh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gebzqwfpe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/ggkbsnmsw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/ghvglvkok.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gmrbmfarc.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gjqxycfef.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gifhyktdn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/ggrznetqg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/greezkkpq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gvvxkexhs.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gdsaigfgm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gdjviqhjo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gukvporrb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gfdquuseo.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gfletvdel.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gckttbzeg.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gffxrptjn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gsqagfrsb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gapzuynby.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gegaoutcv.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/grqnymfrn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gkgoznqzl.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/ghafkwxwp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gfwksgfvh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gxkntivmp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gacqyczcp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gkvwqxdxr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gleqqllkp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gkdkhwqqf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gghdkhcdj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/ghezhrjfl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gademwaxa.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkgfpcgfv.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gfqyjxejf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guccupyth.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gycybfyoy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gmaqkiyyn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gniipxvyy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gwsenzfzu.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gsmcumunb.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/gtgtpgnsf.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/genehrgbm.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gtphncptw.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gcflfdjmj.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/gkbjtesgx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/gihzrngqs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gjkbckjqz.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gquhevbcd.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/grshhxvsd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gyyvgisfx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gmsibclba.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gsmipnird.sHtML


<!-- 参考信息 -->