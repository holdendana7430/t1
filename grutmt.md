代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.fengsongda.top/gtoztgaybz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhaomingkeji.xyz/gtjxguqejb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jyoumei.cn/gtlcwgluml.html

[K05] 深拷贝对象
来源：http://hz.ydzc1.top/gtguuglesk.html

Py:   copy.deepcopy(obj)
来源：http://hz.pengpengdd.cyou/gtklzsyjmu.html

PHP:  unserialize(serialize($obj));
来源：http://hz.snrcjt.cn/gtasldpstw.html

JS:   structuredClone(obj)
来源：http://hz.zhiwuduotai.top/gtmmpnluhz.html

TS:   structuredClone(obj)
来源：http://hz.bjfxy.top/gtpwvlwbvn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.chenjidiqi.icu/gtvjrfwrbl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yanxiufei.cn/gtuxjarksf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jiagoushi.top/gtenyvtinq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cucudq.cn/gtrqobnaki.html

[K06] 解析 URL 查询串
来源：http://hz.hysaishi.cn/gttjcetnqv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ivvv.top/gtjggifklz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xuetiantiany.cn/gtdchopkmb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.birdmap.top/gtjppffdtc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhoulong.xyz/gtsxzghcfw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.chenjidiqi.icu/gtcttzvoem.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sweek.top/gtgwpqfdgx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ybcxt.top/gtbzhbrdxq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhengqikj.top/gtgeozslqh.html

[K07] 进制转换
来源：http://hz.52xcode.cn/gtmijxwxra.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.aibaodan.cn/gtesiyendf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.gotoacloud.top/gtdpxhgcom.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhiwuduotai.top/gtiqdkxndn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.mhx1999.top/gtpwglahgx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.dianchejie.cn/gtbdetcmqw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yongpay.top/gtsqkylroq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.daxiang520.top/gthtynbiap.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zdqjudy.top/gtkrpuejgm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jinqigfzy.top/gtcicddfeh.html

Py:   pickle.dumps(obj)
来源：http://hz.xingfuxueyuan.xyz/gtvbqkcoec.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.0kj1m.cn/gthaswgqaz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gotoacloud.top/gtirjxelli.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhiwuduotai.top/gttcwxvhqx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenjidiqi.icu/gtrlbvtoyb.html

Go:   encoding/gob
来源：http://hz.sweek.top/gtrpuzwxuk.html

Ruby: Marshal.dump(obj)
来源：http://hz.snrcjt.cn/gtbmsnbpha.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.daxiang520.top/gtueqibdfc.html

================================================================================
来源：http://hz.birdmap.top/gtzwiawzjd.html

L. 网络请求
来源：http://hz.ydjk.org.cn/gtkgdjegka.html

================================================================================
来源：http://hz.jianghu66.top/gtnxflzglz.html

[L01] 发送 GET 请求
来源：http://hz.zdqjudy.top/gtjudcucpy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.svipenyu.cn/gtzxxsgdih.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yangfankeji.com/gtdfjnsuae.html

JS:   await fetch(url)
来源：http://hz.chenlongwang.top/gtynojgaab.html

TS:   await fetch(url)
来源：http://hz.pycfn.com/gtzlwhacos.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yueranfly.top/gtbdfcoaoa.html

Go:   resp, err := http.Get(url)
来源：http://hz.birdmap.top/gtcqvzntbk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.wangshuangyany.cn/gtagrhzmqe.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.meibo888.top/gtwhlktisp.html

[L02] 发送 POST JSON
来源：http://hz.jqgfzy.top/gtqsyfcndm.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jinqigfzy.top/gtyosvystk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.chenjidiqi.icu/gtjkxcnbtl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.daxiang520.top/gtpumumtjy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yangfankeji.com/gtpjlyftgd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shanyushiyangkeji.top/gtcdkhdhif.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.tianlin.xyz/gtgtudawcv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.svipenyu.cn/gtassgoued.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.snrcjt.cn/gtqlzsmjms.html

[L03] 设置自定义请求头
来源：http://hz.dianchejie.cn/gtnocuwryh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cdnleiting.top/gtmdcirnfi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gogol.net.cn/gticuoyrhc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ivvv.top/gtochzuoft.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hammf.cn/gtjbqslpxx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.gogol.net.cn/gtjkgrxrcb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.daxiang520.top/gtkdxupgid.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cashguo.top/gtgmxyumqh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xinyue.icu/gtdcvieabm.html

[L04] 设置超时
来源：http://hz.9152youxi.cn/gtiaeqnynh.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hfpthk.cn/gtoaoazqgb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhiwuduotai.top/gtrebpkzoi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuetiantiany.cn/gtrchjkrjf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tian-w.cn/gtwnkkbbld.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yj20258888.top/gtwgwycofb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yongpay.top/gtorsjnflr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hammf.cn/gtokbqhcyp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jqgufenzy.top/gtpvexccda.html

[L05] 上传文件（multipart）
来源：http://hz.gogol.net.cn/gtdavekxjq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hywenlv.cn/gthvqjelvx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.gotoacloud.top/gtaoewcjsj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.sxryk.cn/gtazfqgqeq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.316326.xyz/gtwtrwrdjm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhaomingkeji.xyz/gtanlrofkw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhongyouzk.top/gtngximeer.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yonumen.top/gtpheyitpe.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.sweek.top/gtwuyncdzu.html

[L06] 解析响应为 JSON
来源：http://hz.yuanzhike.top/gtrpwchahx.html

Py:   resp.json()
来源：http://hz.tian-w.cn/gthcqyopsf.html

PHP:  json_decode($body, true);
来源：http://hz.sufxvd.cn/gtviwkoggr.html

JS:   await resp.json()
来源：http://hz.xuetiantiany.cn/gtjodbkhle.html

TS:   await resp.json()
来源：http://hz.jqgufenzy.top/gtxvbezonj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hfpthk.cn/gtqkfyksrx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.havefunace.top/gtbhhafnuj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.gogol.net.cn/gtumtwdtxb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jiagoushi.top/gtovmzoksm.html

[L07] 处理 HTTP 状态码
来源：http://hz.pengpengdd.cyou/gtypkfiknd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.daxiang520.top/gtikvdpbix.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ybcxt.top/gtuvigdfjx.html

JS:   resp.ok;  resp.status
来源：http://hz.sweek.top/gtdknahaol.html

TS:   resp.ok;  resp.status
来源：http://hz.xingfuxueyuan.xyz/gtkzeqwpdq.html

Java: resp.statusCode()
来源：http://hz.zhaomingkeji.xyz/gtbgmjwdat.html

Go:   resp.StatusCode
来源：http://hz.hnqzz.top/gtqyzrwnhs.html

Ruby: resp.code.to_i
来源：http://hz.birdmap.top/gtivbyvsrh.html

C#:   (int)resp.StatusCode
来源：http://hz.chenzaomai.com/gtoqehksal.html

[L08] 并发请求多个地址
来源：http://hz.jlsjyb.cn/gtezmlopbq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.52xcode.cn/gtqgyvaqcv.html

PHP:  curl_multi_init() 系列
来源：http://hz.hammf.cn/gtwuqyiklo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxinkj.top/gtftcdocnr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xylfe.cn/gtryaoznxa.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yj20258888.top/gtupskrojk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.chenjidiqi.icu/gtviaokxzg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinqigufen.top/gtopbitvso.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhongyouzk.top/gtrbzjnmvf.html

================================================================================
来源：http://hz.zhengqikj.top/gtyqanlfer.html

M. 命令行 / 进程 / 环境
来源：http://hz.yueranfly.top/gtczgngkwq.html

================================================================================
来源：http://hz.wangdashe.top/gtcxomtpeq.html

[M01] 读取命令行参数
来源：http://hz.haohaochexian.top/gtzjndqghl.html

Py:   sys.argv[1:]
来源：http://hz.gogol.net.cn/gtpqwwqmli.html

PHP:  $argv;  $argc;
来源：http://hz.zhongyouzk.top/gtiswdzqyk.html

JS:   process.argv.slice(2)
来源：http://hz.sysykeji.top/gtpkzurohr.html

TS:   process.argv.slice(2)
来源：http://hz.jiagoushi.top/gtjjdyctbv.html

Java: args 数组（main 方法参数）
来源：http://hz.xingfuxueyuan.xyz/gteaurtast.html

Go:   os.Args[1:]
来源：http://hz.dianchejie.cn/gtgzpsfirl.html

Ruby: ARGV
来源：http://hz.zdqjudy.top/gthfsmtcur.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hnxiangtu.top/gteyttqvft.html

[M02] 读取环境变量
来源：http://hz.ivvv.top/gtkbstehut.html

Py:   os.environ.get("HOME")
来源：http://hz.yonumen.top/gtqeysplqj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zdqjudy.top/gtuepvkltx.html

JS:   process.env.HOME
来源：http://hz.aizwys.cn/gtkgzpvrjk.html

TS:   process.env.HOME
来源：http://hz.pycfn.com/gtfbqwdcbo.html

Java: System.getenv("HOME")
来源：http://hz.quarkkingdee.top/gtmhfuwxbw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.shanyushiyangkeji.top/gtkxrqxcxn.html

Ruby: ENV["HOME"]
来源：http://hz.aibaodan.cn/gtzvrffkmf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhongyouzk.top/gtgrevcekd.html

[M03] 执行外部命令
来源：http://hz.kuanghao11.cn/gtfggxxmzs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.nanxuanxn.top/gthpwyxnjj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.guannengcc.top/gtmvwxzcpw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.svipenyu.cn/gtyqaticuo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhaomingkeji.xyz/gteywvqonf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.daxiang520.top/gtukrfwkqi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.iojbl.cn/gtkmoxrihh.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hnqzz.top/gtoygcndhh.html

C#:   Process.Start("ls", "-l");
来源：http://hz.316326.xyz/gtxybdjeia.html

[M04] 获取当前工作目录
来源：http://hz.hnqzz.top/gtqonokzlm.html

Py:   os.getcwd()
来源：http://hz.ppjwa.cn/gtmfaznkuv.html

PHP:  getcwd();
来源：http://hz.wangshuangyany.cn/gtnkeolsfc.html

JS:   process.cwd()
来源：http://hz.ydzc1.top/gtfmectgrm.html

TS:   process.cwd()
来源：http://hz.jinghuilouyu.cn/gtabkmsuzs.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.haohaochexian.top/gttdmitssk.html

Go:   os.Getwd()
来源：http://hz.jinqigufen.top/gtktbawxuc.html

Ruby: Dir.pwd
来源：http://hz.hongshengwenyu.top/gthlubpbbu.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.tianlin.xyz/gtveecywhy.html

[M05] 设置退出码
来源：http://hz.shanyushiyangtech.top/gtmzggouon.html

Py:   sys.exit(1)
来源：http://hz.cashguo.top/gtkfmbwkam.html

PHP:  exit(1);
来源：http://hz.xuanzx.com/gtmyahdxbr.html

JS:   process.exit(1)
来源：http://hz.ybcxt.top/gtkaddhato.html

TS:   process.exit(1)
来源：http://hz.xuetiantiany.cn/gtpyvefyqa.html

Java: System.exit(1)
来源：http://hz.dianchejie.cn/gtqzagsqsj.html

Go:   os.Exit(1)
来源：http://hz.sweek.top/gtjsagnmbk.html

Ruby: exit 1
来源：http://hz.sufxvd.cn/gtbnruqmyt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zdqjudy.top/gtmzmialfu.html

[M06] 向标准错误输出
来源：http://hz.hammf.cn/gtbyzrvwrv.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hfpthk.cn/gtwkxcnjco.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ppjwa.cn/gtgjpckbst.html

JS:   console.error("err")
来源：http://hz.ehwqpu.com/gtcsmoyfac.html

TS:   console.error("err")
来源：http://hz.yongpay.top/gtvsjcyojl.html

Java: System.err.println("err")
来源：http://hz.yanxiufei.cn/gtrukeytuy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.svipenyu.cn/gtnhjbttpi.html

Ruby: warn "err"
来源：http://hz.zhoulong.xyz/gthekempzl.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jianghu66.top/gtvoafscdy.html

[M07] 判断是否为主入口
来源：http://hz.yonumen.top/gtyjcnxokz.html

Py:   if __name__ == "__main__":
来源：http://hz.chenlongwang.top/gtsqcnvsod.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.dashuyun.cn/gtaviwwjqg.html

JS:   require.main === module
来源：http://hz.cucudq.cn/gtbhnktjfp.html

TS:   require.main === module
来源：http://hz.nanxinkj.top/gtowqbvhuo.html

Java: public static void main(String[] args)
来源：http://hz.zhixingplan.top/gtszkqvuwg.html

Go:   func main()
来源：http://hz.gotoacloud.top/gtdrplfjub.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhoulong.xyz/gtjxcqmbxo.html

C#:   static void Main(string[] args)
来源：http://hz.zhijiandao.cn/gtfvkahwwg.html

[M08] 获取系统与运行时信息
来源：http://hz.dianchejie.cn/gtzrsedtnr.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hammf.cn/gtmwecxpdn.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.c1oappe.top/gtpvwsampx.html

JS:   process.platform;  process.version
来源：http://hz.zhoulong.xyz/gtdvdmdjyz.html

TS:   process.platform;  process.version
来源：http://hz.shuidangran.top/gtrfivljeu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ydjk.org.cn/gtllsqwiws.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.guowangkeji.top/gtvvuooggl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.birdmap.top/gtppxhximn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hnxiangtu.top/gtznpbdhlv.html

================================================================================
来源：http://hz.kuanghao11.cn/gtwsebiumj.html

N. 数据结构与算法
来源：http://hz.tianlin.xyz/gtmbllkmyn.html

================================================================================
来源：http://hz.cdnleiting.top/gtdymiqnvy.html

[N01] 二分查找（有序数组）
来源：http://hz.zhixingplan.top/gtmbovrfhb.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinqigufen.top/gtpcbuaure.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hfpthk.cn/gtwholxnfr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xylfe.cn/gtntwrelvg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.guannengcc.top/gtkbyytdsk.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.vqdsnc.cn/gtbbpclxfu.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.nwbrower.top/gtxpdctuyq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinqigfzy.top/gtnutbetot.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cdnleiting.top/gtrdzktbpz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yongpay.top/gtfilijeld.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ybcxt.top/gtvpnkoqzm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.gogol.net.cn/gtpzyomadr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hysaishi.cn/gtsbuwbtrw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yueranfly.top/gtqfxnjphb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xziqi.cn/gttnzauzpy.html

Go:   slices.Sort(arr)
来源：http://hz.feifeiyinyue.top/gtznqpysea.html

Ruby: arr.sort
来源：http://hz.chenjidiqi.icu/gtoozknviy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.quarkkingdee.top/gtejewpyxp.html

[N03] 快速排序（分治示例）
来源：http://hz.jinqigfzy.top/gtfjlullug.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.52xcode.cn/gtpjfcdexm.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xuetiantiany.cn/gthzhonkwx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hysaishi.cn/gtuajzwgev.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.0kj1m.cn/gtoswvwbry.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xylfe.cn/gtiypwizmn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.pycfn.com/gtyrekvcix.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ydjk.org.cn/gtxguazdqo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yj202588.top/gtabpyhsag.html

[N04] 斐波那契数列
来源：http://hz.smart0.xyz/gtgddpxjfq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jinghuilouyu.cn/gtajdgimnn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jianghu66.top/gtvpaerxas.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.feifeiyinyue.top/gtwilahbpc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cdnleiting.top/gtdpmxchla.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.nwbrower.top/gtgvwbozxd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.guannengcc.top/gtaspvktcv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yonumen.top/gtyiclopsn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.wangdashe.top/gtvgzahpon.html

[N05] 最大公约数
来源：http://hz.wangdashe.top/gthlqrktjf.html

Py:   math.gcd(a, b)
来源：http://hz.cheryme.top/gtxhceogpg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yuxming.cn/gtmwmwlyei.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hfpthk.cn/gtxejrynlo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tian-w.cn/gtxnygmeoj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hongshengwenyu.top/gtjycbyulw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.tanke756.top/gtelfwsznp.html

Ruby: a.gcd(b)
来源：http://hz.wangshuangyany.cn/gtnalebuzb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.birdmap.top/gtvyrnjeua.html

[N06] 判断回文字符串
来源：http://hz.xuetiantiany.cn/gtltbwknpi.html

Py:   s == s[::-1]
来源：http://hz.xziqi.cn/gtjwjwmaca.html

PHP:  $s === strrev($s);
来源：http://hz.cdnleiting.top/gtlvgqcoan.html

JS:   s === [...s].reverse().join("")
来源：http://hz.snrcjt.cn/gtypyamocc.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gtugnytcue.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xuetiantiany.cn/gtazbrdzau.html

Go:   // 双指针从两端比较
来源：http://hz.yj20258888.top/gtqglzdpwf.html

Ruby: s == s.reverse
来源：http://hz.c1oappe.top/gtowfsebfy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shzxlz.cn/gtzchynvtm.html

[N07] 两数之和（返回下标）
来源：http://hz.wangdashe.top/gtldcajrnt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.daxiang520.top/gtiymflykp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.daxiang520.top/gtxvitvwxf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yueranfly.top/gtlpkjbazx.html

TS:   // 手写 Map<string, number>
来源：http://hz.yvedp.cn/gtasbptjry.html

Java: // 手写 HashMap
来源：http://hz.xylfe.cn/gtoiroekxo.html

Go:   // 手写 map[int]int
来源：http://hz.sxryk.cn/gtwgcwbpyy.html

Ruby: // 手写 Hash
来源：http://hz.zhixingplan.top/gthvxmuflj.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.kuanghao11.cn/gtbajftpdb.html

[N08] 生成全排列
来源：http://hz.gogol.net.cn/gtgulrreba.html

Py:   itertools.permutations(arr)
来源：http://hz.quarkkingdee.top/gtfdgmiqws.html

PHP:  // 手写递归交换
来源：http://hz.wangdashe.top/gtentgqorw.html

JS:   // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtutkzuvmk.html

TS:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtweunagas.html

Java: // 手写回溯递归
来源：http://hz.dashuyun.cn/gtakwxppcz.html

Go:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gthjvxapap.html

Ruby: arr.permutation.to_a
来源：http://hz.shanyushiyangtech.top/gtvrsmkulj.html

C#:   // 手写回溯递归
来源：http://hz.guowangkeji.top/gttichbvhj.html

[N09] 栈与队列
来源：http://hz.chenjidiqi.icu/gtrshmlzar.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hywenlv.cn/gtuisiivdi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ybcxt.top/gtptquajhy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhixingplan.top/gtplivonfm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hnxiangtu.top/gtcehfwokj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.birdmap.top/gtdyidbgpw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.iojbl.cn/gtohzmwuij.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.iojbl.cn/gtykvkqbyx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shanyushiyangkeji.top/gtcqyaeods.html

[N10] 链表节点定义
来源：http://hz.meibo888.top/gtsnkrasnx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shangyingyoupin.top/gtqlnpqxnt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shzxlz.cn/gtqbmhzbdj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cucudq.cn/gtpyooujct.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ivvv.top/gtvbpidgbf.html

Java: class Node { int v; Node next; }
来源：http://hz.ehwqpu.com/gtxtyyjvfy.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.dashuyun.cn/gtjbauwqts.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cucudq.cn/gtymanzykc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yj20258.top/gtdigqqzpe.html

[N11] 二叉树中序遍历
来源：http://hz.shangyingyoupin.top/gtyvuivsip.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jyoumei.cn/gtcwrbubhd.html

PHP:  // 手写递归函数
来源：http://hz.pengpengdd.cyou/gtkfilmeus.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cashguo.top/gtosehetfq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tian-w.cn/gtanzqasal.html

Java: // 手写递归
来源：http://hz.bjfxy.top/gtfmlgldkq.html

Go:   // 手写递归
来源：http://hz.gaohongyu789.top/gtwmszwljk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.daria6918.cn/gtvcaistqr.html

C#:   // 手写递归
来源：http://hz.shuidangran.top/gtovndmzyq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cashguo.top/gtdotsyoga.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.pycfn.com/gthoysqddj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ywan-chungtsiang.top/gtywzgaeur.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yvedp.cn/gtnmshlqov.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.0kj1m.cn/gtvnsqganh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tianlin.xyz/gtetrbuckg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.cucudq.cn/gtscnlpfef.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.sufxvd.cn/gtccnmhuxp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.kuanghao11.cn/gtimrrfszp.html


<!-- 参考信息 -->