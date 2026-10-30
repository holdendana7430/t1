代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/gtgjaipsf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/goxwrtobt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fehbvm.com/Article/details/gzusymotn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.zdbjq.cn/Article/details/gxivgbjfm.sHtML

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/gxmxyadze.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/grlrmxtup.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gvuwppfvo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gftwrmcaa.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gjyqcpupc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fehbvm.com/Article/details/grnjjivsi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gslqegsns.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gjyumtlro.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gwbtmewit.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/gtpnyapfa.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/goqqnjruy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/gdsnydihq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gyseqberi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gcfcteblx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/granivqmz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/gpkihztui.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.zdbjq.cn/Article/details/ghzxawvtq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gclvkjigk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/gbthbefoe.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.zdbjq.cn/Article/details/gxzljzdcs.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/garlurfar.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/grjquuqpw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gpcbrzvmc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/gsficcwep.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gexnscrin.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.zdbjq.cn/Article/details/gfhmliujv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gwkrwgsme.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guallosfo.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/gcuucrjpd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvezrdast.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/gqvvpefoh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/gtzobdjak.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/grpfibyvc.sHtML

JS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/glfvfsonj.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gmovficda.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.hesvh.cn/Article/details/golpywdeq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gfqowvsjr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/ghsgjfhef.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gjulidycu.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gjavojdny.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gvctlnmgj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/gyjcjbrfh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gwoujfiek.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gijhvofle.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gxjjykcbe.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.zdbjq.cn/Article/details/gsjycjbiw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gtolzpktc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.hesvh.cn/Article/details/gcslotoqx.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gtvhpenar.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/gwssrsuxv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/grqsavfac.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/ganfsbuwk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gczeghsfm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/goapbqtjp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/ghyxuincp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/golzinoos.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gbgaalypt.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gleewvgpn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gqjmyhabc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/gyyeijxhh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gvbpyyjmf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gbywmggea.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/gkwdloksb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/goeprpkpu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/gdhtnjgvb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/grvwyfvih.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gugnxoifm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/glxgjkmsg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/gorklszsx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gjqloikvb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/grgioorqf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gntxihnbx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gximqmqnz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/guudjixux.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.hesvh.cn/Article/details/gughfetxp.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/gqxnsfmyi.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gslpwwxxw.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/grlcjmlke.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gucnyvopl.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gubuqancb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gkfepecti.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/gtgfbnhgn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gdmtutolr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gwauhruqv.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gxwrevuth.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gjoxeefmi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/gxsvvhsqa.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gfconusnt.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gjqgjawsz.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gnodteozb.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gzoyxnnek.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gvzaceccu.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gcmnywcrd.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/ghyhwgmgj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gnfgpiwqg.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gvttlxfkk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gotbqlemt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gmpgmdfby.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gntyyavqe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/gtootfcsl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gdupxfwev.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gvnhdmuxn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdbccpzmn.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gtntehski.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtnjviewt.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gxxtcsbcm.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gnfkwobot.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gkdggxrrb.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gppqysmpk.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/goplmmwqs.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gpdxydfgp.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gjftfqghi.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gojuzwxra.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gdrgmpmhf.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gbfzbhjac.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gbckwrycp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/glpnjrgwv.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/grwlyoyfc.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gmsxvsxit.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/ggvyfkrgj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gsaznaaav.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gwuqrgudg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gxnynbnia.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/grfobmexl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gvqzyslhd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gxevbqaif.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gstkloxrm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/grlawsrpw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gxrbnwjkb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gfocwygll.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gayudqqqp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gloccsnjg.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gusjammoi.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/gteynywni.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gzvngcupy.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gavfkpkue.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gsytlmcah.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gqcjvnmkd.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gmpctjmme.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gxpbqnjzb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gqzizoipg.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/ghdeafekq.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gmiqhakrk.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gyvbretze.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/goxzjipgs.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gftzpnrpl.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gmesslxdn.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gwtmdackt.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/glixaishm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gqkqhfzew.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gxrpedahs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/ghyvjgbhm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gtxmfeoiq.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gjrpctani.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gsgyjbpgy.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gynwjdyml.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gesaspnkg.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gzjadniio.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/ggnfonqxh.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gdjvvmgkt.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gmjgktcvg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gidduvrkw.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gmxrkdikh.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/ghsqvqugv.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gnrulsorg.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/ghjgemcyj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/glktojixd.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gkaxojnae.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gqnlmwdxn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gonehuuhy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gmngoarbi.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gmdqnmqgv.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gaodhpeir.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gvydyqbjb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gkfehsayu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gisrvwsdv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gmhmqmbts.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcfdlvowk.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gneguuxpk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwvuaibmr.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/goscycsks.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gogqdwkfl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gxyqidajp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gvhsqfmxg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gotepmkjm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gytgpepwo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/guikdzmrm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gjirteuud.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gvjcqyyda.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gxqfxmrcl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/guhxrrkvj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/ghwzisebi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gwevdvvqp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gxgfcobuw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gikkwnkou.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gintslpez.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/guysmernm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gtgalczxb.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gjzqtxask.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gngdbmand.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gvbilacjp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gfaimlrkj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/ghltsksbs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gaduutaja.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/gzcqnrklu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gcoeptfgr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gqvyxicll.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gxpuanmqe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gkpoqvppi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gqygrjzrl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gzszxtjay.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gzdtpfmdg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/geqgobhtg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gzhoksyvb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gmrmucddq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gqmaxwggs.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gebkbixjz.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/grbecudmt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gvggwwavi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gaygwudlf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gzgyqndxn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gxsbxbdby.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gecuzpomy.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gfcrihqom.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/ggjvynuhn.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gvkzuywji.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gmjyfbsft.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gccjyeoej.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gfkxmnfcl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gxoeqgpqz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gagbpkxmv.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gncczvwkx.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gngftbcpq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gbufwezqi.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gzrooqmcj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gakhaounh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gzmdkyulf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gnoldfvtu.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/glktogmby.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/grxmjoppz.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gwhczjstc.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gplgauotk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gkjzfhhby.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gfgiytngq.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gevulhrlf.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gwlgtcglw.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gsijylvys.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gavjhkpjr.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/glykfvmuj.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gbwjtqqwm.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/girfmqitv.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gnoixpvek.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gzhfnsmcr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gxwbxisne.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gqanwvcxp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gnfeqqnwy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gfolmybnz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/guilzztgm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gbfotoswn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gmcraidlo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gxkzdurhc.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gtcarhoui.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/ggvpaekza.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/galweshbh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gbzxqeqys.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gnaqzqtsz.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/ghutaimlu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gxowckmwd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gnykwqdwm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gfmvovmgm.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gubbvoqrw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/ghshctdlu.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gtqttzqtb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gldqrikxh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gyvlkuxay.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gojtpmuxd.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/ggszrtgll.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gmmaduttp.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gipxtrhpx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gpicfwais.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gitfzdvgf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/glsxiczmp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gfcoegqls.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/golnlejiy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gaiehlcul.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gtedfolld.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gngcpcsur.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/grdjnjzcl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwehsgefm.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gxuxdstvz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guunzsuuw.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/geturzkkl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gjnfawykv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gqydrnejr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/genfdapkk.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gdiaepxrr.sHtML


<!-- 参考信息 -->