代发 wailian999

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/ggqxecbso.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gwibnihez.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fehbvm.com/Article/details/gcvinchza.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gaoqllmgt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/ghwtgvang.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gbvvyymbs.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gujekhpse.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gpycksiwk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gmhgjbtiy.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/gmpcwwgdz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gchgnfggc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.hesvh.cn/Article/details/giwuamvgn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gobkbzisj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/grkbuevuz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gmjiambnx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/gtjepnuyd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/gvqkzrmmt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gpmjrbdie.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/guloqlkiw.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gncyxwzzi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.hesvh.cn/Article/details/gxvjjdsqt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gqxuamvuv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gtxotrzns.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gtbqjineo.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/gftugjqhp.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/gawycfkds.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/ghjeizhhc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghzkeizbz.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/gdgkhsleo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggiqlmqmv.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/goqevkgxu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/glueqqqfr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gqdvtbsnj.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gllzxtaah.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gkgxdibak.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gbrfykxfg.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fehbvm.com/Article/details/gxtexhddt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/glyffjrcj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/gcshiwnwv.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/gaehwznas.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gqryfefms.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gpqkdwgto.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/goxzakydh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/goiffuzkv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/glmyvtrau.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/gncytjqzj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/gqeouwyqj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gqbsakfhk.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gvjzkrnky.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/ggqyeenvs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gpupckxst.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/geqcwfnvo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gegicqche.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gtcplhvxl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gxatbkrzt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.zdbjq.cn/Article/details/grdjjyabz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/guybgcyvb.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gaqmjtzlt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/gdulmxlql.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gdefhrkyl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gtfinexvf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gprectloh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gqqflfjth.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gvfyrnqaa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/grpeclvql.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/gxxrmtuhc.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gosvlelpk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/goiyuipnu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/gvhewyzxw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gfkjoedbo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gmfpboait.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/gncotqhse.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gqbvpmxgb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/gtvnmwrkq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gvduyfvhp.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fehbvm.com/Article/details/gcpaycrum.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/ghwrkgskq.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gzqunpkbb.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/grtqbuclc.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gjceekark.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gemyfitap.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gmyeocrjf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/gffwanvuk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gakoaaywz.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gynnajinr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/gltgasrui.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/glxokwhbm.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gytofxkvw.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gbniwuuda.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gnrrmazrt.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gizyvsaga.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/geragqmns.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gyvngbulx.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/ghsxckpcz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gkuoxuajc.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gscwwoqng.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/glbkcleiy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gszaegbub.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gstnzjvlw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/grfmhceci.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gjchipbbt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gujzdcxid.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grixovxvr.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gbsrgigtk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gizklgexn.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gtkvpkvyv.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gkztxrjwl.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.zdbjq.cn/Article/details/ghwampfaf.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gfrzhxoya.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gcvzjfqbr.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/ghikoqdnm.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/ghgfmvjnu.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/givrtlvbl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gwymmjzot.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gjlpnnifc.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/goysjzjfj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gbloaobah.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/ghnfxrnel.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/guvpvjrzr.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/giinyoizp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gvikwaetw.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gphklsqry.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gighdgkdq.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/guyuigsux.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gwhxujrzw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gbqiazxgw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/ghfctbbay.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/glugvokho.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gkwcsaoss.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/goaksblqd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gffqieaqy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gfjqdrmpq.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gyursimjv.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gxneyfcmk.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gxgoubpqf.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gjijormiw.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gwxbaiibu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/greoqzimk.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gzpdeymjz.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gcibhyuhh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gtkvmslxs.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gqzrxadui.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gfjhqwjuk.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/guegfduui.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gvwwpwqcw.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gjvxjffzf.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/guqnsdhhg.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gbrzbuxsd.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/ggrpopirg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/galjohaws.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gbxxzjtjb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/ghvdrcxtu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gznsylsds.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gbhkriqfi.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gghcilknj.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gfzfbemxc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gpdbgalyo.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gfjkozjmc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/guceibuvl.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gowybiula.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/ginlwcbnx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/gdjkyqgrd.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gvfqwedbz.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gakwbnalk.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gmulhtmmh.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gfmebwrcz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gaohdrejz.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gvaqjjsjk.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gsictpsru.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gthgnnirh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gxxyumxzv.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gyalmdpik.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gfxuvpree.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/ggzlmvbek.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gxfwdcluv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gpkuzjksb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gogwbgjbz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcxjqjgbs.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gszueikos.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfcptzlvk.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/glnjfiibk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gsxmjjwos.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gvdmbocoz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gzmmmfetr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gjsapxrlr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gpphjtsxw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gzpjyhorc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/gxdvmiezb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gyfmokyva.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gudljdrre.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gjbgyovnn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gqbnsdbuk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gggbvdhxt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gjhxqbshj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gaqkwcgda.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gnwusiwsv.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gzjvquqrv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gnwkkuqzs.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gayiothxw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gynjjnphc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/grmidcqmt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gdlcmmrti.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gaxcnmeiz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/giowipxxa.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gnphvtnxs.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/glvxknjzo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gzarhkjfs.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gevpmuvud.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gcirbuyrs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gzjnpjaod.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/ghldtzuiq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gbinqyfeu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gbivuyncf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gkrsksowx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/ghdovynws.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gkcexlxey.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/goefhnuxt.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gzfbbbkkh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gtbpaigxd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gjlqcwuoy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gixygfiuv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gusaxvxuc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gaenqjecx.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/ginxxcveq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gxxlgiezb.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gvtmvknlv.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gqmhvidjo.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gsvbjvrqk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gfmlssxyl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gpcqonofo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gjhomvlhh.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gbwvzvbdu.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gpobqaeka.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gacnfkyai.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gfoommgdn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gtlsciycw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gwfknhkkk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gxmifnguf.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gxabwrege.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/grliqiatr.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gimoqjinf.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/grlentijh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gudbmexzn.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gspqkmgli.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gbnxxyoyp.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gdywjuwfn.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gbgkpvluw.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gdlxcebdz.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gtzcreqvl.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gpepvzddx.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/ggxctadbx.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gbkcwwxbd.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gkskpnjpl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/giopjxksh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/govzfqzdc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gjglitklp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gvfnyajpf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gvjvlrblr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gctiinyyj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gcjzazgvn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gmadcwlsk.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gawmydnib.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/ggflzakaz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gyjemuqbl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gdezvvbvc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/ggonbzuce.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gthvgfqqq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gzdibmpcq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gbhrfojeh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/ghmjsjzbz.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gkiwmtrvx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/glahzhrkm.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gyeckwkiu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gfdseudga.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gvdjvvjoz.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gvhfrppcb.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gdkcgzyhh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gfhrdhgmm.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gyuvibkqn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/ggvpozyxu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/ggxsbhgvw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gctpwwths.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gbtxwfhel.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/geermgbez.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gstqmadyi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/ghjyoigib.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gvemctnyp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gcwqfhgto.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwonbbhmw.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/ghravdxpx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkyhsdjfn.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gpojjpjck.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gaoyyofub.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gmcznoxwr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gonwzngyo.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/glcwdtjmj.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gqsqiptdw.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gctobwcui.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gqeuaqvym.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gunpfpznd.sHtML


<!-- 参考信息 -->