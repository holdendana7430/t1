代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ugxaywmv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2axsawobq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2bvidvnvl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ighabohx.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2irmnshuh.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bkyvnodl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2eyregnle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ifqekadv.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2xepbllut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtvkqest.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2ptjeejxq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2lvwkjxhb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2yhqmvaoq.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2goiybnvt.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vqybsvdn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ggkavmfj.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hqtyzrrc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ztvuqyxo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hsucahuk.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2hfbnpsty.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2pybjkhlr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2hkkdbudh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2mffyhcqk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2xmiojyzg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2avrcqihk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2xnzvvnzo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ianthfte.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2qlhowfbu.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2cnvcwonx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2tkblhwet.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xlzfwfev.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2igrdrbul.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ainnozts.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2hnuocdnl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2dgrhmzjo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2vvjmzpib.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2zmthjaoj.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2yqbwefbj.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2sydqimxu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2gqotqfof.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2lliewswo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2gzckmsuq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2buitpika.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2hrqzkwvs.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2bqjlkyxl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2rhjgayxx.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ppgpqwvh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2twysyjlh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2zgicvdrv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2shbthazp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2txwozfds.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2sibguwif.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2nttjzrxn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2bkhfxlkp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fxorjreu.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fkgbsrmr.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hwwtljcf.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ypicwmwo.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2odhrnrju.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fywbwwhn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2vdpkaokz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2valvwwrk.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2usvbjkdl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2yejliewi.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2llfsjlls.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ohalzsio.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ycqfwmvp.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2lemquvzd.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2obottari.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ztdciohx.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2kdajqcue.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2oektpwhm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2jmuwelyd.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2fmgqxznw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2mhslmqvu.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2opunanzc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nrpzihkw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2netfgnyu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2kovkubay.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2flaukrcd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qmzbymbr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2lbliqlxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wvdsbrej.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2zlovlqhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qrzmcnje.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2tedevjmv.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ndaiocbd.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ieedtziz.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2nnsdpgzu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2eqjyqoxw.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bvjmnias.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mofqlznw.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2rigdmdoc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wnjodhhq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2iwvlwzho.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fpgsolop.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2pfbhizsg.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2czgxdfhc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2gudytybe.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ugqkyjqd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2scwuuojr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2jyanchaq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vhypnegb.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2bxpqnjym.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qrpkpmmo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2wwewyubb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vzdraywp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gmqpchct.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2kfyokcfj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2sbkttmsa.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2mtxalvxt.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2bknjncxk.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2wxnfujfg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ttfbjuvy.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2dodplktv.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2odssahoc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2znsidmfu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2fyktupwt.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2oijfsgjn.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2zykxlomp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2idgpjzbk.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ledtwhfx.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xcqpzvha.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2arvnwojn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ukakrmzz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gywmjxfm.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ntrujzni.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vtyiymdm.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2xrnmajrv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2pbeudaok.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2uzuhsxkg.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qcgicpsf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2wjccufci.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2sggypvsp.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xtvpghnw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dpfwaelm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ygnxszrt.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2uqbwdyir.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2qdtsrroj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ndsqrczl.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2bbiqiiid.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2iunswhqa.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2cikvsjmw.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zbxvhtna.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ezwjvndz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2gggolwen.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2qxqqqpab.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2nlghflpn.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2tegbqcfq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2vylnupmf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2eorcccus.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2dougfozx.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fwvzqlot.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ufxikyij.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2bziluxnt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2wgiivnxb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2mxksfukk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ycgoascf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ufghljpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2euiztyva.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2qftndyvj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ngnxhgcs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rcglzgjs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tmewflom.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2uubrnhdz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gpsqatwo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pahalamd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2fiiigudc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ftgtvnhs.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2cpjncjgg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2sioqgvwx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2sefmxwbb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qqvhxroi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zcpzaecr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ygccgdrp.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2voiumfft.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2sgncbdfi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2orexesyv.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2qwhsmntc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2lgfuzgdk.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2xmnzujda.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2eipwrwsd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2exaiwhtd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ekgispqz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2tyesnjrh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2vxadnnin.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ueqomgqj.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2umvduefw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gpcdhxsu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2gflzuiyu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tnrpnqop.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nkxatqrn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xztbkwdu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2dzgvuvzu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pieewbei.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kqrembvi.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2idzmqvlr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nlrajhao.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pegcrgdw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xehgzato.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxubhybv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2pkebqwlx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2mkxatvqe.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jsbwihyj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2edjecsrp.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ptofcdlm.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xsgwxbmr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2yvcwsrao.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zyzicwsd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pbpbuxmq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2cakbdsdm.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2mchjvigf.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bogzsimp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2fotmgzal.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2kyjzkqzy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2vipsqdhj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2bxaxmrbg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2qymlbwdh.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2vwsmhowa.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2pnxnlvzd.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2jwqsdzss.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2yskvulmj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2wvoxxcvl.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2exyyjlhm.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2izpscype.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2hrmqzbzj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qjqufnri.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tlyggwrf.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2khncklfk.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cfqhtlks.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2famwhdvn.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cbrrnxoc.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2htwjkjtt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2sgkkgohm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dfmtmaec.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ohdrvrra.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ubmfezkb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2dtrswiti.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2limrfifs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ecewecbc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2atvxllhd.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2odzfwefp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2grrydsno.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjowiniu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2sayccpat.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2diqggava.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vglnwyac.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2qrjxasnp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2fyucfzbi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmwotnjt.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2zfbunsus.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2fmbzbtdk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2zgpuegga.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2pkwetoxl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2bprruxiv.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ffeehcgf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2akytbcbu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2vbfdmngl.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tgrexbmx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2mkirilvq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2hqiohaub.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2wpmdslhe.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ingropyx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2gxcghtaj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2idwnlpxw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2pmqjatik.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2hoiyiukh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rinulxkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mioxfbjt.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2djiqznfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kccqlozl.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2mludgwix.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2bpqvafhe.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2hrtzwlko.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2idrimqnd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hajkwffw.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2pqpsefwt.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2daqxjrxs.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2dlswgesw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2imumrzkn.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2uafpiraz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2qevtfuhv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2wghksqla.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dnxxyonv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fzgxvviv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2fqyebqfl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2lvufrwli.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2zekosyha.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2igchttsg.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2osmrflyf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2pyxbjayg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2uxdodsuv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2vyuuwlrj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2zilwbhdv.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kryozgpi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2tlrhdbuc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2peksduua.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxkcompk.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ezbgtkwi.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2tgsnsrzt.html


<!-- 参考信息 -->