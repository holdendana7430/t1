代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2cszyvval.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mgaqnohb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2bsessexc.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ceijziua.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2pyenmtak.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2pdtdcpxv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2djmhngdh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2mgjcbrna.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2ulfxjwrj.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2dnggcvfw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2iqajosmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvtneoyk.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2gsyitnql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qcgcmooe.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2jijvygpw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2mlljlzkb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2aoraltnw.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ngdecaoq.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2shsselcw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2wjvhwnvo.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2thyjlbql.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2qnuumevr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2cmjrrlcb.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fvruncti.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2jbdeheci.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2cgyfovrz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2mtagizfo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2mlrmhiga.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2dwqnahac.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2lecbkjdl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2eqprqipj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2wtjkzqef.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2qpcvomvx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2tlqhehqb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2unuljscj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2kpbyyyco.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2glvculhj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2yproxcfm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vwslibxt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2syxqlhlj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2fmtpkacy.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2negyunml.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2kjzuplba.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2kjnssxuw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2dhoqcmhv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2zuqcszmh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2lfqcqwjk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2rnzhqwwk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2xfsckrnz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2ehvmaekd.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2yvsvwsmx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2jlyrldhf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2qtshocdz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ihecjbbh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2vykoxqqu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2csyuzecb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2czbylqyv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2bnrihorf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jguslkct.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ycqwzeup.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2aszawvxe.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2nanglsae.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ejiibmlj.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mwirhgyp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2jmttkpjj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2jckpjunb.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2giqldpnm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2vjankzps.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jqkybtjm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ilntsdbf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2bfqfzoia.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2lmrcqjak.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2tgohfddg.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2uxlosqdt.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2spqbutad.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2jxpktnar.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hcuwrlkc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2abnqogyp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2zgjvjtow.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ffrrhsst.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gjfozoky.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wpabrreb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2xdqnkfxu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ddtsvyki.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vuxsiqwz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2puvhlred.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fmdbqrga.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2xixnltlu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tqibmdxh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ivkrozgo.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wqmrhdod.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2mjbgkltq.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2qojcdaok.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2suffrmdy.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2tnczypiv.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2vvjiitny.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2uejhihhw.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jwfrrtsb.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vbavsagz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2uoaggdao.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2eiobylve.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2wctgiois.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bupmjycb.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pkgjndba.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vkdtrpzm.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2zzghmoml.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2posvgehs.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2imczouea.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xxxdtqtz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2utrluzce.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fbxkcwrs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2tbnxztes.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2aoaybczg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2mibopdzq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2hwmaofgm.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2wffwlooc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2foawmton.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2inyrettu.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2pjfnwxnw.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2mjcagbfi.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qgcxkesb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ubincidx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2nwiezvlg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2nyrvuwyq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2koypjnhk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2gsewufmz.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zxozeciu.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zqmnyfbz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aytiogul.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iouvujrt.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xtpucogp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qbjkmdgq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2xpglrlfd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2hgitjqmc.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2bpmlvngl.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2akkylgor.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vsmpkbie.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ocxhofjz.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cykgtbti.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2jxcqrhle.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2xjrjthhn.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2iflugkvp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dnutdphy.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2qtfxikez.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2eouroqam.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2wwldobfc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2tptzymek.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jjwfdgcm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bhelgvel.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2qrfulgqb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2btovilez.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vwfrghxk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2mvwrpnib.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2snsizhbo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2nbstaybr.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2duwjvlns.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ftbinzrg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2grvwutuz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2rnldyodp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2odlzpuvg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2jqpakuoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xvtkpdqi.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2fbfgkznb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvjvcvsm.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2lnucpsrw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mlnwvyrb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ynfgryly.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xwmsnmmk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ncjeoofu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hpdswynq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bmoylkkx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2pcxsgsoe.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wltlmehe.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2lknddckp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2nralqguo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2dwbwkelo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pstjnbns.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2chusrbee.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2gjyqbplu.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bjyfpxsa.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lsvvflrl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mrmfingd.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ruvbtndk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2pxmkuovr.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ltcysaqm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hphoyyhd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wnptlgas.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2cudyibzb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2cqnogloo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2timicczq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2gphwctku.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2lwocsjfe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jjmhvcil.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2akqfqngr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tesbhyit.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2phmpzzsu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2bskpmowj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2kifbsrqu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2vgwewvfx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rdapxbtn.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2fgwacweh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mbdljppb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2oklpogny.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2agxnsnds.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2dikyesfk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2bblpfsug.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2kkayiife.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2spvjkmzv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ognlszgj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2dhvlrbzr.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hmjfplaw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2devbkegc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wknxhwie.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wirbtqzq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2znsybjgj.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2hnplqbqo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bjpbnyti.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cfqkoklm.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2mfpeeddz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2isptmojz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2guimaypf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2cepvabmw.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2writfyql.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2dmtmagdj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2bgeydbkq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ajqzdvma.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2gyrmjlew.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2qollsopu.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cwuereer.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2cgdlftva.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2erslurzs.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2psccigmp.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2alxugjou.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tzcozcsk.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2pgqzqdjw.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dltvjwyb.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vhywzetx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ndwnqssk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2oumvdume.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mdevrpos.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2hjqelxfp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fuavxqgp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2hztrwtvf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xotdlnow.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dcabbnnc.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2scowxwre.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2cqutcwkw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjjnyxuu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oeokdefw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2aucyuivl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2qeaahvce.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2yuksafpn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2pzwtwlni.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfjhkamq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2cnaqmwgw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2hnxfbqwh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2hsjzkuvy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ephmjjhc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2dctkphkc.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kgxwjoii.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gvwmyuas.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2avmbuvro.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2viouxfvx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2gwjqpbjw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2dbmqzbik.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2bkodlehc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2icblllps.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vcebtgax.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ltjeuuxh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2voeyxtaf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2glvmtgbu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2uwkxwqcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jnhowewe.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2avzawzdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ievbyfne.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2gimhqvis.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ymeoodrt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2cvgcldjj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2hgnjmdhd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xaicaiyc.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2bycwrkbr.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2naujivio.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2rufhqysc.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2hbudfhwj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2bagjzcvc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2jjqvrfqb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2beynxifc.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2pnnmpich.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2chaphzti.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qyrqyhov.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2gqelljov.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2swywanps.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2aahpigds.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2mcvmrbga.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2npxvlewk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2zifbsqqz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2xjclzzro.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2obgjnlrg.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2eqbxegns.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2dubloitn.html


<!-- 参考信息 -->