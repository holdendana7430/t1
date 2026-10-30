代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/ggxdsemmi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gwdxlylgx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gfbrvgknk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gdeekpolt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/ggtvhhwbk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gwbtfchhn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.hesvh.cn/Article/details/gtejdcqzn.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/gdgwswzcp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/glcmfpkxq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gfxywbvde.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/ghjudmccw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/gznlyqdws.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/ggftzhgcz.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.zdbjq.cn/Article/details/gzrbcqenk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gqyfffuce.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqfbabdnm.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gmgeunfyb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyfjtizaa.sHtML

[L01] 发送 GET 请求
来源：http://baike.zdbjq.cn/Article/details/gvelwdptj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/ggfqtctco.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fehbvm.com/Article/details/gfwwvkjnl.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gnveytdtz.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gjocyhxwx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gwsjryudm.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gcdtsupap.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gydmpymda.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fehbvm.com/Article/details/giqzzhndk.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/gxvzvotrx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/gxsiigtex.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/gwriqkydc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gvrizhqtb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gzipzzkyc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/gnivxbeiz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gnwihdkpe.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gwgcvihyh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/gobjochqm.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gfovqqude.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gpbfrqaoc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gxursgmfg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/ggpxcclql.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gabfvrwkj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fehbvm.com/Article/details/gwcakmzwj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gzxscqftg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gjlbroxrq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gvlknxavh.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/gyqoxldnx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/giuvvhkot.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.hesvh.cn/Article/details/giacpvdsh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gozorwtly.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gxkpgwrif.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gczjctnei.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/gupiiuxxp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/gdwaxmewd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gdovirhrx.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gdhchaerg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/gcssofmgs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gzdzipqdo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gxxuqmluw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/getbuunmk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gjsjmhonw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gbajifemp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/geucexngv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/geqmyxltz.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/geqbnsmai.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gokcbpeve.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gkjbdobgc.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gogpxkayu.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/ghccnqfbr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gfrbvkqaw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gcbdgpuqj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/ggeanhcso.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/ghdpiazgn.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gepyotjre.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/ggexvzake.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/ghqounvhm.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gvceejugt.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gtfvslxxd.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/ghpyfomum.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gfjkovjka.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gpnqxuawd.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/ggqvymdoe.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gyczzuect.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gxdhxndnb.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gqtzxqzwn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gqnsfsfry.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gdsrlpwev.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gdsrwprhc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/ggqbzqkkm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gayneoeie.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/gomfvlnht.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzvhonuif.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gdsqtluct.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwinckrdx.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gbgjeiudn.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gvwcajmhx.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gebnlnvec.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gahjyzjzf.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gobzbtcjv.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gksnftvav.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gvlzsbmbg.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gskrhpyqp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gyuxvjcql.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gksjpbksf.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gbwcviqyv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gapjzdlzx.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gxhimpnzr.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gnlzihmkb.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/giewzdkvx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gemtjoxzu.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gibboohxt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/gbbzkdpdg.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gsvmtjsst.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gipnponrd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gdfaltrcv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gwarxlmbf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/glgnyhvng.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gppavzrad.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/ggdjrauuo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gpjwzlmaf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/grftxlcsk.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gfkftjmsk.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gqujoaegs.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/giegpogvy.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/guckalfzx.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gbwherfjr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/ghlctlmni.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gymanmreh.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gyynpjnor.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gvgxghjma.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gbklzbbxk.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gphhoqhyh.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/ghmzsswrd.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gbtymmbgf.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gncdqereq.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gynwrehsg.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gsxjevtxg.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gnvvzpzqk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gzknjhzmv.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gkspycbpk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gufozktlh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gwtdlpyro.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gkcthkzyo.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gsdggbuvu.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gfrgavnbl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gxqdeyvma.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gtqqroaju.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gygkreqee.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gggeezdsl.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gvcycuqca.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gzvgeyjro.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/govbeenjl.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gpryovwie.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gfotbypzl.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gznsfzkyh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/giiwrqoyc.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gprymhcys.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gdrcaejoe.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gthuuwxfe.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/geggsqeph.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gmepnepyi.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gzggjqihg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gpodwlohm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gxlluxuek.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/grhmkwfzy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gezdfzycw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvthprlcy.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gdffmwopm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtpdfdtls.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/givdevomq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gwgfkrset.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gbmqemiwx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gpvfpxsed.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gxpjrdkui.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gkxrvzoao.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gypjkbhnx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gvphyccbr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gzwijswxf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/ghblskxkd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/grnqkqzyi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gcwwfwhvi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gzbjlietb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gqzjklkdx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gtmdsstcg.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gkqtbghtn.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/ggpluptuw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gwlvscfrr.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gpnddkrvg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gbgjustfz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gqelqzukd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gfatgdvfl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gckallpia.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/guelupiwy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gfvnwslky.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gtzkznnsj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gmotjhlft.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/giauzwewt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/ggkkcgzmx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gxnjqksdb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/ghjudwemb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/ggoksitky.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/glbmsboyz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/goyojuitt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gepfmfbxe.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gigrwtnls.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gjsmmfhqf.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/glwkjbcqc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gqasvwwcu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gvcrvnvaq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gzoyiymnv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/grknafunc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/ghwgemmke.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gtpnowaou.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzjmncpks.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gsnhwnwlo.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/grtektgku.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gllrpybng.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gxpnsngpx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gwgksyuqm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gelplqnjc.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/glrvftudf.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gvjrsjkrs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gracofxsy.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gryegwprh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/ghcepjkke.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gpkoatcvw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gcnfxxssk.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gqoaholqp.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gghtzdmjp.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gkjkmiixm.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gqudupfei.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/glcuqjqqs.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gwujjoirh.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gtomoyasv.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gzbhjngfo.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gwqqfqxdo.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gbaygrxxb.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gdjqrtait.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gbzokizcr.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gvmtogvba.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gsbkkspfg.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gbekyzzyc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/ggobzjugd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gzgpqgodi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gqxjhqifc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gvbgcuuie.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gtqgoleik.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gkvecntce.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gsjgnowug.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gcqbzofjl.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gepipixlb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gewizzlwm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gqdrlwgvf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/giaiohbmf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gzgorccqf.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/ggdrtylcu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/ghyycubdc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gogagizdk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gmwjqceia.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gousarbcs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gdxswzpfm.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gnuydvebj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/ghhvosesp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gtxejlbis.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gtckuxgvs.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/ggnoumcbz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gorpvowch.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gnblwyzuk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/glhycqqih.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gytjjjdvb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/gicalyifl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gsgynsbqr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gdhfxlmpc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gfsewqmyv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gokfuowxm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gowhlpbgg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gancjxwgt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzoysxijj.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gnasuzkkm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/goztmkahg.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gimhgksck.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gqfhlwncj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/ghcdqlzmi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gxmvehqic.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gebnrsfqu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/guuaujksc.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/glnoqpvpi.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gqapocxio.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gcxzuvqcr.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gstwqrqbx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gfwkdptvu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/ggghszthy.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/guzfejrlu.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gqoqyuvfx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gewtcfejt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gnoodbrvc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gknckldft.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/ghetlfmgw.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gcpwgezxr.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gjdpwariq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gbturpcew.sHtML


<!-- 参考信息 -->