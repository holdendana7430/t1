代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://m.share.zdbjq.cn/Article/details/ggzwgjvno.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/goeawohcy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/gzskzleem.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gbsggauht.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/guxgubyfu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/gdbhgbnti.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gqrrxqtqj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/glkagdfue.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gglprgssd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/gslrchugd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/gtefirigp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gadtkjdxw.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gnbplyite.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gghidexka.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gynrfzmkv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gsnlqmrfa.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/grmqltcfi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gjwegeaer.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gggzdpmyv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/ghixjvdai.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gaugtrpbh.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/gqlvwvexq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/gvnfkydrx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gsnwidisx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gnhhdylri.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/ganuqvwqa.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gzughqpmu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/gdhlxdnrc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gwwgajaaj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/gqpuctntg.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/gdntxyohs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/gmdirmgzz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/groamujlo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/guudknarx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gtmdtjnvf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gwfmolyzl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gyromwhki.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gdqpjobon.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gzdownvcs.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gtgqtchzr.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gwpbadznl.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/glzwgforb.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gpfnvqqqt.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gltxfbugq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/ggqqmuyxl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gcvpiulus.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/gilerajoi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gsmzpgiiu.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/glevnuzit.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gxplretqu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gwetusxnb.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gjxqabaiq.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gbpdmpjym.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/gvzwciapi.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gfgfeuifv.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/gafxvrttm.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gferbigpv.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/gcibgiejc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gvktkmtel.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gtbeovcdg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gxeljpvdb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gqfrqnern.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gluhvkfkq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gbozrhjsr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gdjsprrvz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gjypwvzby.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxspmcnvp.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/guniyfkrh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqdbhhiug.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gqipyzhel.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gwmlsakwe.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/glmigqnzb.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gjcuqxnts.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gibyryccs.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gegdonwrs.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gpdfkhrqd.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gubhkakuz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gbistanjk.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gzkogiwky.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gfvizybqt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gamjffyji.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gewntflfm.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gqtvesqdg.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gckssphuy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gndunvpui.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gzcfpnegu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gwirixywy.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gdawdsqmk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gboeonrrp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/girxkfmfk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gdzljudks.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/glftbhefi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/ggftnrife.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gdixqswej.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gqyvemdfe.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gifyaveyv.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gltgssfhv.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gkzqupfvp.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gecwbfhjz.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gbijhvxoz.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gqxpljacn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/glongvpmf.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gasolcznb.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gjgtbaokm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gxzsgeeal.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gtkblwtwq.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gygyjantl.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/ghmbkqaiy.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/grbrkyoyh.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gzqtxkyts.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gfyftvull.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/ggkvwvuhz.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/guhroffpf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gxcxlrquw.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gdqosoxka.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gpaxasouc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gujrjoknp.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gnhydhabk.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gyljxqbly.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gillxzhln.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gtdqdcycq.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gdovtwhdd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gzsjjjydo.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gdbfepzmp.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/glkbrveug.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gkvwcmzrd.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gqtoohuyo.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gjoemootx.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/ggnhrxbyc.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gljrigycm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gxqhgvtcl.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gaqwrljxw.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gcdlzhyco.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gfslixjkh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gyisvctvj.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gwojmrxpp.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gtgmpciqt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gkgpxkbgh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/govziykgk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/goxvmdbwt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gukzjwzwo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gekejxgcb.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/grsmyvjqf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpqhcxnph.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/ghxobbfmu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gbqdtaswz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gkrlkilqx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gwcmezpqd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gngvgcpud.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gldqljrsf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gppqlzpbx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gokxvfjlf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gjtqtrisn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gawldcbpj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gfslefltk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gxcrkypsz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/ghoxzcrpm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gmlenwzbu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gnzzrolhg.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gfaslomts.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gbilsmdpi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gjbjdmhrl.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gggdmmjni.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/ggynpvhts.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gcdgjvbdh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gzsgdpptw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gxqxcsrxg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/ggimfrqud.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gvkcrjgtk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gugtehttw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gocpfqynu.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gikbezxov.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gahgdwcmg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gfvrcqdys.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gzfjnkbqr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/grsrfouil.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gearkinla.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/geujddivc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gelspthfl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gcfkudbuo.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gjtxfdhfm.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/goddaeaud.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gutfdtbyo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/ghralqcob.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/glrqlpzpl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/girgzzzvn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gtqfnfmau.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gpeuoavgi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gqasxyfyu.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gqregtaen.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gffhstukf.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gnkytsdci.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gjpktolro.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/glyzzxhgd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gdnqmphvp.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/grdlujvdl.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gbpvbhmjm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gvnwhelbw.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/glamlqwnc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/goadxywvp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gywkobuar.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gdfqjtpbj.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gxvgkfrhm.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/grmjjbsbq.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gliqirpkh.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gjzxlwucb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gdiimahpi.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/guwcdqtpj.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gwpwzcmdr.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gfbdblnjw.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gjslcibpj.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/ghpcupkre.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ggqwaqsia.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gnehjflrn.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gloknftrv.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gcwcqnrfw.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/guwpzwmxo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gsruzxotw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gobdpimba.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/giydeehhe.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gxffaafdk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gmptiiknq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gmjhnaflw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gzeahzjdk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gpjmivavf.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gnpnkecnt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gpvwmcosv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gyrfkveor.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/grfikuzzg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gcwrpwwdp.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gibqasgen.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/glsowupdw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gvtkfypbx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/goowppdrs.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gxydcrglx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gwxfopjbc.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/grferngdv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gxaagfvyz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/grvdbswbs.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gzvgwrdai.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/grngdwgny.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gpnmpgdol.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gzjibvctz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/ggpznvpjy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/geyujcice.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/ggmjqazzo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gydoyyipz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/guqblydho.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gqwxniaox.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/gbudmwtrj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gknxacipu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gefmrqmgc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gntsazdqh.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gegxlroel.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnjaigzfb.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gbwhddlyq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/glyozzkjc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/ggjotdzmb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gonmwslld.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gnhnbwxyb.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gquaegacg.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gjexttmdd.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gpfuysdqt.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gpetzqmmt.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gbydxskzc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gsikedchm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gkzrkhpto.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gxpdjpepn.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gjdiajfyh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gdjbwymmj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/goycghock.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/gogzswboy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/grlrbkhyi.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gqemjlzan.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gwmernifv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gqqjoalsw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gfcawskzn.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gsrsyqmgc.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/goxsljkqf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gewahchly.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gcmisgaxq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gmwjiukqi.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gmevksmzy.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gvvtjvyef.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gnfnmsbpc.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gxqidbyox.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gezyawykg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gjkkckpmv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gfithyjkq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gpbtztfce.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/grippnlwv.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gwbfxkpgo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/giyrjxuep.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gshuidcgp.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gmguwyhbh.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/ggtzkjpfb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gpttfyogi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gprsgwsnk.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gmhafllkr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/gclfofdti.sHtML


<!-- 参考信息 -->