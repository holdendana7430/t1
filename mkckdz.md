代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.zhengqikj.top/gtyzzinxvh.html

Java: (int) 'A'; (char) 65
来源：http://hz.jianghu66.top/gtbcupvwwo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.haohaochexian.top/gtqfgczprj.html

Ruby: "A".ord; 65.chr
来源：http://hz.yonumen.top/gtuekwqgxb.html

C#:   (int)'A'; (char)65
来源：http://hz.dianchejie.cn/gtjdfnfwtk.html

[A19] 交换两个变量
来源：http://hz.kuanghao11.cn/gtgtztidkd.html

Py:   a, b = b, a
来源：http://hz.snrcjt.cn/gtlygmjmlj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.ywan-chungtsiang.top/gtytxfbyml.html

JS:   [a, b] = [b, a];
来源：http://hz.hnxiangtu.top/gtamhsvgwj.html

TS:   [a, b] = [b, a];
来源：http://hz.cucudq.cn/gtvdlarrhf.html

Java: int t = a; a = b; b = t;
来源：http://hz.ydjk.org.cn/gtvntakksz.html

Go:   a, b = b, a
来源：http://hz.cheryme.top/gtjlnzxmis.html

Ruby: a, b = b, a
来源：http://hz.xinyue.icu/gtenxdxopo.html

C#:   (a, b) = (b, a);
来源：http://hz.pengpengdd.cyou/gtmkidroxr.html

[A20] 读取标准输入
来源：http://hz.zhengqikj.top/gtfllfbbej.html

Py:   name = input("请输入：")
来源：http://hz.yuxming.cn/gtswopgvza.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.jinghuilouyu.cn/gtznrdqlgx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.xuanzx.com/gtggkhoshh.html

TS:   // Node.js：readline 模块
来源：http://hz.jianghu66.top/gtinuhnuzg.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.52xcode.cn/gtdpkmdcbb.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.sweek.top/gtflwzcdxk.html

Ruby: gets.chomp
来源：http://hz.jianghu66.top/gtjtvhrdbh.html

C#:   Console.ReadLine();
来源：http://hz.sysykeji.top/gtmztmfzkc.html

[A21] 保留指定小数位输出
来源：http://hz.ybcxt.top/gtygsszhgg.html

Py:   f"{3.14159:.2f}"
来源：http://hz.svipenyu.cn/gtekduuoms.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.yonumen.top/gtqepkdame.html

JS:   (3.14159).toFixed(2)
来源：http://hz.hnqzz.top/gttjddmlcq.html

TS:   (3.14159).toFixed(2)
来源：http://hz.smart0.xyz/gtxgxkdmgx.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.nanxuanxn.top/gtvomrtwsp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.cheryme.top/gtgxsuzydb.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.bjfxy.top/gtwvblntla.html

C#:   3.14159.ToString("F2")
来源：http://hz.c1oappe.top/gtyxsxdyse.html

[A22] 获取字符串长度
来源：http://hz.nwbrower.top/gtrrexuisk.html

Py:   len(s)
来源：http://hz.daria6918.cn/gthkwtyqbh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.tanke756.top/gtpantzlep.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.tianlin.xyz/gttpypjatr.html

TS:   s.length
来源：http://hz.yanxiufei.cn/gtsxmmnwpz.html

Java: s.length()
来源：http://hz.sysykeji.top/gtsudvllwu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.yongpay.top/gthkfiebbr.html

Ruby: s.length
来源：http://hz.birdmap.top/gttkwgktzm.html

C#:   s.Length
来源：http://hz.zhongyouzk.top/gtrhfulihr.html

[A23] 大小写转换
来源：http://hz.sweek.top/gtcuwkzpnp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.redwolf501.top/gtvrmdboom.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.cdnleiting.top/gtmgdsxpbf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.sxryk.cn/gtcsqmmhpz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.hywenlv.cn/gtowawdgxy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.jyoumei.cn/gtwgzpcccn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.cashguo.top/gtettdesbt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.sweek.top/gtgubekfso.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.cqqwz.cn/gtsgouckey.html

[A24] 去除首尾空白
来源：http://hz.tian-w.cn/gtpystxvty.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.ppjwa.cn/gtbuafgrkt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.jinghuilouyu.cn/gtmwzdtczv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.xuetiantiany.cn/gtogxtszrv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jinqigfzy.top/gtmzpnlrpn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.jiagoushi.top/gtulstvmiz.html

Go:   strings.TrimSpace(s)
来源：http://hz.yongpay.top/gtztamyfyx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.hnqzz.top/gtwgbhcjgl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.birdmap.top/gtxazfrpyu.html

[A25] 字符串比较
来源：http://hz.cqqwz.cn/gttpdmxgtc.html

Py:   s1 == s2; s1 != s2
来源：http://hz.shzxlz.cn/gthdvxkqdl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.mhx1999.top/gtascuihbd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yonumen.top/gtsbrllntr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.sufxvd.cn/gtorohsomx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.gogol.net.cn/gtbatxjzwh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.xinyue.icu/gtkwgkldpk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.ydjk.org.cn/gtknlpzkoj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.iojbl.cn/gtdcfxewpg.html

[A26] 类型转换总览
来源：http://hz.yanxiufei.cn/gtvgvmygtv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.aibaodan.cn/gtjvqquzpu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.dianchejie.cn/gtzfpestek.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.gaohongyu789.top/gtvdvnmxkm.html

TS:   Number() String() Boolean() x as number
来源：http://hz.yuxming.cn/gtqmzgwyzm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.yongpay.top/gtzatlbrwq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.gotoacloud.top/gtannrodgc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.dianchejie.cn/gthxyyqbzq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.c1oappe.top/gtfbflknxy.html

================================================================================
来源：http://hz.aibaodan.cn/gtvkpuucal.html

B. 流程控制
来源：http://hz.hfpthk.cn/gtharvoxon.html

================================================================================
来源：http://hz.9152youxi.cn/gtsjbivoyq.html

[B01] 条件判断 if / else
来源：http://hz.shanyushiyangtech.top/gtgbxtvbwu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.c1oappe.top/gtdvawmyks.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.jinyuanbaomall.cn/gtzjidxoii.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.meibo888.top/gtmaxgpjsj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.haohaochexian.top/gtwnklsten.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.yongpay.top/gtidqnjmbz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.guowangkeji.top/gtndhoyzjz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.snrcjt.cn/gtfrbijwvn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.bjfxy.top/gtqhixtuqu.html

[B02] 多分支 else if / elif
来源：http://hz.sweek.top/gtuwkxvtks.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zycfv.cn/gtcuedlokc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.gzhubu.top/gtjihmwmpc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yuxming.cn/gtjliassgv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ppjwa.cn/gtrxlgenbc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yuanzhike.top/gtkpeorzsc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.xuetiantiany.cn/gtgrvlklbv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.smart0.xyz/gtvukxwsxg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hongshengwenyu.top/gtzdkxxuld.html

[B03] switch / match / case
来源：http://hz.smart0.xyz/gtvfetmhdi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.hysaishi.cn/gtqpgynhmt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.0kj1m.cn/gtdehdlxoj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.shzxlz.cn/gtaotfgmie.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jinqigfzy.top/gtgjsdunyz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.hongshengwenyu.top/gtqoezgrxh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.gzhubu.top/gteuuxuunt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.jqgfzy.top/gtwbeltekl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.xingfuxueyuan.xyz/gtquknfonu.html

[B04] for 计数循环
来源：http://hz.tian-w.cn/gtcvsdjvuk.html

Py:   for i in range(10): print(i)
来源：http://hz.zhoulong.xyz/gtljbpuuil.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.yanxiufei.cn/gtlgqwfsxy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.havefunace.top/gtsovcnhyz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.pycfn.com/gtlmhvbcib.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.svipenyu.cn/gtfjbzpque.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.daria6918.cn/gtlrkudfzw.html

Ruby: 10.times { |i| puts i }
来源：http://hz.zhijiandao.cn/gtmwbjdejg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.yj20258.top/gttuujhbsu.html

[B05] 遍历数组 / 列表
来源：http://hz.daxiang520.top/gtxnuexvxy.html

Py:   for item in arr: print(item)
来源：http://hz.hongshengwenyu.top/gtfuvszgdm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.andypj.xyz/gttkhofxaa.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.hfpthk.cn/gtgvfdmyod.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.sufxvd.cn/gtsnddwdvh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.hysaishi.cn/gtuspddezp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.hywenlv.cn/gtwtdkohls.html

Ruby: arr.each { |item| puts item }
来源：http://hz.haohaochexian.top/gtvkhmfeik.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.gzhubu.top/gtxhfbuxge.html

[B06] 遍历字典 / 对象
来源：http://hz.yangfankeji.com/gtznsdwcxx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.feifeiyinyue.top/gtskkixjvv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.jqgufenzy.top/gtdxuifqaf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hongshengwenyu.top/gtmaxbxzfm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jinqigufen.top/gtevrlixse.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.sysykeji.top/gtastumxup.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.hongshengwenyu.top/gtlupjkvgs.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jinghuilouyu.cn/gtjetzmvwz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.gzhubu.top/gtsvqbkzli.html

[B07] while 循环
来源：http://hz.9152youxi.cn/gtjqxxssqj.html

Py:   while i < 10: i += 1
来源：http://hz.jinqigfzy.top/gtiboccvqe.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yuxming.cn/gtkjxftfpt.html

JS:   while (i < 10) { i++; }
来源：http://hz.jqgufenzy.top/gtbaocqqby.html

TS:   while (i < 10) { i++; }
来源：http://hz.tanke756.top/gtobgyzeqp.html

Java: while (i < 10) { i++; }
来源：http://hz.guowangkeji.top/gtsghtxjpl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.nanxuanxn.top/gtxqddfvhc.html

Ruby: while i < 10; i += 1; end
来源：http://hz.cashguo.top/gticdlrojz.html

C#:   while (i < 10) { i++; }
来源：http://hz.snrcjt.cn/gtlxwgbjqq.html

[B08] do-while（至少执行一次）
来源：http://hz.chenjidiqi.icu/gtpaghuhuu.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.fzhhl.top/gtvnuorvmi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.jyoumei.cn/gtrgqsebqx.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jinqigufen.top/gtpecwxluc.html

TS:   do { i++; } while (i < 10);
来源：http://hz.gotoacloud.top/gtyingkeof.html

Java: do { i++; } while (i < 10);
来源：http://hz.yonumen.top/gtfdtcbkdi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.cdnleiting.top/gtapsngdja.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.jinqigufen.top/gtfbyxytsp.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jinyuanbaomall.cn/gtqcdwszxc.html

[B09] break 与 continue
来源：http://hz.tanke756.top/gtitoslife.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jinqigufen.top/gtoktcvfri.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.wangdashe.top/gtiegorjbx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xingfuxueyuan.xyz/gtqcecvuqr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cashguo.top/gtyuckrajz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yanxiufei.cn/gtwpawkjxm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.0kj1m.cn/gtrbvbdxjc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.tianlin.xyz/gtpnlijetm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ivvv.top/gtoddrfxqf.html

[B10] 遍历同时拿索引
来源：http://hz.ppjwa.cn/gtmilavpfh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.shanyushiyangtech.top/gtajpbhktw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.meibo888.top/gtxllpshqb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.shanyushiyangkeji.top/gtenqmvhnq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.birdmap.top/gtmhzekgfp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zhoulong.xyz/gtazcddcdo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yongpay.top/gteehmgfju.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.fzhhl.top/gtkygstikr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.cashguo.top/gtvzmxpthl.html

[B11] 生成数字序列 / 区间
来源：http://hz.hnxiangtu.top/gtvhvebavo.html

Py:   list(range(0, 10, 2))
来源：http://hz.cheryme.top/gttxjthart.html

PHP:  range(0, 10, 2);
来源：http://hz.zhijiandao.cn/gtwdelobkg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.mhx1999.top/gtxuccmxzc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.fzhhl.top/gttkgqkffk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yonumen.top/gtfxkwxowz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.xuetiantiany.cn/gtencvbsru.html

Ruby: (0...10).step(2).to_a
来源：http://hz.tianlin.xyz/gtprmxkwaj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jinqigfzy.top/gtkidusjwz.html

[B12] 跳出多层循环
来源：http://hz.tianlin.xyz/gtklednzcl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.gaohongyu789.top/gtnnvjrhcs.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.cqqwz.cn/gtqvtqpecj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.fzhhl.top/gthkdehheu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuanzhike.top/gtdpzrappq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuxming.cn/gtsemnkomx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.feifeiyinyue.top/gtmuueizjl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.xuanzx.com/gttwtwffku.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ybcxt.top/gtnovkvxjw.html

[B13] 判断是否为数字
来源：http://hz.zhiwuduotai.top/gtrccaryym.html

Py:   isinstance(x, (int, float))
来源：http://hz.xziqi.cn/gtcpmxpyya.html

PHP:  is_numeric($x)
来源：http://hz.zdqjudy.top/gtwnkkrvga.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sufxvd.cn/gtlhsczqre.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sweek.top/gtdxlswprf.html

Java: x instanceof Number
来源：http://hz.nanxinkj.top/gtjxcfcauc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jinghuilouyu.cn/gtxyamzqog.html

Ruby: x.is_a?(Numeric)
来源：http://hz.nwbrower.top/gtxdhgusem.html

C#:   x is int or double or decimal
来源：http://hz.zhixingplan.top/gtyluagqxu.html

[B14] 判断值是否在集合内
来源：http://hz.nanxinkj.top/gtndgxkork.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jinyuanbaomall.cn/gtonmypsxo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.gaohongyu789.top/gtwtjqhdde.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yueranfly.top/gtdgmqgajc.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.shanyushiyangkeji.top/gtvrlxprpy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jqgfzy.top/gtxzdnzvjp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.cashguo.top/gtwjhbqufl.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.tian-w.cn/gtrxdfytts.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zycfv.cn/gtnwinxzkg.html

[B15] 布尔运算与取反
来源：http://hz.yj20258.top/gttbyzbloz.html

Py:   a and b or not c
来源：http://hz.guowangkeji.top/gtkmgcshmn.html

PHP:  $a && $b || !$c
来源：http://hz.nanxinkj.top/gtjhidmkcn.html

JS:   a && b || !c
来源：http://hz.chenlongwang.top/gtchdwchqa.html

TS:   a && b || !c
来源：http://hz.jinghuilouyu.cn/gtxktrmgok.html

Java: a && b || !c
来源：http://hz.yongpay.top/gtxauhrxan.html

Go:   a && b || !c
来源：http://hz.xziqi.cn/gtomvxumcx.html

Ruby: a && b || !c
来源：http://hz.daria6918.cn/gtuywmcwlt.html

C#:   a && b || !c
来源：http://hz.dianchejie.cn/gtzwlyllha.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.c1oappe.top/gtrazphxqf.html

Py:   if not data: return
来源：http://hz.vqdsnc.cn/gtksmkttyb.html

PHP:  if (!$data) { return; }
来源：http://hz.xinyue.icu/gtntmnjoom.html

JS:   if (!data) return;
来源：http://hz.redwolf501.top/gtnncrscgm.html

TS:   if (!data) return;
来源：http://hz.pycfn.com/gtlvdwjzia.html

Java: if (data == null) return;
来源：http://hz.nwbrower.top/gtcffboloc.html

Go:   if data == nil { return }
来源：http://hz.fengsongda.top/gtkfmhpdxz.html

Ruby: return if data.nil?
来源：http://hz.aizwys.cn/gtydxvzxbh.html

C#:   if (data == null) return;
来源：http://hz.wangshuangyany.cn/gtqccedalb.html

================================================================================
来源：http://hz.ivvv.top/gtsmyrgilz.html

C. 函数与作用域
来源：http://hz.xuanzx.com/gtrxpfjljz.html

================================================================================
来源：http://hz.vqdsnc.cn/gtmfemgtve.html

[C01] 定义函数
来源：http://hz.nanxinkj.top/gtbscxszxh.html

Py:   def add(a, b): return a + b
来源：http://hz.hnqzz.top/gtlajxbiyl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.316326.xyz/gtiipbsxtu.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.tanke756.top/gtrvkdpdgd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nanxinkj.top/gtdjzhlima.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yuxming.cn/gtvmekvixw.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.vqdsnc.cn/gtzruguwtn.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hnqzz.top/gtdbqmhyfl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.andypj.xyz/gtmujvfyad.html

[C02] 默认参数
来源：http://hz.xinyue.icu/gtlpnewexl.html

Py:   def greet(name="World"): return name
来源：http://hz.zhongyouzk.top/gturtqjttw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhengqikj.top/gtcmhbbozi.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ydjk.org.cn/gtouegfxpj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yj20258888.top/gtmhvulpjx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.cheryme.top/gtfhyuqnzs.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ivvv.top/gtbvcvgchk.html

Ruby: def greet(name = "World") = name
来源：http://hz.birdmap.top/gtpmfdkstq.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.cqqwz.cn/gtrydztthl.html

[C03] 可变参数
来源：http://hz.zhoulong.xyz/gtfydhwrxd.html

Py:   def total(*args): return sum(args)
来源：http://hz.gogol.net.cn/gtrknnndxi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jyoumei.cn/gtlyacwddl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gaohongyu789.top/gthkjaozmz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.dianchejie.cn/gtnhqdgpxk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.xziqi.cn/gtdifjkpqj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xingfuxueyuan.xyz/gtgdlfpbdd.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.nwbrower.top/gtlamlfojb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.andypj.xyz/gtqugiiiyo.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhongyouzk.top/gtzlxdckzv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhengqikj.top/gtwoqzestp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.sysykeji.top/gtimuvhxnb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yj202588.top/gtukdrjuzt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yuanzhike.top/gtcfaigduu.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shanyushiyangtech.top/gtmbcxehpy.html

Go:   // 无：用配置结构体参数
来源：http://hz.c1oappe.top/gtuichyzni.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhengqikj.top/gtnknwamzc.html

C#:   f(a: 1, b: 2)
来源：http://hz.sysykeji.top/gthwmdnvqn.html

[C05] 返回多个值
来源：http://hz.birdmap.top/gtlomosrcu.html

Py:   return a, b
来源：http://hz.vqdsnc.cn/gtxijdqgrf.html

PHP:  return [$a, $b];
来源：http://hz.jinqigufen.top/gtenwaogev.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ehwqpu.com/gtxqtwkhio.html

TS:   return { a, b };
来源：http://hz.jinyuanbaomall.cn/gtstydkbuw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.vqdsnc.cn/gtmtmjbeac.html

Go:   return a, b
来源：http://hz.yanxiufei.cn/gtipebzneg.html

Ruby: return a, b
来源：http://hz.yongpay.top/gtwozjvyqc.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.gotoacloud.top/gtvmxdhvsv.html

[C06] 匿名函数 / lambda
来源：http://hz.bjfxy.top/gtpxdbkqbm.html

Py:   square = lambda x: x * x
来源：http://hz.sweek.top/gtxbufwriq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.cdnleiting.top/gtggxlyeoq.html

JS:   const square = x => x * x;
来源：http://hz.hysaishi.cn/gtrakjrpum.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.sufxvd.cn/gtryuzvxxk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.nanxinkj.top/gtemqhscff.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yj20258.top/gtchmigdyi.html

Ruby: square = ->(x) { x * x }
来源：http://hz.ydjk.org.cn/gtrnijwtks.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.tianlin.xyz/gtxwjjldek.html

[C07] 把函数作为参数传入
来源：http://hz.nanxuanxn.top/gtuigibpku.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jlsjyb.cn/gtimakghue.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.sxryk.cn/gtexlldasm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.smart0.xyz/gtstesukpx.html

TS:   arr.map(String)
来源：http://hz.shanyushiyangtech.top/gtghupqovj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.tanke756.top/gtqwxheepi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.svipenyu.cn/gtxbegysif.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhixingplan.top/gtolozfnfy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhiwuduotai.top/gtknvqcpoh.html

[C08] 闭包
来源：http://hz.shzxlz.cn/gtbkxxodsa.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yangfankeji.com/gtzcxruqib.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.tanke756.top/gtleolmmow.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cucudq.cn/gtlwvgjccu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.pengpengdd.cyou/gtanmkpqcz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ywan-chungtsiang.top/gtzhudqqhz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.iojbl.cn/gtcezcuwfo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jqgufenzy.top/gtfvtckiew.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.wangdashe.top/gtonpupelh.html

[C09] 递归
来源：http://hz.zhijiandao.cn/gtfhyuulce.html


<!-- 参考信息 -->