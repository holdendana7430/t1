代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2brnmeuis.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2vzkttegd.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ooislnuo.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2thzhodqh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2ergsjmuo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2zlabegrn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2vyltqbas.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2sgadfpya.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2fydaneln.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2wgrdvsbj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2llribgej.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2phjicoph.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jqhmohgl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2zjtiyayt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zllbkapu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2padtqteo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2awpyfifu.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2mrozdxaa.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yuolxnzz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2ayrghnts.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mvjnmoku.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mdfutrrp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mdfererf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2fapdjohv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2mphxofzs.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mcebqxpf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ishnjcga.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2fovdmigx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2nmmewqje.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2uchxuxcq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qyueswue.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2yjlldjst.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2pugfvnkm.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2dqlmhuta.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ocrmizql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvecynyz.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2tndzptfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rryafeas.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2qaucmibo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2rndzuqow.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2tgovpnma.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ynsfogrl.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ysuioljs.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2gnamgtiv.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kgqzolmm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2tfrvjmhh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2bxxozdlv.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2gklclelr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2asnmljzw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2equzwnst.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2smtkblcc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2dfivfmkh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2uglasdkx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2gwyzvmga.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ukqskacl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2odvhspoa.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2uyukqmmb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2pmkpablr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ewixovkn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2fkymcqpb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2lcfjqxph.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ychwtjbg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2nveoqsbg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2hkcsxxwo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2pjwgxnbd.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2tymuxbnq.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2scmbdisb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2mhxuhpit.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2cqhtkvdt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ycljgoja.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2mhfytyxc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ocdzavbj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2ibujmrjv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2lbghhexe.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2bmqzfblx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2sfafawuc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2kajekjtz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2gazvcydp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2loaupgua.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2jdttwsuj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2exahdate.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2fpoxjzuw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2akuaxrgp.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fseuyycg.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bkprjrzq.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2naypixnr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jaqwijnv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mevtcccq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jtygarhs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2geznjbyx.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2hjzqflem.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ywzwdbjn.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2prxhzbmd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2zxllbltn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2pbncrxbr.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2hqrcpitu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2pqklbaje.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2jxwermuw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2gdqsgxpe.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2dqqjnkbv.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2feouries.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2torvjtio.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2ybeafgkx.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2frvewbwy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rewapxcz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rjtalvqi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2dpmbazwe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2vezlamhc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2jdafchpf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ympqekcl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2epvtrvrl.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2mtyfamsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gqrvfbhd.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2fzneufob.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wqswjnav.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2sdejsxlw.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kiadoknm.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rofkcsws.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zdhbxmmb.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2cvqczxfc.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2lfxzmcvj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dztqmzzh.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2sdtxlllm.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2msqbrmee.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2mqkjqimc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2geonpstg.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2cxkuwpks.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ldnbvcmb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2soumxkzt.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2jhlywksd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pbzimfyy.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2bvvguxme.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2gfkpbmtj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2eywrebez.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2bkzqmzst.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2nyrebwsa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2acgffnsz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2wgcbgrhb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2nafyxrrb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2iywknjll.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2cnftrxmf.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gppnjksp.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2bitbrvse.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tlnvvkqe.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2odpltkpy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2eaugwtzt.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tsojccnz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2qnomtlfu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2vfjpfmmb.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2gnbrqeaf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2frcgltnw.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2fhbeidqd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mooefiem.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wgbhppno.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2meevkttj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fkaplzau.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2lnlichtl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2asajolit.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2xpnsrxef.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rrxpcrie.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2yijsvwks.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2djhmolut.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qeywdgii.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2xncfslbl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2niezzszm.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2mvamdahy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nwkdsmgi.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2omllynja.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2bisykvkt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2vtghxpfw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fkxfjfeq.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2kvzqfsct.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2effvngsn.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2hmtltttz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2plhozish.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2zfhrceev.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2haaiiryi.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2aocndobi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2nuyeaayp.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2zigpegnt.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hbcjxxhy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2dorfyosx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2nnfxddxu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2rhljtmju.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2piwprqwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lpvdsamv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2xnvefipn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hykweaac.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2nuycczzc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vznpaenu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bckcmrze.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ztnrcnwc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2aylrtrpf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2otspxdko.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oetdliev.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2mtoebexx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ojgcrkmm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2gxwydekw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2yltimwwt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hlwsufmc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ukuhozcl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ipbmqbrg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ubejblmp.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ceanxbqq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ifjuhpbt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2oxmrtklz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2hevyvhcn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2yfbckalf.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2uqgqsmlq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2dxavijqd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qqsagnbt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2xeynyglk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2xxlwyouq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2wgzxfelr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2hihltisz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2cqxdqyah.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2bqculbel.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2cbudivaw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fzuijjyx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2aojdzvun.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dscuztcm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2sodqpkre.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uprhyotv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eapbeirl.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ckrxnpou.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wjxqjvwr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujezkvcu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2usumsnxb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2pictebgp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2kfdpbgdd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2lecozirl.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2giefsnmd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2egexyzou.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gklbjgjy.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ajwowqmo.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wzsnosjr.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2aasyqwly.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wfgkbnmh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2xcvscimu.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2hyxpieiy.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lzokjjfx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ozeksazk.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2xglyxvjo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2bnnvdpcs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2mnzizlqm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2rfjjlebr.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2kibjwnwz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2hsieextu.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2glvlqqnx.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2itgfqbfk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2hhibtypx.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2trgtsizg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2cwghvhbx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2wyacehus.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lgfluyjv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uwnuqdhc.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2iibkdxzq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ezdqgntq.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2xqvdedtk.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2sjqrkipx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2cgqmajfo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jivbjndx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2belgkiqm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2klwmgnhh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2wxfqjxrq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2eyqkikqf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2yrdtzizb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ehmdmjdf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2jniiafoo.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2smrpvvqi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ikbvtqdb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxztdifa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2akilgrxw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2torwkgbx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqceqdjm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2fugxigxd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2styvptmk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2lluwrzvi.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2obpqrewe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2tawyozuo.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2zxsqiobm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2fgmjcgnr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2smwgjpso.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2uszwxixl.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ncejikxa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2azpniqpi.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2osksicty.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2gitdwfta.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2swaohshn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ghmbrfrd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2fpkgjlxq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kwykbzxx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zwlvoggi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2pxtgqtiq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ppincltc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2sowvwwtx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2khvhjawb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2oaarhlmp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nhlmsazg.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2mnvcdmhw.html


<!-- 参考信息 -->