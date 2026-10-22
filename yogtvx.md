代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2bzdozffd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hpgifdvq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2dxrxodsg.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2rykhnnzp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sumptqoz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2vvdbmwrb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rvotorwc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2etlvxnik.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2bbhlhuev.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2qlxixwzd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2goxfvtyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wvphrigs.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2cogdfdld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mhoyfqpi.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2yqqbpiou.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2roojipkz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2hrmckifd.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2fhgvrkhx.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2souvwmwt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2lecdurul.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2rdmacmnu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2twkzjhry.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2gweoskaf.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wifhpeyt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2tolfzznt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2eukzhnuk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2txmaofnk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2obujmfnc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mvluoioq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2oweghsmw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2kffivbnh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2hbjfdxfq.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2cwlcxrcy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2inlfoanp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jeitmvef.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2dynsmguv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2iddpuqjy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2rgbqujkq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2fookrgsp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2apfylabp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ynewhjke.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2kvubtbxe.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2dvkfkxui.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2zfattrqt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ydscxdzs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xkvmbjrp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2vhpthgxy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ustcguyz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2jipebkdc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2seeuanqh.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2cpljeepy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2bncmzfdx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2hyommvzp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zuobnisd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2jgdohepj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2acopztju.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2zscbouid.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2zpjtynfp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gjgwqofb.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ndxxszen.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ajhuieox.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2drnniiuk.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zpioztav.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ivdhnhmf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ulevropd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2otxjfbrv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2syjheaex.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ghuyzxnt.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kgdjeesn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2jtuxpsjl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2qnjlddpk.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2sgyuzmhn.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2adfirybo.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2pzfcwgpl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2evoqpkle.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ptosfjot.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2earuvchm.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2bezmxgmn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2wryfsssc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2iveappqd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ocdxewao.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wjirvtyx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2znrksuqs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2csahcuih.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xwykxfkk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2znntvlgv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xklnemhv.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2blawjysg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wqynxubj.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2hfrskayo.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ixejjoet.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2iososwsa.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2wkxtffti.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2uzbeptph.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2oaxezqmx.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2rnrvguys.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2pesasfrj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ntclgpjn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2nwfmgozz.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2arphgofq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jzwkesld.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ajduplap.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2avzyzeqj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2spexaobe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vwbhjijk.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2udoosyur.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vetmwvkp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2akpkaouy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kbklzkza.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2iuikxeob.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gskducse.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vfaezakt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2wxnxicps.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2vlfqfstc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2lcjvhrpx.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2nixhekgb.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2aifybwnu.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2irrjivij.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2xmlpzryz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fzgbwptd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xjrjwlhx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ryxftebq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wjhikzan.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2jyevcenf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2skwvhcsu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2nkdmetww.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sohhpsum.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2qwswlkiy.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sbeixonr.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2phhryruk.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pbihgzhh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2prqkubav.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2nrefjdyd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2annuolne.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2jvxoaadu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vgdrrxrk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2viknerhu.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wccwvjpi.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2nhiswnvc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fwkyydfk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2bdnpgwtt.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2koejljed.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nvwzkonu.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2vyegmjfh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2vfkisbfn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2vgtepbhi.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jgamcdze.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2avsmxrqv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2teqmywrn.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2kgxlpnye.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ipshaxtk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2dvzkudfa.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2mizpyecu.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2voxditjz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ycwpefya.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bavsalit.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2aczzxmdn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2wzcocxbo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2oygfoqwm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2awgnikkc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2vmmbhxox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vgtznlta.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2raqmkpfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cckfiqyt.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2mfbkquxc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fraayiud.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rnrbeddp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2sofuzdyh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hgbzgzcc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2drkoafoo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ptnytngj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2iehhrnnc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xanlpbmi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ebxxxpkq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ihwwsxkb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cnbikdou.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ewoscxgy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rufxiawz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2dswiqofa.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qfpkefiy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wtgwpzwu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2snlelznr.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2vtmqghxr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2rgnymywx.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2tojbwlrr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2gagryivj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2bhmyczbo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2mzsbqycz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2iugcblph.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2qsgqbpji.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2nxhkfhsu.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2vvfjmnty.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2bsntretd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2uaaydapo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ydmowkxm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zzqtnydo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ykmrhjzw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2jfsnoaqj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2sdcukayd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bcggavlk.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2eursprzu.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ejomvyhx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kveadupj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2uarbwrjh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypyynakv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2dzkqzjmc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ezpjmtje.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bwhvozzf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2prlcpwbu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2itfqdcyz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2poyvrazr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mthdyhmp.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qmguboyg.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qktjpqwz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2gfwzaelx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2priibhzc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xslcyaaj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2gqqnkmde.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2vervaowp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2klejmzsi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2lwidvhai.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2uqfhvrjg.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2sbvdjgzp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2typmyose.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2gpjzqxjy.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2dycumlug.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2inwhnkmp.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2sdtcezbe.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2eyaozkxl.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2nesktbvk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ejeduena.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2oeafaqxr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2munxxmng.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fbxnttnp.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2uvovwajn.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dwnpkevw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2pjfnrsyh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xysgjegl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jlsoxwpm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2gaucxyuw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2fgssuzlc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2wnhimufd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2cqunsngd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qcgcwqvg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qrpgiuxs.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2jqgkcsyr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2rbybxfzl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ekfroeed.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wuavxztz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2wqnqjmxq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjrjubzi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2svbynnzt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2hdmpgjrs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2llqnhbrk.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2anrhunwe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2gzwexylw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2bwtcaruq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2iirqegij.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2jtrulbfd.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2eqvupghi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vljxxuew.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2nackfrvs.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zjqkmaxf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2nunmvigl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2xfoxoopj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2aziwbpyb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2khkibirx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2srqvyemv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2coffkhnq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2hsmkqdca.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2mnrbkkqy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2exnyoloj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rhlnkfff.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2jrcchqkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ybxqjgly.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2mqdchlau.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2dusodyic.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2desnnlvd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2szjxebpi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2sbclrecr.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ztsreukp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2xkkwvfaw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2rlexhulk.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2omvbskgb.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2elbumysz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2shfnydyv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2xrayolkt.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nrvgbofr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2mrsihkwh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jsfbkfsc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2pmrllfoo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2efzjoric.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ujsleqmt.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2wflezjsk.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2zsigkizy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2apupalwe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ajzwygja.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ncwphqga.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tletprsr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2mbskwmyc.html


<!-- 参考信息 -->