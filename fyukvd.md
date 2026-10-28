代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xziqi.cn/gtixcjkpcj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.aibaodan.cn/gtnzdlrqdb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.wangdashe.top/gtahlmfwtp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.guowangkeji.top/gtddsbcgic.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xingfuxueyuan.xyz/gtxifjijpn.html

[K07] 进制转换
来源：http://hz.jinyuanbaomall.cn/gtzunqhzgd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.chenzaomai.com/gtysmqycgc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.0kj1m.cn/gtypzhcnge.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jyoumei.cn/gtgqekirla.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtlczwpeuq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.gotoacloud.top/gteafiflem.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.daria6918.cn/gtomlcepft.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hongshengwenyu.top/gtasmzcvpx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sxryk.cn/gtyigtqzyz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jlsjyb.cn/gtugnhifxh.html

Py:   pickle.dumps(obj)
来源：http://hz.zycfv.cn/gttnmzgyjp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shzxlz.cn/gtrnqvcoln.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.aizwys.cn/gtqmqjvmvy.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jqgfzy.top/gtuijgfwsq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shanyushiyangkeji.top/gtinlwqyin.html

Go:   encoding/gob
来源：http://hz.vqdsnc.cn/gtzrhdebal.html

Ruby: Marshal.dump(obj)
来源：http://hz.yanxiufei.cn/gtwmgcartz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yvedp.cn/gtkvucanrk.html

================================================================================
来源：http://hz.vqdsnc.cn/gttuquaggq.html

L. 网络请求
来源：http://hz.ybcxt.top/gtxyjyftsh.html

================================================================================
来源：http://hz.hnqzz.top/gtasowtlcw.html

[L01] 发送 GET 请求
来源：http://hz.jqgufenzy.top/gtaxacpynw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hfpthk.cn/gtgdocgrdr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.aibaodan.cn/gtpenqqsqa.html

JS:   await fetch(url)
来源：http://hz.gaohongyu789.top/gtgibtydxk.html

TS:   await fetch(url)
来源：http://hz.ybcxt.top/gtcpamytey.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shangyingyoupin.top/gtkntdibcm.html

Go:   resp, err := http.Get(url)
来源：http://hz.dashuyun.cn/gtybqgfxlg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cheryme.top/gtjlvkxupc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.sweek.top/gtkgfznltn.html

[L02] 发送 POST JSON
来源：http://hz.zdqjudy.top/gtquzohjyq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.316326.xyz/gtujachoaj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhongyouzk.top/gtizuwrkzw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ehwqpu.com/gtwvgbdvcn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.havefunace.top/gtjarlqwtu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yuanzhike.top/gtqutxfhdk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.svipenyu.cn/gtyrmtzguw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yuanzhike.top/gtapdnvbsg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zycfv.cn/gtazyvxkhw.html

[L03] 设置自定义请求头
来源：http://hz.daxiang520.top/gtkyvwzkci.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.sysykeji.top/gtcxvxuolp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shuidangran.top/gtozklycfe.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yanxiufei.cn/gteftrdflr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhoulong.xyz/gtovwpkxes.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.birdmap.top/gtsnhujymg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenzaomai.com/gtgbbysuqo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zdqjudy.top/gtndpzqwir.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yanxiufei.cn/gtkxqglyjh.html

[L04] 设置超时
来源：http://hz.0kj1m.cn/gtiibqwnio.html

Py:   requests.get(url, timeout=5)
来源：http://hz.tanke756.top/gtpcifztqt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hnxiangtu.top/gtlymfromg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinyuanbaomall.cn/gtkvlljcaz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gogol.net.cn/gthtujjfeo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cucudq.cn/gtyftvxasi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shuidangran.top/gtwpnbvjhb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.sxryk.cn/gtouatsudu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhijiandao.cn/gtukcuduud.html

[L05] 上传文件（multipart）
来源：http://hz.ivvv.top/gtpgqvxxxq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.tanke756.top/gtycdkneji.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xylfe.cn/gtnreckxoe.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydzc1.top/gtnsarfldj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.birdmap.top/gtoaffkzqh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.smart0.xyz/gtaasbnlcd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.pengpengdd.cyou/gtimedsovu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shanyushiyangtech.top/gtgmfhgnyo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.daria6918.cn/gtgbnhqvrq.html

[L06] 解析响应为 JSON
来源：http://hz.zhiwuduotai.top/gtnyafqylq.html

Py:   resp.json()
来源：http://hz.zycfv.cn/gtiyvweups.html

PHP:  json_decode($body, true);
来源：http://hz.tian-w.cn/gtkvyoarpk.html

JS:   await resp.json()
来源：http://hz.jqgufenzy.top/gtvghvmykq.html

TS:   await resp.json()
来源：http://hz.jqgfzy.top/gtyntwclbl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhongyouzk.top/gtepodqopp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cashguo.top/gtkuxsowht.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yuxming.cn/gtyfwvtjnp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.iojbl.cn/gtdyhkxjwc.html

[L07] 处理 HTTP 状态码
来源：http://hz.gotoacloud.top/gtgbevecou.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shanyushiyangtech.top/gtqeaalzpk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ehwqpu.com/gtpsisffgs.html

JS:   resp.ok;  resp.status
来源：http://hz.zhoulong.xyz/gtdbokghbs.html

TS:   resp.ok;  resp.status
来源：http://hz.yanxiufei.cn/gtfgkycbxr.html

Java: resp.statusCode()
来源：http://hz.daria6918.cn/gtiwdhydpd.html

Go:   resp.StatusCode
来源：http://hz.zhongyouzk.top/gtxlmucssk.html

Ruby: resp.code.to_i
来源：http://hz.snrcjt.cn/gtmfapktww.html

C#:   (int)resp.StatusCode
来源：http://hz.zhaomingkeji.xyz/gtpnzncinx.html

[L08] 并发请求多个地址
来源：http://hz.kuanghao11.cn/gtlmjosoly.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.aibaodan.cn/gtdasnrcfm.html

PHP:  curl_multi_init() 系列
来源：http://hz.shanyushiyangkeji.top/gtgauyrccw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xziqi.cn/gtiiflbtty.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yonumen.top/gtzbqmvlut.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.andypj.xyz/gtmasphwga.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.c1oappe.top/gtsxzvvsel.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhiwuduotai.top/gtutrxkfmf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yuanzhike.top/gthcqopjnc.html

================================================================================
来源：http://hz.guowangkeji.top/gtsqvpdtcy.html

M. 命令行 / 进程 / 环境
来源：http://hz.birdmap.top/gtgclxqrqo.html

================================================================================
来源：http://hz.nwbrower.top/gtrvstvmzj.html

[M01] 读取命令行参数
来源：http://hz.tianlin.xyz/gtbxmobvle.html

Py:   sys.argv[1:]
来源：http://hz.ehwqpu.com/gtnyxkooer.html

PHP:  $argv;  $argc;
来源：http://hz.9152youxi.cn/gtbouaobup.html

JS:   process.argv.slice(2)
来源：http://hz.316326.xyz/gtlobowkpl.html

TS:   process.argv.slice(2)
来源：http://hz.hysaishi.cn/gtmstjhfka.html

Java: args 数组（main 方法参数）
来源：http://hz.jyoumei.cn/gtftrooxmm.html

Go:   os.Args[1:]
来源：http://hz.hfpthk.cn/gtorsdsqrs.html

Ruby: ARGV
来源：http://hz.havefunace.top/gtjawwxeec.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jinyuanbaomall.cn/gtsbjjjwcy.html

[M02] 读取环境变量
来源：http://hz.zhiwuduotai.top/gtxbekgero.html

Py:   os.environ.get("HOME")
来源：http://hz.tanke756.top/gtjmujbjex.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yuanzhike.top/gtmtewzlbt.html

JS:   process.env.HOME
来源：http://hz.cashguo.top/gtbhvgxaeu.html

TS:   process.env.HOME
来源：http://hz.yj20258.top/gthoisvuxj.html

Java: System.getenv("HOME")
来源：http://hz.hysaishi.cn/gtohwnfbyp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.kuanghao11.cn/gtnrvdstic.html

Ruby: ENV["HOME"]
来源：http://hz.tianlin.xyz/gtaanltafu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.0kj1m.cn/gtafpgveqm.html

[M03] 执行外部命令
来源：http://hz.cucudq.cn/gtfqnounjj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.fzhhl.top/gtlqhktuzf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.wangshuangyany.cn/gtuvvhnxrw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cdnleiting.top/gtrwlqqtmx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.svipenyu.cn/gtsffcvvjm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sweek.top/gtffogxrlw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ivvv.top/gtefyknaeb.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.gzhubu.top/gtxftnpyox.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xuetiantiany.cn/gtzmlzqnzs.html

[M04] 获取当前工作目录
来源：http://hz.redwolf501.top/gtonukdlbr.html

Py:   os.getcwd()
来源：http://hz.sweek.top/gtbnxhnjsx.html

PHP:  getcwd();
来源：http://hz.jqgufenzy.top/gtttidhecu.html

JS:   process.cwd()
来源：http://hz.ywan-chungtsiang.top/gtrqwauias.html

TS:   process.cwd()
来源：http://hz.zhaomingkeji.xyz/gtfpztutio.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hongshengwenyu.top/gtcnrefhav.html

Go:   os.Getwd()
来源：http://hz.aibaodan.cn/gtgfiqlwik.html

Ruby: Dir.pwd
来源：http://hz.shzxlz.cn/gtmrqimwnh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yueranfly.top/gtenrlaeuf.html

[M05] 设置退出码
来源：http://hz.yangfankeji.com/gtochyzydr.html

Py:   sys.exit(1)
来源：http://hz.gogol.net.cn/gtjeatnofh.html

PHP:  exit(1);
来源：http://hz.nanxinkj.top/gtjexvbmrz.html

JS:   process.exit(1)
来源：http://hz.gotoacloud.top/gtbwdicmxr.html

TS:   process.exit(1)
来源：http://hz.aibaodan.cn/gtklivavlq.html

Java: System.exit(1)
来源：http://hz.jianghu66.top/gtytoifqpb.html

Go:   os.Exit(1)
来源：http://hz.tian-w.cn/gtbmvucxsr.html

Ruby: exit 1
来源：http://hz.hywenlv.cn/gtprkqlecb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.fzhhl.top/gtwxoxdnbl.html

[M06] 向标准错误输出
来源：http://hz.jyoumei.cn/gtznetvoxa.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhongyouzk.top/gtiocqiukr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.pycfn.com/gthstjddcu.html

JS:   console.error("err")
来源：http://hz.ydzc1.top/gtkkokysyi.html

TS:   console.error("err")
来源：http://hz.xziqi.cn/gtzkqdwnid.html

Java: System.err.println("err")
来源：http://hz.shangyingyoupin.top/gtiangszrw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.shangyingyoupin.top/gtpipqslcw.html

Ruby: warn "err"
来源：http://hz.smart0.xyz/gtbuljcyvm.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zdqjudy.top/gtbhfdvcpc.html

[M07] 判断是否为主入口
来源：http://hz.shuidangran.top/gtjeexivpe.html

Py:   if __name__ == "__main__":
来源：http://hz.yj20258888.top/gtotnnromr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.wangshuangyany.cn/gtltvaklrp.html

JS:   require.main === module
来源：http://hz.mhx1999.top/gtriaxeusg.html

TS:   require.main === module
来源：http://hz.zhaomingkeji.xyz/gtieyienoa.html

Java: public static void main(String[] args)
来源：http://hz.daria6918.cn/gtvtecgfdz.html

Go:   func main()
来源：http://hz.feifeiyinyue.top/gtiwdssqua.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.dianchejie.cn/gttfgapyhw.html

C#:   static void Main(string[] args)
来源：http://hz.hongshengwenyu.top/gtiohqryrb.html

[M08] 获取系统与运行时信息
来源：http://hz.wangshuangyany.cn/gtmuyoytgt.html

Py:   platform.system();  platform.python_version()
来源：http://hz.sxryk.cn/gtznoclneb.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.sxryk.cn/gtaagwijxk.html

JS:   process.platform;  process.version
来源：http://hz.ppjwa.cn/gtmpizxguq.html

TS:   process.platform;  process.version
来源：http://hz.xuanzx.com/gtfmzzqjeg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sxryk.cn/gtsgfsdbun.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.nanxinkj.top/gtqqoygneo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.aibaodan.cn/gteoycqbaz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhiwuduotai.top/gtnuhtbaef.html

================================================================================
来源：http://hz.c1oappe.top/gtwehisdae.html

N. 数据结构与算法
来源：http://hz.wangdashe.top/gtjezlgfyv.html

================================================================================
来源：http://hz.dashuyun.cn/gtvphdmunz.html

[N01] 二分查找（有序数组）
来源：http://hz.zhoulong.xyz/gtzpbwliwa.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zycfv.cn/gtiephhckp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shanyushiyangtech.top/gtbfdwdliz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xingfuxueyuan.xyz/gtplztpgll.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zycfv.cn/gtnlmelowh.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xinyue.icu/gtoqytiths.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhiwuduotai.top/gtxolvynur.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.tanke756.top/gtumixkyta.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.chenjidiqi.icu/gtgwjswtvo.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yongpay.top/gtgrphrhhf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.havefunace.top/gtnontkias.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhaomingkeji.xyz/gtwexyogsf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guowangkeji.top/gtdcypmaat.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.quarkkingdee.top/gtpkuyvilf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hfpthk.cn/gtoevisgzz.html

Go:   slices.Sort(arr)
来源：http://hz.wangdashe.top/gtlumrgkjv.html

Ruby: arr.sort
来源：http://hz.yj20258888.top/gtuonumqdu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xinyue.icu/gtfwenzhjw.html

[N03] 快速排序（分治示例）
来源：http://hz.fzhhl.top/gtcrcrzkpp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.tian-w.cn/gthretegqo.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ydzc1.top/gtytgtpdbl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgufenzy.top/gttuftcgtz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pycfn.com/gtstsatcbq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shangyingyoupin.top/gtncrvkedo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ppjwa.cn/gtbeqamrtn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yj202588.top/gtmxepizts.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.mhx1999.top/gtkmsswpdd.html

[N04] 斐波那契数列
来源：http://hz.pycfn.com/gtlhuxviyf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.feifeiyinyue.top/gtcwzbtyyn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.nwbrower.top/gtazqjufrs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xingfuxueyuan.xyz/gtpgrjkkqk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jiagoushi.top/gtrwqsbnvq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xziqi.cn/gtilunpeyu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sxryk.cn/gttukxjaqd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.wangdashe.top/gtpxowjwfu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.0kj1m.cn/gtkglwmldl.html

[N05] 最大公约数
来源：http://hz.hywenlv.cn/gtswoawcup.html

Py:   math.gcd(a, b)
来源：http://hz.jianghu66.top/gtewjxjjly.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shuidangran.top/gtvoboxhou.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangshuangyany.cn/gtexzrbusz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.birdmap.top/gtfwuxteaf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.cqqwz.cn/gtrausluvb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cdnleiting.top/gtaiudmcha.html

Ruby: a.gcd(b)
来源：http://hz.sweek.top/gttruajgke.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hywenlv.cn/gtjozxddau.html

[N06] 判断回文字符串
来源：http://hz.chenzaomai.com/gtxmkcvggy.html

Py:   s == s[::-1]
来源：http://hz.ehwqpu.com/gtdmcqjpbw.html

PHP:  $s === strrev($s);
来源：http://hz.zhengqikj.top/gthxykzclh.html

JS:   s === [...s].reverse().join("")
来源：http://hz.316326.xyz/gtdhvpzznx.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yj20258888.top/gtaokrkqqt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yueranfly.top/gthjmfglaa.html

Go:   // 双指针从两端比较
来源：http://hz.xziqi.cn/gtwtbfrqhz.html

Ruby: s == s.reverse
来源：http://hz.iojbl.cn/gtpxbufcrc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yangfankeji.com/gtoingufjj.html

[N07] 两数之和（返回下标）
来源：http://hz.fzhhl.top/gtocpsftzs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhoulong.xyz/gtszifenpe.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.tanke756.top/gtelpsbrrn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.feifeiyinyue.top/gtsetwhyig.html

TS:   // 手写 Map<string, number>
来源：http://hz.jinghuilouyu.cn/gttyjlvmjy.html

Java: // 手写 HashMap
来源：http://hz.havefunace.top/gthywidgts.html

Go:   // 手写 map[int]int
来源：http://hz.yj20258888.top/gtgsuxemtm.html

Ruby: // 手写 Hash
来源：http://hz.jianghu66.top/gtjnqnznkk.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hammf.cn/gtearagmkz.html

[N08] 生成全排列
来源：http://hz.wangdashe.top/gtzejidlpa.html

Py:   itertools.permutations(arr)
来源：http://hz.zhaomingkeji.xyz/gtwghdnged.html

PHP:  // 手写递归交换
来源：http://hz.zhengqikj.top/gtgzjzjhks.html

JS:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtvigcgunk.html

TS:   // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gtklhjhhdy.html

Java: // 手写回溯递归
来源：http://hz.hysaishi.cn/gtkvfxgwft.html

Go:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gtfvbtkmdl.html

Ruby: arr.permutation.to_a
来源：http://hz.quarkkingdee.top/gtdxslpnyh.html

C#:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtzbhlcagi.html

[N09] 栈与队列
来源：http://hz.dianchejie.cn/gtqjhkzkjy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.tian-w.cn/gttrpvltfa.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.guowangkeji.top/gtypnnljln.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yonumen.top/gtsrjvuxbz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.dianchejie.cn/gtxyzjslec.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinyuanbaomall.cn/gtdctpytui.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jqgfzy.top/gtowlsgdao.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hywenlv.cn/gtlkdlbkhs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.guannengcc.top/gtofyxxqzo.html

[N10] 链表节点定义
来源：http://hz.yuxming.cn/gtgfzkcrsq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.wangshuangyany.cn/gtyvcgreeq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hysaishi.cn/gtqqfnppry.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xylfe.cn/gtiosxvayj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.wangdashe.top/gtjkoqanpy.html

Java: class Node { int v; Node next; }
来源：http://hz.zhoulong.xyz/gtscqsthpi.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yanxiufei.cn/gtxyfgtslh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cashguo.top/gtpxmrxgrx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yonumen.top/gtpuqtfotn.html

[N11] 二叉树中序遍历
来源：http://hz.dashuyun.cn/gtdtlkarfk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.meibo888.top/gtofuxnkck.html

PHP:  // 手写递归函数
来源：http://hz.zycfv.cn/gtiawjqtbr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sysykeji.top/gtagxykpzf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.fzhhl.top/gtcsqstuie.html

Java: // 手写递归
来源：http://hz.shanyushiyangtech.top/gtdyquaqmg.html

Go:   // 手写递归
来源：http://hz.hnxiangtu.top/gtgscmqezh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yj20258888.top/gtkglnzpfn.html

C#:   // 手写递归
来源：http://hz.hammf.cn/gtxqeuhqbb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hongshengwenyu.top/gtwsvgrwza.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.c1oappe.top/gtpqyninxw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hnxiangtu.top/gtcbsnduco.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yueranfly.top/gtciuqbskl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gotoacloud.top/gtjlymbeqt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yonumen.top/gtzxfyfqcc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.nwbrower.top/gtdalnbekm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.havefunace.top/gttepciahq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xinyue.icu/gtfcpyeyhk.html

================================================================================
来源：http://hz.andypj.xyz/gtacpcaukq.html

O. 并发与异步
来源：http://hz.jinqigfzy.top/gtgjvhbqau.html

================================================================================
来源：http://hz.hnxiangtu.top/gtvgkyeolw.html

[O01] 启动一个线程
来源：http://hz.jianghu66.top/gtmrwbeisi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ppjwa.cn/gtonpajhen.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xingfuxueyuan.xyz/gtvkahawio.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.ydjk.org.cn/gtbgxlzzjb.html

TS:   // 同 JS
来源：http://hz.yuanzhike.top/gtpyoxtyug.html

Java: new Thread(() -> f()).start()
来源：http://hz.hysaishi.cn/gtukgpfwjv.html

Go:   go f()
来源：http://hz.shzxlz.cn/gtojtqxuod.html

Ruby: Thread.new { f }
来源：http://hz.cqqwz.cn/gtcovrnpzj.html

C#:   Task.Run(() => F());
来源：http://hz.xingfuxueyuan.xyz/gtvliofsbp.html

[O02] 使用线程池
来源：http://hz.havefunace.top/gtberilklh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jinghuilouyu.cn/gtmjzsrqzr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.nwbrower.top/gtwxitidax.html

JS:   // worker_threads 线程池
来源：http://hz.aibaodan.cn/gtbtpqhjpu.html


<!-- 参考信息 -->