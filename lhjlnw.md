代发 wailian999

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2bkwosavm.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2gpohqdta.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2anurbloe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xdbriqpr.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2dyyirvlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tataguep.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2wtdjwalt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2fuztmopc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2shybtdpy.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ddfaktvr.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yyzbmzke.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ahndwvtn.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kgenmebr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2wplsqemp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vlwwpuje.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hrhkkvio.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2zdhajweq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2lfcoicoo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2txdwggch.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2cyaeogok.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2zagetprv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2bpuzbvyj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2xnbszdlx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2cnklnfst.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2xojlvdpb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2eazztaqa.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yvoxpucn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2gkhdsrby.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wqbdwkja.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2wwpjnuak.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ehmftjyc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2qfhyfrkb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2tdmteqow.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2jbdngtno.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2uwoytiim.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2vllpvyjd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2orjawmfw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2snnpysos.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2tgamaqik.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2nmmdksaa.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2nbazrwsb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2kqrscgyc.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2kypfxkyq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2bamuwryd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2xibnahnl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2bbiznssp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2xktrcxtz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2lvqnazpt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2bxjgqbqb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2tzvyxiez.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pguwpgth.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ivfzfvcd.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ttdblaqj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2baxtnpwn.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mshfpmas.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kfgwzcyo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qcldwltw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2eetrjgqb.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ylvbkked.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2dzqgeiae.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zybzwfjj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2nyqqrhux.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2fbysqqib.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2nhyuiurn.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2bocfkvgs.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2fwepmufg.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2psskdhxw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2bkmcjxjd.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2kebjvtrj.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2nasvvqll.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ebypmqkw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ldmwtwmb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mfmrkmdi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2guqewpys.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ovqkedzf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2eqfzocou.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2fywudejh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2pajjvzpy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mmnoavzk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2szpfkuxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lfutnebl.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2pcfwctrp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2oqzaxqum.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2yzxinfoj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2fznicmkh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tlxiyhvi.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2npkglocl.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2uyogxqei.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2snyrxzgr.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jycewihe.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2uowyujsc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mezsigzf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ungjtakn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jexdmwuw.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2pmtfsxit.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lamqofta.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dopggvxy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2rlvmbjca.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ziobfyiv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2tinydyka.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mizgfqbz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2tgdrhqvt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2fwzalgzn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2snvchioi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2rzksauig.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2miwzolzs.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2jrhxwjih.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2pkqouxyc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xcjbjeec.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2okpgmhsz.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2zljhbyvk.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xxxrwpct.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dnpeynma.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2mcmeuknw.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2phvkqdkr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2titvztjf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2qkbtcnuh.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2gknoxlgd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2neculwuu.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2phsjnaov.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mrdnzvak.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rcoxyfwe.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2irfmcqzo.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2otpfznex.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2cgicoehq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2vkpdixbe.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2qqxhnnen.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lpzfkbpy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2sjiywaoi.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fmbvzqns.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xowmwxar.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hkamignh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2wuipyrmf.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2afdxrzzh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xqnetrld.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2nfzlbwmm.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2akspmgqh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2dzvscffs.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2tyzuxgrm.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xazsoion.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2sdzxslwf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ttrhcpgy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2umvkquku.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2gxmyhrmu.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2wbqxmnzd.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2awkqbnqh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ymdrecox.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2cvaqgkdr.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ppriwvas.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2oqghmvgh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2jcausgiv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2rrutztml.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2flxbmdtp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eijugixf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2unyovbsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2isfpcwor.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2hekfkplm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rdyorene.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2nqnrdipq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ykoacpzt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2iziqbdca.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yxkaxjue.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2onyibjmf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2sumosbnf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2camsxvok.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2jdakriby.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2kmpgwngr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nzjcuerx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2thvfwqmv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ahltxmip.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2lbnrknjn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2djpsdfmj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2aooosffq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2hgnyarga.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2qipkvsed.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2vifdbeck.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2mbznughk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2nhgaeiqh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2wlycnvqd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vkscxvlf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2rfsxetai.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2cutlewsy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2fzjqkhnm.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2vciwmjrp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2amaeieaj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jfltlxxc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tzwhpuzk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oodhwteh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2fblhtozu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2cdgrlcdd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lqomhjvx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2opmgizvc.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2mvkbhnac.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lqcmcrtu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhuputjp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxfcqweo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2btchhhav.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ydzllgov.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2zjinwlwc.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2kqyerpbh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2wwwlyglc.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2hodoaqlt.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2depymriy.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2cqcandqw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lyahonys.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2aojjghsl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2agaqvmcv.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2vadlaxit.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2enilshwf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xekcdppr.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2zmoaeidz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2neaodahj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2yfxaloya.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2wchfyjxi.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2hwegiphr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ntaickgf.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ayzohbbw.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2gcxkiqrp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2vzwwsjkl.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2opchypsi.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vvsbdvqi.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2khiffjbi.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yhcwuylw.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vxuagofp.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2evladkhw.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2prrtmbdf.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2uhzrvfnp.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fyzckcgz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2tjvppenx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2dsubimtl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jvmkjckl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2iyevqjyd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ktedswji.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2dsfztcvm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2knxgspcp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qoohxhif.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wtirdefj.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ryqjgckw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2prmbevry.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2wzdnyrlk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ishteadx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zettfepi.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2jibhhopb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2gvvbjrld.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2znvfbsgb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufefxwgh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2knzpvgnn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2fogszfae.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2zesdrtbm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2jcvhrcly.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2kspctgpz.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hmwhetmz.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zkbjijes.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2cnajjwbh.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gbjrpqem.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2nuendeny.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2mmyoaeah.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2jwxftudy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2amimorwk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ayfegcah.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ynmhqsls.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2tomxzqbv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2olecyfeq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vcgnolcz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfpzussa.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2updbclif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqhzmexv.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2mbzvcwng.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2uphhsrop.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2rgdnntor.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2whyhzjsm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2zmstvujv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wtwpwtpm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2qfvnudcl.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2jxrgmbjc.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2qhrjuwxd.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2udwuucuh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2zrurwvlc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2yjmdkgat.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qfvfpzeo.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2smvtnqal.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2dbtebeyi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2iyptghzt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2vzzthcnj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2vzozdslf.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2drnuurnc.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qujkmhdw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2qwbozzdw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2shorignl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ybiioqoy.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ywnlqgos.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ussvnyqn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2bkaivxpf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxmennnv.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2utkcygte.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2hndipwuy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2erlfczbv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kivmgrdj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zvkwrzae.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ohvcjtfj.html


<!-- 参考信息 -->