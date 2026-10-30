代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdchkipg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmlkjjnd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbdlsiik.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggumcidse.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/geatvfuca.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvperhut.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfurzqlbe.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvruqwnwx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fanxiaobao.xyz/Article/details/geqxaiemf.sHtML

[K07] 进制转换
来源：http://3g.fanxiaobao.xyz/Article/details/ghvgpmhgk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gqrmajqvt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fanxiaobao.xyz/Article/details/gickqgfqb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gwkmlrvui.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtkznzhi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/ghwyyebdk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fanxiaobao.xyz/Article/details/gstzjnrrn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzivzwwmn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/glxedenjh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwskguebu.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/ggkepdlnd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gifddvkdr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkbzieps.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fanxiaobao.xyz/Article/details/gzlbvqzpj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fanxiaobao.xyz/Article/details/gbzmuwgxx.sHtML

Go:   encoding/gob
来源：http://wap.fanxiaobao.xyz/Article/details/gghidftqk.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdkpzyih.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fanxiaobao.xyz/Article/details/gqplzzccx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqosytutu.sHtML

L. 网络请求
来源：http://wap.fanxiaobao.xyz/Article/details/gkmfuzjli.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkojjvywx.sHtML

[L01] 发送 GET 请求
来源：http://baike.fanxiaobao.xyz/Article/details/gghpnqjet.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvtagpsk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrpusntk.sHtML

JS:   await fetch(url)
来源：http://mobile.fanxiaobao.xyz/Article/details/gncpddtqo.sHtML

TS:   await fetch(url)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjbxmhds.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyixilfvm.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfshqpjl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjjipjvq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnbscdkn.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbmuyctw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fanxiaobao.xyz/Article/details/gwindrnma.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnelwunn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqbivubz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fanxiaobao.xyz/Article/details/ginyregyj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fanxiaobao.xyz/Article/details/gdomqragr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fanxiaobao.xyz/Article/details/gddfpylrn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fanxiaobao.xyz/Article/details/getvlzdla.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fanxiaobao.xyz/Article/details/gpbyxucod.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fanxiaobao.xyz/Article/details/gclczdwvq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbktikln.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gvkjdvbxe.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fanxiaobao.xyz/Article/details/gwcphyfef.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fanxiaobao.xyz/Article/details/ghjbdpxly.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fanxiaobao.xyz/Article/details/guypqbooj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdhyhmle.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaxqfltl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fanxiaobao.xyz/Article/details/ggiblcxwx.sHtML

[L04] 设置超时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkbukluo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fanxiaobao.xyz/Article/details/geskeabew.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fanxiaobao.xyz/Article/details/gkphcglej.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsiagobl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fanxiaobao.xyz/Article/details/ghdipyrwx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fanxiaobao.xyz/Article/details/gqjgompbi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fanxiaobao.xyz/Article/details/gukpkpvlo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guspzcmye.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glujzzlfy.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fanxiaobao.xyz/Article/details/gkfdiqmoq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fanxiaobao.xyz/Article/details/gqizucbmn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fanxiaobao.xyz/Article/details/gohewydgp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fanxiaobao.xyz/Article/details/gqpnuolhs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fanxiaobao.xyz/Article/details/gkljinwck.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fanxiaobao.xyz/Article/details/gocjtoecl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gosytucnv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fanxiaobao.xyz/Article/details/gxiqrdjou.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gshzwqtus.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjkxzoyp.sHtML

Py:   resp.json()
来源：http://www.blog.fanxiaobao.xyz/Article/details/goargourk.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrfbcsyl.sHtML

JS:   await resp.json()
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxarauug.sHtML

TS:   await resp.json()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafafbgdz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsrnaxzy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghltndsbl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fanxiaobao.xyz/Article/details/gqbpqnrwn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fanxiaobao.xyz/Article/details/gozfpkwsy.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gipryjvsy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvpcecpt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gburfjeqw.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fanxiaobao.xyz/Article/details/gapbprobn.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgcoivnq.sHtML

Java: resp.statusCode()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjopydnj.sHtML

Go:   resp.StatusCode
来源：http://mobile.fanxiaobao.xyz/Article/details/gqydpxvcz.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fanxiaobao.xyz/Article/details/gufqcrzsn.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fanxiaobao.xyz/Article/details/goinutyfm.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fanxiaobao.xyz/Article/details/gonrnirwd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtauenevj.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fanxiaobao.xyz/Article/details/geostrskp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gxuriqlwd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gcqlhbccm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fanxiaobao.xyz/Article/details/gezalsilo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjzizeqm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fanxiaobao.xyz/Article/details/gchbqwfme.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gfjznbyul.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhlhjmne.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fanxiaobao.xyz/Article/details/gklnlfiil.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcvupjvh.sHtML

[M01] 读取命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gcnovrhvf.sHtML

Py:   sys.argv[1:]
来源：http://3g.fanxiaobao.xyz/Article/details/gitvyflle.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyzgorbe.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gqtzbigvl.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gizvwhqov.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyehkvbq.sHtML

Go:   os.Args[1:]
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoulemql.sHtML

Ruby: ARGV
来源：http://read.share.fanxiaobao.xyz/Article/details/gujwjreem.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdljnvxnv.sHtML

[M02] 读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/geeyazhtu.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/gzhazyvde.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvwcueow.sHtML

JS:   process.env.HOME
来源：http://baike.fanxiaobao.xyz/Article/details/gbjnjswav.sHtML

TS:   process.env.HOME
来源：http://3g.fanxiaobao.xyz/Article/details/guuyxwnrh.sHtML

Java: System.getenv("HOME")
来源：http://3g.fanxiaobao.xyz/Article/details/gbjagldyv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fanxiaobao.xyz/Article/details/gncbfgopr.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fanxiaobao.xyz/Article/details/gigngzcpl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqiudkwh.sHtML

[M03] 执行外部命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmtfwgxz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gujqtalye.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fanxiaobao.xyz/Article/details/giptdoddh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzmocskb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gletwqhes.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbddwost.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fanxiaobao.xyz/Article/details/gypaoeazn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgfnhnhv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghaubfywt.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgbtehjk.sHtML

Py:   os.getcwd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvzhpsyo.sHtML

PHP:  getcwd();
来源：http://mobile.fanxiaobao.xyz/Article/details/glonbiwag.sHtML

JS:   process.cwd()
来源：http://blog.fanxiaobao.xyz/Article/details/gevyauetn.sHtML

TS:   process.cwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcdfovoo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fanxiaobao.xyz/Article/details/gevfceuqy.sHtML

Go:   os.Getwd()
来源：http://blog.fanxiaobao.xyz/Article/details/gnoiwffic.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboqbtjjj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fanxiaobao.xyz/Article/details/guppfnjpv.sHtML

[M05] 设置退出码
来源：http://blog.fanxiaobao.xyz/Article/details/gjgahryoj.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbumqeoo.sHtML

PHP:  exit(1);
来源：http://read.share.fanxiaobao.xyz/Article/details/goexooffo.sHtML

JS:   process.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gejyljkqb.sHtML

TS:   process.exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/giursyldg.sHtML

Java: System.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gxxiqnqtg.sHtML

Go:   os.Exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/galalqrxs.sHtML

Ruby: exit 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwcnttep.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fanxiaobao.xyz/Article/details/gcvyqxizh.sHtML

[M06] 向标准错误输出
来源：http://blog.fanxiaobao.xyz/Article/details/gqrssktur.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfamjetr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktgjdypo.sHtML

JS:   console.error("err")
来源：http://wap.fanxiaobao.xyz/Article/details/glvnuyumo.sHtML

TS:   console.error("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gcingpang.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfntlzgsf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fanxiaobao.xyz/Article/details/gmupzyedm.sHtML

Ruby: warn "err"
来源：http://wap.fanxiaobao.xyz/Article/details/gtnmkixxm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyvpsbgk.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fanxiaobao.xyz/Article/details/gyokalxof.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fanxiaobao.xyz/Article/details/gkcdfbjcf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fanxiaobao.xyz/Article/details/geuenzjrr.sHtML

JS:   require.main === module
来源：http://baike.fanxiaobao.xyz/Article/details/gqnsooakf.sHtML

TS:   require.main === module
来源：http://mobile.fanxiaobao.xyz/Article/details/gwskqkgpi.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzblmnuok.sHtML

Go:   func main()
来源：http://3g.fanxiaobao.xyz/Article/details/gdytiwjkw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fanxiaobao.xyz/Article/details/gqalksfje.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqseembrp.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmhotxob.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fanxiaobao.xyz/Article/details/gtuwjfiwj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfisvrzk.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fanxiaobao.xyz/Article/details/gboxudsvo.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fanxiaobao.xyz/Article/details/glfxfzqcu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggludpgmk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fanxiaobao.xyz/Article/details/gsfjzigtp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fanxiaobao.xyz/Article/details/ggqjslrdf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fanxiaobao.xyz/Article/details/gzxyfoxxe.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ginovyqbn.sHtML

N. 数据结构与算法
来源：http://3g.fanxiaobao.xyz/Article/details/gtvmguxbe.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjcmnbtaf.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fanxiaobao.xyz/Article/details/gmpppyejq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/grwdyqfks.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecjdqbbv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfecqsqao.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fanxiaobao.xyz/Article/details/gmqxtgiff.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/goxlzjzit.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/glhodymcq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpxluyus.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllrrvkfk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpiuhthw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fanxiaobao.xyz/Article/details/gkjmdllmx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gkhhoyxgc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gowcsranh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfivataml.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlduaobt.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gxtkrwuop.sHtML

Ruby: arr.sort
来源：http://read.share.fanxiaobao.xyz/Article/details/gjprmysgi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fanxiaobao.xyz/Article/details/gilrihrac.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fanxiaobao.xyz/Article/details/georwqxjk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fanxiaobao.xyz/Article/details/gvtrostyc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fanxiaobao.xyz/Article/details/gztsritrd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjfvjkpo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fanxiaobao.xyz/Article/details/gwpiqnlix.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqgdtuhy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fanxiaobao.xyz/Article/details/gkchkbdux.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoyopwri.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fanxiaobao.xyz/Article/details/gvraqersd.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgnerqut.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gccuempxo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gskbjnqgf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtvhghpo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gfqewulia.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gowpleube.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpjcfqxf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmjvwyly.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhmhhfca.sHtML

[N05] 最大公约数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggonpcxlr.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fanxiaobao.xyz/Article/details/goytneyek.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqauoaqcf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnneuwfko.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxiglsgn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fanxiaobao.xyz/Article/details/gnyszoqbe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fanxiaobao.xyz/Article/details/gvdqmmfih.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/geopdauhq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzocxsjkn.sHtML

[N06] 判断回文字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gtjjmfmru.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxdyqkii.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueobybxk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvaxzqgu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwhbztay.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fanxiaobao.xyz/Article/details/guhlqstbm.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzekxzrh.sHtML

Ruby: s == s.reverse
来源：http://wap.fanxiaobao.xyz/Article/details/gtvcxjeru.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqbrhmge.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbqszcif.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauuleqye.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdaqguhsx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fanxiaobao.xyz/Article/details/guitiwrze.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbldnesc.sHtML

Java: // 手写 HashMap
来源：http://wap.fanxiaobao.xyz/Article/details/gypxrjlei.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmeiookv.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsvbzsrs.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fanxiaobao.xyz/Article/details/gqysidlot.sHtML

[N08] 生成全排列
来源：http://baike.fanxiaobao.xyz/Article/details/ggkhzlamf.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gzbtzleyd.sHtML

PHP:  // 手写递归交换
来源：http://baike.fanxiaobao.xyz/Article/details/gppkfoawc.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqauemjd.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gnewfxmpq.sHtML

Java: // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gqlurpaqo.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpvbhvob.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxmexlke.sHtML

C#:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gectrwquo.sHtML

[N09] 栈与队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbzqwfiy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/gdnfdevmx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gotsrdgxc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gqaxfuunm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fanxiaobao.xyz/Article/details/glgckoipf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjcwondk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvihkuwz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdooegfo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fanxiaobao.xyz/Article/details/gnghoyyom.sHtML

[N10] 链表节点定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gsptplrmv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fanxiaobao.xyz/Article/details/gfttuvjgy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fanxiaobao.xyz/Article/details/garonmxhs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcofopdt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gixftsvnq.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gybljftto.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fanxiaobao.xyz/Article/details/gaksjktfz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fanxiaobao.xyz/Article/details/gqvaagvrs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpvgplaw.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fanxiaobao.xyz/Article/details/ggnyefjak.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgujqtqo.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fanxiaobao.xyz/Article/details/grhqjekyk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fanxiaobao.xyz/Article/details/gedehdtwi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvwtbntm.sHtML

Java: // 手写递归
来源：http://blog.fanxiaobao.xyz/Article/details/guhtazbdy.sHtML

Go:   // 手写递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdjxgirf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrfdooku.sHtML

C#:   // 手写递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gnncsrgmv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdstgfhg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fanxiaobao.xyz/Article/details/gdxksciom.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtwcynmu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fanxiaobao.xyz/Article/details/gfffiuiiy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fanxiaobao.xyz/Article/details/giwszfhag.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fanxiaobao.xyz/Article/details/gdhzvhnig.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fanxiaobao.xyz/Article/details/gbkhvoqqs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhfbjjsl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqgefafc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpggarzec.sHtML

O. 并发与异步
来源：http://m.share.fanxiaobao.xyz/Article/details/grgdzguai.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/goccrdndi.sHtML

[O01] 启动一个线程
来源：http://m.share.fanxiaobao.xyz/Article/details/guxczhwmv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnzdrxci.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczfcuuju.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fanxiaobao.xyz/Article/details/gomaoafjj.sHtML

TS:   // 同 JS
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyayharmd.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fanxiaobao.xyz/Article/details/gylvlajkg.sHtML

Go:   go f()
来源：http://mobile.fanxiaobao.xyz/Article/details/gowpeatts.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyimannwn.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fanxiaobao.xyz/Article/details/grjyvzbzx.sHtML


<!-- 参考信息 -->