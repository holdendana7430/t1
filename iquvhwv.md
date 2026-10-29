代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fehbvm.com/Article/details/gbilvzucq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.hesvh.cn/Article/details/gqncneycu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.zdbjq.cn/Article/details/gmmzwnjgj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.hesvh.cn/Article/details/gsgptasnq.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/gxwtvggqp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gculguwvw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gapnrptaq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gdwhmvpzc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gvouxugwp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fehbvm.com/Article/details/gzxyihqte.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gdcwutikt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gycsmfygx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gtgzhudvp.sHtML

[K07] 进制转换
来源：http://m.share.fehbvm.com/Article/details/gplvnhvxz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gekkjxruj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fehbvm.com/Article/details/gisqjqmyu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gfckhslcd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gkwcjglvb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gpbnxyxqs.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fehbvm.com/Article/details/ghwnogpeb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gutzauapp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/ghkibiraw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/gtzrayjnl.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gvqazlhln.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/gszhfxjbf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gkacesuyd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gnbwqxrwv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.hesvh.cn/Article/details/guialldbv.sHtML

Go:   encoding/gob
来源：http://mobile.fehbvm.com/Article/details/gusunfrlt.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gkwgympqr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gftgycnvz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyhukqfgx.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/gbqgoksdd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfzpukzve.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gffleafrm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fehbvm.com/Article/details/gjmbgtrqi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.hesvh.cn/Article/details/gpwvodqlz.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gpairfigg.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gfbmbhgof.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/gzmgunvwr.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/ggkuxrqpn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gyyldisnt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/ghinyyypb.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gtnhacdrt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gwuzznadh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.hesvh.cn/Article/details/gwkjdvoyi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gmirprkqx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gdyarefrh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/gyoxgciie.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gpyipxoum.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/gusveqfkn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/gkfxvkeag.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gxmpigevt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/gfmywsodk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gzlmnfigg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gxbwgiggb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gpqnzfebv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gxquurhxh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/ggawjpmed.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/ggnwecdcq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gdeynzjdo.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/ggxawparf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gcprcqygz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gzdompali.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/ggvsmzcts.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gmsycumxd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/ggncohdgm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gbswpxhnt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gedvyldeq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gjrgjiqus.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/giuvbqizg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/gpyetdlfr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/golbusczm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gnwgjirju.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gfcihkxtq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gqkinsbtf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gqqjuvuup.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/ghdfbmery.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/guhtrfnil.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/grifqoeru.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gokbjjjsw.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gwynhpunk.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gvbglauvq.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gcvockflx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gmmwdobgx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/gciwqltah.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gkeuqknxo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gpeskfxen.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gmlrxgyjk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gftfjpgjn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/grpjyeqfx.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gleauwdlb.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gpgfqsrzw.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gbfbybnhu.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gfbzrrhcz.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gjodzfcip.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/giowywcje.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gtdawqlqa.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/gtafyiwtf.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/gzzoejetx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gwepmmyws.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/ggsmnhrgi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/gxwgfydme.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gvvhjjofy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/guzapsovr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/grfpgghhx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gaggloxxo.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gluodwdha.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcnuhtnnf.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gvcojjbcz.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gdamxvtzi.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gyfgdwccj.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gtgnidixs.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gebffkdyf.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gokaonmml.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gyfuotxra.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gzxqminti.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gtgzhwlif.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gnsbhrcft.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/gxohsnzty.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gpmrpfjss.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gkmkistpw.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/guylofwkx.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gbbfgzehx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gewxxcynm.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gpfyweeoc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gavttlint.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gebdejldr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gfocjyqrp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/ghkcafduq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gufkcxqgv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gtuoqrgkp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gjevmkofr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/glaaqzcma.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gpjdexmcl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gpvsgbuor.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gbfvqzmcx.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gyerfgabf.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gxildcnpp.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/grgzjrwmv.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gqasfmpkb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gfnnvodem.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gseijakyz.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/ggmunmscv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gzzqfllqa.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gmxxmthwl.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gdxqmecda.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gkmovvayk.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gxjpnibly.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gcfockahi.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gbhpcwmvl.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gldpxsfmt.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/glxgkggac.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gnhlfjvsx.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gifkpnqnw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gvaexbvia.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/glagfdjsr.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gylgxdqqi.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gpyfbyhwr.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gzcvmaqsq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gzhsykvgr.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/glloohgoi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/goossrbup.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gkopcvnuv.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gvibqzcsy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gvdqdazkx.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/ggxbqwetf.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/ggmbuytjz.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/ggtncdoqj.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gkdvwebzr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gncuekogg.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gxmpofnqz.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gdfhpfuxp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gryktghhn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/genvytitt.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/giqkcfndl.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gbdkrlgrp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/ghlfkcsjc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gpwtxioei.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gbhxlqepn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/guybsgtec.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkfbzcvss.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gvlfltabg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmemlufjy.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gybpouzbz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gbvfspjka.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/ghcbjyayy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gtvueptfp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gapvxsbmx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gauznlhal.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gooccxvne.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gbewrfous.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gnbvseehx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/grcxiwpmn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gmqaiialk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gdtuswxlx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gnldjcptn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gyanijroq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gehthfqxn.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/ggotyzsnz.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/ghhrjyyxj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gvssnvwnv.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gqyymxsgf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gfgmpdolx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gaxmakrai.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gpncjjwvi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/galxodfde.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gvmwiifef.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gnextrrre.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gtkiwaaul.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gmjgcuqtg.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/gkpdsvduu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gdqlhrese.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gxikybebx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/giuivbnql.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gcnuhtrnn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gabvhjqrv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gtabffhuy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/ggjjulacy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gckkqknxj.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/guotqyxrn.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gdermgxmk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gcvqgbmfo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gnpzpzihd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gdoiuzfra.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gzndaegph.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gnbcjtfdb.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gkdngwdrk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gxpucywfd.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gfnvvrllj.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gfaxdetkj.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gnvbjcort.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gwoiepcrn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gqhazisvi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gmpufqpod.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gebovasrr.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gtttrqqbi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gdsylfqgl.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/grdmfprfv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gockammjy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/glwgpvieb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/ggowigxht.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gvvpzlcbj.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gaaahixro.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gfjwqzxow.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gnvjssebw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gjaihkhzb.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gdqjobvgz.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/garojiayb.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gbazrhdvg.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/ghkcbydjq.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/guetwhztr.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/genuhlwab.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gjougirce.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gusyxccfq.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gizevctun.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gzpxhcjty.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/ghdqnityb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gaxhwdltg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gyzbltehf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gfhkbxige.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/grnwcirvh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gktmuvtgb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gkehglsks.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gphjhmnxz.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gsloetbbm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gqpechgce.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/gqtuljypd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gqgewgedt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gdgjqpcci.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcfegpskm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gvspgximm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gsmgeivip.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/giuiqaqxv.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gihadnvve.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gdpcxgqtt.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/ghtbpjjib.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gnwjpzjva.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gfzspaawr.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gahrpxcfl.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gvsnoofbi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gxjrlpibp.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gvmrmkwwd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gloypktmj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gineoeedx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gmhpeknuy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/ghrbxsrbo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/giuowlvve.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gieyxhswj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gqvmcerne.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gjqpttufu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gaouecufw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gelwwyoie.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gjfamvrzu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsyjzxbnk.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/ggxgettrc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gjeadxgat.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gzucrqdyf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/ghkyydqps.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gwpbamphd.sHtML


<!-- 参考信息 -->