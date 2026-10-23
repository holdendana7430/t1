代发 wailian999

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3lzrhimin.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zhvakorl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3dwkdjeqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dufutqba.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3fwjfasbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3monhgyfy.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3nkxedcqv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3nuzxkcew.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3fphffvnh.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3iwleysqp.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vjvycdbq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3xioynvkf.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mahkeqfc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3wpxmdasq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qtyihcgy.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fafhnfqr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3bmkdlxvn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3fbtektax.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ffqhgscp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3soepvncn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3frdozwxh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3vnttesft.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3pvtpphsa.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ifmdgvnj.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3krfpznfj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3jkpmpobh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3cvvfdtxu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3pxvzooce.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3samvsdyt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3rqvnynin.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3qiwoglec.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3jpukcvqy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3qjjdxkgb.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3goiunxju.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ombzkmjl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ybntcmkb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3othuvvor.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3xtsorxbe.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3akqlzxja.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3hlyspgnz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3purcdrbn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3hwwwyigy.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3xrrzwvnt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3gguywjaz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3nisyubbq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3mfnmbndt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3hjgmielm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3wytsxizt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3mxlxgewn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ltearysj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rmeqbfhy.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3stjsrlvc.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dnxlgaxw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3iwvzperd.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3aafnasac.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bvaxcgev.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3heftemwe.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ptyazmvf.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3qubmxays.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3acwvbekm.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3kzaqcqft.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3hjhswpnr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3btrkrpxd.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3nqnbgvrm.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3hbmraeja.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3vtcwrjnc.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wusimcua.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3qzftzysi.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mzjhsren.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3fvfvmhyq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3yglibucj.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3mavpwwnp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3iuygmlme.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3thxqpdup.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3jqyginei.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3cfjnctyj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3dbywsnom.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bhqabczz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qopvqklu.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ndutmxhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ecrlfxhk.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xudvvubb.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3lulalxkd.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3hxhnxnms.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3srzudmjl.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nfhxozki.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3dyyzjwfq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tcjqwdnx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3sqbvsolq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3fpmdeyjg.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ixcuvtwj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3prdnmhdu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3cxcvreev.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3gpwzwpkl.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3yyfbwhvf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mknkdvxh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qfzeqwyd.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3zxjjuvcv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ngindruo.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3qjifjstq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3qtohbjwg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ihrcpnat.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3etgsklev.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3luucoqgp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3iioylmcf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3rypfrkji.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3azdqiqiw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3lyxtxzfn.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3qlhbagdr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ylyxolhl.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3bdkmjdyd.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3lkguezww.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zhtkkira.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3styjljiy.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3yeybjlvy.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3kygpwbch.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3lyjuspqv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3qhttlvlv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hikttayn.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3yqxjyhdc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wfrzscwb.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tinxrdug.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3oxrgptqh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ptuxeppx.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3duaiutih.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3xuurngve.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ftvoctdb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vuxmrcid.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3yznskgjy.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3uobmezox.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3swykxcms.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zvowpixb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3bptusxly.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3rrfuywzu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kijqgmjk.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3kmkpfnck.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3dhdwbgst.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3cvxfrguk.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ojemodtk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3otjcelfq.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3bshpcmbd.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3elxjjpsl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3lfqznuwi.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3paihdpjk.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3xjzxmvtw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3hgojztbm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ffswvzpu.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3rxoirsct.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3yxhjmfaf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3mqaomtmd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3kzpwjniw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3cpghcfoc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3jkatnbbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hzfypigt.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3gldoyrny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3glzxoyhn.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jbrfhezk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wmjwynph.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pldcpgyt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ydjbcexv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ocdqsyet.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3irqvzrxi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lhkcfvdu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3kkydisax.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3glapxbmm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3vnbkkjwv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hjwhrbpo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3rgazjdld.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zggaahwt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tdxhxrtu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3qmnwabgs.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xlwyesqw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qhwvdmih.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hfhciijo.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3lycxvbfa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3wnczvnzq.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3rsaecsju.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3rvnacfps.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ogwtmptm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vzdbjtvg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3nhtpqunx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3lgnuwsvi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3lvhsiupd.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3knqlurdl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3umsldxgm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3pprdktpw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xhljchyu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bagyband.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3mqxrkklo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3lcmgrigl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vfletgoo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zrmbzcnr.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3vzmjwncy.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ncqycfvf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3opaagalz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bumucttb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3jyaonbuc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3krccsudv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3mpccigme.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3kvsmcwks.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3cghiuhki.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hrzcqajy.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ulmopyfx.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ekiqaqkj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vzpvokqk.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jepbijtd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ouahvvhv.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3zggkywfj.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lhveasno.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qusijjeq.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3cawzinpb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3kyiexsji.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3izmwswia.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3wdxhtvjp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3pdijrtlv.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3iteusova.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3nsotkejz.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3dbguikrq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3uluzoypd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3mixqkedb.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3dkdxmazg.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3izqdcxgs.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yrwxkycc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3avyjhgfe.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dcbqjsgv.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lmtdbpce.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3oghadbmp.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nohijtnt.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3dhbjtdoj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ozdrcabm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cowrvfet.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ajpsfgkq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3elntyqcq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ooljxqqc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3sveywdxp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3befrabib.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3adtfdvqy.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3cisntfam.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3yvhsgojr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpvhljcb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ynvjvknr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3jlwxliwp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3iqqvwvnp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3morkvaqa.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3pfztyozg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3yypscimg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vjpzhfza.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3kcoujzqc.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3tfrxtebo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ihwsrnkt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3caiscihc.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jurewreh.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fmbrtyei.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3emiigbqx.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tcxdwafx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3aonqcbda.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3smdsqcbp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3gusatsyn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3jpprjamt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fxzyayyx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xxymkxpv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3ujequlhp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wpudcpvr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3oitawuid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emxsqkyz.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3mbfdtlng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhfgwdgw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3eppubaeu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3rqaafhqb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3xbhahyed.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3uwtqexht.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3krsgbjnd.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3lqpznhlm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3vmhnwinl.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3opgviwgw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3zxodqvot.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hfzwjzyo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3fsyjzmet.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3tibttwqu.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3whzxdlyj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3curlnwwn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3zezqtcwe.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3kjrocopn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3romyjodu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3xongptqq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3gsywropz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3fsweapqn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3hrtpfezd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3exqccxhx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3njnfbhku.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3xgpenxwf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3maxrftlf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3xmmnblou.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvoebnni.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3dtipibjf.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3nswmdhob.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3yhwmxngk.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fklzypdk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fhixrvuy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3xvmihmsj.html


<!-- 参考信息 -->