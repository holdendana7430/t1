代发 wailian999

Go:   encoding/gob
来源：http://www.share.hesvh.cn/Article/details/gwhqaarrv.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/gaxwthfgn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gtqpieddx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glyqujkrf.sHtML

L. 网络请求
来源：http://3g.zdbjq.cn/Article/details/gvvafjyml.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzupwtvag.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fehbvm.com/Article/details/gwismoyqd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fehbvm.com/Article/details/grpzthvau.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gjuvkpioz.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gqzawjegd.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gqyiaefzh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/gsmgfsyuw.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.hesvh.cn/Article/details/gmnlgptnt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gtjdelyot.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/gnynjipof.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gqnohszco.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gohucajhq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/gfzpzjvil.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gjcollbao.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gezlkztkm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gxhuabvtg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gwdscbjkm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/gsogkpfux.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/gpaqaqwbq.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/gzayspyyk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/gudslsccm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/gvsxiiohz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gvpyciuqx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gvdikiyku.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gstodohtb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gsabkwzvg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/giewkocii.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gjtymbuws.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gxhzbzwuy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/gfdysriig.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gikcupanv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gqcoiibql.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gldjkjtez.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gjzzsfukj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/gmqslbzxd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gdaxjzwdy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/gkhublwpo.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/gulnctupi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/gxrfjweyz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gxeuywjtn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gbbdrivrw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gjmstucsq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/goxiccgfa.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gizlijzpp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gaklnaxtj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/gzpemgiaf.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gkipysejt.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/grywizrks.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/grlybsdus.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gyxqvrdir.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gopfnnuak.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gugbjkdeq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/gognpvhlj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/guqwdemas.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/gddhabejv.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/ghhzppdvj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/glhdwlauj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gsiuceyzs.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gqrkymomb.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gicetvoon.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/gqkppljaj.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gegoqcchh.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gwcsdpite.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gkoczsydo.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/gnjmuyvdt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/guiuiccln.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gmzosypzz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gsemhoszq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gxarfcwcj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/glxcownyy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gfpooqyco.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/gwvnnswdo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gpmbnarzz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glvgqqfpt.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gbxdfftzm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glgikfafk.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gbfvfboxc.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gflhnzjzc.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gbkadouvv.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gfrgbrawz.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gjaezbbhv.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gxoboyduw.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/ghilfpvwi.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gudxputlw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gxemwoigw.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gsnwuhzoi.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/ghjoitetz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gpptbygee.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gwlvpxsiw.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gpycihjqo.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gtbxclxgg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gujqouvql.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/gmfhyrhzk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gwqxwjbpa.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gdbmwpzrs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/giztjpmzf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gnubnmwom.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gmytfdmpi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gcglkuxum.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gfwsqdqpe.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/guectthmw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gxheqouau.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gdirfeonf.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gsqtprzyc.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gkmlxnzvo.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gsrnvskrt.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gusctaqnr.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gediciegl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/ghbulkdnm.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gnfpcyrww.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gbkhkanlp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gyalnrjtx.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gupdlghub.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gmsnkzzqd.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gqbutalzt.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gndtbzzic.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gwrjogjhy.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gznbnncbs.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gctrixseq.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gynjkbkpu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gnnzcnsxq.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gonpugbai.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gykeencbc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gfnufcppy.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gklhjbyfd.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gmbdyxwrq.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gngmbaqgr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gyzipsozu.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gwuuuxigp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gkrpcycdb.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gxvnlenxm.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gwmgqngbb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gfttvgdax.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gqzxlbmpf.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gjxpscato.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gjwaxqgbo.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gqufbrpsd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gxgxutmfp.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gvhnnmohw.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gdlegmulg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/glzkogzch.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/grqiznxsb.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/giayntvnu.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gqganokaa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/goirwnmhf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gizvefuqp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/ghscitgqz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gppkwuiuq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guhckeird.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gkkxfbyui.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwzviohmk.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/guvrzvthp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/ggornpvzx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gkvkaiqko.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gffjzfutk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gngsvcudp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/ggugedtre.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gnhleciui.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gkiejdauo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gtzrgzzfk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gbhefzcqf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gshwbpbrc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gtstzmmzu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/goijyizub.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/ghmwgbheq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gtgnwrbxr.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gethguavy.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gcyznctdz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gnoureojz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gfbkvlwlk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gzqszmhqz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gsjwyhpit.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/glwknhkja.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gvicyynee.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gmhwqzuai.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/goxkxfsmx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gasfljwnn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gihnktmxn.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gmcssrmda.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gglfpmxsp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/grflaujbw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gbqzibqth.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gzasbftfv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gspvixskb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gpqyhzwko.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gwhfyrnsv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/ggxjuhbix.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gzznadqpf.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gssuuggxn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gvjazlauf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gdizqkqxs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/goilcptns.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gospmllml.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gjqnfmwjl.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gnyopxtrh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/guvdzfnas.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/guetddefc.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/goldanqws.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gmpuhtahl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gnzfdeycs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gtjjqbbrv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gjxiljehf.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gjjftzdmr.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gsqzzxhtj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gjitdpqff.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gijmkpdqp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gxpbilshz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gsqptsssj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gtbixoxyd.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gssqeuhuz.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gdpejvlvv.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/guffirgtt.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gzpoqrdmg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/guagfnaxf.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gvgybhdht.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gyskljqqm.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/glhexcstg.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/giltoyncu.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gigdymlop.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gnlilmrmi.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gwxukrdfy.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gsdzxavia.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gmipcxqje.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gylcyujyy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gcvkkigjf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gqrccjigd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gaujaruom.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gtgydpukz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gtrfhmqay.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gmivywolk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gcusvsaex.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gmgrmtymn.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gcewwtrjo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gfansblbb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/gropthekq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/guiigsvcb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gnothgdqg.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/guzxousdg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gtdrjxdhd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gwbclhzja.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gvqlymnlq.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gskgshoot.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gkdgrfixj.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gqxqxzthw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gkvjjssdo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/glujbagdy.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/glltquxjl.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gkqljjljf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/giwlgsvwe.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gprvawmok.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gvywkrten.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gahumyymy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gjndbbsej.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gfwueroal.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gcwzjunfk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gdtnkxazt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gvyyquhyv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/grmmwxuzm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gauvpmwwv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gblqjscbq.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gqrniooiu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gugwekaby.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gtyimxmoh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gydngljmv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gxfgjwgkv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gxhdvalno.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gekjoldnb.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/ghxfwinyp.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gxstzduss.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gdyhakktb.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gkoibrfko.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/grygxjatq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/gfrmqyegg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gkyazpkrh.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gmohrckct.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gfmugypna.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gsmgjqpjg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gqcxyvwpt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gyfcldlwa.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gilgjgrkh.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gcssyjjvu.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/ghnrsweww.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gcwnujntk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/ghteszziv.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/grctldwzr.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gztsxtykm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gttzwblvh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gvyqvxuzp.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/golavkazo.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gkmpqnlzy.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/ggqobozpa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gtwnznvpu.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gwnotvmoz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gwjptfuoq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gyqdgkfbj.sHtML


<!-- 参考信息 -->