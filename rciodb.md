代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.0kj1m.cn/gtyowwzrdx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.smart0.xyz/gtbcykmjui.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hnxiangtu.top/gtjbkycqkb.html

Py:   pickle.dumps(obj)
来源：http://hz.kuanghao11.cn/gtrzrtdcaq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.daxiang520.top/gtnixtggnv.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yuxming.cn/gtvmddyjar.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.kuanghao11.cn/gtttbipdoo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yuanzhike.top/gtcgkpfgsu.html

Go:   encoding/gob
来源：http://hz.andypj.xyz/gtumgdlzty.html

Ruby: Marshal.dump(obj)
来源：http://hz.yj20258888.top/gtmfvikrbp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.fzhhl.top/gthvguyngy.html

================================================================================
来源：http://hz.zhijiandao.cn/gtiamljkqq.html

L. 网络请求
来源：http://hz.cqqwz.cn/gtlhiudbby.html

================================================================================
来源：http://hz.yuxming.cn/gtkjlpexpv.html

[L01] 发送 GET 请求
来源：http://hz.shangyingyoupin.top/gtzhqmzxhu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.nwbrower.top/gtlihjjfmb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.pycfn.com/gtbjozkysn.html

JS:   await fetch(url)
来源：http://hz.sxryk.cn/gtmtcqcnaj.html

TS:   await fetch(url)
来源：http://hz.wangdashe.top/gtzewojevb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.aizwys.cn/gtxkmgsszk.html

Go:   resp, err := http.Get(url)
来源：http://hz.fzhhl.top/gtikddqrhh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.chenlongwang.top/gtvurdbsny.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.snrcjt.cn/gtpzyhqihx.html

[L02] 发送 POST JSON
来源：http://hz.xuetiantiany.cn/gtkhhygnvg.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhoulong.xyz/gtmtlfsfgo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.tanke756.top/gtmakxkkul.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.birdmap.top/gtwjwejzwq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sufxvd.cn/gtdhualmtb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jyoumei.cn/gtgumxqxua.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.redwolf501.top/gtyysdjvjy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.wangdashe.top/gtwanbmric.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.birdmap.top/gtjlpppnsy.html

[L03] 设置自定义请求头
来源：http://hz.zhiwuduotai.top/gtmehjbfhn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nanxinkj.top/gtaewgrodr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yuxming.cn/gtokbxfyzx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxinkj.top/gtnayvrfoz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhoulong.xyz/gtrrabegtq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.gogol.net.cn/gtgawgbnil.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhijiandao.cn/gtwsspaviz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ppjwa.cn/gtzogsgzms.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gotoacloud.top/gtozltdiyg.html

[L04] 设置超时
来源：http://hz.jyoumei.cn/gtftxsjrbe.html

Py:   requests.get(url, timeout=5)
来源：http://hz.0kj1m.cn/gtwdnkdrth.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhiwuduotai.top/gtqsutqdwk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.mhx1999.top/gtltjdtdxj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhaomingkeji.xyz/gtahxwcvmd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yonumen.top/gtvdrgvspd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.pycfn.com/gtmngcfybr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.nanxuanxn.top/gtshvcnoii.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.chenzaomai.com/gttzctspzp.html

[L05] 上传文件（multipart）
来源：http://hz.feifeiyinyue.top/gtjwgnkgpl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.fengsongda.top/gtzkgpnqyd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.redwolf501.top/gtmjghtvnh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.feifeiyinyue.top/gtmtjpnmls.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jyoumei.cn/gtbvyzxrzo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.chenjidiqi.icu/gtljtegqrg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhengqikj.top/gtfofaypow.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yonumen.top/gtusseyonk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hfpthk.cn/gtyirqiczs.html

[L06] 解析响应为 JSON
来源：http://hz.xinyue.icu/gtsvhjmxpn.html

Py:   resp.json()
来源：http://hz.yongpay.top/gtpieypjei.html

PHP:  json_decode($body, true);
来源：http://hz.nwbrower.top/gtokppadbj.html

JS:   await resp.json()
来源：http://hz.wangshuangyany.cn/gtbikxkgyz.html

TS:   await resp.json()
来源：http://hz.yongpay.top/gtjkvusoiy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.sufxvd.cn/gtdjegeqpt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.316326.xyz/gttfofefay.html

Ruby: JSON.parse(resp.body)
来源：http://hz.daria6918.cn/gtrdrariuh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.sweek.top/gtjnujheve.html

[L07] 处理 HTTP 状态码
来源：http://hz.fzhhl.top/gtoznglbbj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.52xcode.cn/gtyaukvteh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.wangdashe.top/gtwsuwdvai.html

JS:   resp.ok;  resp.status
来源：http://hz.yuxming.cn/gtfidskejj.html

TS:   resp.ok;  resp.status
来源：http://hz.chenzaomai.com/gtsgksvdoo.html

Java: resp.statusCode()
来源：http://hz.yj20258.top/gttibjdxkd.html

Go:   resp.StatusCode
来源：http://hz.jinyuanbaomall.cn/gtqjyqukql.html

Ruby: resp.code.to_i
来源：http://hz.ehwqpu.com/gtheygtcib.html

C#:   (int)resp.StatusCode
来源：http://hz.ppjwa.cn/gtxtlhubzi.html

[L08] 并发请求多个地址
来源：http://hz.zhixingplan.top/gtizxrgthl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jyoumei.cn/gtrqxzefxr.html

PHP:  curl_multi_init() 系列
来源：http://hz.xingfuxueyuan.xyz/gtsffaldhy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhongyouzk.top/gtqbdwjjde.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydzc1.top/gtaqybhzdj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ivvv.top/gtohgjmvgz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.quarkkingdee.top/gtbohalmdx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ywan-chungtsiang.top/gtbgjtbycs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.0kj1m.cn/gtshlxzubz.html

================================================================================
来源：http://hz.ydzc1.top/gtpwmjbjdg.html

M. 命令行 / 进程 / 环境
来源：http://hz.dashuyun.cn/gtjmvpbuka.html

================================================================================
来源：http://hz.jqgfzy.top/gtjvexjtxs.html

[M01] 读取命令行参数
来源：http://hz.yongpay.top/gtkasplben.html

Py:   sys.argv[1:]
来源：http://hz.c1oappe.top/gtdkherozj.html

PHP:  $argv;  $argc;
来源：http://hz.zhaomingkeji.xyz/gtktdswmrm.html

JS:   process.argv.slice(2)
来源：http://hz.tanke756.top/gtxjxqwgev.html

TS:   process.argv.slice(2)
来源：http://hz.gotoacloud.top/gtwfapeprb.html

Java: args 数组（main 方法参数）
来源：http://hz.ehwqpu.com/gtfrsjwzac.html

Go:   os.Args[1:]
来源：http://hz.hongshengwenyu.top/gtjhhovfcd.html

Ruby: ARGV
来源：http://hz.gotoacloud.top/gtznzguhkq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.wangshuangyany.cn/gtiyiporgu.html

[M02] 读取环境变量
来源：http://hz.gogol.net.cn/gtmxkfxegt.html

Py:   os.environ.get("HOME")
来源：http://hz.shzxlz.cn/gtxycnblkh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sxryk.cn/gtfcvjudxp.html

JS:   process.env.HOME
来源：http://hz.zhoulong.xyz/gttghvwxiz.html

TS:   process.env.HOME
来源：http://hz.zycfv.cn/gtaeudtphd.html

Java: System.getenv("HOME")
来源：http://hz.zycfv.cn/gtwifvjegp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.shzxlz.cn/gtrmfofhhq.html

Ruby: ENV["HOME"]
来源：http://hz.guowangkeji.top/gtxslocumj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hnxiangtu.top/gtfyeihhpm.html

[M03] 执行外部命令
来源：http://hz.ybcxt.top/gtjbchohcc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xuanzx.com/gtpragpbzn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ydzc1.top/gtbzhdlcet.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj20258.top/gtzasdixla.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gaohongyu789.top/gtqdaibvvm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hywenlv.cn/gthznwljnn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.fzhhl.top/gtvmgdsicf.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.kuanghao11.cn/gtzzqbyami.html

C#:   Process.Start("ls", "-l");
来源：http://hz.52xcode.cn/gtrmiqnnzr.html

[M04] 获取当前工作目录
来源：http://hz.tianlin.xyz/gtrxbthlya.html

Py:   os.getcwd()
来源：http://hz.hnqzz.top/gtzggsapzs.html

PHP:  getcwd();
来源：http://hz.feifeiyinyue.top/gtwqvyiiog.html

JS:   process.cwd()
来源：http://hz.zhiwuduotai.top/gtlkddrtva.html

TS:   process.cwd()
来源：http://hz.c1oappe.top/gtjavviwke.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yonumen.top/gttklnfffe.html

Go:   os.Getwd()
来源：http://hz.kuanghao11.cn/gtbdjplqfn.html

Ruby: Dir.pwd
来源：http://hz.dianchejie.cn/gtuzwwbqrf.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jyoumei.cn/gtqodxrcbp.html

[M05] 设置退出码
来源：http://hz.jianghu66.top/gthwunbxls.html

Py:   sys.exit(1)
来源：http://hz.zhaomingkeji.xyz/gtnaylayvm.html

PHP:  exit(1);
来源：http://hz.jianghu66.top/gtdxskmdpm.html

JS:   process.exit(1)
来源：http://hz.yanxiufei.cn/gtyjetzfyn.html

TS:   process.exit(1)
来源：http://hz.jinyuanbaomall.cn/gtylfwledb.html

Java: System.exit(1)
来源：http://hz.xuetiantiany.cn/gtbeclcduo.html

Go:   os.Exit(1)
来源：http://hz.zdqjudy.top/gtshtbgcma.html

Ruby: exit 1
来源：http://hz.hammf.cn/gtuoeylnww.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.dianchejie.cn/gtpsrmomac.html

[M06] 向标准错误输出
来源：http://hz.guowangkeji.top/gtnzsdcacl.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jianghu66.top/gtdezlrfig.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.vqdsnc.cn/gtfqzreekr.html

JS:   console.error("err")
来源：http://hz.vqdsnc.cn/gtgimwacim.html

TS:   console.error("err")
来源：http://hz.yj20258888.top/gtxiqfhxal.html

Java: System.err.println("err")
来源：http://hz.dashuyun.cn/gtcyukpfku.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.snrcjt.cn/gtsexubapg.html

Ruby: warn "err"
来源：http://hz.yonumen.top/gtwekddzoe.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yj20258.top/gtsdcetbnr.html

[M07] 判断是否为主入口
来源：http://hz.zhengqikj.top/gtiqpskvxu.html

Py:   if __name__ == "__main__":
来源：http://hz.xingfuxueyuan.xyz/gtkzdxfekt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shzxlz.cn/gtinziuogw.html

JS:   require.main === module
来源：http://hz.yueranfly.top/gtcjrbxgyw.html

TS:   require.main === module
来源：http://hz.guowangkeji.top/gtnwdukqmi.html

Java: public static void main(String[] args)
来源：http://hz.feifeiyinyue.top/gtbpbkgefg.html

Go:   func main()
来源：http://hz.ydjk.org.cn/gtyvfwzutd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinqigfzy.top/gtkqxkbdjv.html

C#:   static void Main(string[] args)
来源：http://hz.kuanghao11.cn/gtfnsjfbgd.html

[M08] 获取系统与运行时信息
来源：http://hz.xylfe.cn/gtbxrajion.html

Py:   platform.system();  platform.python_version()
来源：http://hz.feifeiyinyue.top/gtjbcfpzfj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yuxming.cn/gtonrtlals.html

JS:   process.platform;  process.version
来源：http://hz.yuanzhike.top/gtfnybfeek.html

TS:   process.platform;  process.version
来源：http://hz.shangyingyoupin.top/gtlhvhaegd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.fzhhl.top/gtrdfxymaf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yj202588.top/gtycdxgfkc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jqgfzy.top/gtshuirgbr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.wangdashe.top/gtpzbgpakd.html

================================================================================
来源：http://hz.kuanghao11.cn/gtehykxtzn.html

N. 数据结构与算法
来源：http://hz.bjfxy.top/gtauaoxzoj.html

================================================================================
来源：http://hz.jiagoushi.top/gtdlpuhxgb.html

[N01] 二分查找（有序数组）
来源：http://hz.yonumen.top/gtcrvquour.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.c1oappe.top/gtjybniqry.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jianghu66.top/gtapsawmdy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xinyue.icu/gtvboyldbo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhoulong.xyz/gtbivzkald.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtonjzozvc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jiagoushi.top/gtdpleiajh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xuanzx.com/gtpskflmoe.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hywenlv.cn/gtmwalbulg.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ppjwa.cn/gtwigcnaop.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xingfuxueyuan.xyz/gtkqsalwme.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ehwqpu.com/gtvwrkucty.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yueranfly.top/gtithuppad.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gogol.net.cn/gttacrxgsd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.nwbrower.top/gttdxdrvgp.html

Go:   slices.Sort(arr)
来源：http://hz.jiagoushi.top/gtmpwxoskl.html

Ruby: arr.sort
来源：http://hz.zhixingplan.top/gtbpnhzttv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.bjfxy.top/gtlrkndshl.html

[N03] 快速排序（分治示例）
来源：http://hz.hywenlv.cn/gtxuinpxde.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yongpay.top/gtqbcsacjr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jinqigfzy.top/gtolqhfvoa.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigfzy.top/gtzvzejybc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.smart0.xyz/gtkmkheedt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.quarkkingdee.top/gtdgkxfgkk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ywan-chungtsiang.top/gtzqkbljnn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.redwolf501.top/gtpjcbkzlr.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhongyouzk.top/gtymezumme.html

[N04] 斐波那契数列
来源：http://hz.yj202588.top/gtgmyomcmx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.havefunace.top/gtktutntmg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.mhx1999.top/gtnwrwhmqu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.aibaodan.cn/gtmfjhptti.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnqzz.top/gtuihpnkng.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shzxlz.cn/gtfkrouxxp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.chenjidiqi.icu/gtsfszygpa.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.tian-w.cn/gtdestybka.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhongyouzk.top/gtdndhvcng.html

[N05] 最大公约数
来源：http://hz.52xcode.cn/gtyaeqqacl.html

Py:   math.gcd(a, b)
来源：http://hz.wangshuangyany.cn/gtloqupxav.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.nanxuanxn.top/gteddkxcij.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sufxvd.cn/gtcnhubwms.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ybcxt.top/gthanimvzw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yvedp.cn/gtyfzjdlqu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cashguo.top/gtqobcksfz.html

Ruby: a.gcd(b)
来源：http://hz.xuetiantiany.cn/gtzpfbrxii.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.chenjidiqi.icu/gtctpeuqeg.html

[N06] 判断回文字符串
来源：http://hz.jinqigufen.top/gtvrcrfinv.html

Py:   s == s[::-1]
来源：http://hz.xziqi.cn/gtxdvhspfs.html

PHP:  $s === strrev($s);
来源：http://hz.daria6918.cn/gtmmcficos.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jqgufenzy.top/gtgernhyjk.html

TS:   s === [...s].reverse().join("")
来源：http://hz.tian-w.cn/gthjdoijqt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ehwqpu.com/gtjzdkwlze.html

Go:   // 双指针从两端比较
来源：http://hz.pycfn.com/gtlhnaycfk.html

Ruby: s == s.reverse
来源：http://hz.pengpengdd.cyou/gtulimxkeq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hammf.cn/gtvicyxlap.html

[N07] 两数之和（返回下标）
来源：http://hz.pycfn.com/gtsoemuvoi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shuidangran.top/gtrprgagkt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhixingplan.top/gtkxgnoild.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.guannengcc.top/gtyeppakkh.html

TS:   // 手写 Map<string, number>
来源：http://hz.jqgfzy.top/gtxlohckew.html

Java: // 手写 HashMap
来源：http://hz.zycfv.cn/gtjeuzxorm.html

Go:   // 手写 map[int]int
来源：http://hz.nanxinkj.top/gtxzjiwruu.html

Ruby: // 手写 Hash
来源：http://hz.ydzc1.top/gtqhrlzyco.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.snrcjt.cn/gtxuwhuzcr.html

[N08] 生成全排列
来源：http://hz.wangdashe.top/gtobqrpnkt.html

Py:   itertools.permutations(arr)
来源：http://hz.zhaomingkeji.xyz/gtmpmxhpln.html

PHP:  // 手写递归交换
来源：http://hz.yanxiufei.cn/gtijqmcjuu.html

JS:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtbraosgnk.html

TS:   // 手写回溯递归
来源：http://hz.hnqzz.top/gtkjxxmule.html

Java: // 手写回溯递归
来源：http://hz.gotoacloud.top/gtvwfhayhj.html

Go:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtxdnsntqf.html

Ruby: arr.permutation.to_a
来源：http://hz.yangfankeji.com/gtcnuiehuf.html

C#:   // 手写回溯递归
来源：http://hz.316326.xyz/gtconlasjg.html

[N09] 栈与队列
来源：http://hz.shanyushiyangkeji.top/gtsxltooyh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xingfuxueyuan.xyz/gtteosjtcz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yanxiufei.cn/gtnpqghfuf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.snrcjt.cn/gtovjpvqjo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ppjwa.cn/gtytnvwcgr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yanxiufei.cn/gtdotxvfyp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.dashuyun.cn/gtkndcawlv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yvedp.cn/gtcwoxsgld.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ydzc1.top/gtndokbtes.html

[N10] 链表节点定义
来源：http://hz.daria6918.cn/gtbthfpnqx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.cashguo.top/gthbknosnf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.gotoacloud.top/gtbcczfcnb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.wangdashe.top/gtyjahmxfj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.chenzaomai.com/gtgvmsnegy.html

Java: class Node { int v; Node next; }
来源：http://hz.cqqwz.cn/gtysdoeoon.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.haohaochexian.top/gthmnqkrze.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.chenzaomai.com/gtslguddon.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.quarkkingdee.top/gtauiybwvv.html

[N11] 二叉树中序遍历
来源：http://hz.cucudq.cn/gtjpuvfqff.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cdnleiting.top/gtbhpxyplm.html

PHP:  // 手写递归函数
来源：http://hz.xziqi.cn/gtddsilmdi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jianghu66.top/gtheziuuzx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhengqikj.top/gtptagbtif.html

Java: // 手写递归
来源：http://hz.c1oappe.top/gtomkxnwcn.html

Go:   // 手写递归
来源：http://hz.yanxiufei.cn/gtdpsfmcji.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zycfv.cn/gttltbrmas.html

C#:   // 手写递归
来源：http://hz.yongpay.top/gtzqhzizdv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jyoumei.cn/gtnwyaikon.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jqgufenzy.top/gtiifsqitb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jinghuilouyu.cn/gtgpjxnmna.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gaohongyu789.top/gtjbwmtetu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.fengsongda.top/gtkkwpcezw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jiagoushi.top/gtostrrmvv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.tian-w.cn/gtfrjrkmnr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ywan-chungtsiang.top/gtpxqvzfec.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenzaomai.com/gttflewihw.html

================================================================================
来源：http://hz.birdmap.top/gtgscmkaby.html

O. 并发与异步
来源：http://hz.yj20258.top/gthosvckiz.html

================================================================================
来源：http://hz.mhx1999.top/gtlzocmnor.html

[O01] 启动一个线程
来源：http://hz.c1oappe.top/gttgtnckag.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yj20258.top/gtefyuclph.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ybcxt.top/gtqtametcu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.nwbrower.top/gtqqhlvyqj.html

TS:   // 同 JS
来源：http://hz.shangyingyoupin.top/gtyrazmlir.html

Java: new Thread(() -> f()).start()
来源：http://hz.gogol.net.cn/gtqyfjowyy.html

Go:   go f()
来源：http://hz.andypj.xyz/gtqltsekce.html

Ruby: Thread.new { f }
来源：http://hz.xziqi.cn/gtlmimzjcc.html

C#:   Task.Run(() => F());
来源：http://hz.jinghuilouyu.cn/gtzhckoqyq.html

[O02] 使用线程池
来源：http://hz.ppjwa.cn/gtnoozrxpl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yj202588.top/gtlgeenifc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.xziqi.cn/gtilerxmgw.html

JS:   // worker_threads 线程池
来源：http://hz.chenlongwang.top/gthuvraoor.html

TS:   // worker_threads 线程池
来源：http://hz.quarkkingdee.top/gtqodsxzmz.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xinyue.icu/gtniqzpyti.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.sysykeji.top/gtdefldhxq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hnxiangtu.top/gtcnywxijt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yongpay.top/gtbrdthihu.html

[O03] 加锁保护共享数据
来源：http://hz.daxiang520.top/gtmsffrvct.html

Py:   with lock: shared += 1
来源：http://hz.cashguo.top/gtwfanbcpt.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.sxryk.cn/gtmytjeosm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ybcxt.top/gtegmpthol.html

TS:   // 同 JS
来源：http://hz.zhiwuduotai.top/gtzfiuetlj.html

Java: synchronized (this) { shared++; }
来源：http://hz.cashguo.top/gtvzeqbkpo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ydzc1.top/gthbkutkaf.html


<!-- 参考信息 -->