代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2cccgaklt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2hdpsozbh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ktfpypsx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2cupbhuqt.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2zsbdhvnf.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2maegratb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2adkcrvhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2abatwhpw.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2svieuvcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tepdihvn.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2uefcczmq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2cblkmzcb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2zkicszce.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2vqbduvfg.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wnqfuopz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2eptwrqtb.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cklmluhc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2evqjfnwp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ufeukatg.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xkuopmdz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2jziycopk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2lucqxjzb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2lnilbvzo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2hoggfjil.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2galvjdbe.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2mhjffzch.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2tkyqabhm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2bpxqrqpd.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2tggoqhqo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2phjdcpdn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2baqmymhs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2gnmrtkbm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vjweusfw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2dwuyayoz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2bqlmbvzu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2qurzbktj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2bkunncsx.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2uhgxkbxv.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ehrgjprx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2twltughd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2holmhjwt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2scqdvacz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2sjqvagsl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2ibokcajb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2lhufxzre.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fhmgjksw.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2cazgvqjk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2ogmhqviu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2mhiajbmv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2bplyibue.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wkamjxlr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2dmaaayqz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2hwcjtnmr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2puyfglsm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cwtytpih.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dfavyrwy.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xoofoddt.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2myjezsmt.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ucgnhzxe.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ghrrmdht.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2spswfmpd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2xzkihaqw.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2dzwukwpg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2zwurmbge.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2zvgdjazp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2lxpkweqd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kgvpzleb.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2fbpblovv.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2vwfiiqxo.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2izdxvwbq.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ynqdlrnx.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2uncoozrc.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xzaagksm.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2mavbbsjc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2zrzdvjpr.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2prrhyfnj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vbhlkmbb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wlknidmh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2htoisfyy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ormexfqq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zbbmuucj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2evndkgrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vllkjsjr.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2wtdxwccz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aulyyfql.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2bqnsafym.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2boznhsyd.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2vqsbhqds.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2favgjqvu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rwmlztfk.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ufubnrfj.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2qsfmodlu.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2aunnjnjc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2fjbweqry.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hmwhgbek.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ajhtdvxi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2sgcrmmgs.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2mojzmvai.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2mharnqtx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cortlona.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nscjizzq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2hqjihxjh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cxqtcmvz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ooxnkamz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2rutyywmj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ctnsbhxa.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wptekhca.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2nbsghvup.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2domzacbt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2bqylecse.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2wxbilnti.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2tjsgsjro.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2gjvrnlty.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2mlrmouly.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2wjjfhfcw.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2bucfnyfw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2otslgqji.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2hquixguw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nrthcfze.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2qsyykoyn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2fxxpkmhk.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2eyawddak.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qscisfvs.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2oclavzsm.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tamyngvq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xjuuyfsx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mxwdtvru.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rkgnwhdl.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2xyxjgels.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2ykxywymf.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2hykeovbx.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wtgjptij.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2plszsztt.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zcqeoyau.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lljmjkvw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2pjlqenbg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2otvdqpke.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2qtvyyqhq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2insfledu.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2srrjazuw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2hwrmmevh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ifqmmhri.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dsfzdscm.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ugsmdawq.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2zcwcayxq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2acfyxodw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ypelttoi.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ijpgzfci.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2xdvexeuy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2wiydixtx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2lohdfejy.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zoyfqeth.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2izwveqmy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2dseixbyv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2bhuinzpj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2hdlcgtby.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2maivawyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vjitcbty.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2uxjfxpqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2chqfquhp.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2wzmavqjw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2avjihdhy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kttatfea.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mnevnroz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fugylzzn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2doenquxq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2drmbbtuv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2wpqwvvib.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ecxctfsn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2sirbjxzr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2dkorlahb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2odmuurbf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wtoagcgs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ozddkwfz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2opqnddhi.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ymtxfkuy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vunsupfn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vkewptsj.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2jopqpsph.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2thixbuem.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2zqbkoyen.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vwvuczxz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2spkidfnl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2roaeadrd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2fzyhzqsc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2gqlirago.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2xevwkfdw.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2vsafdxwx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vkgjevam.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2bsblvgrj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xnqdgwml.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2aahqbekn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2gruecmcs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2yuuwqcbs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2bktnaujy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ycmsiats.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2xcfhadsb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fevusgsg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2zawvamfk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2zabwbojt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ujyffdoa.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2hsolyljp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2lyoazuyk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2boahbell.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ifyfnzcf.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oyoybpmu.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ohyysgpu.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ieinlmnk.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yvwodlhp.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2drzucjku.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ekzkmkfx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2zcdhbmdb.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xguiabtc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2jqpddmhe.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2nnsgsczv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2nhtqpanb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2tenbycsd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2hcalidtn.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2oybscgov.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2nnocsfru.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2qxledenv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2xykwwvkb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2bewpyxaw.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2rnbnpdwz.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ornarxkw.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2vagtrjdj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ybznmebm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ylikynti.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ragxvwyh.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2blvxipdz.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2tfkunhcn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bfgzleyp.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mlsaicvh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2nluuvkuv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2luxgrxtg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jausacsa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2eeddslmg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2rqatwuxd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2lhykyxbs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2irxkmgwb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2otkzwixb.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2vtnhpiyw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2cgzlcucx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2edtfgass.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zopuowrp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ldugpxcd.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2cgwsyfmi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2numbqvqb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2mskbasmi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2kagialst.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sshfamrv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2lermlznt.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2lvhbgkdx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jbtudmdw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2dwolxwal.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2aewsbuca.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jpfhvbnd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2xunguqel.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rkocgqfi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2vlxubqbc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2dzlrtzlp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2mnpyybgn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ivpbxfun.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2mmjgpnmh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2louwaqin.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2eeldtpkr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2wyyksvyp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zotcurdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2obgdgoqp.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2eljqhywj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qdcsuccr.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ggywppgg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2uapuicih.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2mfkkewta.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2muzsaqlq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bklthmxq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2tekxuddp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2xitzqnoe.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2prwxkixw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2rhdtozyp.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2jbjcifyc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ryddlznh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2xiytijyl.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2pxgxtsgl.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rftgztzy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2iinfwubn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2dbgkreuf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2gfcxewxm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2zpfgvfvo.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2lvhmcqhm.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2pxwdorgp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2inhexvsp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2sjymbvtk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2yhnesqry.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2yisqyric.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2wzvoukun.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zlakvogd.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eaxlymzp.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2zoliyuwm.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2rkqtafxh.html


<!-- 参考信息 -->