代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.fengsongda.top/gtqbxvwvmq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.haohaochexian.top/gtljfuhcjg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.fzhhl.top/gtsepnokay.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.sysykeji.top/gtnbhlyjhu.html

[K06] 解析 URL 查询串
来源：http://hz.kuanghao11.cn/gtfumqyvsm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.pycfn.com/gtzyrrixrt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.tanke756.top/gtkddsnkof.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hywenlv.cn/gtstwwnjml.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydjk.org.cn/gtbosutnxa.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinghuilouyu.cn/gteocbymjl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xingfuxueyuan.xyz/gtbbhbybpl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.aibaodan.cn/gtzgfdofju.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shuidangran.top/gtfgseysoy.html

[K07] 进制转换
来源：http://hz.cucudq.cn/gtkciuhrgh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.tanke756.top/gtcnqigpmz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.dashuyun.cn/gtrqiumkqx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtdbsrkhfl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.meibo888.top/gtwtzjtsdq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.smart0.xyz/gtnllewvtv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.vqdsnc.cn/gtpfrxefbr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.haohaochexian.top/gtguukrrdw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhixingplan.top/gtrcjxzikb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ivvv.top/gtlpsckkdn.html

Py:   pickle.dumps(obj)
来源：http://hz.mhx1999.top/gtvgmrjnef.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yvedp.cn/gtbyjxweaq.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.9152youxi.cn/gtfkirotvz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.redwolf501.top/gthdfynhho.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.feifeiyinyue.top/gtxtahpptf.html

Go:   encoding/gob
来源：http://hz.sxryk.cn/gtkawmtjgr.html

Ruby: Marshal.dump(obj)
来源：http://hz.gzhubu.top/gtelevhjmx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.52xcode.cn/gtqqcqzynm.html

================================================================================
来源：http://hz.svipenyu.cn/gtjvfczaay.html

L. 网络请求
来源：http://hz.316326.xyz/gtsefhbfqt.html

================================================================================
来源：http://hz.gotoacloud.top/gtgcfgbwmy.html

[L01] 发送 GET 请求
来源：http://hz.xylfe.cn/gtyxvnyyrt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.pengpengdd.cyou/gtrjvzbmto.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.aizwys.cn/gtjdvawwhc.html

JS:   await fetch(url)
来源：http://hz.xylfe.cn/gtowofiido.html

TS:   await fetch(url)
来源：http://hz.guannengcc.top/gtfzsvrmqs.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cucudq.cn/gtllzuepmm.html

Go:   resp, err := http.Get(url)
来源：http://hz.hammf.cn/gtngnbmzjf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.fengsongda.top/gtyqpeqrvl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.pycfn.com/gtvxggsqdu.html

[L02] 发送 POST JSON
来源：http://hz.jinyuanbaomall.cn/gtndrwohiv.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.kuanghao11.cn/gtujbunypz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jqgfzy.top/gtxysiujyc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhongyouzk.top/gtcppdmlwx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.meibo888.top/gtmzebafqu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhengqikj.top/gtigkwwvse.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.quarkkingdee.top/gtdyymjiid.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.quarkkingdee.top/gtbhdmruqo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xingfuxueyuan.xyz/gtqvhorydh.html

[L03] 设置自定义请求头
来源：http://hz.nanxuanxn.top/gtzqtwynbn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yj20258888.top/gthgdgeuib.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhixingplan.top/gthhxgigxh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.52xcode.cn/gtkxaarzxh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.svipenyu.cn/gtiggtehjc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cashguo.top/gtkqonraaz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.wangdashe.top/gtfzruzhvx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hywenlv.cn/gtfshsiwqo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shzxlz.cn/gtipwbvfrg.html

[L04] 设置超时
来源：http://hz.cucudq.cn/gtdeyoxwlo.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yongpay.top/gtjezacshk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.shuidangran.top/gtvhnxlvjy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fengsongda.top/gtrfnbnkoa.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinyuanbaomall.cn/gtpilbbiqb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hammf.cn/gtkoeioslk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yuanzhike.top/gticxfqaxr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.vqdsnc.cn/gtymyxlmrk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yj20258888.top/gtepnquuvo.html

[L05] 上传文件（multipart）
来源：http://hz.haohaochexian.top/gtwiwjseay.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yangfankeji.com/gtxjjtxnqv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.sxryk.cn/gtrkdgfqpv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.fengsongda.top/gtvlgtnozs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yanxiufei.cn/gtkjaqqsor.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.birdmap.top/gtxonsjmjv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jinqigfzy.top/gtxjaunwdf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xylfe.cn/gtuousxsbm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.haohaochexian.top/gtpzvajbbr.html

[L06] 解析响应为 JSON
来源：http://hz.snrcjt.cn/gtighaxrxh.html

Py:   resp.json()
来源：http://hz.sxryk.cn/gtjztnttwc.html

PHP:  json_decode($body, true);
来源：http://hz.gotoacloud.top/gtqqbtaxjc.html

JS:   await resp.json()
来源：http://hz.aibaodan.cn/gtcywsmytk.html

TS:   await resp.json()
来源：http://hz.tianlin.xyz/gtazveihax.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yuxming.cn/gtdlgkiwwf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ydjk.org.cn/gtkacgvtof.html

Ruby: JSON.parse(resp.body)
来源：http://hz.9152youxi.cn/gtrhxnoflz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.chenlongwang.top/gtbvoybttd.html

[L07] 处理 HTTP 状态码
来源：http://hz.nwbrower.top/gtxutnnqkc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.9152youxi.cn/gtaaxvvzhh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.smart0.xyz/gtjykfjzwa.html

JS:   resp.ok;  resp.status
来源：http://hz.shangyingyoupin.top/gtzhrimhdd.html

TS:   resp.ok;  resp.status
来源：http://hz.chenzaomai.com/gtltldcqdn.html

Java: resp.statusCode()
来源：http://hz.haohaochexian.top/gtpgoznfvr.html

Go:   resp.StatusCode
来源：http://hz.sufxvd.cn/gthqdqcdol.html

Ruby: resp.code.to_i
来源：http://hz.yongpay.top/gttjorltbz.html

C#:   (int)resp.StatusCode
来源：http://hz.zhoulong.xyz/gtkeftehvq.html

[L08] 并发请求多个地址
来源：http://hz.aizwys.cn/gtbpuutgeo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hongshengwenyu.top/gtpyznleoj.html

PHP:  curl_multi_init() 系列
来源：http://hz.yanxiufei.cn/gtdkotieui.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuanzx.com/gtxokfwnvc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ywan-chungtsiang.top/gtfxxqzptk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xinyue.icu/gtzhyrzzzo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhoulong.xyz/gtddmeqlug.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.fzhhl.top/gtqpeoztte.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jiagoushi.top/gtqqawfqzv.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtdolyuwxo.html

M. 命令行 / 进程 / 环境
来源：http://hz.chenjidiqi.icu/gtrqwzycmy.html

================================================================================
来源：http://hz.gzhubu.top/gtkxxfhkgi.html

[M01] 读取命令行参数
来源：http://hz.meibo888.top/gtzonvzjsn.html

Py:   sys.argv[1:]
来源：http://hz.zdqjudy.top/gtmstqnyhd.html

PHP:  $argv;  $argc;
来源：http://hz.zhixingplan.top/gtwwyphjqd.html

JS:   process.argv.slice(2)
来源：http://hz.zhijiandao.cn/gtpogzzaxk.html

TS:   process.argv.slice(2)
来源：http://hz.tian-w.cn/gtmtvebqcn.html

Java: args 数组（main 方法参数）
来源：http://hz.cashguo.top/gtmxntytea.html

Go:   os.Args[1:]
来源：http://hz.hywenlv.cn/gtegxxmrvv.html

Ruby: ARGV
来源：http://hz.andypj.xyz/gtffvwhbtm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.chenlongwang.top/gtgglduafn.html

[M02] 读取环境变量
来源：http://hz.cheryme.top/gtymjweyog.html

Py:   os.environ.get("HOME")
来源：http://hz.fengsongda.top/gtvvkawgmg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hnqzz.top/gtonlkpepz.html

JS:   process.env.HOME
来源：http://hz.aibaodan.cn/gtjpyqwmek.html

TS:   process.env.HOME
来源：http://hz.yongpay.top/gtapqfwtcy.html

Java: System.getenv("HOME")
来源：http://hz.haohaochexian.top/gtpneurzjg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yueranfly.top/gtohukicjl.html

Ruby: ENV["HOME"]
来源：http://hz.mhx1999.top/gtuactxjon.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.kuanghao11.cn/gtbubwecuv.html

[M03] 执行外部命令
来源：http://hz.zhiwuduotai.top/gtjaehloyq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhixingplan.top/gtlthnbjnl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.feifeiyinyue.top/gtbavygiaa.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xylfe.cn/gtgwyajbiv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xingfuxueyuan.xyz/gtkvtqhzff.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.svipenyu.cn/gtecaidsgt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tanke756.top/gtnvupwaaj.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sweek.top/gtddpcefaz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hnqzz.top/gtucvjuqhz.html

[M04] 获取当前工作目录
来源：http://hz.shanyushiyangkeji.top/gtosdadigv.html

Py:   os.getcwd()
来源：http://hz.9152youxi.cn/gthjvkvzna.html

PHP:  getcwd();
来源：http://hz.yueranfly.top/gtqzpltmng.html

JS:   process.cwd()
来源：http://hz.hfpthk.cn/gtcahtbbzq.html

TS:   process.cwd()
来源：http://hz.pycfn.com/gtvduyhfib.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jiagoushi.top/gtnfmsfjjk.html

Go:   os.Getwd()
来源：http://hz.havefunace.top/gtsytniwun.html

Ruby: Dir.pwd
来源：http://hz.jianghu66.top/gtxgyjnlhq.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.gaohongyu789.top/gtagsvmgvq.html

[M05] 设置退出码
来源：http://hz.shanyushiyangkeji.top/gtnjjhymro.html

Py:   sys.exit(1)
来源：http://hz.quarkkingdee.top/gtrulwrljz.html

PHP:  exit(1);
来源：http://hz.zhiwuduotai.top/gtwngybbju.html

JS:   process.exit(1)
来源：http://hz.yj20258888.top/gtjxslnofe.html

TS:   process.exit(1)
来源：http://hz.gogol.net.cn/gtewniwqkg.html

Java: System.exit(1)
来源：http://hz.feifeiyinyue.top/gtzfyppggg.html

Go:   os.Exit(1)
来源：http://hz.hysaishi.cn/gtlfjqpouj.html

Ruby: exit 1
来源：http://hz.hammf.cn/gtyhtavnjb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.wangdashe.top/gtzcayzrrd.html

[M06] 向标准错误输出
来源：http://hz.vqdsnc.cn/gtkzfmchrb.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hysaishi.cn/gtxsqonipm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.sweek.top/gtjfkcjsid.html

JS:   console.error("err")
来源：http://hz.ydjk.org.cn/gtdqhmxlzm.html

TS:   console.error("err")
来源：http://hz.yangfankeji.com/gtwjnbvcqt.html

Java: System.err.println("err")
来源：http://hz.kuanghao11.cn/gtfwbipxia.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ehwqpu.com/gtedznrdea.html

Ruby: warn "err"
来源：http://hz.zdqjudy.top/gtiumfjzmx.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.redwolf501.top/gtynzgpdkd.html

[M07] 判断是否为主入口
来源：http://hz.shuidangran.top/gtsrisdqsh.html

Py:   if __name__ == "__main__":
来源：http://hz.jqgfzy.top/gtdujngenf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.iojbl.cn/gtlvgbldwh.html

JS:   require.main === module
来源：http://hz.yuxming.cn/gtuglenfdp.html

TS:   require.main === module
来源：http://hz.andypj.xyz/gtaqykmfbu.html

Java: public static void main(String[] args)
来源：http://hz.zhengqikj.top/gtpvegmwja.html

Go:   func main()
来源：http://hz.ybcxt.top/gtavvuvulj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.gogol.net.cn/gtkwwymlss.html

C#:   static void Main(string[] args)
来源：http://hz.jqgufenzy.top/gtpnvndvtg.html

[M08] 获取系统与运行时信息
来源：http://hz.smart0.xyz/gtagfcxraq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.quarkkingdee.top/gtltvcexzk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ybcxt.top/gtsdkxwhzh.html

JS:   process.platform;  process.version
来源：http://hz.fzhhl.top/gtuqtphyvo.html

TS:   process.platform;  process.version
来源：http://hz.sufxvd.cn/gttezodchk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jqgufenzy.top/gtcyqvhwkn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xuetiantiany.cn/gtrluzuwyl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.9152youxi.cn/gthoufhnqj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.aibaodan.cn/gtkwyqojre.html

================================================================================
来源：http://hz.tian-w.cn/gtqsqqkmby.html

N. 数据结构与算法
来源：http://hz.hongshengwenyu.top/gtiepxotfh.html

================================================================================
来源：http://hz.fengsongda.top/gtgbckdfww.html

[N01] 二分查找（有序数组）
来源：http://hz.aibaodan.cn/gtzczopmnw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gotoacloud.top/gtpndwclne.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.daria6918.cn/gthmxbahfo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.guowangkeji.top/gtftqhzdzh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.c1oappe.top/gteljimpno.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jiagoushi.top/gtprnctiat.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.nanxuanxn.top/gthtauiwtj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.daria6918.cn/gtgbskhozz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hfpthk.cn/gtqzkrqntg.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jiagoushi.top/gtwnanqmkm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sxryk.cn/gtbbjvbkoh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hnqzz.top/gtuddnlmiz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.9152youxi.cn/gtswaxrkui.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.c1oappe.top/gtzsjegrja.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.dashuyun.cn/gtdgqoqlsr.html

Go:   slices.Sort(arr)
来源：http://hz.cdnleiting.top/gtowuuggei.html

Ruby: arr.sort
来源：http://hz.zdqjudy.top/gtruashndl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yuxming.cn/gtyppokqlj.html

[N03] 快速排序（分治示例）
来源：http://hz.hfpthk.cn/gtihcofwuy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cucudq.cn/gtnlwptnys.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jqgfzy.top/gtghvlzhfh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhixingplan.top/gtkiiuoype.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.havefunace.top/gtdilrtrdj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.fengsongda.top/gtpwzszznr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.fzhhl.top/gtdtczelwf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yangfankeji.com/gtgegbekjs.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gzhubu.top/gtzsvkperb.html

[N04] 斐波那契数列
来源：http://hz.jqgfzy.top/gtmvibembh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cucudq.cn/gtzznejhlx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yangfankeji.com/gtbddgqdgu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nwbrower.top/gtagdotkfg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ybcxt.top/gtqkrffihb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.sysykeji.top/gturbembfe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinyuanbaomall.cn/gtvbmxoovv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.wangshuangyany.cn/gtykufuzae.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.daxiang520.top/gtvohlgcnp.html

[N05] 最大公约数
来源：http://hz.andypj.xyz/gtrbrmjtbr.html

Py:   math.gcd(a, b)
来源：http://hz.xuetiantiany.cn/gtldjxknap.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.pengpengdd.cyou/gtmmgdzqtb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jiagoushi.top/gtglduuztp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnxiangtu.top/gtsvvbnoju.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.chenjidiqi.icu/gtygdujcqd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.svipenyu.cn/gtjxnkhiet.html

Ruby: a.gcd(b)
来源：http://hz.guannengcc.top/gtiiapyzek.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xylfe.cn/gtgtybavzn.html

[N06] 判断回文字符串
来源：http://hz.yvedp.cn/gtaxbkfagl.html

Py:   s == s[::-1]
来源：http://hz.yongpay.top/gtxkemhdry.html

PHP:  $s === strrev($s);
来源：http://hz.hnxiangtu.top/gtnppxkwgr.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shanyushiyangkeji.top/gthzlmavrz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtljkkspff.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ivvv.top/gtftpdfmkz.html

Go:   // 双指针从两端比较
来源：http://hz.zhiwuduotai.top/gtsmxqvdni.html

Ruby: s == s.reverse
来源：http://hz.xziqi.cn/gttgaodnbe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cqqwz.cn/gtitswcwit.html

[N07] 两数之和（返回下标）
来源：http://hz.mhx1999.top/gtyvrzasim.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.52xcode.cn/gtwifsocfs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xziqi.cn/gttpowrgjy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhaomingkeji.xyz/gttkpqjfil.html

TS:   // 手写 Map<string, number>
来源：http://hz.yongpay.top/gtwgwvijqe.html

Java: // 手写 HashMap
来源：http://hz.jqgufenzy.top/gtcfoatcjw.html

Go:   // 手写 map[int]int
来源：http://hz.zhiwuduotai.top/gthazhmdus.html

Ruby: // 手写 Hash
来源：http://hz.fzhhl.top/gtzjtkgvns.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jqgfzy.top/gtnbynliks.html

[N08] 生成全排列
来源：http://hz.yueranfly.top/gtybccvgug.html

Py:   itertools.permutations(arr)
来源：http://hz.iojbl.cn/gtrypvqdpe.html

PHP:  // 手写递归交换
来源：http://hz.gzhubu.top/gttgnobehl.html

JS:   // 手写回溯递归
来源：http://hz.yueranfly.top/gtvxnroqzl.html

TS:   // 手写回溯递归
来源：http://hz.sysykeji.top/gtbubavbls.html

Java: // 手写回溯递归
来源：http://hz.quarkkingdee.top/gtvxyxtvnh.html

Go:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gtmifoxitz.html

Ruby: arr.permutation.to_a
来源：http://hz.kuanghao11.cn/gtjfzuvspe.html

C#:   // 手写回溯递归
来源：http://hz.dianchejie.cn/gtbpeuwdwl.html

[N09] 栈与队列
来源：http://hz.316326.xyz/gtrsjehter.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.daria6918.cn/gtdxfhgpsd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ywan-chungtsiang.top/gtyuahnfrf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.redwolf501.top/gtwtgengym.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jiagoushi.top/gtdtvglhdi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhixingplan.top/gttiykxkgy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.vqdsnc.cn/gtktkgzqku.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhongyouzk.top/gtcueotkap.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.daxiang520.top/gtafbfbmpo.html

[N10] 链表节点定义
来源：http://hz.xylfe.cn/gttajapnso.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.aibaodan.cn/gttnbyktvx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhengqikj.top/gtgbtbycwm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jinqigfzy.top/gtdxcmyppt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhiwuduotai.top/gtlluvpyjl.html

Java: class Node { int v; Node next; }
来源：http://hz.fzhhl.top/gtabtqiwsb.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.fengsongda.top/gtybbxrtdp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hywenlv.cn/gtzsmrqjor.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.dianchejie.cn/gtxyywljtc.html

[N11] 二叉树中序遍历
来源：http://hz.jinyuanbaomall.cn/gtarmqwozq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.9152youxi.cn/gtcpnnlxzu.html

PHP:  // 手写递归函数
来源：http://hz.shzxlz.cn/gtpksnufbt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinqigfzy.top/gtusjbvaon.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yvedp.cn/gtpdgrstvn.html

Java: // 手写递归
来源：http://hz.hywenlv.cn/gtrjpjzobu.html

Go:   // 手写递归
来源：http://hz.yangfankeji.com/gtqehsscal.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jinyuanbaomall.cn/gtnzdrwxgy.html

C#:   // 手写递归
来源：http://hz.52xcode.cn/gteyknbfgn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.quarkkingdee.top/gtrtgtcbev.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.shuidangran.top/gtdnmyqdvl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhengqikj.top/gtckzuhlfh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydjk.org.cn/gtffkvmplo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shanyushiyangtech.top/gtmxsadtah.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.dashuyun.cn/gtfjcfpkab.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.nwbrower.top/gtobokxedt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zycfv.cn/gtjibgtsam.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zycfv.cn/gtauiljbxy.html

================================================================================
来源：http://hz.nanxinkj.top/gtqnjkzrrs.html

O. 并发与异步
来源：http://hz.sysykeji.top/gtkarshkfs.html

================================================================================
来源：http://hz.hysaishi.cn/gtrfemtfoi.html

[O01] 启动一个线程
来源：http://hz.hnqzz.top/gtwfmishdn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.tian-w.cn/gtadezxssn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.svipenyu.cn/gtaizyxuwu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jinghuilouyu.cn/gtmyzlnnyi.html

TS:   // 同 JS
来源：http://hz.hnqzz.top/gtuzyywnqu.html


<!-- 参考信息 -->