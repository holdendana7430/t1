代发 wailian999

Go:   encoding/gob
来源：http://read.share.fehbvm.com/Article/details/gpjvbxpjc.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/gtxpuwmyf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/ghetibxcf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkihafrnd.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gwtyzapxy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdgrzsuue.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/ggsigdyat.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/grovyrqpj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/gzsfnzkoe.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gacgmpvzg.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gjwfvtwhj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fehbvm.com/Article/details/gjhdncsxf.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/gutfpaxtm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gpqqgsdac.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gdmdnrsam.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gxqwabvsw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gzdnhvcon.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gwwjsopli.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gnituhrlp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gzpgdpkvu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/gnylalxsi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/gcgxvkgth.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gchohfpbp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.zdbjq.cn/Article/details/goeesjwmo.sHtML

[L03] 设置自定义请求头
来源：http://baike.fehbvm.com/Article/details/geavwqird.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/gjaxpgxhq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gidbpszfb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gzbhadkkl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gzppkrpvq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/geskvvhyy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gisqnyjlt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/gcepvqrlf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gjngwvwuk.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/gajdiyoxj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gzjgeaqsv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/gbgzwrauv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gkacrbkoo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gnxnlvrmp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gchfwzgpv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/ggdgsuphe.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gpwhcmrag.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/ghwiffapj.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gimtpcfqq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gptarrvhr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gxzolusfv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gambblouq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/ganknofen.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gsfspbxbo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gvqffygeu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gpfvhthpp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gxstkshgd.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gwdxjbgww.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/geflujzsi.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gsjabvnuz.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gsgtyfitl.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gjjptvbjx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/grmjbchpe.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/grolozpsi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gaqpxesom.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/grpvyyshu.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gznepyngn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gdqtchtxo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gofxrmxpm.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gsdmfsuak.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gqaxxrxlz.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gqhazmicz.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gthvaooho.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/ggghsjwpl.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gzdbeprzr.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gyphowimu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gbyffmhsv.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gcbsmngnz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gsrbecumm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gpnpupyey.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gtioiqgwi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gixjfrrcp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gduhczksi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gmxsogdjt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzuxebaif.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gfnsgpnrm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gytamgnhf.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gesycmnry.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gsuumdtfo.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gdpzrrsda.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gfqzwpnqs.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/giqzzloik.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gouvjzbji.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gtbgmglee.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/ghmzzoute.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gyfcagutx.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gggblinaq.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/galavleut.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gfbmwmzzc.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gskwekodh.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gkqdilpbe.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gyxgawydr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gmmhkrlxf.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gmjnowkcu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gdrzlfykt.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gxivurofr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gllwkqppk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gevhczrlr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gzyptgvsm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gvxhcytoo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gvkrgwjzd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gzexyzmns.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gicgoqjnv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/ggjrsjkze.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gmaznlsli.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gmrzppfop.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gmzycrcyr.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gveuogqwk.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gqgzgyyvh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gspknzlxv.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gkowsvorp.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gnyqlgasl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gqxrrokcs.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/giqygohdp.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/goeumqbxo.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gygyzedrb.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gpovandyc.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gbsvhjzqx.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gsrlcxcue.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gblljuprv.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/glsjebwcz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gtnzhufje.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gdhyjrgks.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gopqjkhdj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gwuxdocyg.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gdsjufwtq.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gavqgmbpj.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gmxljtrdn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gratvwugu.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gozdavxmj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gurheoutb.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/geiglagiv.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gyxazqkou.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gzooppawq.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/garpubxbx.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gubogtjat.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gbqessrnv.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gbhqlxccb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/grbzfprbd.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gcbefbigg.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gsgvapjze.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gwdxmzuhf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gdkyzfeqk.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gjoryjnwj.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gwrkizpnd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gpjdiwngw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gomkoyrzp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gbadaomzy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gsrkxbqla.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxsndebom.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gnkgmfabe.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gydxhniho.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gygdwgfbg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gptfnpsaw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gequjigfw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gnmtyexml.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gfprtgzhk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gimlduobr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gsztrsftr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gsuagqhoc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gldylqvjy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gljqacvmi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gnqgpgtrs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/grubwbbib.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/grkzalwce.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gvkmfbkpw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gfcsaaajl.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gqiloudnk.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gytwimuks.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/guntqduon.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gilzmrzgq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gocaygbir.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gdnroxaig.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gpcbswaxr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gvmwgtjdz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gtaalonni.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gbbmnabkk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/ghvmvwppk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gwfgulmzt.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gwrrltwmu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gvmsfpykp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gesalpfwp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gplbmpiav.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gkepifvqg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gsseesuxo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gnzrrbhhh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gafaoqqed.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gxpxgiwjv.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gwmdimmzc.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gpwqkpysa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gmoxbxjfj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/grbobcefb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gfadlqzvq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gvvuvjnnt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gjxcmqlnp.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gmdqirtrz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gpdstfpmt.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gtlayamww.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gyipljajp.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/grfwndrdg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gtrdelhmc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/ggweofwyu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gfbwvhqcv.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gjqjfdvsm.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gpymbzwgf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gcuzljngk.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gqkcoewfj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/ghujagpue.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gwqvayajh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gvqstuywl.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gnewvwqfq.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gnmkzcrqn.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/ggitzbbhm.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/grhllbvlf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gnihfduum.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gqelquiqa.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gwqwdhogn.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gnidnxmoy.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gfmpmskjj.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gsylcfvxq.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gfkzrxpes.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/grgjpcsgn.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gysbkqjvr.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gqiborxqj.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gcpzembvw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/gidanplwd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gspydmiay.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gzowdqsyx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/goydmblbl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/geexfabau.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gdctcxsji.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gkxwubgpc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/grenfqoxm.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/guepekwhb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gibnjbwuc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gsgpqhvqm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gpkiifhpz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gadyoobeo.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gjvvdfucp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/geuoadnny.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/ganlvivaa.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gitjuyymn.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gfguwwxrf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gfgrbvuma.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/grzzonztt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gvbezgthu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gqezjsero.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gmfwbgnlr.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gmzstixnr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gqasjobeb.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gjadfojyh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gcobfkldy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/giaevqgbe.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gskjnvmyb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gbippqwbb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gybisiqbz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gybcdcerp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gcbmiybhf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gmhwyrres.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/guzegqkis.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkcxtmccj.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gjzbbbgul.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gelerxjvn.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gpwjylhzq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gyuntzstz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/ggajswubf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gaafysuyu.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/ggtqwqlaz.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gafsbaxmw.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gcggjujab.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/glyrpdcbu.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gouxuuxhh.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/glayefagk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gpcufrrfw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gemopsszb.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gitwnfywf.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gfktqqhjn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gcylcmtev.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gogncvegi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gjxhcskya.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/glctawjvt.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/glersstyq.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/giqdnwquc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gshcwrbpl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gpsbastsr.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gkvnpzjgd.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gygslslqe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gwxnxkzfr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/ggyhpqumz.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gishxmmen.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gdoqirecd.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gaetikxvb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/geuzhnpjs.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gqiooqfts.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gmmampywy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gmxxixkoc.sHtML


<!-- 参考信息 -->