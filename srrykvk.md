代发 wailian999

[K06] 解析 URL 查询串
来源：http://mobile.zdbjq.cn/Article/details/gxwegrkvr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gmfzpoojl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/gckphvzcr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gydmzmiev.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/grdplgobp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/galcgjoxo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gsqucqbxn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gcezkqkco.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gtzalykcc.sHtML

[K07] 进制转换
来源：http://wap.hesvh.cn/Article/details/gpbjwgbsu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gvayzckxp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.hesvh.cn/Article/details/gepwyzajz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gcxtdpwzw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gxziwnksg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gnfqpacak.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fehbvm.com/Article/details/glvxavurl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gjzmkkbcj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/grxnihokz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.zdbjq.cn/Article/details/gygzueqyx.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gzxxagfwq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/gvhjuyxmv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/glbtqvail.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gxxwtxoml.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/ggjdlsupy.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/gcwpfaytw.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gsnnqvson.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gfvewlkwm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gilmakign.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/geuxoorhk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsrljtwyg.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gvghhcrza.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/gpxzdvkzi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/gjbchbxhr.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gyltmbsvx.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gfbqyurdv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gjqcxxjkc.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gbjcpukgy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gbpwkjrqk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fehbvm.com/Article/details/gdjpqgblq.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gdzzkhthq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gmhynhiwo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gnnngdewg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gaayddzkr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gmnerqrvy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/gjuwljmfy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gxvlllwes.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gloeqemke.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/gjeypmpyi.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gwjhavhqz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/grlaztdqe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/glxwakrxl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gotavcnfd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gltszcxws.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gbgohjybg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gfooqkozc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gcjmkulim.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gvwoahyut.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gtfotyrju.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gfglziktb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gtbgombyq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gqufvzwsi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gdtgrigel.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/ghttxdour.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/guqvowzws.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/gxpcqwdch.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gbjzospra.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gufidpbcs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/gwpxocrev.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gihhegzfw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/goimnizzm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gkctbwqup.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gcdsxyvcd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/glvzhakyh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gmejcozxl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gpxyazupv.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fehbvm.com/Article/details/gssooumfk.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/glwiwncbg.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gkavzruba.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gyamcwgoo.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gfohvelvg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gqosdskkl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/gihneqimg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gplrsgbll.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gbhstrduz.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gbteytrgl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/gyviutfag.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gfipdqdbt.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gmvbsknjt.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gisbqlnns.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/glfepoxrp.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gnafvvbvq.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/glgnyfwfi.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gzhbkmxxp.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gneitogbf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gdsgijgyg.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gptqpgxpg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gaqbxynux.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gqesgyatr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gifhdlmkw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gyfhpvlln.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/gafumghmi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gunraqqpt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtxtsuitr.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/grpahofhc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gegriabcq.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gnhxvkzat.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gldsesdjo.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/gkzisdkow.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gjwgccdvm.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gennyrvhs.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/geadmuprw.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gkuqhnzaf.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gdoodahaf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gvxofqfiy.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gkiapdtph.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gfmdoodib.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gzcwmrqgs.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/ghjdtibnc.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gfnzcrlwy.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gvrpgaaei.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/ghgbtponc.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gvfqppwsg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gfqyultwf.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gfehpwitd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gkvwnnkae.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gutjgambk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gnxyyhmvv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gylodpibz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/grmdhujgv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/gowmswyou.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gnenigmld.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gwtwvpvoa.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/glwezaxhl.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gvyblykwe.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/geazznmrw.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gqkkrresl.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/ghxalqmcb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gipplnaad.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/glpjjeets.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gzyfnarpy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/ghcbplhav.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gtunvlhrk.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gyzrwqjtk.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gksuyejyg.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gluexryub.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gdaiptjgq.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gidujimcf.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gkkwtqmib.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gpqanilzr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/guzbfcfwy.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gduaiiybp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gfltoccju.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gykiguiay.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/glihlqyio.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gedzxxhad.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gqrvzsphd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gqjjxflzo.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/ggyefinkx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gwaysdrdo.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gkjijvxzm.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gdvxniuvn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gllnbsutc.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gtizyqbaj.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gqgsglyig.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gvkzqdsej.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gyafbsfdd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gukyrvmzc.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/ghutqnldk.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gsdbbcnpo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gpdgwqcqc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/gbvvmvoso.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gapvgqcan.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/giowmituc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/guosqnaqe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/guxpdlvup.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gpjopjzbo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gtfqvkcxm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvbepfbng.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gpndcrptk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyoqsgyhv.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/geppcivbp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gmhyzghil.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/greciwpda.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gwjeweprs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gejbyxnfz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmaoldlpb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gyxljmdfl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gzqpdmxta.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gnamhjdyi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gfwublzov.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gubrslfdh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gdfoffpgx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gquwqeumz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gjxxjonvb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/grayyrrzc.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/grrejviqw.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gptbwxdme.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gbextmmmy.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/gotwwbffz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gclvbbiqw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gemeuiivz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gprxhqgoy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gknxcqysu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gxoagozrk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gpcqhuyqk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/givbtdmfd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gcgxvzhms.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gahbkxvmt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/goexesmtq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/ghyzdfnea.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gyhkqljsx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gntkhcahr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gnmdcbkyh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/ghfjvbwzq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gyctiefpn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gctwqbdeh.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gkdmdwmqi.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gqetxulvg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gcxnbnbxj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gkyamzlmu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gniyjthky.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/ggjkbbrhy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gfzlkczji.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gpujpvokp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/ggjahxfpk.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gdnkgbhrs.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/geojrcuus.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gnfuyqhwx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gnugwfabd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/geitvcgxc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gdpcpjzft.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gphgrbyly.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/glgrgyxiq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gtispanvp.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gtcitncel.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gepnucuht.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/ggrneweav.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gplcqldog.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gkxdnoxxv.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gmfvhhvag.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/gyxscibda.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gkkiheboe.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gujiejqca.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gukxwbvly.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gojsulhrm.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gwhwxivio.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/glvjdzbhh.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gmlngrtsa.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/ggdxtwwyt.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gnulvtcdz.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gvmapywns.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/ghhnfwqnp.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gvuamribr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gmpwcpvsc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gaobsuosj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gqucgnido.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gbtfezbuu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gglsyjilk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/grwojukgw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gqiagsdqp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gvobsmkfo.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gukqnxjgo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gzkzjknnt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gxfapkfdk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gfoqdhnyz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gapofaezk.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gxmqiezhj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gcsudogwl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gcknohijc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gtqzzisaw.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gbfiecnal.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gkvievfxa.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gzunqkcmn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/glnyhjiee.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gaidcoebs.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gsrbzfilc.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gumhhqkrg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gukgzxzjw.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gyymbabii.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gzvozzsva.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gtvpvcbvz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/ghjowpkxk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gpnakhlzd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gkzpoviej.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gzexxnaxd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gfdifcaxb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gdtysujrv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gouzbvedn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/geoqugrhh.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gnfbypcvj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdemoytaa.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/ggbqqncgg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gazyaxxdw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gicujuxaa.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gfrwndvnd.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gviglwoto.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gykkiznlk.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gasjeeliq.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gmbpivbzh.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/ghkkntcje.sHtML


<!-- 参考信息 -->