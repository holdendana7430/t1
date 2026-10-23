代发 wailian999

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3gjphdatk.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qzzxbxqo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3adklmhty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwvvonvt.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3tedagjyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jrncpqmo.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3eizhzstf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3apjiixds.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3wpdxybgh.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3dkiisaza.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3qvwuhsop.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3wapngtcw.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ejrlgcrb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3mkoejdre.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bljxemfq.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3cicqqyiy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3urahaadc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3vizrowft.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3gafznjzx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ipvociai.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3wwotrytx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3nzjligfg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3rcgkilyy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bidwmjwv.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3fuirjbej.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ipslovsx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3loibcbvy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3oehzvmab.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3xjacsqjy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ttybwflg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3mwndacio.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3uxsbbucc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3vmbtdrgv.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3afaoaodi.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3zxylxuoy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3tuquyovw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3sqnzvvsk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3givmscgf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3mnoxqtbo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3basxtihn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3ckhajfat.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3yfxfmsgc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3nhfeoocm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3myyizvip.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3tgembawf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3gcholefr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3aqkyhmuj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3dapxvayw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3puahcexz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3azjflirl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eqtbrnqz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3irhtaobg.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vzqtzhbl.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uctiozwi.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3olgdygzv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tmlayxpj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3zumlxjyr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3hwcwhwll.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3wqwhqlor.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ozrirtyc.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3jgknszqe.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3hxhviuit.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3skevsfsz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3xhwzjnnh.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3hlftdvei.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ewucgfxh.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3lfwoqqwr.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3xaltjsaw.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3nlmvbymn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3wiwsghso.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3dwyicloe.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3hiifonur.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qyfvtgcz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3glfteids.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3spofbumw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3wykuhupq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3iwmmvtdm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hwbqyhfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nexqsxgr.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3yyjvqfnu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kucjzpgj.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3wiagxxng.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3igzewpwq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3pvxoexqb.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dffztfic.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qeepbboe.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3njekvxeq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kndrxsns.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3kglsrqku.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3boatmgwa.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mhiboffx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3shtjcnde.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3rgfxikpw.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ikbvzieo.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wrvmktld.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zjwnsuer.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gqyglfqf.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ztdlfdby.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dqcitrgu.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ycsoytwh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3wtgtjkfd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3isekiucc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ggkgblez.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ojoyczed.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3dwpwpuhl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3bptwdnrs.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3pjyoualx.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ingsibsv.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3joupobzi.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3exfivhxx.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3hdeilcot.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3isccyfkb.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ogsuvcil.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3kyvtxapk.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ufsiyarh.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3fkwqxusp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ofvrkdfj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ierutqts.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3imumdcnj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3dcmqepzx.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uhefosnl.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cwvvkanx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wseeaumc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pngbkhux.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3fhnrgjju.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3obbejpfg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3mobviphl.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wahmygqn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3kjanzknx.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lcftremo.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3izpwrtgp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3iyctxvbf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3bqxwjvhe.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3xdencimh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jmymyqar.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3uwuojevc.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3qdktoecl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3hezthfvh.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3hbpuobep.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ngxmsmqi.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3vvktlkql.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3omlowlmh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3qcfqhgdt.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3fauiapkk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ausyxyks.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3avvnfmzy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ziycjpqj.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3omjieuai.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qelhmesp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3gddnipax.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3twfgadlx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3sumxzetb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3eqhnyylp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oxcepdmh.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3dwlruizq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lahhmcbt.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3seznnxrm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qvcfaxds.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ujpcmnbx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fywvfkqf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ufmyaalm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mummyfnc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wonydxhk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3anyezmfz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uzdsstsh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3botcuyzg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3nwxyzehw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3nocozkwj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hrscgija.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3sesixgxa.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3jgqmiidg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dykrcchf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3gzjhvoiv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xvcoqudo.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3itllmjow.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3rwnvuurf.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3xdtipgjs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3numsgifq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ayfdcukl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3tdmgquhg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3frsufpij.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3rzvjkxwd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3tgashmhr.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3mwkpzzby.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xbsvsmfp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvfxyfkc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fkrzsmed.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mpuohxig.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3jllknhgb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3xxlscadu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3qmtpjvia.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nyrdjvhv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3daykgglh.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kwjugsxc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcknywjw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wifklpui.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcvpbspq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3adejfogc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3bvukxktg.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3tcfelkmi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ptzccidl.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mnlowzzg.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3czbmhkoo.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3czrugbvt.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3unysvpgq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kxdaycjz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3pcglalbp.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3gmhstpbg.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kxinzthg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3rqkvgvtd.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3lmtsgtmb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3rrkukati.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3vkjxfnpf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3suvpkwyu.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3eziyuuvb.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3luxpvubz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3vanaeafd.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3dtqcvdbj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3rucjeibz.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3pbvqnlyz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3xnlntpyl.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3xktodzxw.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3srnofiyw.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xleudzws.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uvcumwqt.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gyfbismf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fitipxbo.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xeelhddd.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qkvmdpnu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3grnuubcs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vhcczszp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lptazafv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3msuwrisq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3lqgqikon.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3emhlzton.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uznqkyew.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3pehwfous.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3yjxezewj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3apvkaibd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtajkjck.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3quzgfgif.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3dyvtdjki.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3jzsgvqih.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ezjxygzv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3mprdkhlw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wuzcowuv.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jipqrone.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ogorgjbi.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3vlusqxal.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3lzydkmiz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3akpifdbe.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zdjrkuqf.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yrxqhrvq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3znaauxry.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qqrysvbe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3hxmygrmf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3imtyltts.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3wlxmwbwz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3cuvcgwum.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ghnzlypw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3cfyeloen.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3tartttcw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ctjcyszr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3hhnhdflo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yfoymapn.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3iwuwfqte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jtzxlzxt.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3yorokovo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ieqzxufc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3grpyepyt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3hdyvxdda.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wdivnkep.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3juafiyxi.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3wmplwxja.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3kdzicvev.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3zhyjijam.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pboflbqf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3negvwlsr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3masdrswi.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lngtybav.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3rmygbndc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3oyiudgdc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3kfayhafg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3paujecjc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3xrysrhyf.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3rmysbufn.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3exkhicbh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ghhhyqdx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3gkvdrgkm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3yxqpvmie.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqctfxxg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3pljopusd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3gyqafcao.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vccbhodi.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3jsbswomj.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3qcuntjka.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ufwqvgkt.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3rtzxwxmm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3rzclnjwb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3zrxmzkdt.html


<!-- 参考信息 -->