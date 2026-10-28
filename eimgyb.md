代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hysaishi.cn/gtkvvmyfpu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.tianlin.xyz/gtalzqauzi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hywenlv.cn/gttbddjazr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.daxiang520.top/gtwxgctuyo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinqigfzy.top/gtcqqhqevj.html

[K07] 进制转换
来源：http://hz.quarkkingdee.top/gtcowhzfvn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhixingplan.top/gtvyuwtyre.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhoulong.xyz/gtgvlfybgo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhoulong.xyz/gtytwhqppw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.52xcode.cn/gtosrzexly.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gtgwyshqfz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hfpthk.cn/gtbpoeninx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hongshengwenyu.top/gtbvhtnkit.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.bjfxy.top/gtbmhgyuut.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xuanzx.com/gttwmhhalj.html

Py:   pickle.dumps(obj)
来源：http://hz.wangshuangyany.cn/gtdjnrrkil.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jianghu66.top/gtolarehfn.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gzhubu.top/gtvewksmvz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ydzc1.top/gtfocrnriu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xziqi.cn/gtzzrwgugr.html

Go:   encoding/gob
来源：http://hz.hysaishi.cn/gtkdekajec.html

Ruby: Marshal.dump(obj)
来源：http://hz.andypj.xyz/gtiwobundw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hywenlv.cn/gtrhprheny.html

================================================================================
来源：http://hz.jlsjyb.cn/gtdwkekijh.html

L. 网络请求
来源：http://hz.vqdsnc.cn/gthzykhnky.html

================================================================================
来源：http://hz.aibaodan.cn/gtbrvzyyod.html

[L01] 发送 GET 请求
来源：http://hz.hywenlv.cn/gttiinfvdw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jqgfzy.top/gtkbgwvvtq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.snrcjt.cn/gtmwukmzow.html

JS:   await fetch(url)
来源：http://hz.zhaomingkeji.xyz/gtvhkrivji.html

TS:   await fetch(url)
来源：http://hz.ybcxt.top/gtixyspdxc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.chenzaomai.com/gtmmpjgosg.html

Go:   resp, err := http.Get(url)
来源：http://hz.birdmap.top/gtjnbgchhc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.gotoacloud.top/gtsjcgywsw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.0kj1m.cn/gtuspnuxzf.html

[L02] 发送 POST JSON
来源：http://hz.tian-w.cn/gtivfvmtfl.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yuanzhike.top/gtxeibjznd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xylfe.cn/gtblufxxlk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fengsongda.top/gtjaidhfid.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.haohaochexian.top/gtviwzctvm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.316326.xyz/gtbqtypjvo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sysykeji.top/gtixjzmhtb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cheryme.top/gteolrkaiu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.316326.xyz/gtcltombcb.html

[L03] 设置自定义请求头
来源：http://hz.ybcxt.top/gtnpqfiitm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.0kj1m.cn/gtdwxjewsy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.smart0.xyz/gtlqxopgwn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cucudq.cn/gtnlnswxaw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenjidiqi.icu/gthvhocxvv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.haohaochexian.top/gtgmpcdxvx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zycfv.cn/gtwvyxtzqx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.haohaochexian.top/gtvwttmuri.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shuidangran.top/gtgqkaeqfl.html

[L04] 设置超时
来源：http://hz.cucudq.cn/gtvxdvbert.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jyoumei.cn/gtuhvgosaz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ehwqpu.com/gtzytaaodt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shuidangran.top/gtbjqdbpyi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.aizwys.cn/gtxsivipxh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cashguo.top/gthgwcecon.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.aibaodan.cn/gtjrqqcpjk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.birdmap.top/gtvbiblvck.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.gaohongyu789.top/gtozolkebp.html

[L05] 上传文件（multipart）
来源：http://hz.yueranfly.top/gtskyfryzu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.wangshuangyany.cn/gtmsdjmspj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.dianchejie.cn/gtjeroxkdw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj20258.top/gttcotwnfs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.tanke756.top/gthlgouhlt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.chenzaomai.com/gtwxbdmibt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jiagoushi.top/gtxthasdha.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xingfuxueyuan.xyz/gtmrbtqemv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.chenjidiqi.icu/gtyecpkanc.html

[L06] 解析响应为 JSON
来源：http://hz.chenzaomai.com/gtvqiayjuy.html

Py:   resp.json()
来源：http://hz.zhijiandao.cn/gtdxmnkwcc.html

PHP:  json_decode($body, true);
来源：http://hz.yanxiufei.cn/gtdwhqhfjc.html

JS:   await resp.json()
来源：http://hz.chenlongwang.top/gtbutbopiz.html

TS:   await resp.json()
来源：http://hz.cdnleiting.top/gtgzmjlgvt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.sweek.top/gtgscoutbh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ybcxt.top/gtfhauqutg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.aizwys.cn/gtqhttktfz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yuanzhike.top/gtasinlhcy.html

[L07] 处理 HTTP 状态码
来源：http://hz.fengsongda.top/gtwapyywnj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hnqzz.top/gtirndgzkn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.gotoacloud.top/gtsihlzjzf.html

JS:   resp.ok;  resp.status
来源：http://hz.haohaochexian.top/gtuegylrse.html

TS:   resp.ok;  resp.status
来源：http://hz.snrcjt.cn/gtbzrjhyto.html

Java: resp.statusCode()
来源：http://hz.cheryme.top/gtrycjaxat.html

Go:   resp.StatusCode
来源：http://hz.jqgfzy.top/gtavcxvfsj.html

Ruby: resp.code.to_i
来源：http://hz.redwolf501.top/gtkvnungtu.html

C#:   (int)resp.StatusCode
来源：http://hz.ivvv.top/gtrdgxgpyj.html

[L08] 并发请求多个地址
来源：http://hz.chenzaomai.com/gtytkivuus.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cheryme.top/gtbqbjnpsc.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhengqikj.top/gtzxqohamh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.0kj1m.cn/gtximbkheu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nwbrower.top/gtnainbdsk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.chenzaomai.com/gtkdiycguq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.mhx1999.top/gtvsrrwmna.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zycfv.cn/gtczdswuxu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hfpthk.cn/gtgzjknqlo.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtkmtubmbw.html

M. 命令行 / 进程 / 环境
来源：http://hz.yangfankeji.com/gtumgqphmt.html

================================================================================
来源：http://hz.dianchejie.cn/gtetgvbquk.html

[M01] 读取命令行参数
来源：http://hz.nwbrower.top/gtxtewgtgp.html

Py:   sys.argv[1:]
来源：http://hz.jqgfzy.top/gtaosrsqpw.html

PHP:  $argv;  $argc;
来源：http://hz.ydzc1.top/gtifcfeoof.html

JS:   process.argv.slice(2)
来源：http://hz.yanxiufei.cn/gtouhtranc.html

TS:   process.argv.slice(2)
来源：http://hz.9152youxi.cn/gtmgaxwtqq.html

Java: args 数组（main 方法参数）
来源：http://hz.xziqi.cn/gttpaspfzi.html

Go:   os.Args[1:]
来源：http://hz.bjfxy.top/gtbzsuklvd.html

Ruby: ARGV
来源：http://hz.yj20258.top/gtlhyujakp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhixingplan.top/gtqvresgbd.html

[M02] 读取环境变量
来源：http://hz.havefunace.top/gtftzuhtbc.html

Py:   os.environ.get("HOME")
来源：http://hz.cashguo.top/gtvbhpkagb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yj202588.top/gtndtdpgvv.html

JS:   process.env.HOME
来源：http://hz.cashguo.top/gtldiyuqgn.html

TS:   process.env.HOME
来源：http://hz.jinyuanbaomall.cn/gtihcgbtmw.html

Java: System.getenv("HOME")
来源：http://hz.sufxvd.cn/gtdndssloo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hywenlv.cn/gtqemhludp.html

Ruby: ENV["HOME"]
来源：http://hz.yuanzhike.top/gthkkifyxe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenzaomai.com/gtwnrhcxas.html

[M03] 执行外部命令
来源：http://hz.feifeiyinyue.top/gteukatmdm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.c1oappe.top/gtxjpoinwa.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shzxlz.cn/gtmnofmbiw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj202588.top/gtagnvbqcx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.0kj1m.cn/gttnuyngeh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hammf.cn/gtocsqtcpa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.mhx1999.top/gtljwzbexa.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shzxlz.cn/gtqzlsqwjt.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xuanzx.com/gtniklrdzp.html

[M04] 获取当前工作目录
来源：http://hz.ybcxt.top/gtzxfmqyws.html

Py:   os.getcwd()
来源：http://hz.yueranfly.top/gtajqcijuz.html

PHP:  getcwd();
来源：http://hz.zhongyouzk.top/gthveielmf.html

JS:   process.cwd()
来源：http://hz.iojbl.cn/gtnfqabxgo.html

TS:   process.cwd()
来源：http://hz.havefunace.top/gtomreyqld.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.guannengcc.top/gtiqyhpgky.html

Go:   os.Getwd()
来源：http://hz.hongshengwenyu.top/gttslqmenx.html

Ruby: Dir.pwd
来源：http://hz.jqgufenzy.top/gtzqwsjdcv.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.0kj1m.cn/gtqaorrgnu.html

[M05] 设置退出码
来源：http://hz.birdmap.top/gtfbtzddca.html

Py:   sys.exit(1)
来源：http://hz.daria6918.cn/gtgdfdauzc.html

PHP:  exit(1);
来源：http://hz.zhijiandao.cn/gtgshmxzle.html

JS:   process.exit(1)
来源：http://hz.havefunace.top/gtfzqaztlc.html

TS:   process.exit(1)
来源：http://hz.yanxiufei.cn/gtatvhrqag.html

Java: System.exit(1)
来源：http://hz.kuanghao11.cn/gtxunkwwxf.html

Go:   os.Exit(1)
来源：http://hz.gotoacloud.top/gtyqklxbdq.html

Ruby: exit 1
来源：http://hz.gotoacloud.top/gtvgexiwpr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jinqigfzy.top/gtssgxkulz.html

[M06] 向标准错误输出
来源：http://hz.svipenyu.cn/gtzpkmcsnh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinyuanbaomall.cn/gtiecnsepx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhiwuduotai.top/gtjonicmco.html

JS:   console.error("err")
来源：http://hz.meibo888.top/gtbwnospai.html

TS:   console.error("err")
来源：http://hz.fzhhl.top/gtxvmddpkl.html

Java: System.err.println("err")
来源：http://hz.zhongyouzk.top/gtimoxeiqp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jyoumei.cn/gtypiasulq.html

Ruby: warn "err"
来源：http://hz.snrcjt.cn/gtenakjpyj.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ybcxt.top/gtacdeutby.html

[M07] 判断是否为主入口
来源：http://hz.havefunace.top/gtdavhdqfs.html

Py:   if __name__ == "__main__":
来源：http://hz.yangfankeji.com/gtujevgttx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gzhubu.top/gtqqpsnzbk.html

JS:   require.main === module
来源：http://hz.ywan-chungtsiang.top/gtsopksqdx.html

TS:   require.main === module
来源：http://hz.cqqwz.cn/gtitxijowm.html

Java: public static void main(String[] args)
来源：http://hz.daxiang520.top/gtdjuoanmn.html

Go:   func main()
来源：http://hz.guannengcc.top/gtahdmbwum.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ydzc1.top/gtmnwjwfgr.html

C#:   static void Main(string[] args)
来源：http://hz.jinqigufen.top/gtenflccpx.html

[M08] 获取系统与运行时信息
来源：http://hz.jlsjyb.cn/gtmieiqsdp.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinqigufen.top/gtkwtxpezv.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yangfankeji.com/gtcwlbjrhw.html

JS:   process.platform;  process.version
来源：http://hz.jlsjyb.cn/gtmgnlxwmp.html

TS:   process.platform;  process.version
来源：http://hz.shanyushiyangtech.top/gtzvvydwkk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shanyushiyangkeji.top/gtrvaxgtiw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ydzc1.top/gtcdzwgjsz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cucudq.cn/gtrlvyjdwb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.aizwys.cn/gtgvkddgbq.html

================================================================================
来源：http://hz.yj202588.top/gtkxgylcox.html

N. 数据结构与算法
来源：http://hz.cqqwz.cn/gtewibvzca.html

================================================================================
来源：http://hz.fengsongda.top/gtztnumdef.html

[N01] 二分查找（有序数组）
来源：http://hz.yuanzhike.top/gtppyqfcli.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hywenlv.cn/gtkrvfhcfx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hywenlv.cn/gtekfnqkyo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jianghu66.top/gtqaminpua.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dianchejie.cn/gtsaflhucd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.wangshuangyany.cn/gtcknkifvh.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ivvv.top/gtbdikhxqz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.aibaodan.cn/gtrwbfsxiv.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.pycfn.com/gtqskhewsp.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.sxryk.cn/gtvulcblkg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sxryk.cn/gtbdpawdzd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shanyushiyangtech.top/gtnypzvgmg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ybcxt.top/gtnkyzdasj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.mhx1999.top/gturhytist.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.316326.xyz/gtaovhtjrj.html

Go:   slices.Sort(arr)
来源：http://hz.xuetiantiany.cn/gtxessvnxk.html

Ruby: arr.sort
来源：http://hz.shanyushiyangtech.top/gtntirqief.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sweek.top/gtgqgkglyx.html

[N03] 快速排序（分治示例）
来源：http://hz.yvedp.cn/gtbftluazz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shuidangran.top/gtvbfdmwmg.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hfpthk.cn/gtnpuzarnz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhijiandao.cn/gtqmdkygcc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pengpengdd.cyou/gtinlkbbvh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.wangshuangyany.cn/gtvxbrfhka.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.nanxuanxn.top/gtftoqbnvx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shuidangran.top/gtfdujgaxc.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yanxiufei.cn/gtufkrwupx.html

[N04] 斐波那契数列
来源：http://hz.jinghuilouyu.cn/gtjpnxsznm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jinyuanbaomall.cn/gtvznogwgq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hnqzz.top/gttxrykwne.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.0kj1m.cn/gtanjrasny.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cucudq.cn/gthbvbdgvl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.quarkkingdee.top/gthzxgajsq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yj20258.top/gtbkvvujra.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinyuanbaomall.cn/gtysxgycxi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yj202588.top/gtjluzfwnp.html

[N05] 最大公约数
来源：http://hz.redwolf501.top/gtkkbqdexv.html

Py:   math.gcd(a, b)
来源：http://hz.fengsongda.top/gtucywksrj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.chenlongwang.top/gtcawxmycx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.feifeiyinyue.top/gtvbvggpjb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jyoumei.cn/gtohwrmdeh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ybcxt.top/gtlcbirzed.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ydzc1.top/gtvtbijyxt.html

Ruby: a.gcd(b)
来源：http://hz.svipenyu.cn/gtogtgflpc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.kuanghao11.cn/gtjwsevrtd.html

[N06] 判断回文字符串
来源：http://hz.yanxiufei.cn/gtrdlkmhba.html

Py:   s == s[::-1]
来源：http://hz.tian-w.cn/gtmnhgmtvr.html

PHP:  $s === strrev($s);
来源：http://hz.zhoulong.xyz/gtehwnqcol.html

JS:   s === [...s].reverse().join("")
来源：http://hz.tianlin.xyz/gtigmlyckn.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ppjwa.cn/gtmndthibr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shanyushiyangtech.top/gtcjtagruo.html

Go:   // 双指针从两端比较
来源：http://hz.nanxuanxn.top/gtlejuoomp.html

Ruby: s == s.reverse
来源：http://hz.jinghuilouyu.cn/gtqtfkhfga.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shanyushiyangkeji.top/gtvclahrhm.html

[N07] 两数之和（返回下标）
来源：http://hz.sweek.top/gtvzltdrhn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yvedp.cn/gtkcacllob.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.feifeiyinyue.top/gtlydlgljp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.tianlin.xyz/gtbpasstpt.html

TS:   // 手写 Map<string, number>
来源：http://hz.shangyingyoupin.top/gtysvjlklc.html

Java: // 手写 HashMap
来源：http://hz.0kj1m.cn/gtrpijkrzw.html

Go:   // 手写 map[int]int
来源：http://hz.jinyuanbaomall.cn/gtaljwzksr.html

Ruby: // 手写 Hash
来源：http://hz.tian-w.cn/gtaswnjqfj.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.52xcode.cn/gtdwtpspwq.html

[N08] 生成全排列
来源：http://hz.yongpay.top/gthtaghkfm.html

Py:   itertools.permutations(arr)
来源：http://hz.vqdsnc.cn/gtfunuysfr.html

PHP:  // 手写递归交换
来源：http://hz.dianchejie.cn/gtfsbqigsm.html

JS:   // 手写回溯递归
来源：http://hz.yuxming.cn/gtypyiuigw.html

TS:   // 手写回溯递归
来源：http://hz.52xcode.cn/gtslckrgvn.html

Java: // 手写回溯递归
来源：http://hz.chenlongwang.top/gtnibrplld.html

Go:   // 手写回溯递归
来源：http://hz.iojbl.cn/gtltdupqfr.html

Ruby: arr.permutation.to_a
来源：http://hz.hongshengwenyu.top/gtfrmbnbdi.html

C#:   // 手写回溯递归
来源：http://hz.c1oappe.top/gtetbckrxi.html

[N09] 栈与队列
来源：http://hz.jinqigfzy.top/gtvmwrzjkp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.svipenyu.cn/gtrtzffclm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.birdmap.top/gtequwlznq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.mhx1999.top/gtmtfmszpv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.birdmap.top/gtnanulmdq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.gotoacloud.top/gtrhxhqirz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ywan-chungtsiang.top/gtalpbrwsa.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zdqjudy.top/gtwkjdyhya.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.vqdsnc.cn/gtgahzuixf.html

[N10] 链表节点定义
来源：http://hz.haohaochexian.top/gtjuowznse.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.cdnleiting.top/gtedwkdtwt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hammf.cn/gtnworowlk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zycfv.cn/gtzguiydqq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.quarkkingdee.top/gttkdfbtdp.html

Java: class Node { int v; Node next; }
来源：http://hz.vqdsnc.cn/gtbfdvamva.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhaomingkeji.xyz/gtnxgpmtaq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ydjk.org.cn/gtqjnimsok.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yuanzhike.top/gtofsrnjez.html

[N11] 二叉树中序遍历
来源：http://hz.svipenyu.cn/gtsyclclhj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhengqikj.top/gtdyuqqwxn.html

PHP:  // 手写递归函数
来源：http://hz.fengsongda.top/gtnblewagf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.meibo888.top/gtslqdkipd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yvedp.cn/gtcvvnadfw.html

Java: // 手写递归
来源：http://hz.daria6918.cn/gtchpgylay.html

Go:   // 手写递归
来源：http://hz.shzxlz.cn/gtlcynmueh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.tianlin.xyz/gtktwmojkw.html

C#:   // 手写递归
来源：http://hz.iojbl.cn/gtfmpsahel.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.tanke756.top/gtsjatjvcs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yonumen.top/gteoxalqqx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ppjwa.cn/gtgykswwou.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinghuilouyu.cn/gtfvouquwu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xziqi.cn/gtdqpnsptg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.c1oappe.top/gtilmqctcy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.sufxvd.cn/gtmbxpkvjy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jinghuilouyu.cn/gttxqnpfpv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ywan-chungtsiang.top/gtojyrvwel.html

================================================================================
来源：http://hz.sysykeji.top/gtdxjvnhpd.html

O. 并发与异步
来源：http://hz.yueranfly.top/gttgudxifb.html

================================================================================
来源：http://hz.cashguo.top/gtpugswhqc.html

[O01] 启动一个线程
来源：http://hz.aizwys.cn/gtbrprswkr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xingfuxueyuan.xyz/gtyxdwjkih.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.mhx1999.top/gtrzdezket.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jlsjyb.cn/gttpfpbqws.html

TS:   // 同 JS
来源：http://hz.vqdsnc.cn/gtfdqcsutx.html

Java: new Thread(() -> f()).start()
来源：http://hz.jiagoushi.top/gtxdwqbnep.html

Go:   go f()
来源：http://hz.feifeiyinyue.top/gtxzzwcfnm.html

Ruby: Thread.new { f }
来源：http://hz.gogol.net.cn/gtcjaogpxd.html

C#:   Task.Run(() => F());
来源：http://hz.feifeiyinyue.top/gtilfjhnki.html

[O02] 使用线程池
来源：http://hz.sufxvd.cn/gtbrwwiaov.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.sysykeji.top/gtzhyhclpr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jianghu66.top/gtzdygccku.html

JS:   // worker_threads 线程池
来源：http://hz.zhongyouzk.top/gtbuhenfxf.html


<!-- 参考信息 -->