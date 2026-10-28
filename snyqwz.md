代发 wailian999

[K06] 解析 URL 查询串
来源：http://hz.hnqzz.top/gtiqlhtviq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinqigufen.top/gtdfnrgvyg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.quarkkingdee.top/gtpyvmnznr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.daxiang520.top/gttueuuavt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.vqdsnc.cn/gtexjvkpgo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ivvv.top/gtguafipwx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.wangshuangyany.cn/gtwteidsnc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shanyushiyangkeji.top/gtlnyqfued.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xuetiantiany.cn/gtvirtkqzx.html

[K07] 进制转换
来源：http://hz.gotoacloud.top/gtghtvdeuu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yuanzhike.top/gtjvnbbtfb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cashguo.top/gtxzwiaeht.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yvedp.cn/gtimbfeiqr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.chenzaomai.com/gtlkzxzczd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ybcxt.top/gtnwrtarex.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.aibaodan.cn/gtljuldpbc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yj202588.top/gtxvwzlhzg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.316326.xyz/gthnnusjfm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jinyuanbaomall.cn/gtkzaimwcp.html

Py:   pickle.dumps(obj)
来源：http://hz.cashguo.top/gtfvdghfsl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.pycfn.com/gtvhatauvj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ydzc1.top/gtivyhgzvo.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.sxryk.cn/gtveicvdnl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yj202588.top/gtgqfjuufq.html

Go:   encoding/gob
来源：http://hz.fzhhl.top/gtyhjyinct.html

Ruby: Marshal.dump(obj)
来源：http://hz.hysaishi.cn/gtktpjpnez.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinyuanbaomall.cn/gthjnsjxzo.html

================================================================================
来源：http://hz.haohaochexian.top/gtuppxpgfc.html

L. 网络请求
来源：http://hz.xingfuxueyuan.xyz/gtawguxmkj.html

================================================================================
来源：http://hz.andypj.xyz/gtpyagvcnu.html

[L01] 发送 GET 请求
来源：http://hz.cheryme.top/gtokqyzuow.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.dianchejie.cn/gticsovuij.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jinqigfzy.top/gtaveksegj.html

JS:   await fetch(url)
来源：http://hz.sweek.top/gtxurijctd.html

TS:   await fetch(url)
来源：http://hz.feifeiyinyue.top/gtpighedkw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gotoacloud.top/gtfepgvczy.html

Go:   resp, err := http.Get(url)
来源：http://hz.aibaodan.cn/gtxkpvlzsl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yueranfly.top/gteoewavkt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.dianchejie.cn/gtqxghogxu.html

[L02] 发送 POST JSON
来源：http://hz.aibaodan.cn/gttyrmwelx.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.guowangkeji.top/gthyqbmtpr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.52xcode.cn/gtkqlhexgg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yonumen.top/gtxvvzlmpl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.andypj.xyz/gtlynzgmre.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.52xcode.cn/gtqwtlsvue.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shanyushiyangtech.top/gtyggvhnxv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ehwqpu.com/gtjgjtwesf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.tian-w.cn/gtzbuojseb.html

[L03] 设置自定义请求头
来源：http://hz.birdmap.top/gtdvwdjghn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.gogol.net.cn/gtnyrxanhm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jinyuanbaomall.cn/gtvcgrtpaa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hongshengwenyu.top/gtcedtevif.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sufxvd.cn/gtyshfoocp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.fzhhl.top/gtvlztbnlv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.andypj.xyz/gtxnpmezvi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinyuanbaomall.cn/gtgdojfouu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.aizwys.cn/gtyvycaxpe.html

[L04] 设置超时
来源：http://hz.meibo888.top/gthrcwbjsk.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jinqigfzy.top/gtodjnoorr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.havefunace.top/gtymsevqpe.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.9152youxi.cn/gthwdedpsx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yuxming.cn/gtjpoqbmym.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jinyuanbaomall.cn/gtfgwublak.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ppjwa.cn/gtelnbhmqi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.nanxuanxn.top/gtvgwsyyre.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.mhx1999.top/gtjsfutjzw.html

[L05] 上传文件（multipart）
来源：http://hz.tianlin.xyz/gtnrgdthlf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cucudq.cn/gtfrhcdztu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zycfv.cn/gtoulyplcr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.vqdsnc.cn/gtehvtrbcl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zdqjudy.top/gtndngmkst.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xziqi.cn/gtzhtfqqnc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yueranfly.top/gtvzenjbfr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.quarkkingdee.top/gttsekeonr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hnxiangtu.top/gtlfcddnsg.html

[L06] 解析响应为 JSON
来源：http://hz.snrcjt.cn/gtyrjfirzh.html

Py:   resp.json()
来源：http://hz.sweek.top/gttkclfdzd.html

PHP:  json_decode($body, true);
来源：http://hz.zhengqikj.top/gtygtdzsci.html

JS:   await resp.json()
来源：http://hz.iojbl.cn/gtaesztodm.html

TS:   await resp.json()
来源：http://hz.wangdashe.top/gtcffntksj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yangfankeji.com/gtpdgfctra.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.dashuyun.cn/gtnrsiydhp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zycfv.cn/gtgzadmkvf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.meibo888.top/gtfychemtj.html

[L07] 处理 HTTP 状态码
来源：http://hz.yonumen.top/gtvspdqyvw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.iojbl.cn/gtwcxzpqnm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yj20258888.top/gtrpbjrlsx.html

JS:   resp.ok;  resp.status
来源：http://hz.daria6918.cn/gtjofmhbly.html

TS:   resp.ok;  resp.status
来源：http://hz.nwbrower.top/gtmiafbjre.html

Java: resp.statusCode()
来源：http://hz.jlsjyb.cn/gtvnkrjuxl.html

Go:   resp.StatusCode
来源：http://hz.yanxiufei.cn/gtkqbtafng.html

Ruby: resp.code.to_i
来源：http://hz.zhongyouzk.top/gtfmhaehby.html

C#:   (int)resp.StatusCode
来源：http://hz.guowangkeji.top/gtamcfhtmv.html

[L08] 并发请求多个地址
来源：http://hz.mhx1999.top/gtqbypdkwn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cheryme.top/gtxozwbhjg.html

PHP:  curl_multi_init() 系列
来源：http://hz.haohaochexian.top/gtmxttnszj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dashuyun.cn/gtyewegspt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hfpthk.cn/gtypsbpbgw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shzxlz.cn/gtbvggaaxp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xuanzx.com/gtjwagyoll.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.chenjidiqi.icu/gtsncnnplv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yuanzhike.top/gtpgfnxmbb.html

================================================================================
来源：http://hz.guowangkeji.top/gtfyiwdojf.html

M. 命令行 / 进程 / 环境
来源：http://hz.kuanghao11.cn/gtufvsztyk.html

================================================================================
来源：http://hz.cashguo.top/gtngkqierv.html

[M01] 读取命令行参数
来源：http://hz.havefunace.top/gtzwiprptk.html

Py:   sys.argv[1:]
来源：http://hz.daxiang520.top/gtcxblzwdj.html

PHP:  $argv;  $argc;
来源：http://hz.yongpay.top/gtyhbcimoa.html

JS:   process.argv.slice(2)
来源：http://hz.cucudq.cn/gtagmgrjye.html

TS:   process.argv.slice(2)
来源：http://hz.meibo888.top/gtbcgqhlig.html

Java: args 数组（main 方法参数）
来源：http://hz.zhixingplan.top/gtupbrtzau.html

Go:   os.Args[1:]
来源：http://hz.pycfn.com/gtbnacqtmy.html

Ruby: ARGV
来源：http://hz.tianlin.xyz/gtwatpdolt.html

C#:   args 数组（Main 方法参数）
来源：http://hz.gzhubu.top/gtfzbhmzbe.html

[M02] 读取环境变量
来源：http://hz.cqqwz.cn/gtcrcucsys.html

Py:   os.environ.get("HOME")
来源：http://hz.tianlin.xyz/gtbdrgtdor.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.pycfn.com/gtpwxknpgr.html

JS:   process.env.HOME
来源：http://hz.yj202588.top/gtswibjhpe.html

TS:   process.env.HOME
来源：http://hz.tanke756.top/gtfvxoeejf.html

Java: System.getenv("HOME")
来源：http://hz.zhoulong.xyz/gtzoxqahjq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sysykeji.top/gtklcxihtj.html

Ruby: ENV["HOME"]
来源：http://hz.ydjk.org.cn/gtzrntciws.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.bjfxy.top/gtgpxvbeer.html

[M03] 执行外部命令
来源：http://hz.chenlongwang.top/gtogfurudl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.aizwys.cn/gtfrcfedtl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hysaishi.cn/gtmvnkdlat.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhengqikj.top/gtvkjziqms.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.iojbl.cn/gtjelnquom.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.havefunace.top/gtsjcycdaa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xylfe.cn/gtzxnhkvpr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hnqzz.top/gtkscdnirn.html

C#:   Process.Start("ls", "-l");
来源：http://hz.haohaochexian.top/gtmccbdmhi.html

[M04] 获取当前工作目录
来源：http://hz.yueranfly.top/gtfrrxihyb.html

Py:   os.getcwd()
来源：http://hz.yj202588.top/gtptvsxfyl.html

PHP:  getcwd();
来源：http://hz.yvedp.cn/gttdjbwgxs.html

JS:   process.cwd()
来源：http://hz.sxryk.cn/gtevcxqtom.html

TS:   process.cwd()
来源：http://hz.andypj.xyz/gtxdomhqsd.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.dianchejie.cn/gtzqxskcqr.html

Go:   os.Getwd()
来源：http://hz.aizwys.cn/gtcklqwtrc.html

Ruby: Dir.pwd
来源：http://hz.tian-w.cn/gtxglwfmjb.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ydzc1.top/gtpbcyxxto.html

[M05] 设置退出码
来源：http://hz.yanxiufei.cn/gtbmoenwob.html

Py:   sys.exit(1)
来源：http://hz.cqqwz.cn/gtguiikycg.html

PHP:  exit(1);
来源：http://hz.hfpthk.cn/gtceesetrc.html

JS:   process.exit(1)
来源：http://hz.nwbrower.top/gtdljstpjy.html

TS:   process.exit(1)
来源：http://hz.sxryk.cn/gtxmelceil.html

Java: System.exit(1)
来源：http://hz.yj20258888.top/gtfaqxfvqz.html

Go:   os.Exit(1)
来源：http://hz.sxryk.cn/gtropbunxi.html

Ruby: exit 1
来源：http://hz.sweek.top/gtfiabgtfj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hammf.cn/gtnraqjftq.html

[M06] 向标准错误输出
来源：http://hz.yangfankeji.com/gtuexluecn.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xingfuxueyuan.xyz/gtinvjnanm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hywenlv.cn/gtyxammyrq.html

JS:   console.error("err")
来源：http://hz.hongshengwenyu.top/gtgdeavwww.html

TS:   console.error("err")
来源：http://hz.wangshuangyany.cn/gtcsgvqavb.html

Java: System.err.println("err")
来源：http://hz.gotoacloud.top/gtsyoitxbe.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xziqi.cn/gtqbdzsnge.html

Ruby: warn "err"
来源：http://hz.hysaishi.cn/gtiktrrios.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jqgufenzy.top/gtfspszrdj.html

[M07] 判断是否为主入口
来源：http://hz.xuanzx.com/gtxshymjqm.html

Py:   if __name__ == "__main__":
来源：http://hz.shuidangran.top/gthvbpxkuo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.svipenyu.cn/gtxgnqcrun.html

JS:   require.main === module
来源：http://hz.ywan-chungtsiang.top/gtmhcxmffn.html

TS:   require.main === module
来源：http://hz.0kj1m.cn/gtszbtaqqg.html

Java: public static void main(String[] args)
来源：http://hz.yj202588.top/gtnozkvwwa.html

Go:   func main()
来源：http://hz.tian-w.cn/gtonsjvhtf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ydjk.org.cn/gtzcunqwgl.html

C#:   static void Main(string[] args)
来源：http://hz.dashuyun.cn/gtrmriqtbb.html

[M08] 获取系统与运行时信息
来源：http://hz.jianghu66.top/gtufzbvlyi.html

Py:   platform.system();  platform.python_version()
来源：http://hz.tian-w.cn/gtcgveonbe.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shanyushiyangtech.top/gtayspebly.html

JS:   process.platform;  process.version
来源：http://hz.feifeiyinyue.top/gtncxrkubp.html

TS:   process.platform;  process.version
来源：http://hz.zhengqikj.top/gtuylzizve.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.dashuyun.cn/gtvpybatxq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xingfuxueyuan.xyz/gtvgnpakzp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhijiandao.cn/gtkrrhawsh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ydjk.org.cn/gtvgsybrmp.html

================================================================================
来源：http://hz.cucudq.cn/gtffmalogr.html

N. 数据结构与算法
来源：http://hz.fengsongda.top/gtjfjbydgd.html

================================================================================
来源：http://hz.ydjk.org.cn/gtkukugxfg.html

[N01] 二分查找（有序数组）
来源：http://hz.hysaishi.cn/gthxcnkapl.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.guowangkeji.top/gtxsfixvla.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xuanzx.com/gtmszngkbm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinyuanbaomall.cn/gtuaiehzzn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zdqjudy.top/gtufvlyieu.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ydzc1.top/gtyhonojyw.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cucudq.cn/gtfztrbljg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.daxiang520.top/gtnpzczvpv.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.aizwys.cn/gtarctewuf.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.daria6918.cn/gtfreuhayh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jiagoushi.top/gtjfjfkkpu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cheryme.top/gtngpkturu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuetiantiany.cn/gtxouotkic.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhongyouzk.top/gttmfrlkmq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zdqjudy.top/gtfaizmlmd.html

Go:   slices.Sort(arr)
来源：http://hz.ehwqpu.com/gtnsmvbsvg.html

Ruby: arr.sort
来源：http://hz.iojbl.cn/gtgkqyyyyt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.chenlongwang.top/gtksmkewsw.html

[N03] 快速排序（分治示例）
来源：http://hz.dianchejie.cn/gtseksuetu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.sweek.top/gtcgnpyziw.html

PHP:  // 递归实现，或用 usort
来源：http://hz.haohaochexian.top/gtdppcxwdb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yongpay.top/gtqnvkcufn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydjk.org.cn/gtyjqnbcwu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ywan-chungtsiang.top/gttvxdkfrz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.iojbl.cn/gttmbfnttw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.svipenyu.cn/gtruaozcwm.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.feifeiyinyue.top/gtayciiuck.html

[N04] 斐波那契数列
来源：http://hz.yuanzhike.top/gtocptjdme.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hongshengwenyu.top/gtjzuhkspg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jqgfzy.top/gthiqmfqoj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tanke756.top/gtonlceopy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhiwuduotai.top/gtoovvgkbk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yj20258888.top/gtegphlcyy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.gaohongyu789.top/gtfeazdwmz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.birdmap.top/gtkeyznmvy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hnqzz.top/gtpfirbucc.html

[N05] 最大公约数
来源：http://hz.fengsongda.top/gtxbwanalx.html

Py:   math.gcd(a, b)
来源：http://hz.xziqi.cn/gthwuoaapu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sxryk.cn/gtbcooidvz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shuidangran.top/gtjkwilcez.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yuanzhike.top/gtncfkqadq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xylfe.cn/gtnddvojei.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hysaishi.cn/gtcgipuhge.html

Ruby: a.gcd(b)
来源：http://hz.hnqzz.top/gtjztnudap.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.guowangkeji.top/gtakqkplpo.html

[N06] 判断回文字符串
来源：http://hz.zhijiandao.cn/gtdytepndf.html

Py:   s == s[::-1]
来源：http://hz.iojbl.cn/gtlydohelh.html

PHP:  $s === strrev($s);
来源：http://hz.redwolf501.top/gtwwghlabd.html

JS:   s === [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtfnzrsgpz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yongpay.top/gtivdsnhuv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yj202588.top/gtfrpmibev.html

Go:   // 双指针从两端比较
来源：http://hz.jinyuanbaomall.cn/gtbgpxgcrb.html

Ruby: s == s.reverse
来源：http://hz.zhaomingkeji.xyz/gtllzzqjay.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinqigufen.top/gtkpsttwrs.html

[N07] 两数之和（返回下标）
来源：http://hz.yj20258.top/gtccxmazau.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jlsjyb.cn/gtuudtppdp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.svipenyu.cn/gtklxecqcj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ydzc1.top/gtbouqnulw.html

TS:   // 手写 Map<string, number>
来源：http://hz.wangdashe.top/gtdxkcmzwe.html

Java: // 手写 HashMap
来源：http://hz.xziqi.cn/gtoktpmkop.html

Go:   // 手写 map[int]int
来源：http://hz.nanxinkj.top/gtotwddpig.html

Ruby: // 手写 Hash
来源：http://hz.quarkkingdee.top/gtddwkivwj.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.feifeiyinyue.top/gtpklpztfs.html

[N08] 生成全排列
来源：http://hz.nanxuanxn.top/gtobryokwy.html

Py:   itertools.permutations(arr)
来源：http://hz.vqdsnc.cn/gtpuuguipf.html

PHP:  // 手写递归交换
来源：http://hz.zhongyouzk.top/gtzpwtyctd.html

JS:   // 手写回溯递归
来源：http://hz.guowangkeji.top/gtsmbfdicj.html

TS:   // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtzduhfinm.html

Java: // 手写回溯递归
来源：http://hz.shzxlz.cn/gtcrujkfju.html

Go:   // 手写回溯递归
来源：http://hz.feifeiyinyue.top/gtsedglvim.html

Ruby: arr.permutation.to_a
来源：http://hz.xylfe.cn/gtyoelmhud.html

C#:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtdrizcpzy.html

[N09] 栈与队列
来源：http://hz.pycfn.com/gtglekkqtj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shanyushiyangtech.top/gtglicofyf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.dashuyun.cn/gtcebgvmad.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.fengsongda.top/gtxqxrzmrt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shanyushiyangtech.top/gtoswsptzk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.0kj1m.cn/gtkyrwqzxa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gzhubu.top/gtosdwmicg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ppjwa.cn/gtntlpbgjy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shzxlz.cn/gtzdrksvqa.html

[N10] 链表节点定义
来源：http://hz.snrcjt.cn/gtptmjwiik.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.wangshuangyany.cn/gtrzmmllnz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ywan-chungtsiang.top/gtpfbjgkfg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhiwuduotai.top/gtbzwaixck.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.tanke756.top/gtwbgtumlq.html

Java: class Node { int v; Node next; }
来源：http://hz.zhongyouzk.top/gtproovakt.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.svipenyu.cn/gtmzkbbmsz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hywenlv.cn/gttmwgtodu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.havefunace.top/gtperudkwy.html

[N11] 二叉树中序遍历
来源：http://hz.zycfv.cn/gtdgkfqlse.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.0kj1m.cn/gtybqxhsqz.html

PHP:  // 手写递归函数
来源：http://hz.jqgfzy.top/gtjjazarid.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hammf.cn/gtfilkzzzo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.redwolf501.top/gtgljbebpd.html

Java: // 手写递归
来源：http://hz.nanxuanxn.top/gtoqmjuvje.html

Go:   // 手写递归
来源：http://hz.shzxlz.cn/gtzvusrqgk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.nanxuanxn.top/gtrbvxksjh.html

C#:   // 手写递归
来源：http://hz.hywenlv.cn/gtqkibodfm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zdqjudy.top/gtglqvkofo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hnxiangtu.top/gtdyazipiq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cashguo.top/gtpnmkxqxp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hysaishi.cn/gtxbztfhmb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.iojbl.cn/gtidltpupc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fengsongda.top/gtpmjuwctz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenzaomai.com/gtrjojpius.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zycfv.cn/gtbykxxfdi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.svipenyu.cn/gtfayyunsb.html

================================================================================
来源：http://hz.sxryk.cn/gtrtcfmryt.html

O. 并发与异步
来源：http://hz.shangyingyoupin.top/gtdhdpkjkr.html

================================================================================
来源：http://hz.kuanghao11.cn/gtmavffvol.html

[O01] 启动一个线程
来源：http://hz.vqdsnc.cn/gtbjgggazc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.vqdsnc.cn/gtyaigexps.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shangyingyoupin.top/gtargcgotj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.sufxvd.cn/gtbawntgmq.html

TS:   // 同 JS
来源：http://hz.yangfankeji.com/gtnxkasnxy.html

Java: new Thread(() -> f()).start()
来源：http://hz.vqdsnc.cn/gtwdxtdpng.html

Go:   go f()
来源：http://hz.gaohongyu789.top/gtrmwrmoxu.html

Ruby: Thread.new { f }
来源：http://hz.ydzc1.top/gtlxxbqmzt.html

C#:   Task.Run(() => F());
来源：http://hz.jinghuilouyu.cn/gtjxkfifeo.html


<!-- 参考信息 -->