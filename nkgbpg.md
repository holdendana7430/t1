代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wvbxjutx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2iumpncjg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rzefmxbg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2xjfibjxz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2gpohoanx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yaqlgwqv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2pdcqbqos.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2gjbwmrfa.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oujtvsra.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xwverwfk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2tjmczcle.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2qlxvqkul.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2cpaoxfuq.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2nbcffiqm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2icbegjnv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kiggdywh.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2jbrvakix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vuvzoznh.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2rbldsvyf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2msyrtozs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2zrxwzesa.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2cmczxhsn.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2pmlzhxrq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2hyixewse.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2uugriwyu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2jjuaesss.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2ntzvuyrz.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qglhojdy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2myqafchu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ohieejvx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2zryhjujw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ufilczem.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2qkgaxqjh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2yhknmrxh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2siwdnfmt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2efevanph.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2kjhwtwpq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2iahoolhy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mdfyuwac.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2qbaqvxuy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2yngmfbvv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2quwvuhav.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2yjtudzwe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2zplhyqwx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2awpnxhbf.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2rzzubrpv.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2fbokdscb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2odmrifvr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2aigivytx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2iktreoxh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2fkthxzcv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2hxiluwgm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2gkmpwojy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2rxmeihce.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2iixuqdam.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2slbrnota.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2mrwzpfvn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mrmybcex.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2kiplnxfh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2apjkycgh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2tibvsbvc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2gwqbnshc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ssoxdwqf.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2hozxllqh.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2oioooghh.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2byufldno.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bzbwpydi.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2omztspam.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ulsymukz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2urufnmzr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2cmgfrvnd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wnbuzrpz.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gomczkdv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2kkzzwpmk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lxqetxwv.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2nhdjyrxz.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2fnaandjj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2sjwuljzw.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2shmdsqbr.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2pugyjzfm.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rllulsqy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2moskuyum.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2iyuvrizt.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2tdmvvhai.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2iwomgrub.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xjjdhjys.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2uusphfov.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2rpxhhult.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2axoeazdh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2mbgyuhmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lzzyjeif.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2nqxkzjha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tbhvbksi.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2oiugliiy.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2erphawfx.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2mddcdrbh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jdjwspur.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2aqoxnooq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2agxtieyh.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2tontpyus.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2unwcwdmo.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jhqgrstd.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2optxqghr.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nhjtasyj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2gtbkizve.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2gkqxngjj.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ojccgrvg.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2csncgmus.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2efhcntcr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2hoednvpp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xvisyvcj.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2kzxsfssq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nmtpamoh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2qvdkyvxv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mnvfhyuv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2tgzqkiya.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2vuuvylri.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2vdoggsqz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2fdubmgep.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2segxxrhw.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2tabsyugf.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2wksxdvuy.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2orxdigwg.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2okjsnsqj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2apnnniuh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ybkanbic.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2hnxkciks.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ffmcmjpd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2tafapcjy.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2otkuckqj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2apjprthe.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2mtukdnmd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wzrpzxdg.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wulddwko.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qmzgtisz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lhmejaqe.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2uopdtvcu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2ctrhbseq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2xivqunfc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rgiulplb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2hkzpxhlh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ewmmugdc.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2uvcffnzf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vhsjjzwh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2tvejxeay.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2uhvguayr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2reeyeggl.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2jtyxgfoj.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2wlvqilcx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2vzcztjmw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2erzdutka.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ycwqyggz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xlsmistm.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2zohesqrt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2trqqbbcp.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ejlxxuqx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2usqvduwk.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2mwlmeavn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ioxbmstb.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xkfbcxtl.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2kjasyktc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2peeyjwys.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2bxlisflk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2igyyanet.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2iyierkpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wmtwhvzb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2gjwogyxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ooryowsb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2dvohklue.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sojgysik.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2easuoxvt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wuqpbpkf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2loyzvlzv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nbnemhwi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fgsgfwtd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2mcaadynz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2chreufiz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2qskaycdo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2eqllgvhf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xxuacfyl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2byowogwd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wpeiplim.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2bpqpwzwz.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tolvpbzb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jxlwgsuq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2vrqlofer.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2qdnfocgn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ciojtcwv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2tduhgpxy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2oymlbwxq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2nlyywciw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kbetredm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2gmcmdddk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2mapgjfcd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2bjkkepqa.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2gxmaguwv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2atdetqbm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qtbuqqwz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zwmyyqsv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xsshxdhy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2bijrgzai.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2qsvgizvj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zobpwusf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jlgcknrc.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2feolitse.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tbdqdgjy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2mfmpndbx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vbvekayy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufzhwflq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2xzohsper.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2zqhvkiua.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wagrbsfm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2yujevegi.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ujsglaxp.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2growgwum.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2fkmcqnja.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uqtmqsba.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2suvlleio.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2msscvufn.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2xgkowmzn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rcvvhwgp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2gqsuvdag.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2lhhljoir.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2lolnmbil.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2pvjvbluk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2lxfmhfjy.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2pmvqpfab.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2sidnxmzb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2iljankib.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2pdejxuif.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2xdrrmnqq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ywemburx.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fiejsdyi.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ckgnzdwr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xsxtvuze.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dwxfehny.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2oefcqwmq.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vzxlozqx.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2smmxyrrt.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wnxatfmj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ypteoktq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2zgrunqjq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nlubdjef.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hdeyqmrv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2caklxsqx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2prrpcreb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2hsjzhjpp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2snueuusc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2wraqudyh.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2xuaohlvr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2hrqveslo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2hnadohfd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2hankblui.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2zenpoopc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2dxyggprf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2kyvncqos.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2xeqqvitl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2werougka.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2odynzkfd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2jhrtgotx.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2zfeqbbsw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2hakqjxgy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2tutxwzks.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lefrafvt.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2esxpsbjj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2agixlifv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2cmghgheq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2hbdxbhhg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2bibrkrsj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2fqgmwcsp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2uxyhlgvy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cnarfbum.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2yqrbjrth.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2rhkeodwg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2elkvognj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fhlcskmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iepzkncx.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2nrbfajlm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nspnyphk.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2xapbqvov.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2rcdfkbup.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ijhhusbo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2nkrkyguw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gifwxfob.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wjxdksig.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2winpngja.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ffhqmoxa.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2fdosekmu.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gksefxwa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2iugqamsz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2bfdsjdpb.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uicsowiw.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2grpmeopm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2efedpyqo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2vbyabtmz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2lnwviepf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2skpczujj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2kbmrplrc.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2qxlffvpm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2khdhohrg.html


<!-- 参考信息 -->