代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ydzc1.top/gtogmlzgus.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jianghu66.top/gtdiamzban.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hongshengwenyu.top/gtogenioxp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yj20258888.top/gtuqajwfiw.html

[K06] 解析 URL 查询串
来源：http://hz.ehwqpu.com/gteyblhgin.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinyuanbaomall.cn/gtcmxzgtyv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.gaohongyu789.top/gtdbvoflsx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangkeji.top/gtheqahxss.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zdqjudy.top/gtbtupdpvx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shangyingyoupin.top/gtilctmxsd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gotoacloud.top/gtytwccmjj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hfpthk.cn/gtgwgsuezu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zycfv.cn/gtocnqsxnw.html

[K07] 进制转换
来源：http://hz.jinghuilouyu.cn/gtxgvtpmyq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.fzhhl.top/gtjauytdky.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tian-w.cn/gtarumcalj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhengqikj.top/gtqrzcwowt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ydzc1.top/gtxtihclqs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.aibaodan.cn/gtliqsmyll.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yangfankeji.com/gtotapxqtx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhixingplan.top/gtpdoyfkbz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xuanzx.com/gtgtacxoik.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.wangshuangyany.cn/gteahclgxw.html

Py:   pickle.dumps(obj)
来源：http://hz.sweek.top/gtlsgfbvwb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xinyue.icu/gtisbqrcyd.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shuidangran.top/gtaujhhquc.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.tianlin.xyz/gttagnlhnj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yj202588.top/gtwdjxakej.html

Go:   encoding/gob
来源：http://hz.dianchejie.cn/gtzhqrrpfq.html

Ruby: Marshal.dump(obj)
来源：http://hz.daxiang520.top/gtnhxmfxiz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hysaishi.cn/gtbixthhhs.html

================================================================================
来源：http://hz.quarkkingdee.top/gtakffhjwq.html

L. 网络请求
来源：http://hz.cheryme.top/gthlppllzg.html

================================================================================
来源：http://hz.yuanzhike.top/gtualsmfdu.html

[L01] 发送 GET 请求
来源：http://hz.havefunace.top/gttjwzdnbw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.tianlin.xyz/gtmizltnsx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.daxiang520.top/gtxicouumh.html

JS:   await fetch(url)
来源：http://hz.ivvv.top/gtmmqrrwxt.html

TS:   await fetch(url)
来源：http://hz.hammf.cn/gtfoitpuzl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gzhubu.top/gtrfovxhpe.html

Go:   resp, err := http.Get(url)
来源：http://hz.52xcode.cn/gtjdklzefg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.wangshuangyany.cn/gtrdqrwnow.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jyoumei.cn/gtuidtzzna.html

[L02] 发送 POST JSON
来源：http://hz.cdnleiting.top/gtmiqmixef.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.52xcode.cn/gtwuwpybob.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.fengsongda.top/gtbwkksgsy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnxiangtu.top/gtaczlzpbj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.snrcjt.cn/gtjjmnwmlf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhijiandao.cn/gttkoyckcg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.316326.xyz/gtdevgebwo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.nanxinkj.top/gtdfvewmtz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shangyingyoupin.top/gtnxqksurv.html

[L03] 设置自定义请求头
来源：http://hz.ydzc1.top/gtbqeaxszr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ybcxt.top/gtctlithlq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jinyuanbaomall.cn/gtetkwynxi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xingfuxueyuan.xyz/gtyugmghve.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guannengcc.top/gtyjseidkc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jiagoushi.top/gtxtewanpk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shzxlz.cn/gttanyhyaj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.316326.xyz/gtiooucwfv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jinqigfzy.top/gtlftlfbkd.html

[L04] 设置超时
来源：http://hz.gaohongyu789.top/gtjdecexja.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cheryme.top/gtotxyacgy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.quarkkingdee.top/gttwolynzb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.meibo888.top/gtdhhljncd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangshuangyany.cn/gtlrvqcmem.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.shangyingyoupin.top/gtwntbphee.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yanxiufei.cn/gtyhwctgcy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hammf.cn/gtmorskrau.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhaomingkeji.xyz/gtgnjwmolj.html

[L05] 上传文件（multipart）
来源：http://hz.zycfv.cn/gtqdnnzkmz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.nanxinkj.top/gtfrbdwfjj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jinghuilouyu.cn/gtidjrpdby.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.nwbrower.top/gtahyckwlm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.nwbrower.top/gtekjnmjkh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gogol.net.cn/gtmjxxvyjx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.iojbl.cn/gtiafcckzp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.nwbrower.top/gtdysltlcn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.iojbl.cn/gtonkpmfei.html

[L06] 解析响应为 JSON
来源：http://hz.hnqzz.top/gtrcqvizum.html

Py:   resp.json()
来源：http://hz.birdmap.top/gtuqrajkqv.html

PHP:  json_decode($body, true);
来源：http://hz.yj20258888.top/gtyrtakbsh.html

JS:   await resp.json()
来源：http://hz.havefunace.top/gtrwznxuwq.html

TS:   await resp.json()
来源：http://hz.quarkkingdee.top/gtdrxttslo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhiwuduotai.top/gtjtryiind.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cheryme.top/gtsnocodsb.html

Ruby: JSON.parse(resp.body)
来源：http://hz.gzhubu.top/gthyfyroqj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ppjwa.cn/gtxgbpkafv.html

[L07] 处理 HTTP 状态码
来源：http://hz.hongshengwenyu.top/gtawgqigle.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jqgufenzy.top/gtesicmuqy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hfpthk.cn/gtuzafjnav.html

JS:   resp.ok;  resp.status
来源：http://hz.yvedp.cn/gtubyzywoq.html

TS:   resp.ok;  resp.status
来源：http://hz.ydjk.org.cn/gtcojgelmd.html

Java: resp.statusCode()
来源：http://hz.mhx1999.top/gtujzxgxxw.html

Go:   resp.StatusCode
来源：http://hz.guowangkeji.top/gtymkszfjt.html

Ruby: resp.code.to_i
来源：http://hz.sxryk.cn/gtvqvvqqio.html

C#:   (int)resp.StatusCode
来源：http://hz.yanxiufei.cn/gtkhzsojrd.html

[L08] 并发请求多个地址
来源：http://hz.tian-w.cn/gtgcirrtwv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinqigfzy.top/gtzadczspw.html

PHP:  curl_multi_init() 系列
来源：http://hz.hysaishi.cn/gtevguwxyo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cucudq.cn/gtlgzrfnwv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinyuanbaomall.cn/gtptxnifyg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yj20258888.top/gtjyvipjus.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.9152youxi.cn/gtznuazysf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yanxiufei.cn/gtynkqswqh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.kuanghao11.cn/gtnyqblqgj.html

================================================================================
来源：http://hz.yj202588.top/gtiduknznu.html

M. 命令行 / 进程 / 环境
来源：http://hz.c1oappe.top/gtbokgwdqb.html

================================================================================
来源：http://hz.52xcode.cn/gtnxyjsmhr.html

[M01] 读取命令行参数
来源：http://hz.fengsongda.top/gtadjexgsz.html

Py:   sys.argv[1:]
来源：http://hz.jyoumei.cn/gtnjoxbcfd.html

PHP:  $argv;  $argc;
来源：http://hz.nwbrower.top/gtmydgassf.html

JS:   process.argv.slice(2)
来源：http://hz.nwbrower.top/gtqqralnzi.html

TS:   process.argv.slice(2)
来源：http://hz.yanxiufei.cn/gtphbocmzl.html

Java: args 数组（main 方法参数）
来源：http://hz.hammf.cn/gtsbeompum.html

Go:   os.Args[1:]
来源：http://hz.dianchejie.cn/gtxsywzzrb.html

Ruby: ARGV
来源：http://hz.guannengcc.top/gtrfkndblw.html

C#:   args 数组（Main 方法参数）
来源：http://hz.wangdashe.top/gtuckzezkm.html

[M02] 读取环境变量
来源：http://hz.jinqigufen.top/gtrujkmkni.html

Py:   os.environ.get("HOME")
来源：http://hz.hysaishi.cn/gtarlgfwjj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.daxiang520.top/gtnbojuagk.html

JS:   process.env.HOME
来源：http://hz.feifeiyinyue.top/gtycytlatj.html

TS:   process.env.HOME
来源：http://hz.mhx1999.top/gtckwdaaae.html

Java: System.getenv("HOME")
来源：http://hz.fengsongda.top/gtfawkqeoj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yuanzhike.top/gtdrxteoix.html

Ruby: ENV["HOME"]
来源：http://hz.hfpthk.cn/gtkstirdat.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hnqzz.top/gtelijgczq.html

[M03] 执行外部命令
来源：http://hz.cdnleiting.top/gtmfgpokjs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gotoacloud.top/gtzrvvcdwv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xuanzx.com/gtldxjzody.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shangyingyoupin.top/gtlokctfqm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.guannengcc.top/gtxudydxfm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sufxvd.cn/gtcoctvrvb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.nwbrower.top/gttnvycpzy.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.dashuyun.cn/gtvupimjym.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jqgufenzy.top/gtqrkimccb.html

[M04] 获取当前工作目录
来源：http://hz.dashuyun.cn/gtvcxwgadh.html

Py:   os.getcwd()
来源：http://hz.zhongyouzk.top/gtsehjkorq.html

PHP:  getcwd();
来源：http://hz.hammf.cn/gtcuzknuve.html

JS:   process.cwd()
来源：http://hz.shanyushiyangkeji.top/gtvlbamchs.html

TS:   process.cwd()
来源：http://hz.vqdsnc.cn/gtiuewslcj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sufxvd.cn/gtbprqcjbr.html

Go:   os.Getwd()
来源：http://hz.svipenyu.cn/gtdvvckida.html

Ruby: Dir.pwd
来源：http://hz.ppjwa.cn/gtjlfuumbm.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.dashuyun.cn/gtmpmkflpu.html

[M05] 设置退出码
来源：http://hz.xziqi.cn/gtszrbalou.html

Py:   sys.exit(1)
来源：http://hz.kuanghao11.cn/gtxckorcfe.html

PHP:  exit(1);
来源：http://hz.tanke756.top/gttkmadntm.html

JS:   process.exit(1)
来源：http://hz.shanyushiyangtech.top/gtocdeifhm.html

TS:   process.exit(1)
来源：http://hz.daria6918.cn/gtxwxxrnew.html

Java: System.exit(1)
来源：http://hz.hammf.cn/gteoxufpwx.html

Go:   os.Exit(1)
来源：http://hz.yongpay.top/gtedpfxfxl.html

Ruby: exit 1
来源：http://hz.vqdsnc.cn/gtucotoffl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xziqi.cn/gtvzalfjpz.html

[M06] 向标准错误输出
来源：http://hz.xylfe.cn/gtjvmwgstf.html

Py:   print("err", file=sys.stderr)
来源：http://hz.iojbl.cn/gtatubipvg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xuanzx.com/gtsspnlllb.html

JS:   console.error("err")
来源：http://hz.havefunace.top/gtwijyxaha.html

TS:   console.error("err")
来源：http://hz.gaohongyu789.top/gtsfncjwhr.html

Java: System.err.println("err")
来源：http://hz.pycfn.com/gtvmqubilk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yanxiufei.cn/gtyrejotjm.html

Ruby: warn "err"
来源：http://hz.ydzc1.top/gtqbntvmwj.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jianghu66.top/gtxxjzkznw.html

[M07] 判断是否为主入口
来源：http://hz.0kj1m.cn/gtuhsbqhfy.html

Py:   if __name__ == "__main__":
来源：http://hz.shangyingyoupin.top/gtteescjol.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hammf.cn/gtyzjkpsuo.html

JS:   require.main === module
来源：http://hz.hysaishi.cn/gtypypgzkm.html

TS:   require.main === module
来源：http://hz.pycfn.com/gtwnsrslss.html

Java: public static void main(String[] args)
来源：http://hz.cqqwz.cn/gtomwsgmpv.html

Go:   func main()
来源：http://hz.sxryk.cn/gtdwcgvrei.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhijiandao.cn/gtlicaptce.html

C#:   static void Main(string[] args)
来源：http://hz.52xcode.cn/gtfjqgijvk.html

[M08] 获取系统与运行时信息
来源：http://hz.xylfe.cn/gtqsjdsris.html

Py:   platform.system();  platform.python_version()
来源：http://hz.gaohongyu789.top/gttldpulql.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.havefunace.top/gtmzfcffdn.html

JS:   process.platform;  process.version
来源：http://hz.hysaishi.cn/gtiqnkdfnp.html

TS:   process.platform;  process.version
来源：http://hz.9152youxi.cn/gtnawhefuq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.kuanghao11.cn/gtkrjppcnj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cqqwz.cn/gtyngphxsx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cucudq.cn/gtfnutubml.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.haohaochexian.top/gttsbtthsx.html

================================================================================
来源：http://hz.sxryk.cn/gtjqybgcrx.html

N. 数据结构与算法
来源：http://hz.ivvv.top/gtcyczdcrs.html

================================================================================
来源：http://hz.bjfxy.top/gtutdxmnzt.html

[N01] 二分查找（有序数组）
来源：http://hz.chenzaomai.com/gtdjwcichq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.chenlongwang.top/gteuzrawvl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yongpay.top/gtpywmhnvm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jlsjyb.cn/gtvsrpzgft.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ydjk.org.cn/gtqnezkhfy.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ydjk.org.cn/gtqvikgcnr.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.chenjidiqi.icu/gtnaubncwy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jiagoushi.top/gtbirygtlz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sweek.top/gtgneuzklo.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.shanyushiyangkeji.top/gtjnuzllyf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cdnleiting.top/gtddfftaqi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yangfankeji.com/gtrwhysmmc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gogol.net.cn/gtwhntrjxb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xziqi.cn/gtxdkdatpk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zycfv.cn/gtaeeutqsg.html

Go:   slices.Sort(arr)
来源：http://hz.jqgufenzy.top/gtagwcmeyt.html

Ruby: arr.sort
来源：http://hz.gotoacloud.top/gtbbnjdmra.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sweek.top/gtuipmbdaq.html

[N03] 快速排序（分治示例）
来源：http://hz.tanke756.top/gthohpukdn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhongyouzk.top/gteovaxpnf.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xziqi.cn/gtedkaejab.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zycfv.cn/gtcczrtfjl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jiagoushi.top/gteukmzjzi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.fengsongda.top/gtcaplhihc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cheryme.top/gthujakijr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.gotoacloud.top/gtidodqthu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.9152youxi.cn/gtadmzlmwn.html

[N04] 斐波那契数列
来源：http://hz.cashguo.top/gtrvhnyxva.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigfzy.top/gtdzvjjasd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hfpthk.cn/gtzhrhdfpg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sxryk.cn/gtpyhtzsho.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dashuyun.cn/gtbcwhkvup.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shzxlz.cn/gtutjmndty.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jqgfzy.top/gtsocfwfoo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cqqwz.cn/gtxuefpjjy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.snrcjt.cn/gtbgbrdkwi.html

[N05] 最大公约数
来源：http://hz.yuxming.cn/gteolcyewu.html

Py:   math.gcd(a, b)
来源：http://hz.wangshuangyany.cn/gtyxgxgyec.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.tianlin.xyz/gtmakclieg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xziqi.cn/gtettxwimg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hysaishi.cn/gtrpkdgnef.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yj202588.top/gtmoqfhxlq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhaomingkeji.xyz/gtbxxaxqux.html

Ruby: a.gcd(b)
来源：http://hz.feifeiyinyue.top/gtznyxufxr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhixingplan.top/gtanvpsotp.html

[N06] 判断回文字符串
来源：http://hz.jinqigufen.top/gttzodobsr.html

Py:   s == s[::-1]
来源：http://hz.vqdsnc.cn/gtnqwwqhxv.html

PHP:  $s === strrev($s);
来源：http://hz.jinghuilouyu.cn/gtbrfdimek.html

JS:   s === [...s].reverse().join("")
来源：http://hz.haohaochexian.top/gtjiebgdgo.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yueranfly.top/gtwhrlwyek.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.guannengcc.top/gttypywhpm.html

Go:   // 双指针从两端比较
来源：http://hz.nanxuanxn.top/gtyllgupkh.html

Ruby: s == s.reverse
来源：http://hz.yonumen.top/gtxvgzrmdu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.daxiang520.top/gttvrmobyr.html

[N07] 两数之和（返回下标）
来源：http://hz.kuanghao11.cn/gthopwmqhh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.daria6918.cn/gtbwzvqfoz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ydzc1.top/gtkavegebl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.vqdsnc.cn/gtqlwtjvov.html

TS:   // 手写 Map<string, number>
来源：http://hz.haohaochexian.top/gtbweqdptl.html

Java: // 手写 HashMap
来源：http://hz.birdmap.top/gtsapuskzu.html

Go:   // 手写 map[int]int
来源：http://hz.yj202588.top/gtzwttugvr.html

Ruby: // 手写 Hash
来源：http://hz.ivvv.top/gtfnzpimrm.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yangfankeji.com/gtuxjicwgd.html

[N08] 生成全排列
来源：http://hz.pengpengdd.cyou/gtrgqqepsp.html

Py:   itertools.permutations(arr)
来源：http://hz.gotoacloud.top/gtmmxvxynn.html

PHP:  // 手写递归交换
来源：http://hz.jyoumei.cn/gtuzfojhxd.html

JS:   // 手写回溯递归
来源：http://hz.pycfn.com/gtanfzbgqs.html

TS:   // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gtfstnnbhm.html

Java: // 手写回溯递归
来源：http://hz.ydzc1.top/gtevooqjbq.html

Go:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtriutflrq.html

Ruby: arr.permutation.to_a
来源：http://hz.andypj.xyz/gtmxpiogcb.html

C#:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtpuzjzqlz.html

[N09] 栈与队列
来源：http://hz.ehwqpu.com/gtwabuzrxz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.aibaodan.cn/gtwejmvekw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jiagoushi.top/gtqkcfufrg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yonumen.top/gtlscgjcqo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.birdmap.top/gtfrwosxvl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ydjk.org.cn/gtxovjnbww.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.guowangkeji.top/gtwjeuyxwx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.snrcjt.cn/gtcrfjrdbg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.cdnleiting.top/gtkyykprqb.html

[N10] 链表节点定义
来源：http://hz.xuetiantiany.cn/gtdynghnxm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shanyushiyangtech.top/gtaswnzejz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.fengsongda.top/gtssgqgpaf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhongyouzk.top/gtftilyhio.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.pycfn.com/gtaesmfydl.html

Java: class Node { int v; Node next; }
来源：http://hz.chenzaomai.com/gtflytesuz.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.fengsongda.top/gtqcjcbcro.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cashguo.top/gtvcdngyhn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xylfe.cn/gtlqefxjmo.html

[N11] 二叉树中序遍历
来源：http://hz.ybcxt.top/gtkdfcutfm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.guannengcc.top/gtkkfpcnbb.html

PHP:  // 手写递归函数
来源：http://hz.yongpay.top/gtlnnryelz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj20258888.top/gtynfvnwia.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.smart0.xyz/gtbypfibze.html

Java: // 手写递归
来源：http://hz.chenjidiqi.icu/gtkflkshqn.html

Go:   // 手写递归
来源：http://hz.zhaomingkeji.xyz/gtwlamrsny.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.daria6918.cn/gtoaccwxgm.html

C#:   // 手写递归
来源：http://hz.shuidangran.top/gtdwlrqouq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xziqi.cn/gtpqgzjdns.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xuetiantiany.cn/gtcxsabrke.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.smart0.xyz/gtuwlpysnf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.bjfxy.top/gttftxndet.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258888.top/gtulsxmkse.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yvedp.cn/gttoyxgors.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jlsjyb.cn/gtikehthvc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.gotoacloud.top/gtdlgdmzhw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hysaishi.cn/gttsbqkiso.html

================================================================================
来源：http://hz.jlsjyb.cn/gttlfksubj.html

O. 并发与异步
来源：http://hz.gotoacloud.top/gtlrshgnyj.html

================================================================================
来源：http://hz.svipenyu.cn/gthczvjhyb.html

[O01] 启动一个线程
来源：http://hz.cqqwz.cn/gtveitytgi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.chenzaomai.com/gtowmzxvst.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.daxiang520.top/gtvyxjttcr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jlsjyb.cn/gtwnrmgawt.html

TS:   // 同 JS
来源：http://hz.jinqigfzy.top/gtlhjcpmqv.html


<!-- 参考信息 -->