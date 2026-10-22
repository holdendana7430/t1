代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2flvkbvbj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zozsaqon.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2dybsxfzf.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ffcrcdhh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dyzyteto.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ppdgiarl.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mhzxqshr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2erbvvezc.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2svghibih.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2dzwzcvtb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2qvzreutk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftofyffm.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2fuwynogw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yrtdaple.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2ghieodxk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2sotfzhfb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2mwbmcbwe.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2shujlovh.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2dfxtrnut.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2evtghiwz.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2imnnwmiy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2bwvuaaok.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bqodoxzd.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zthbsqnr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2bnioeqpd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2gbbaqujf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2gphpdpnl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ognuzwbi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ntgzdkih.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2kuwnzlux.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2vsshmiqg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2panklexa.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2jdfvomdg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2shsotunl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2smmspmpe.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ougtiwko.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2lufyxnpl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2hqgtrrgs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2hgikihkt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2wsvxpcoa.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2elciscgs.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2twncenkz.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ewtssrym.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2pfnhhryj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2hqxalear.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2yedtjcyj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2frxkbeaa.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2vhmftfel.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2bqkcxnto.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2vvsannau.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ixotsfoi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2ipejkuwe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ylahjjzj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2fivzzqqh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2pbxebods.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2jtptnvbf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2bzjjbqlx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2qreygvuh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iwbvtyqa.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2gqdrndtc.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zlslgcoz.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hivfaxot.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kngdufck.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ixhyqghf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2wlqgfyeo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2fgxxbtfp.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2yyrqzjxh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2oonblgay.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2guotvmti.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2dcjucqoj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2cgmuqmxq.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wuzxtrhf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qcyvdzjo.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2iafyavih.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ybhjnocv.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2dlaslswj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2cmocfdyh.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2scynhthr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2dgubkfaf.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2oefqxvao.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2autnkyaq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bgistvvz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2enrcjgcr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2mrronmaq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2lxzvhfrc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2kuvmvdmu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wygexfvz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2oahqxrev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jcwbfhtq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2erebratt.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vaygizjr.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2svpeszxd.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rpnicrkj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2wmjteejv.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2crakllut.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2gjxpusoa.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2jusvdjwb.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2mfzxyrmi.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2zawkdwpl.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lrhzrbpp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2goovczos.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2mhahpqdn.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2dfiyazhh.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xbxgzrvd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qyfaxsic.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2coqvjfot.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2evoqylty.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2zxmbbppm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ejkjxbra.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2xpgfmild.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wcygbopp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jthvjzcz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2kqdacfon.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2eauwnhas.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2tlttjwwj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2fgqyytin.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2mwopsgsj.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dsumcpjg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2bkzyefcb.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bosdeykx.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2aydqytog.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ynygpxia.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vcbxswrd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2lasvtiey.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2xxdnmcub.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2lpdklbvb.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2drlowqok.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2odglqnjt.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fbdsdrvg.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ydzegyec.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2axyhslpx.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2adurubyv.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2abatalch.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2zacqgsdd.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2dcmpgcpf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pfoyogxz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2gddczonq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mgsquwiw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2wopaysnj.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bxjnnaxv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2lnftntlb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ezcrdudm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hnnvkjgt.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2reimqplf.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2xrsepayc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ctdfjrwj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2cjteuqsp.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2drdjcsml.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2hduvbaqz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2wxjftqiz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2hpiourny.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2smyiauqc.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2apizvkqw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2mzfmzgmo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2hdsbuqwp.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2hyyusshe.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2taymccvw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2kkqnpryn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2crredaqj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2dxnqhoqp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2tslmwnum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jzvwbquc.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2fsfyytaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mdyargty.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ixdfxfqe.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uwlflfex.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2woymgoja.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ztnfhfji.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2aqvjmhuz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dybudvvg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uzytyxer.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2hhsfgqep.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gvbamzsa.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2atazxndo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2deslsxek.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2hnebkpci.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dharrrid.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qizipjro.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2eaynniih.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2axaifuam.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2bxdhdwmx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2iwfmhlwn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ohmcxljl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2vkwogmpm.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2gjpsxazb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2chzlxpzy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vwumyhng.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cwtyseig.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2vupqgtsl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2rdlkjhgi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2aavljuyn.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2wjzajmrp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zellnjqh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2uhrjhtyv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zcufrxjk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2maczbfic.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjyceaks.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2nbgwazgk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qjtsiukq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2uhihfltf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2qopsisja.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rzawqnos.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywujfmnd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtzlwanr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xxothjyr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2djymaiye.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2csllmeqj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cnxyjcvm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2tlrxghjr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ereayudw.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wsoqvrlk.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2aqqcnvef.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lvordgde.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ksuvmwso.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2aczopzvk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2gycebsri.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dsalndfs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2lknquhdo.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ypvwxktl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2jrwmuilm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2wmebhgjh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2fmuskcqy.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2bhgqqotb.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2mcuqghsx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2fsahlagj.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2putsoiat.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2bwittnaq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2rsduhent.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2dohefaie.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2gcpxzeuq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xujrscdc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qhojmket.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hgutsyww.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uattiubk.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2rutvkoaq.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2siazrqfc.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2drruupeq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ilurwfax.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nfownyko.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zdgiqitx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ouhdxhox.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bqkopanv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ymrcmvzi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ffenlazq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2bbrxxbwy.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2phrslacw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2cydizjei.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2xonhhzri.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2nmerrmbq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2egpizgoo.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ktcvmgix.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2fhfhfklq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2rwonoxbq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivkjkadx.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tetzonxq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2aaxhivbo.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2reahyzyq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2lnmclrkp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rwcpmcep.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mxdxbyku.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2slamxadc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2gbbhbdeg.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jhfsxhxn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2mjngxzmp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2xchgefxt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ffyxqebx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2svjexjhb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2gurdwvsr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2mgkrsfry.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2gxaohsol.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ktdvelrd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zewpkqtn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omzntbfd.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2dkxpkuhg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fmnvxrjy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2qmxdoddh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2oyvsrdkv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2wxdlrnwt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2lxehzssk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2pvupeugq.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ljlefrfo.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2hzgdshec.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2eklxhtzh.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2uftzufxi.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2wvbfsfal.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2uinalbop.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2daxxwegi.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2eiodnxyp.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2woomohda.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2heqfckwc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ppfjoiuh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2dwnyfdch.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2tehgllni.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2snltvrtn.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2kwcplndq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2ivjeqzcp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2kecjdepy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2aqsajdos.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ivibtpmq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ewwwskue.html


<!-- 参考信息 -->