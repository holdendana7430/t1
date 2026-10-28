代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.yj202588.top/gtmykgliza.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhaomingkeji.xyz/gtumqwnwxi.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhiwuduotai.top/gtzkwusnqm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.gzhubu.top/gtqlxganno.html

Go:   strings.TrimSpace(s)
来源：http://hz.fengsongda.top/gtaqnqcjyw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.guowangkeji.top/gtxqkhcfcj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.hywenlv.cn/gtfhxnttte.html

[A25] 字符串比较
来源：http://hz.ivvv.top/gtgzlposkc.html

Py:   s1 == s2; s1 != s2
来源：http://hz.shzxlz.cn/gtfjuhqolc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.haohaochexian.top/gtkjnngzon.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.sxryk.cn/gtfvxgndld.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.snrcjt.cn/gtnzpjgbwq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.redwolf501.top/gtwjtanxmw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.aibaodan.cn/gtnshigfpe.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.cashguo.top/gtmrjentib.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.snrcjt.cn/gtrxssacvh.html

[A26] 类型转换总览
来源：http://hz.yonumen.top/gtdclgcatp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.yj202588.top/gtlgkiqics.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.vqdsnc.cn/gtuvooeqdn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.feifeiyinyue.top/gtgpsmssvr.html

TS:   Number() String() Boolean() x as number
来源：http://hz.jlsjyb.cn/gtqzxwkjjx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.dashuyun.cn/gtvfdnyrjw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.jinyuanbaomall.cn/gtdxodxnuc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.jinqigfzy.top/gtaiwdbsrg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.zycfv.cn/gtjtkeqsqg.html

================================================================================
来源：http://hz.guannengcc.top/gtflevdvfs.html

B. 流程控制
来源：http://hz.chenjidiqi.icu/gtopvzrvde.html

================================================================================
来源：http://hz.hywenlv.cn/gtunozcgpn.html

[B01] 条件判断 if / else
来源：http://hz.zhongyouzk.top/gtjtymdwsd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.nanxuanxn.top/gtibwmsptu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.tian-w.cn/gtwxpjimfr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.aibaodan.cn/gtumukfcpk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.shanyushiyangkeji.top/gtttlxssyn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.vqdsnc.cn/gtorignsbh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.vqdsnc.cn/gtdsvnilse.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.jinqigufen.top/gtwkjnsheq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.birdmap.top/gtlivitfgj.html

[B02] 多分支 else if / elif
来源：http://hz.tianlin.xyz/gtskuktsih.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.cheryme.top/gtdtbsxygw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.pengpengdd.cyou/gtssnshmkz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.aizwys.cn/gtmkwkjose.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yvedp.cn/gtjuapciod.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhengqikj.top/gtajrxjrke.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.52xcode.cn/gtjwvgvwry.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.dashuyun.cn/gtnpjgtvjz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.nanxuanxn.top/gtlvfghoog.html

[B03] switch / match / case
来源：http://hz.meibo888.top/gtbsknieqb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.daxiang520.top/gtmwhjjtfo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.yangfankeji.com/gtozofmqip.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yanxiufei.cn/gtygurlwiu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jqgfzy.top/gthtxonywo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.zhixingplan.top/gtkjzxoowj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.hnqzz.top/gtqlnaybhs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.dianchejie.cn/gtnyopqggk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.zycfv.cn/gtaopjctfs.html

[B04] for 计数循环
来源：http://hz.ydzc1.top/gtalfhlkch.html

Py:   for i in range(10): print(i)
来源：http://hz.c1oappe.top/gthdpgynol.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.vqdsnc.cn/gtxoutuzup.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.chenjidiqi.icu/gtklzuetbl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.birdmap.top/gtwajufsma.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.cucudq.cn/gtejefivok.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.wangshuangyany.cn/gtwbtgtxep.html

Ruby: 10.times { |i| puts i }
来源：http://hz.xylfe.cn/gtcrijjqoj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.sysykeji.top/gtfkbbaujd.html

[B05] 遍历数组 / 列表
来源：http://hz.ivvv.top/gtwompdvjt.html

Py:   for item in arr: print(item)
来源：http://hz.jqgufenzy.top/gtzhpgtowo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.ydjk.org.cn/gtbrxliskm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.tian-w.cn/gtimlffshw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.jinghuilouyu.cn/gtdqponhse.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.fengsongda.top/gtsvhbgwhd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.gogol.net.cn/gtrvxsjpey.html

Ruby: arr.each { |item| puts item }
来源：http://hz.316326.xyz/gtmisauyhj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.hfpthk.cn/gtrxdscmmn.html

[B06] 遍历字典 / 对象
来源：http://hz.ehwqpu.com/gttqstbmqe.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.zycfv.cn/gtojyytrxm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.gotoacloud.top/gtkjhyxsca.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.tian-w.cn/gtnwjerzrg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ybcxt.top/gtgzvobiqo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.redwolf501.top/gtyfqpqsht.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.mhx1999.top/gttdwrzuux.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.fzhhl.top/gttlllawio.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.yongpay.top/gtgsykolns.html

[B07] while 循环
来源：http://hz.yongpay.top/gtdyytrlik.html

Py:   while i < 10: i += 1
来源：http://hz.52xcode.cn/gtfdgbuhqn.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.chenjidiqi.icu/gtytsvhzcd.html

JS:   while (i < 10) { i++; }
来源：http://hz.jinqigufen.top/gtqssmnqag.html

TS:   while (i < 10) { i++; }
来源：http://hz.jinyuanbaomall.cn/gtpiopzumb.html

Java: while (i < 10) { i++; }
来源：http://hz.iojbl.cn/gtgyigulgl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.chenzaomai.com/gtfyuxafgp.html

Ruby: while i < 10; i += 1; end
来源：http://hz.snrcjt.cn/gtspyvrhnv.html

C#:   while (i < 10) { i++; }
来源：http://hz.yanxiufei.cn/gtctkdhvcy.html

[B08] do-while（至少执行一次）
来源：http://hz.cucudq.cn/gtmyqigsme.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.snrcjt.cn/gturlwcqzj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zdqjudy.top/gtuerkwxak.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yuxming.cn/gtpqwnnssm.html

TS:   do { i++; } while (i < 10);
来源：http://hz.daxiang520.top/gtdwbuojxu.html

Java: do { i++; } while (i < 10);
来源：http://hz.yonumen.top/gthbyyejcr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.chenzaomai.com/gtbicorbzn.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.tianlin.xyz/gtvvruaaxo.html

C#:   do { i++; } while (i < 10);
来源：http://hz.52xcode.cn/gtivqrnwwo.html

[B09] break 与 continue
来源：http://hz.haohaochexian.top/gtftwnnvkn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.xuetiantiany.cn/gtbygoxuwa.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.sysykeji.top/gtuzziszlw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nwbrower.top/gtmpcsyqpv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gaohongyu789.top/gtefqtkppe.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.52xcode.cn/gtrslkulvy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.0kj1m.cn/gtartentzw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.feifeiyinyue.top/gtvfbnxfpp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenjidiqi.icu/gtawevcvkk.html

[B10] 遍历同时拿索引
来源：http://hz.shzxlz.cn/gtppcgvyaq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.cqqwz.cn/gtwzxhrcot.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.0kj1m.cn/gtfxkodunc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.xuetiantiany.cn/gtpvtkwfkb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zhijiandao.cn/gtkzholzpf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.shanyushiyangkeji.top/gtjpbipndz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.0kj1m.cn/gtfcwjnvko.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.gzhubu.top/gtiuwlohoz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jianghu66.top/gttjtqlmnn.html

[B11] 生成数字序列 / 区间
来源：http://hz.jqgufenzy.top/gtbuyemkqh.html

Py:   list(range(0, 10, 2))
来源：http://hz.shzxlz.cn/gtevucyhhn.html

PHP:  range(0, 10, 2);
来源：http://hz.smart0.xyz/gtycemevkn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.0kj1m.cn/gtfbswqedg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.sysykeji.top/gtxarshdtn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jinqigufen.top/gthouyqsia.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zhengqikj.top/gtsucszcnv.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zhijiandao.cn/gtzoqmewtr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.meibo888.top/gtgsysbzbs.html

[B12] 跳出多层循环
来源：http://hz.316326.xyz/gtgnydqxab.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.c1oappe.top/gtfstwcvoc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.ywan-chungtsiang.top/gtshiqmwbl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cdnleiting.top/gtldkaaoxq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhoulong.xyz/gtjvyqhsoo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.dashuyun.cn/gtekbzhhbt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yj20258888.top/gtsukwzrdj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yj20258.top/gttejmcxfl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.tianlin.xyz/gtiiznrdfo.html

[B13] 判断是否为数字
来源：http://hz.zhixingplan.top/gtsaziscde.html

Py:   isinstance(x, (int, float))
来源：http://hz.ydjk.org.cn/gtkfdeemca.html

PHP:  is_numeric($x)
来源：http://hz.jyoumei.cn/gtqutrlljd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sufxvd.cn/gthjcokvtw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.52xcode.cn/gtfujokpth.html

Java: x instanceof Number
来源：http://hz.sxryk.cn/gtukooqgwc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.smart0.xyz/gtjxtjwfph.html

Ruby: x.is_a?(Numeric)
来源：http://hz.snrcjt.cn/gtqxjwshta.html

C#:   x is int or double or decimal
来源：http://hz.mhx1999.top/gthkegykbc.html

[B14] 判断值是否在集合内
来源：http://hz.birdmap.top/gtzxaacopw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hammf.cn/gtpatzekkt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.smart0.xyz/gteclqhyxn.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jlsjyb.cn/gtgfuuqluc.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.nanxinkj.top/gtgalohygy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ywan-chungtsiang.top/gtcyimkkne.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.guowangkeji.top/gtzarjepck.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jyoumei.cn/gtrqmgsiwu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.sxryk.cn/gtfzzjagod.html

[B15] 布尔运算与取反
来源：http://hz.xziqi.cn/gthhxdbbxe.html

Py:   a and b or not c
来源：http://hz.quarkkingdee.top/gtyllujgbf.html

PHP:  $a && $b || !$c
来源：http://hz.jlsjyb.cn/gtxrxvqaxl.html

JS:   a && b || !c
来源：http://hz.andypj.xyz/gtsvxnatff.html

TS:   a && b || !c
来源：http://hz.fengsongda.top/gtxmjhoxjt.html

Java: a && b || !c
来源：http://hz.chenlongwang.top/gtvmfczwmj.html

Go:   a && b || !c
来源：http://hz.wangshuangyany.cn/gtvzydmyxk.html

Ruby: a && b || !c
来源：http://hz.nwbrower.top/gttsscmrgi.html

C#:   a && b || !c
来源：http://hz.feifeiyinyue.top/gtoaaamnoh.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hysaishi.cn/gtvnbdvlhn.html

Py:   if not data: return
来源：http://hz.shanyushiyangkeji.top/gtpwesrxqh.html

PHP:  if (!$data) { return; }
来源：http://hz.hongshengwenyu.top/gtueutaqym.html

JS:   if (!data) return;
来源：http://hz.gzhubu.top/gttyhbaoew.html

TS:   if (!data) return;
来源：http://hz.ehwqpu.com/gtvuuqskqw.html

Java: if (data == null) return;
来源：http://hz.chenjidiqi.icu/gtxqohsakl.html

Go:   if data == nil { return }
来源：http://hz.pycfn.com/gtuukfxkai.html

Ruby: return if data.nil?
来源：http://hz.c1oappe.top/gthiircush.html

C#:   if (data == null) return;
来源：http://hz.pengpengdd.cyou/gtuvtvhvvz.html

================================================================================
来源：http://hz.dashuyun.cn/gthxrwwsqw.html

C. 函数与作用域
来源：http://hz.wangshuangyany.cn/gteyfwidja.html

================================================================================
来源：http://hz.52xcode.cn/gtdyyehohf.html

[C01] 定义函数
来源：http://hz.nanxinkj.top/gtnlpakosa.html

Py:   def add(a, b): return a + b
来源：http://hz.ivvv.top/gtmdgnwjos.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhoulong.xyz/gtjakjzper.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yangfankeji.com/gtdhymjvhq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cdnleiting.top/gtzdgwsvsy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.chenjidiqi.icu/gtviqzdazw.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yvedp.cn/gtmhrsplem.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jinghuilouyu.cn/gtskzuogik.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.chenzaomai.com/gtefhkdwcv.html

[C02] 默认参数
来源：http://hz.feifeiyinyue.top/gtjkgcmhzn.html

Py:   def greet(name="World"): return name
来源：http://hz.jqgfzy.top/gtgottanjw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yanxiufei.cn/gtjljeojyv.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.shangyingyoupin.top/gtxgsdwezw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.pengpengdd.cyou/gtnvokrwbt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yongpay.top/gtsqkoimlv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.chenzaomai.com/gtcpivpogg.html

Ruby: def greet(name = "World") = name
来源：http://hz.hysaishi.cn/gtmruudeho.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xziqi.cn/gtijotampv.html

[C03] 可变参数
来源：http://hz.jianghu66.top/gtcjoxbzjz.html

Py:   def total(*args): return sum(args)
来源：http://hz.yonumen.top/gthddfyibv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.kuanghao11.cn/gtvbaeudmh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.aibaodan.cn/gttrqoeprd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.svipenyu.cn/gtkiacnsul.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.havefunace.top/gtrsylqzlq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.smart0.xyz/gtubgahebw.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zhoulong.xyz/gtylndfpnw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.wangshuangyany.cn/gthotnivxc.html

[C04] 命名参数 / 关键字参数
来源：http://hz.smart0.xyz/gtwrxjmxqa.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hfpthk.cn/gtllknwcon.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yuxming.cn/gtgqgtudwd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yj20258888.top/gtqxqvjeql.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.smart0.xyz/gtvsyhozld.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.quarkkingdee.top/gtrratdbvk.html

Go:   // 无：用配置结构体参数
来源：http://hz.yj202588.top/gtilqqzati.html

Ruby: f(a: 1, b: 2)
来源：http://hz.tian-w.cn/gtubfihzqm.html

C#:   f(a: 1, b: 2)
来源：http://hz.kuanghao11.cn/gtprptmidz.html

[C05] 返回多个值
来源：http://hz.haohaochexian.top/gtxxjbwuqk.html

Py:   return a, b
来源：http://hz.yj20258.top/gtsmtizqnm.html

PHP:  return [$a, $b];
来源：http://hz.dianchejie.cn/gtqdpbhxcq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhijiandao.cn/gtghmfijmm.html

TS:   return { a, b };
来源：http://hz.zhiwuduotai.top/gtupcivfch.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hfpthk.cn/gtjnrgqbrs.html

Go:   return a, b
来源：http://hz.cheryme.top/gtemfojisk.html

Ruby: return a, b
来源：http://hz.zhiwuduotai.top/gtscsfkvba.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.meibo888.top/gttixsabfh.html

[C06] 匿名函数 / lambda
来源：http://hz.vqdsnc.cn/gtqqaxinry.html

Py:   square = lambda x: x * x
来源：http://hz.hywenlv.cn/gtvblqjdcz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.xuetiantiany.cn/gtvjycdjyu.html

JS:   const square = x => x * x;
来源：http://hz.xziqi.cn/gtuuanhvyc.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xylfe.cn/gthjergztz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhengqikj.top/gtxaddzgpk.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hongshengwenyu.top/gtaitjrynv.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhengqikj.top/gtjyjyyzyc.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.gotoacloud.top/gtmpybfvby.html

[C07] 把函数作为参数传入
来源：http://hz.yj202588.top/gtuicfnfpq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zdqjudy.top/gtuqelnbzl.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yangfankeji.com/gtjhckqzdb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yangfankeji.com/gtwijuucmg.html

TS:   arr.map(String)
来源：http://hz.yj202588.top/gtlcywaiqm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhijiandao.cn/gtjwwaxczz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.cucudq.cn/gtvoorqfej.html

Ruby: arr.map(&:upcase)
来源：http://hz.shuidangran.top/gtyzfxbshl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhoulong.xyz/gtallkbllb.html

[C08] 闭包
来源：http://hz.pengpengdd.cyou/gtnatzchni.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.wangshuangyany.cn/gtesoqfhxf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.hammf.cn/gtjhlskooo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.52xcode.cn/gtsqwnvglu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hnqzz.top/gtugvymwuf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.redwolf501.top/gtjgykaqij.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yangfankeji.com/gtecvzkusi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xuanzx.com/gtzynqrcvy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hammf.cn/gttytqrysl.html

[C09] 递归
来源：http://hz.yvedp.cn/gtvpqtpgbd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.sysykeji.top/gttzkjlucr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ywan-chungtsiang.top/gttzxstsld.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.c1oappe.top/gtqhqakyva.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ehwqpu.com/gtckenxfsl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.cqqwz.cn/gtqcnrfijs.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.snrcjt.cn/gtsrxjctgw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.snrcjt.cn/gtdahrwitw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jianghu66.top/gtryjqbnzr.html

[C10] 变量作用域
来源：http://hz.yueranfly.top/gtifsitlee.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhixingplan.top/gtwsktjcnm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hnqzz.top/gtimgzbgee.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yuanzhike.top/gtdghugofx.html

TS:   同 JS
来源：http://hz.vqdsnc.cn/gtihuohgre.html

Java: 方法内为块级作用域
来源：http://hz.xuetiantiany.cn/gtwxjdgpdb.html

Go:   花括号块级作用域
来源：http://hz.andypj.xyz/gteiaursly.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.haohaochexian.top/gtortkkvtb.html

C#:   块级作用域
来源：http://hz.jqgufenzy.top/gtxfxjlbje.html

[C11] 模块导入与导出
来源：http://hz.ywan-chungtsiang.top/gtjlbohdgi.html

Py:   from module import func
来源：http://hz.nanxinkj.top/gtbmtjgayg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yj202588.top/gtclqyjqus.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yueranfly.top/gttpkjamnq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.guannengcc.top/gtbwujkemf.html

Java: import java.util.List;
来源：http://hz.ivvv.top/gtrtwniysu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.nwbrower.top/gtxvhlufzs.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.daxiang520.top/gtrpkzxypk.html

C#:   using System.Text;
来源：http://hz.zdqjudy.top/gtknkxbrto.html

[C12] 立即执行函数 IIFE
来源：http://hz.chenlongwang.top/gtjgkkefxv.html

Py:   (lambda: print("run"))()
来源：http://hz.snrcjt.cn/gtzqjgzyys.html

PHP:  (function () { echo "run"; })();
来源：http://hz.havefunace.top/gtltqpnwzw.html

JS:   (() => { console.log("run"); })();
来源：http://hz.vqdsnc.cn/gteoqwczmt.html

TS:   (() => { console.log("run"); })();
来源：http://hz.feifeiyinyue.top/gtoencibnt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.havefunace.top/gtaldjvufg.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.pycfn.com/gtmzibqtcd.html

Ruby: -> { puts "run" }.call
来源：http://hz.ivvv.top/gthapiyjvj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.snrcjt.cn/gtnnwbhvcd.html

[C13] 类型声明 / 类型注解
来源：http://hz.yvedp.cn/gtwoiwuaar.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.shzxlz.cn/gtxlqllpbd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sufxvd.cn/gtnyzklmwi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hnqzz.top/gtrnwtneoj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.svipenyu.cn/gtltcopvbu.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xylfe.cn/gtdlzyhlmc.html

Go:   func add(a, b int) int
来源：http://hz.cdnleiting.top/gtzqtflqik.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.gaohongyu789.top/gtkepcddzh.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.316326.xyz/gthsudzvle.html

[C14] 泛型函数
来源：http://hz.hywenlv.cn/gtjjypprwl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.daxiang520.top/gticmodebi.html

PHP:  // 无泛型
来源：http://hz.andypj.xyz/gtlatuvjid.html

JS:   // 无泛型
来源：http://hz.birdmap.top/gtcjqubqfl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yueranfly.top/gtvvzgkcaf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.mhx1999.top/gtrxkrbtuv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.cqqwz.cn/gtpngeboue.html

Ruby: # 无泛型
来源：http://hz.bjfxy.top/gtjtxkanxh.html


<!-- 参考信息 -->