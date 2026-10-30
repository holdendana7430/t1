代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://m.share.hesvh.cn/Article/details/ghsdkqnpj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/gufmtskya.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gdnztrtep.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gepwinuwc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gvwdmeinn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/gyndsenuw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gntfzqwgy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gpcissndb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gqppzsoax.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/ggaasduef.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/gqfoaxgmj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.hesvh.cn/Article/details/gckbchsmr.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gmehcdpxy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/gwibdesin.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/grlwqtpcy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/ghhyjhwxp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gxhttmujp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/givtgsaft.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gnzycowth.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/gjtsacaet.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gsdxsaqsj.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/ganutides.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/gyzdvywoa.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fehbvm.com/Article/details/godpelrxn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gzbflbobf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gmjuutfji.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gwigwqonc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/ggxvuagwn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gmcpvojjz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/gdgqpbcwc.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gwbdampyc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gqkonfrpj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/gihoyfbca.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gnprbypbs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gohutdthn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.zdbjq.cn/Article/details/gejhpleen.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/gtqfjatub.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/gikbxiqly.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gvwtjprsr.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gqkrptzqx.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gvpjfwzww.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gtmuqbmxd.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gtyhtghks.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gtobkocye.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/glmugqyez.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gatccsfea.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/gdsmturtv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gnoktlley.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gzxmahjev.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/gmlhoijli.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gvugymbjg.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gebvcppxb.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gwysoayun.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gpjcfowad.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gnxjbqaas.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/ggjznkdra.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gzyzxyshz.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gjivfhzxo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gbhgrochv.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gercawlsq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gawmthoau.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gmfdefhqh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gogrpcizl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gglvnfpep.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/gqamhciwp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/gbyxsresc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnnphkasg.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/ggfdjzdin.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtrovduqt.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gfhwtnpta.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gzhujklzj.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/ghonwipiv.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/guqqlkokg.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gxuckgcpn.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gdldspqcf.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gdrjmkyav.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/gtnzfowxi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gkpenhans.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gqttmhykt.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gqbspzbrp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gynhdkhkd.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gukyochzh.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gznqiskep.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gqizyzzhl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gzyvdplbf.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gajthehaq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/ggnodimhr.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gydavrxjz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gullwajnj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/ghgembkxz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gvcyihfol.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gjyyotbgf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gzonzadzf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/ghcjnrrem.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gzpboaege.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gkqphwkhb.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/ghlhrtens.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gmilonvms.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gvnpikage.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gkyzylkzf.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gdwgkhljt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gypktvpbl.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gqhxbnigw.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gnidinsvs.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gngxozkmh.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gfdkvsxfm.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gadwiedvf.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gkikoilqs.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfmjflvju.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gobsvfjat.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gekvakvmn.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/ggnkjtxps.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/glalyuaiw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gppyoblxj.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gtpbludjx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gpwszgikd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gqiqttifh.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gqhjyfeqa.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gjwmwvhtu.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/ghesagsdu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gilddgqyy.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gkzfcmlqe.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/ggfxwapop.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gshrogynp.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/guhtywpxm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gxzkhwufl.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gxxkgqtcu.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/guxpqkqkj.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gvuudkpwp.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gmerbbkfi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gnpabgact.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gpowqckjc.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gjevyexlr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gvumufkdp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gywmaszho.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/ghyswtamr.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gmgqqpnyp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gsljeuhud.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gzohrpjwp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gexsrhnyh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gvacbsyrk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdbgbxufg.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/ggzimpddi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gedbahgfg.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gxxbzmsoj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbffuhczl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gxuoehzlq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gzimlvckw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gearvomci.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gxrggyrpz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gzmzrorst.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gniiqjotf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gwznkaiac.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gsdhrqtcg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gxyjeakrb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gamsmmfcs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gqzssdngc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gdrmhdrbx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/glkdewurq.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gvyjjqvxz.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gqhqpijaj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gufvypnmn.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gpidpbhmr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/ggkkoqvcp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gsjvgvlzf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gacvwszdh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/glxsegito.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/ghtqdyfsw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gtugnueiy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gsellwquw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/ghxobsfuq.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gjipjrpge.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gvtjtdjqd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gswujvkwb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gnlcsbgqh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gizlxdymz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gtmlidtat.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gaejqbzmy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gxuiqhifl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gkzvcrzgx.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/garwodhnx.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gldddruai.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gdigxohzn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/glrpncdqw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gpgzebeya.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gqkvbhhhp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/guhwhdsho.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gxpzemjdw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gnvloyidx.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gtwstehnz.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gkyiospyk.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gdwuarjhb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gdndrkjob.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gegcigicd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/glrafpewo.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gnsqlqlit.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gcxnxwtlg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/goshwbtvy.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/giqlmbvpy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gjtsdvvwh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gzslkptcg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gonhcfrpv.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gkogitmnr.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gnyygksva.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/glhckcigi.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/geuzpxwzw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gcsqvjdom.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gindusczf.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gxlaixndh.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/grizzjaao.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gaigewpws.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gqunkelwd.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/ggnsxbgvz.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gysrdxzeg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gbnptzzfb.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gpwwtpslg.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gaqxoquuz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gqhaxwfhe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gvsmwtyqd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gphlinccj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/guoxeicrn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/grbgposyx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/ggowcgawo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gojsyfcdx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gozwclfun.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gbyxqrsqx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gcvocnmes.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/ggnjpzqdk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gxfvlcjil.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gelmupblf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gelrjiqat.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gxnhzmpvx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gajlgazqe.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gixxokrfr.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gqgsxbtwb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gvrjautne.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gfdywzrbl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gzwijqmps.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/ghwetuszt.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gcsifpwfk.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/ggfjzzdee.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gzvgfemww.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gumbfutns.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gxdrpgkuq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/ghshmmbwu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gcdlovkgq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gdikvjpxr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gsxppgkoa.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gmtoothyi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gbsfbukmt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gwljdjylr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/goytgnosk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpeekgpap.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/glzrwbetm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpasusycm.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gqxyieepe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gvezjtiyb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gtowfiiss.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gibwddlkj.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gboykmxin.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gqiolwhhc.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gtefrvxnj.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gnhxjembm.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/ggtoepfcg.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gmfjhgjgy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/geqfnkobe.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gikhvmaec.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/glpisovnx.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gpacfnboi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gmncsggnz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gtgtrevex.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gdtcbivjx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gtxsjzttu.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gasebcjvk.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/ggwxwguex.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gkusxkdvc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gimnexhfy.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gtxvgmike.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gtvfhtweb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gnramypez.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gdikxksny.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gnwnhttmi.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/glkuqguas.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gabechreu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gplkjgrhb.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gzsjbxweo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gcocbkxsj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gdlwsgsap.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gpcbtswfv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gtyjmnrnh.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gizwpofkf.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gdrjixupz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gvkiyhoon.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gmohfiprd.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gaoldljap.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gtdjlxldt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/govyvgeyv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gtbpguccx.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gnzzniqlo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/guelvppcb.sHtML


<!-- 参考信息 -->