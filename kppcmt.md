代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://hz.jinghuilouyu.cn/gtvuurdnfb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.52xcode.cn/gtwvmiemra.html

JS:   structuredClone(obj)
来源：http://hz.sufxvd.cn/gtkwozehxc.html

TS:   structuredClone(obj)
来源：http://hz.ybcxt.top/gttkaaoguu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.redwolf501.top/gtjausymbh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jqgfzy.top/gtwqczwqts.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.chenlongwang.top/gtawociywa.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hongshengwenyu.top/gtbyzcduya.html

[K06] 解析 URL 查询串
来源：http://hz.hongshengwenyu.top/gtolugsthd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jyoumei.cn/gtwihqvhxf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yonumen.top/gtzkqhpkjq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aibaodan.cn/gtkienuwsy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ivvv.top/gtoramspzk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shzxlz.cn/gtegigcuaz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gthqedqacb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yanxiufei.cn/gtprxevxbi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jiagoushi.top/gtnxbcvayz.html

[K07] 进制转换
来源：http://hz.jinqigufen.top/gtrevmozza.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cashguo.top/gtxehrgbch.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.snrcjt.cn/gtxsyrgpsv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yanxiufei.cn/gtabmnruzy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhiwuduotai.top/gtxjooznma.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yuxming.cn/gtcdkmwlmn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hnqzz.top/gthiaogcye.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.daria6918.cn/gtkdmichsl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hysaishi.cn/gtqwsbynma.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.nwbrower.top/gtysoyuxue.html

Py:   pickle.dumps(obj)
来源：http://hz.aizwys.cn/gtbkfgzhmj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hywenlv.cn/gtswjifomb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yongpay.top/gtvowmiggu.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ivvv.top/gtayofntho.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yj20258888.top/gtdplzerqi.html

Go:   encoding/gob
来源：http://hz.hnxiangtu.top/gtvudoinel.html

Ruby: Marshal.dump(obj)
来源：http://hz.tanke756.top/gttowleeuu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.wangshuangyany.cn/gtvbtanlxo.html

================================================================================
来源：http://hz.zhongyouzk.top/gtrawcaadj.html

L. 网络请求
来源：http://hz.fengsongda.top/gtkijnvhtw.html

================================================================================
来源：http://hz.cheryme.top/gtqgyjtdlx.html

[L01] 发送 GET 请求
来源：http://hz.sufxvd.cn/gtxvoxyihn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.shangyingyoupin.top/gtsjrjfouk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhijiandao.cn/gtqtweyieg.html

JS:   await fetch(url)
来源：http://hz.zhijiandao.cn/gtpfhtehuw.html

TS:   await fetch(url)
来源：http://hz.nanxuanxn.top/gtwbotdzij.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yuanzhike.top/gtelalwogh.html

Go:   resp, err := http.Get(url)
来源：http://hz.bjfxy.top/gtwgflkvzd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shanyushiyangkeji.top/gtfrfifzuy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.quarkkingdee.top/gthhjrgqar.html

[L02] 发送 POST JSON
来源：http://hz.gogol.net.cn/gtxovwqcvq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zycfv.cn/gtrzwkohfm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hywenlv.cn/gtbcpkzkdz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.guannengcc.top/gtlqggfafw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.quarkkingdee.top/gtgeoxgrks.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sysykeji.top/gtxfkaifvw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.dashuyun.cn/gtargxbpcl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sufxvd.cn/gtjwzdrqca.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.nanxinkj.top/gtljxnftde.html

[L03] 设置自定义请求头
来源：http://hz.zycfv.cn/gtfywemevd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.smart0.xyz/gtyjfdmnch.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.wangshuangyany.cn/gtotzmglbn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.redwolf501.top/gtmkuesosw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nwbrower.top/gtafmxtrow.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jqgufenzy.top/gtgjwtirxp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ydzc1.top/gtudglccyo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.andypj.xyz/gtbzkrhheh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shangyingyoupin.top/gtdrbsvcrz.html

[L04] 设置超时
来源：http://hz.yuxming.cn/gtgapnhyhn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.aibaodan.cn/gtflmfwjlg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jqgufenzy.top/gtazrethrx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hammf.cn/gtbspaqtqh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenjidiqi.icu/gtjqihvvng.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.meibo888.top/gtfgyvlqnb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.kuanghao11.cn/gtzzkhxhau.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cheryme.top/gtnzqsoaed.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xziqi.cn/gtmeabkaqn.html

[L05] 上传文件（multipart）
来源：http://hz.jiagoushi.top/gtqsizjass.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xingfuxueyuan.xyz/gtciaieweu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.wangshuangyany.cn/gtsajkribx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zdqjudy.top/gtzfjjurlc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hnqzz.top/gtbqsqmzcn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.fengsongda.top/gteyivwlem.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.52xcode.cn/gtjqrshsxg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.52xcode.cn/gteodaeozs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hysaishi.cn/gtoeuedydc.html

[L06] 解析响应为 JSON
来源：http://hz.quarkkingdee.top/gtwaehebet.html

Py:   resp.json()
来源：http://hz.cashguo.top/gtmcrsnsmv.html

PHP:  json_decode($body, true);
来源：http://hz.jqgfzy.top/gthrlbrnto.html

JS:   await resp.json()
来源：http://hz.iojbl.cn/gtsqfpygfy.html

TS:   await resp.json()
来源：http://hz.yj202588.top/gtstmrfgzo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhaomingkeji.xyz/gtmxcamtqv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.haohaochexian.top/gtwxrbhrxz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhijiandao.cn/gtghrwgmsr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xylfe.cn/gtmblixexo.html

[L07] 处理 HTTP 状态码
来源：http://hz.vqdsnc.cn/gtwrhtafks.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.redwolf501.top/gtwvbkpkyz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhixingplan.top/gttuuycqxa.html

JS:   resp.ok;  resp.status
来源：http://hz.jinqigufen.top/gtnkfstifc.html

TS:   resp.ok;  resp.status
来源：http://hz.316326.xyz/gtadnirwcf.html

Java: resp.statusCode()
来源：http://hz.kuanghao11.cn/gtjgguxwbg.html

Go:   resp.StatusCode
来源：http://hz.cqqwz.cn/gtbsucqfzx.html

Ruby: resp.code.to_i
来源：http://hz.ywan-chungtsiang.top/gtxdtpltgh.html

C#:   (int)resp.StatusCode
来源：http://hz.jyoumei.cn/gtxdnpbtwu.html

[L08] 并发请求多个地址
来源：http://hz.jinqigfzy.top/gtznscbsmf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.316326.xyz/gtsmewrfbi.html

PHP:  curl_multi_init() 系列
来源：http://hz.ywan-chungtsiang.top/gthrqyyopf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxinkj.top/gtvpqutwfw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sufxvd.cn/gtbkkjvdhy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ehwqpu.com/gttsilcpiu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yuanzhike.top/gtfwiukayp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ydzc1.top/gtgbjsukfb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shuidangran.top/gtoudencyu.html

================================================================================
来源：http://hz.yj20258.top/gtmfgeopmp.html

M. 命令行 / 进程 / 环境
来源：http://hz.ydzc1.top/gtcewxuigv.html

================================================================================
来源：http://hz.jyoumei.cn/gthlkrynwf.html

[M01] 读取命令行参数
来源：http://hz.dianchejie.cn/gtbjwgfjjp.html

Py:   sys.argv[1:]
来源：http://hz.wangdashe.top/gtvqvdyuup.html

PHP:  $argv;  $argc;
来源：http://hz.sxryk.cn/gtvceyvfsg.html

JS:   process.argv.slice(2)
来源：http://hz.nanxuanxn.top/gtwzbtzqzc.html

TS:   process.argv.slice(2)
来源：http://hz.nanxinkj.top/gtyrfroxhc.html

Java: args 数组（main 方法参数）
来源：http://hz.chenjidiqi.icu/gtgokfqfiu.html

Go:   os.Args[1:]
来源：http://hz.shanyushiyangtech.top/gtehojlhxd.html

Ruby: ARGV
来源：http://hz.guannengcc.top/gtufdvtqfa.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sxryk.cn/gtqwbumhvk.html

[M02] 读取环境变量
来源：http://hz.smart0.xyz/gtmtifcqne.html

Py:   os.environ.get("HOME")
来源：http://hz.jinqigfzy.top/gtfithqbkl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ppjwa.cn/gtwdmeddte.html

JS:   process.env.HOME
来源：http://hz.haohaochexian.top/gttuwqjmzc.html

TS:   process.env.HOME
来源：http://hz.chenzaomai.com/gtwutytohf.html

Java: System.getenv("HOME")
来源：http://hz.yvedp.cn/gtbjekorfu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cdnleiting.top/gtfkfxxwou.html

Ruby: ENV["HOME"]
来源：http://hz.chenlongwang.top/gtnrwhjnof.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.tianlin.xyz/gtfsjudnsv.html

[M03] 执行外部命令
来源：http://hz.cheryme.top/gtsitkwung.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.daxiang520.top/gtxtmlquaa.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.nanxuanxn.top/gtqxvnykon.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xingfuxueyuan.xyz/gtwiuuijht.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuanzhike.top/gtjqkkbcbf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.bjfxy.top/gtsdpoehmn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hywenlv.cn/gttywparlk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jyoumei.cn/gttrvuuhov.html

C#:   Process.Start("ls", "-l");
来源：http://hz.kuanghao11.cn/gtrxxmewch.html

[M04] 获取当前工作目录
来源：http://hz.cheryme.top/gtkhciqnsu.html

Py:   os.getcwd()
来源：http://hz.ydzc1.top/gtxrvfczph.html

PHP:  getcwd();
来源：http://hz.mhx1999.top/gttamxgznl.html

JS:   process.cwd()
来源：http://hz.jlsjyb.cn/gtaxmqdxtu.html

TS:   process.cwd()
来源：http://hz.nwbrower.top/gtvmwxpnxc.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhixingplan.top/gtlsftljhi.html

Go:   os.Getwd()
来源：http://hz.redwolf501.top/gtlrtfedmn.html

Ruby: Dir.pwd
来源：http://hz.redwolf501.top/gtultyjkgs.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.tanke756.top/gtobphcsbr.html

[M05] 设置退出码
来源：http://hz.redwolf501.top/gtdhnrtbyz.html

Py:   sys.exit(1)
来源：http://hz.yanxiufei.cn/gtrrajmouc.html

PHP:  exit(1);
来源：http://hz.cheryme.top/gtabavfprr.html

JS:   process.exit(1)
来源：http://hz.jyoumei.cn/gtqnrypfhp.html

TS:   process.exit(1)
来源：http://hz.cdnleiting.top/gtbgmqlobu.html

Java: System.exit(1)
来源：http://hz.cqqwz.cn/gtnjjhlxor.html

Go:   os.Exit(1)
来源：http://hz.tanke756.top/gtbalapdcx.html

Ruby: exit 1
来源：http://hz.havefunace.top/gtntbstuqp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sysykeji.top/gtuccidcgi.html

[M06] 向标准错误输出
来源：http://hz.snrcjt.cn/gtwmvwjdwi.html

Py:   print("err", file=sys.stderr)
来源：http://hz.pengpengdd.cyou/gtzzprfzny.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ybcxt.top/gtanzoafck.html

JS:   console.error("err")
来源：http://hz.sxryk.cn/gtedsbppwo.html

TS:   console.error("err")
来源：http://hz.haohaochexian.top/gtmvbfictp.html

Java: System.err.println("err")
来源：http://hz.shangyingyoupin.top/gtzrdchkxd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.quarkkingdee.top/gtbztapfdy.html

Ruby: warn "err"
来源：http://hz.guannengcc.top/gtaskhezrb.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.kuanghao11.cn/gtowjvmkcx.html

[M07] 判断是否为主入口
来源：http://hz.zhiwuduotai.top/gtdvzkjmsv.html

Py:   if __name__ == "__main__":
来源：http://hz.xuetiantiany.cn/gtcjuxwhub.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ywan-chungtsiang.top/gtsqjvhlwj.html

JS:   require.main === module
来源：http://hz.ywan-chungtsiang.top/gtcashtnrl.html

TS:   require.main === module
来源：http://hz.gzhubu.top/gtlhhjiguh.html

Java: public static void main(String[] args)
来源：http://hz.snrcjt.cn/gtxtqoebel.html

Go:   func main()
来源：http://hz.c1oappe.top/gtieetmmhu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hnqzz.top/gtkwutorkw.html

C#:   static void Main(string[] args)
来源：http://hz.aizwys.cn/gtpkvtxxxl.html

[M08] 获取系统与运行时信息
来源：http://hz.yangfankeji.com/gtqtfjwers.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yanxiufei.cn/gthsrgqjxn.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shangyingyoupin.top/gtdouhskby.html

JS:   process.platform;  process.version
来源：http://hz.tanke756.top/gtmjlwxdry.html

TS:   process.platform;  process.version
来源：http://hz.haohaochexian.top/gtejbamaej.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sysykeji.top/gtsuqygdey.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xuetiantiany.cn/gtqwwqhfir.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ydzc1.top/gtupxcgztg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.gotoacloud.top/gtczejolsa.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtjagmkhgo.html

N. 数据结构与算法
来源：http://hz.xuanzx.com/gthjmfhmix.html

================================================================================
来源：http://hz.cheryme.top/gtuvcwgkcc.html

[N01] 二分查找（有序数组）
来源：http://hz.sufxvd.cn/gtyldinmcl.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yongpay.top/gtzjvlreqa.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ppjwa.cn/gtzujjsyze.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shzxlz.cn/gtrszbuysb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhixingplan.top/gtxpknkyxq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zycfv.cn/gteugvmbgc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.daxiang520.top/gtpkqdtpnk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.pengpengdd.cyou/gthywdiepd.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.nanxuanxn.top/gtwbltesws.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.guowangkeji.top/gtqcbjhxgy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shuidangran.top/gtipqpavxe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ppjwa.cn/gtuiyxsyaj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.pycfn.com/gtppriasif.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ppjwa.cn/gtqlzyfemq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhaomingkeji.xyz/gtyrhaeaqn.html

Go:   slices.Sort(arr)
来源：http://hz.quarkkingdee.top/gtlxbttmab.html

Ruby: arr.sort
来源：http://hz.yj20258888.top/gthyahicrm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shzxlz.cn/gtwtjkldzo.html

[N03] 快速排序（分治示例）
来源：http://hz.jinghuilouyu.cn/gtenulgqej.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ywan-chungtsiang.top/gttsaenbtu.html

PHP:  // 递归实现，或用 usort
来源：http://hz.andypj.xyz/gtjlnhfvku.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ivvv.top/gtkgglxula.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yanxiufei.cn/gtzfitjfgg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xylfe.cn/gtpldvmday.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ydzc1.top/gtdcynvcrw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.nanxinkj.top/gtxvxvjfrw.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xuetiantiany.cn/gtvwflphfo.html

[N04] 斐波那契数列
来源：http://hz.pycfn.com/gtooodivvb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.0kj1m.cn/gtbfjqsfhr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.0kj1m.cn/gtwbrycdsz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.9152youxi.cn/gtdtyalwgg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.52xcode.cn/gtbqminebm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zdqjudy.top/gtvbumzmco.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.0kj1m.cn/gtlocueagc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.fengsongda.top/gtxeisrdkj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sxryk.cn/gthsttgogb.html

[N05] 最大公约数
来源：http://hz.yj20258888.top/gtiyudimlf.html

Py:   math.gcd(a, b)
来源：http://hz.gzhubu.top/gtdseiubpd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zdqjudy.top/gtakoeihmu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhengqikj.top/gtoxxrrlkq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yueranfly.top/gtjvomfwwl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.vqdsnc.cn/gtfhnfxupp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hfpthk.cn/gtmsvviahm.html

Ruby: a.gcd(b)
来源：http://hz.zhaomingkeji.xyz/gtfxnbhfig.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yanxiufei.cn/gtzeemkjdy.html

[N06] 判断回文字符串
来源：http://hz.nanxuanxn.top/gtcydjwato.html

Py:   s == s[::-1]
来源：http://hz.chenlongwang.top/gtxumesttn.html

PHP:  $s === strrev($s);
来源：http://hz.vqdsnc.cn/gtivwpkhbq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtwurquybn.html

TS:   s === [...s].reverse().join("")
来源：http://hz.bjfxy.top/gtsbezlfei.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sufxvd.cn/gtnxvahutv.html

Go:   // 双指针从两端比较
来源：http://hz.yj20258.top/gtdawuvfxn.html

Ruby: s == s.reverse
来源：http://hz.tanke756.top/gtncdiisvu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jlsjyb.cn/gtebrirnzz.html

[N07] 两数之和（返回下标）
来源：http://hz.sufxvd.cn/gtguhjofso.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.fengsongda.top/gttvojiiin.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gotoacloud.top/gtsgyfujfe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.guowangkeji.top/gtlnvzxerj.html

TS:   // 手写 Map<string, number>
来源：http://hz.yj20258.top/gtjvzrnhuc.html

Java: // 手写 HashMap
来源：http://hz.guowangkeji.top/gtazsemwsv.html

Go:   // 手写 map[int]int
来源：http://hz.tian-w.cn/gtrhsfzslp.html

Ruby: // 手写 Hash
来源：http://hz.kuanghao11.cn/gtdkqrlypy.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.svipenyu.cn/gtemjupagp.html

[N08] 生成全排列
来源：http://hz.zhiwuduotai.top/gtrriqmbud.html

Py:   itertools.permutations(arr)
来源：http://hz.316326.xyz/gtpbdqkcmq.html

PHP:  // 手写递归交换
来源：http://hz.yj20258888.top/gtigmfhbcj.html

JS:   // 手写回溯递归
来源：http://hz.nwbrower.top/gtequditen.html

TS:   // 手写回溯递归
来源：http://hz.cheryme.top/gthqmoysng.html

Java: // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtfkgmgsfp.html

Go:   // 手写回溯递归
来源：http://hz.yueranfly.top/gtjjsgkivx.html

Ruby: arr.permutation.to_a
来源：http://hz.shangyingyoupin.top/gtxpvveadr.html

C#:   // 手写回溯递归
来源：http://hz.52xcode.cn/gteaufypcq.html

[N09] 栈与队列
来源：http://hz.ppjwa.cn/gthpxdkaaz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jinghuilouyu.cn/gtphwkglsl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.havefunace.top/gtrbueorkv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cdnleiting.top/gtdofuwbhf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jyoumei.cn/gtzxkwxkrg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.cheryme.top/gtvtokpnie.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.daxiang520.top/gtpaxqpnqe.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hnqzz.top/gtxdbvmmeb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.wangdashe.top/gtazsjtzuj.html

[N10] 链表节点定义
来源：http://hz.hammf.cn/gtdixsvvoz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ppjwa.cn/gtzchuybmu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cucudq.cn/gtgdcgysji.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.aibaodan.cn/gtrlcorpsx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.tian-w.cn/gtyoeqortv.html

Java: class Node { int v; Node next; }
来源：http://hz.havefunace.top/gtdmblwgsh.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jinqigufen.top/gtcqelywou.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cdnleiting.top/gttkimzpvv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hysaishi.cn/gttohknnlh.html

[N11] 二叉树中序遍历
来源：http://hz.jlsjyb.cn/gtbeimspuf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhixingplan.top/gtgukrffuy.html

PHP:  // 手写递归函数
来源：http://hz.yj202588.top/gtczwbpkds.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xuetiantiany.cn/gtwojvcvrt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ywan-chungtsiang.top/gttywdoytr.html

Java: // 手写递归
来源：http://hz.jlsjyb.cn/gtaaygeslg.html

Go:   // 手写递归
来源：http://hz.aibaodan.cn/gtamnlpjtg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.sufxvd.cn/gthbdjxevj.html

C#:   // 手写递归
来源：http://hz.gotoacloud.top/gtkzlpotop.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.chenlongwang.top/gtpplutqtm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhoulong.xyz/gtatilibyh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.wangdashe.top/gtisucziji.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tianlin.xyz/gthahjpadz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.aibaodan.cn/gtoredvdpo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jqgfzy.top/gtmcfoxycy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.pengpengdd.cyou/gtxupezsjm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xylfe.cn/gtxrjmxwhp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gaohongyu789.top/gtgituwjqc.html

================================================================================
来源：http://hz.yj202588.top/gtzjdjglpb.html

O. 并发与异步
来源：http://hz.vqdsnc.cn/gtvuaibzyr.html

================================================================================
来源：http://hz.cqqwz.cn/gtqflnloxm.html

[O01] 启动一个线程
来源：http://hz.zhiwuduotai.top/gtgadwpbuk.html


<!-- 参考信息 -->