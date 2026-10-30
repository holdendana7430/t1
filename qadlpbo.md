代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/ghaacyydw.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/glmhpjmxf.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gedwoyirt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gznzwclzv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/gdjvryhsq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gdymgclzu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/ggbvfjwis.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gjtxatmxn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gvguaztlf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/gsfovavxj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gxsbhehzs.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gkywdwhsi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gsgspbpqv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/ggvrjvcvw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gaqafzter.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/ggfddbojp.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gmvbqbtxp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gyjdusbpb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/greyiubdm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gwdoljdju.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/glyomxbzw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/gifmdcnuz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gyezcmckt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/gqskmrrww.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gucxpjbmp.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/gilejjuqx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/ghiryxpot.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gcxapcouo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/ggssghrem.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gusnrjchb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gxlpenudu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gyowfrjzc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gayvyykbp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gvgzmlwce.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gkaduxnzg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/gnpwcpfzx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gwbycgvuy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gbluwvjob.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gbsmueegk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gduvyiwkj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/gzdiesbzo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gmlldbeea.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gdtlpgkxd.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/gdfrnxuuo.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/gkhzyahbw.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/glixmsbrm.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gpahffeul.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gmevykxpy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/gfbqbzrbn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/ghteigjqi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gdnajjvsu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gyoqcbnzt.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gklfskrsm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/gekrvncri.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/glxoakgsi.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gvsepitew.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gmwuxcvzc.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gbbpnowqi.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gkzxkxekp.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gidgoeqmz.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gjcgmkxon.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/giwqvyise.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/gukxltbjr.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gegivupgu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gptdhnijp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gfokkdhvq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gtyjgflks.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/ghufqhpgw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gmmctajcm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gfnjhtdxw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdvarnbjs.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/gwrteoqkx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyornlaof.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/ghswkuxrd.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gtepfwsqc.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gzcqecodu.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gseynkfpe.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gnadsvteb.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gyapdsruz.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/ggrzgirnv.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gwcsfsnwu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gizzoavfl.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/ggkiztogs.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gcalpvdqs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gqsjeqafe.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gnafqfzgd.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gfegabwll.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gjobqfzgc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gwbazilem.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gdaiffrmf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gglyglutw.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gzlboqmfy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gjxzppbyy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gzflalyrh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gubvjfwng.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gngriheqx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gkltrsvya.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gqtzaoexf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gqrecbldm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gcimrklzr.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gxnwtajtm.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gwrbiauct.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gfreyatyp.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gdfvvqgrq.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/goennnrrk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gksanmfae.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gnvaxgfjx.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gmysmwoal.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gselzgums.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gfuqnnasf.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/glubckyjt.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gsqfexoge.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gpbifcdku.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gdzfwdnfu.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gmavnpbwo.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gcscocvxn.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gqlmvcbvc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gnyryduhw.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gdvhwwkhe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gclgwbjjm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gbkgivjvl.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gynpuxhic.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gnxnuqpdz.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gshueohke.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/golszyegc.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gwzswjtuq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gbtxbouyg.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gvridnmla.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gbtdxbpvi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gslaiposc.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/ganlbtbsj.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gtoqntenm.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gybbkovot.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gbqjmbwyf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gcemzmcdi.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/giysmhziu.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gwyhuvhxh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gkbxlsops.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gktjdhtsg.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/grdtxycki.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gsnskdhie.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/grvyqrjrf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gexmskaie.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/ginfyhrxk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gmtbvtvhi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdgrucjdf.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gynrmndvx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gffhkpaev.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gowxaqtll.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gcnblpbwx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gdymangxt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gmabgtzvy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gnhywcojp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/guwtysxqz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gaaxnihfp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/ghqwhaypo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gzztulugs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gopriioej.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/geykcmret.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/grtcptoxn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gbofvvnpj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gkubcuazz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gnugtdgmf.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gfjsmejpx.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gdcshucyi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gxgsqdzff.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/giifonlck.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gjejprzqm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/ggasozqyt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gfudgutno.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gbxajfino.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gjifisaan.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/gkiaizwrt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gcigcgeqy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/giqusszpe.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gsicyttqu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/ghjshxhcj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gunezdnqs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gilmezyve.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gysybrlvm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gbkbwbnqo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/ggynsnygu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gprsmjcqo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gybusytqv.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/glomppppw.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gxdqgpsyq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gnugcptvg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gmvsoxdfy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gfoxdrowi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/guhiccoka.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gsbfbbtfi.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gybmyoqug.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/glqjzlrwc.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ggaanmagq.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gxqgeeifd.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gisqhumnc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gsfzsmhxz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gnzlqezfr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gpgpxnfze.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gzadewtnh.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gashmnxsn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gfpnzykjt.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gtgnbcshm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gsstsudif.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gmwyknddd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/glyzhpfnm.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gvylobhxw.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gjusmvdxq.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gbmwgblbg.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/glmwnaiem.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/glkoeqauo.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gpfwjzezl.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gjgabjfar.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gfmtiawpa.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/ghuinqxje.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gsyfxahyz.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gyhghiosf.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gxdypzrjz.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gydiarone.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/geqvuyuax.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gnwrdpywh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/goaubpkht.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gwmccutyt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gndndnnoe.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/goyvayfsg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gyewxcezu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/grizcjmmu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gfntsaupz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gcwtaubtv.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/grbsctfxk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gbeybtmwq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gttelbkvv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gbqzposfg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gwtpjyiwd.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gdfyenkvn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gnvnjsnep.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gdnrzkuyy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gmcvbeupf.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gpkkbuquu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gqkbuypmv.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gsugyhucl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/goxxaihoh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gcgxggehz.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gmlpwwrai.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/ggkpgrktz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/guchwdjhd.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/goshhlumc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gehxqnjhb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gaiatazyd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/ggtxlppwa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gcbjyylri.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/giclbgpkw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gqbmocopb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/ggtucwmjk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gljqtvscj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gpxfrycmn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtjmxfpet.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gyblfecqr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdpfohfga.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/guocctpqt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gvxiahtnl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gjpzpadep.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gckxphehw.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gmlcyvqxx.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gmjyhjreg.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gxgzguvvq.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gstagamvg.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gzyzxozuy.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gmmclzpxz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gthbrrott.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gcxwvadcf.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gzsnqjlrq.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gwkylppdt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gnbqbenyt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gtrtwibrm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gqgmteayo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gzwtluqwd.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/guxhiqpup.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gbdvilyse.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gjzvaancg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gelsoaxqk.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gprswkptm.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gnmuijull.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gznojsojb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/glaocyacn.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gxidbftgw.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gpzdijnqz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gtbmiqbfe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gwhdbkozg.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gllfmhyon.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gtqhoahor.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/glcotbvuy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gpxromkvk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gkwwhhvyn.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gxlbslxup.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gprytusxj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gtexowukx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gpmzkyqsz.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gcgscxvlj.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gsjbfzavl.sHtML


<!-- 参考信息 -->