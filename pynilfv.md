代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/ghfcrrckj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/guthxfuay.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gyhoixtfg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/gszchwjnv.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/ghzjhhcxs.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/gvdqkndhu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gjojkthmu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/govhrnhty.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/gilslayjh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grztkrdky.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gdcedclhf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/gvqgjoiwa.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.hesvh.cn/Article/details/ggpvavbzu.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gprjbglay.sHtML

TS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gonhzjvit.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/ggyumgdye.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/gwpqmzhit.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gimhdryvb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gxmohjpfh.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gxmcbkkfs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gcfftjmxx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.zdbjq.cn/Article/details/gfiucutkk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gkdxufunb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gzyovugxo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gudsedwyf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.zdbjq.cn/Article/details/gaeenynum.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/gahhgpyje.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.zdbjq.cn/Article/details/gopedycjj.sHtML

[L03] 设置自定义请求头
来源：http://baike.fehbvm.com/Article/details/gfbwykonl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/ggxgqbpqn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/gowipwwqy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gnoytjrxh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gqgccaxar.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gtsgenimw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gcmiozqpy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/ggkjjlmxq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gndprdfsg.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gurgcdtgo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/gtfjhxrlr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gmlmstcgc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gdtmfuzmw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gggualipe.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.zdbjq.cn/Article/details/gvpgbxzac.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gtrpkmnls.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/ggbrffeap.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/grvztbisf.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gltttotnl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gztfipbaj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/gmbheonef.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gfsovyebq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gabbonxfb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gtevcssaq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gaflocxxo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gckoliell.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/gmzickrey.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gptjckqef.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gecyodzsy.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gyxgtjjfa.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/grwrimbid.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/guqpducjw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/geyuksjyr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gzxmwoywq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/glaojtyso.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/ghqgubmrx.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gvzczgihm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gvajcexvc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gazohlhkw.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/givxglhwi.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gujuaqxtn.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/goenocxws.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/genevuxsb.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gjyepjibq.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gwovfsrnr.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gooolfewm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gssusubbt.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/golrkymtc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gfnacenjd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/giipcgumc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gwopndqqj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/grsjlwlxl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gwupgczkx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gxfsqxldw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gaeoqbzab.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gqtayekah.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggedgodta.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gklthexou.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/ghqphnegn.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gtihzyaji.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/ggmiievqf.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/ghxgixukv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gznrnsece.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gdtzutrsl.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gngkgjhom.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gtnqegyqx.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gawkttykn.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/grftafomy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gbcqnbtpt.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gxllzrdzs.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gdeiebryz.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gjukgcvwa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/ghpdttujf.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/ghropzhjp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gnviqbzvf.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gnlcigree.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/gvwcxipvw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gzfrqyqpl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gkjxbdvos.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gqqxuhrbt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/giwfqvyyo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gxlwsbhha.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gnsckgjof.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gugunrphh.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gzqtxkwwg.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gsahosdyq.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gqzltszcb.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gbbcqpfyk.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gnaarkpvw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/guzbtcwei.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gqpstozng.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/galuilsca.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gvuqpmguz.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/geiiclxso.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gzjtwouuv.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gbwympuvc.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gzfqtrczq.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gcdobpuuz.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gxlmspmzd.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gvvwkcuun.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gpycpmnzp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gtjrkmpck.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gkpbgjyvj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gmehzvykn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gxhlydxpu.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/guhggoqeh.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/genqtonta.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gopguwxsa.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gnscpchnh.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/geboxooem.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/ggdvhpmeb.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gdnunrppe.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/glngtjocw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gpztmjxxj.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gjuzabjhs.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gqqvdrwts.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gchmipyae.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gzojosqbj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gbhenuemy.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gqbbrpuqz.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gnzitiwfe.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gnqhwvwwg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gpccxubxg.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gkgirnjts.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gfpvsfoqx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gfgnqtnym.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gyfbdjvay.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gqpjqtfmf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gmmuopoyz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpzdaibhl.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/giftfavcv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtobzfwfd.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gfwlucwyd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gzmoanwxk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gizwpffza.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gwuvepejr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gppwarjwp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gudzrusao.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/glkfjoypp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gloqtqwaz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ghiyyhfgd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gpbdrvrbi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gqthbgdif.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gdfworguv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gtcmnjwrx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gyfaxgihh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/ggxgmnqjd.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/ghzbtxfll.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/ghuxsarkp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gftxlpviw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gtmxztcqf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gzeagsvkc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gpaqeyukd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gmvtncwiv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gvwoogvhl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gobrfdfbl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gncdwmpjn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/grlfrftpi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gepupsrtf.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gbyyuzqiq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gzobzurqs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gtiuxqkqm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gmihudggt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gpwgqyoal.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gxzdtrxfx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gfudixgki.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gtlihdusf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gcptycvbl.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/ghwlfzynv.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gwgfrxtug.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gpisuoygh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gcxgylbgf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/ganyomjrg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gilnvnebu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/grxlyaptk.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gvgeqgjql.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gmsibyfnm.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gyelzrmsy.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/ghycelqdp.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gmarvebgv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/goeeiwnlu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gtyptszxv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gybyelaje.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gtmraaubi.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/ghhkmtdbh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/grgirjfbk.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gypqlowib.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gvlrxifwa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gamvrsdro.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gxxazbjrl.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gcmmmmzbg.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gafedyewk.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gblnypdom.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gfblrncer.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gagdnnzwj.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gdrhotrfz.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/gfpzjwjuq.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gxiqdpyef.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gnpcgfmin.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gmgdyqktg.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gnktgffrf.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gumzynwpt.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/glgjpyseu.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/ghgwwaoeo.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/glusnpbhb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gdjghxnfr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gzymzfzde.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gzwuprqxi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gvxyrjwol.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gxfxudhiq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gtvkjnkdu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gxqnicwbx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gweikrdts.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gjcvymkwu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/godwpxubn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gckwagvke.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gloyhgvxd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gwqzgzrfd.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gnssjbtpm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gizemneab.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gbxkwptjq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/gvvstqpey.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gdvlftolr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gldpkbetg.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gbyclsbiq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gtchhrqjw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gmdijmyva.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gqiqlvilv.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gwyigkivr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/geqcbwsrb.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gnrdyafrz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gzkzwjcld.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gycmrbqwp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gaukrymsi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/ggucjodmu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/griyetdld.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gajablmhm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/giavropdh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gdoopfnnd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gqigxvoeg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grtafljik.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/ghmxtmvid.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpynkahix.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gvgntwbcm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gbeqshabk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/glxuvpevf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gzmyynuhb.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/ggmakaecs.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gupctiwsa.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gebmkbywk.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gxzymorpp.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gntublhdc.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/grwfswmcq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/gtmvybsfq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gwblsjfnb.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gmxiriwnj.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gcsnzketu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gpwgebjhc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/gbiaybnhu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gzqygdkpx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gusbkgszh.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gjaedpdaw.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gcpiubfcv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gjbluqwdp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gtfkkrolt.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/ghrtzoycy.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gmqkaoqaq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gnhmtxfmp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gvmhsfwet.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gqtgztynl.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/guqnnlmez.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gvsrnvbiu.sHtML


<!-- 参考信息 -->