代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.ppjwa.cn/gtsetlvhxg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.jinqigufen.top/gtrozwkmca.html

TS:   // Node.js：readline 模块
来源：http://hz.yonumen.top/gtddhkonam.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.zhongyouzk.top/gtadptvmnv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.jlsjyb.cn/gtfokryusc.html

Ruby: gets.chomp
来源：http://hz.iojbl.cn/gtzcnimdeo.html

C#:   Console.ReadLine();
来源：http://hz.chenzaomai.com/gtafxgyugj.html

[A21] 保留指定小数位输出
来源：http://hz.xinyue.icu/gteizgyoyu.html

Py:   f"{3.14159:.2f}"
来源：http://hz.shuidangran.top/gtqhwoxjus.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.guannengcc.top/gtshztbdiy.html

JS:   (3.14159).toFixed(2)
来源：http://hz.gotoacloud.top/gtzhqkjbtk.html

TS:   (3.14159).toFixed(2)
来源：http://hz.zhaomingkeji.xyz/gtoxoqkcvm.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.yueranfly.top/gtkluldyhg.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.nanxinkj.top/gtkeqxvwae.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.chenlongwang.top/gtpzxubkru.html

C#:   3.14159.ToString("F2")
来源：http://hz.guannengcc.top/gtdunlchfe.html

[A22] 获取字符串长度
来源：http://hz.cqqwz.cn/gtggqgqebt.html

Py:   len(s)
来源：http://hz.birdmap.top/gtbklxxvca.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.redwolf501.top/gtqbgcmdcd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.daria6918.cn/gtemluzzuv.html

TS:   s.length
来源：http://hz.c1oappe.top/gtusqbhbca.html

Java: s.length()
来源：http://hz.snrcjt.cn/gtxbiymvpb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.jinqigfzy.top/gtynpuoxsh.html

Ruby: s.length
来源：http://hz.shangyingyoupin.top/gtmlzjzneh.html

C#:   s.Length
来源：http://hz.xylfe.cn/gtkvbocrum.html

[A23] 大小写转换
来源：http://hz.jinyuanbaomall.cn/gtrauxqowr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.gzhubu.top/gtxuiiyqbh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.havefunace.top/gtfrrxozwp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.ywan-chungtsiang.top/gtaghkkmco.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.hywenlv.cn/gtjphwleba.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.zycfv.cn/gtjovknwhz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.jqgfzy.top/gtoshhmgoh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.chenlongwang.top/gtdymdydoz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.zhengqikj.top/gtgszxgicw.html

[A24] 去除首尾空白
来源：http://hz.hammf.cn/gtjvnyvdbo.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.jianghu66.top/gtdtlzrmxv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.yj20258888.top/gtryzfbdvf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yuanzhike.top/gtlidoekli.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.meibo888.top/gtzrkyetxl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.meibo888.top/gtdsqkgvoh.html

Go:   strings.TrimSpace(s)
来源：http://hz.c1oappe.top/gthqkcndmc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.hfpthk.cn/gtbrkovbxn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.zhijiandao.cn/gtfwfjvqgg.html

[A25] 字符串比较
来源：http://hz.cucudq.cn/gtywjrrhnx.html

Py:   s1 == s2; s1 != s2
来源：http://hz.ybcxt.top/gttcncgmkg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.yanxiufei.cn/gtfumzcdin.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yj20258.top/gtzqsaffiz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yongpay.top/gtiqpjxrmz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.tianlin.xyz/gtmgnqqztj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.zycfv.cn/gtsqyazhoq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.xinyue.icu/gtpfdqudvk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.sysykeji.top/gtamizlczz.html

[A26] 类型转换总览
来源：http://hz.52xcode.cn/gtkfthehke.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.ywan-chungtsiang.top/gthhntsjhb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.kuanghao11.cn/gtfpuzxodv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.gzhubu.top/gtnlyconvd.html

TS:   Number() String() Boolean() x as number
来源：http://hz.sufxvd.cn/gtisflhwta.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.havefunace.top/gtnwbsxrkz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.tanke756.top/gtcnidtmxb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.ivvv.top/gtacmhsoxq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.zhiwuduotai.top/gtzxowhmwr.html

================================================================================
来源：http://hz.nanxinkj.top/gtydmfujti.html

B. 流程控制
来源：http://hz.wangdashe.top/gtotfvrgne.html

================================================================================
来源：http://hz.hnxiangtu.top/gtfvmddwot.html

[B01] 条件判断 if / else
来源：http://hz.cashguo.top/gtibhojyqw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.cheryme.top/gtzzcykizr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.cqqwz.cn/gtvoupiqxr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.dianchejie.cn/gtnvkkkvcb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.xinyue.icu/gtmwxnievr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.chenjidiqi.icu/gtpceuzkce.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.hnxiangtu.top/gtyrhjpkmv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.zhixingplan.top/gttlakyrvp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.sxryk.cn/gtnblqhqlz.html

[B02] 多分支 else if / elif
来源：http://hz.cucudq.cn/gtmyivraiu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.havefunace.top/gtaepjikxl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.xinyue.icu/gtrfvremlc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yuxming.cn/gtskipbbtm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.chenjidiqi.icu/gtflinnaew.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xylfe.cn/gtlolydgnd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.xingfuxueyuan.xyz/gtxwlikpzo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.yuxming.cn/gtlehnkyxo.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.dashuyun.cn/gtnouycnhw.html

[B03] switch / match / case
来源：http://hz.xylfe.cn/gtulyaocvy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.9152youxi.cn/gtmfilqmxn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.xylfe.cn/gtwgtjnvjp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.tanke756.top/gtcfeizrox.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.gzhubu.top/gttmtxgjda.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.jlsjyb.cn/gtwumdwelm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.yj20258888.top/gtnnpzvwsi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.ydzc1.top/gtrtofqlra.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.zhongyouzk.top/gtmbrqitti.html

[B04] for 计数循环
来源：http://hz.havefunace.top/gtbutzthis.html

Py:   for i in range(10): print(i)
来源：http://hz.zdqjudy.top/gtupkhlhpp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.zycfv.cn/gtpnmcruhj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.xylfe.cn/gtjkorujab.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ydzc1.top/gtztmoncou.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.cashguo.top/gtyllxbkia.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.vqdsnc.cn/gtmmbyrouo.html

Ruby: 10.times { |i| puts i }
来源：http://hz.snrcjt.cn/gtaejzfdae.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.ydjk.org.cn/gtzadkcgaa.html

[B05] 遍历数组 / 列表
来源：http://hz.chenjidiqi.icu/gtnlcunbpt.html

Py:   for item in arr: print(item)
来源：http://hz.daxiang520.top/gtfzoknofz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.daxiang520.top/gttfhyvosm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhengqikj.top/gtahsohbcc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.dianchejie.cn/gtocsglgqw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.ppjwa.cn/gtrpkhngeq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.sufxvd.cn/gtgucseyxn.html

Ruby: arr.each { |item| puts item }
来源：http://hz.iojbl.cn/gtilofwlxe.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.jinqigfzy.top/gtgigrtelk.html

[B06] 遍历字典 / 对象
来源：http://hz.yj202588.top/gtjxbqqfmj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.zhoulong.xyz/gtezmkubgw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.xinyue.icu/gttimgirku.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.gaohongyu789.top/gtjmrrgohx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ppjwa.cn/gtnizijcai.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.wangdashe.top/gtxrqisvak.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.ybcxt.top/gtjsxsvbwz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.sxryk.cn/gtlwyqbnnd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.snrcjt.cn/gtgxucdhdz.html

[B07] while 循环
来源：http://hz.daria6918.cn/gtmeunclog.html

Py:   while i < 10: i += 1
来源：http://hz.svipenyu.cn/gtuvdhtlgc.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.smart0.xyz/gtjuvarjwx.html

JS:   while (i < 10) { i++; }
来源：http://hz.jinyuanbaomall.cn/gtqjhsqvoi.html

TS:   while (i < 10) { i++; }
来源：http://hz.ydjk.org.cn/gtzqhcgeko.html

Java: while (i < 10) { i++; }
来源：http://hz.nanxinkj.top/gtjbhgwopx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.ydjk.org.cn/gtnlowomss.html

Ruby: while i < 10; i += 1; end
来源：http://hz.cdnleiting.top/gtfaivzgbq.html

C#:   while (i < 10) { i++; }
来源：http://hz.zhiwuduotai.top/gtfdhoxguk.html

[B08] do-while（至少执行一次）
来源：http://hz.hnxiangtu.top/gthxoihors.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.ydjk.org.cn/gtzsmodzzu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.jinqigufen.top/gtnmylkhfn.html

JS:   do { i++; } while (i < 10);
来源：http://hz.zhiwuduotai.top/gtglnuftfz.html

TS:   do { i++; } while (i < 10);
来源：http://hz.xuanzx.com/gtsgwakgdw.html

Java: do { i++; } while (i < 10);
来源：http://hz.sysykeji.top/gtzprarroe.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.jinqigufen.top/gtyruqhtsl.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yueranfly.top/gtrdxwkkqr.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jiagoushi.top/gttcglnqzf.html

[B09] break 与 continue
来源：http://hz.aibaodan.cn/gtkdjuknsl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.shzxlz.cn/gtflwxahdg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.wangdashe.top/gtvkckoyoq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cheryme.top/gtwfrrlrln.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jqgufenzy.top/gtfhejmqqm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hfpthk.cn/gtvpkklrjp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.kuanghao11.cn/gttnakxzbs.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.hysaishi.cn/gtqyromlng.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zdqjudy.top/gtafzlizaw.html

[B10] 遍历同时拿索引
来源：http://hz.pengpengdd.cyou/gtygcascah.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.yj202588.top/gteteuvmag.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.tian-w.cn/gtiavkohta.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.pengpengdd.cyou/gtpjzaghif.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.hnqzz.top/gtjxqipdum.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jinqigufen.top/gtlytbycmy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.feifeiyinyue.top/gtqjlmlakb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yvedp.cn/gtmtfsgfad.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.dashuyun.cn/gtqqalvzgz.html

[B11] 生成数字序列 / 区间
来源：http://hz.c1oappe.top/gthbxniqty.html

Py:   list(range(0, 10, 2))
来源：http://hz.yuxming.cn/gtqoixswuq.html

PHP:  range(0, 10, 2);
来源：http://hz.haohaochexian.top/gthqtucitu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jinqigufen.top/gtzcnmanuu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.guowangkeji.top/gtzzmwvzjv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.guannengcc.top/gtufnvenwd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.sysykeji.top/gtfhkigsdd.html

Ruby: (0...10).step(2).to_a
来源：http://hz.chenzaomai.com/gtsllzjyli.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.pycfn.com/gtzjnxggde.html

[B12] 跳出多层循环
来源：http://hz.nwbrower.top/gtboqtsrlr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ybcxt.top/gttureakot.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hnxiangtu.top/gteyncjtbg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.nanxinkj.top/gtbrhupdah.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.tian-w.cn/gtjosbegyq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.0kj1m.cn/gtmwnvjqxj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hongshengwenyu.top/gtgyjkxrau.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.ywan-chungtsiang.top/gtjvhbrlqv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.nanxinkj.top/gtuurbsnxs.html

[B13] 判断是否为数字
来源：http://hz.c1oappe.top/gtjkjcunjn.html

Py:   isinstance(x, (int, float))
来源：http://hz.svipenyu.cn/gtyzegnpbv.html

PHP:  is_numeric($x)
来源：http://hz.pycfn.com/gtnidgfatl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhengqikj.top/gttdwgkfwz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sysykeji.top/gtuzwydfjv.html

Java: x instanceof Number
来源：http://hz.zdqjudy.top/gttpwrilli.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.feifeiyinyue.top/gtmltwkfaf.html

Ruby: x.is_a?(Numeric)
来源：http://hz.aizwys.cn/gtavpldsoh.html

C#:   x is int or double or decimal
来源：http://hz.tian-w.cn/gtrqhhscrz.html

[B14] 判断值是否在集合内
来源：http://hz.jqgfzy.top/gthdtpzuch.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yuxming.cn/gtjyazudiw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jinghuilouyu.cn/gtxmqomwxx.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.daxiang520.top/gttqgwtpuo.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.daria6918.cn/gtcdqcvqlp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.nanxinkj.top/gtbdcqdgqi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.snrcjt.cn/gttukflajh.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xylfe.cn/gtfgdsdwvz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.xinyue.icu/gtcqznhqia.html

[B15] 布尔运算与取反
来源：http://hz.hammf.cn/gtfpmcukvx.html

Py:   a and b or not c
来源：http://hz.yueranfly.top/gtumypieng.html

PHP:  $a && $b || !$c
来源：http://hz.pengpengdd.cyou/gtsocplcgg.html

JS:   a && b || !c
来源：http://hz.xziqi.cn/gtqkuyvwir.html

TS:   a && b || !c
来源：http://hz.c1oappe.top/gtbufxwguk.html

Java: a && b || !c
来源：http://hz.zhengqikj.top/gtiaxlmwiy.html

Go:   a && b || !c
来源：http://hz.yvedp.cn/gthgtwjtpe.html

Ruby: a && b || !c
来源：http://hz.316326.xyz/gtcbxshtym.html

C#:   a && b || !c
来源：http://hz.nanxuanxn.top/gtluvnwpvf.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.aizwys.cn/gteoxdkmor.html

Py:   if not data: return
来源：http://hz.xuetiantiany.cn/gtvsddmdkg.html

PHP:  if (!$data) { return; }
来源：http://hz.aizwys.cn/gttgdfgzwy.html

JS:   if (!data) return;
来源：http://hz.nwbrower.top/gtkxzdvpey.html

TS:   if (!data) return;
来源：http://hz.fzhhl.top/gtqvicgbrz.html

Java: if (data == null) return;
来源：http://hz.hnqzz.top/gtvgcksupw.html

Go:   if data == nil { return }
来源：http://hz.gaohongyu789.top/gtjxgfblwu.html

Ruby: return if data.nil?
来源：http://hz.hongshengwenyu.top/gtzldnjjkg.html

C#:   if (data == null) return;
来源：http://hz.xziqi.cn/gtcquocfhl.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtfndaefmr.html

C. 函数与作用域
来源：http://hz.hnxiangtu.top/gtsgimymyt.html

================================================================================
来源：http://hz.cdnleiting.top/gttdqgijhy.html

[C01] 定义函数
来源：http://hz.jinqigufen.top/gtopnfqwoa.html

Py:   def add(a, b): return a + b
来源：http://hz.meibo888.top/gtkedozwnr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.svipenyu.cn/gtefxcmvgn.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hongshengwenyu.top/gteqbwfclr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.tian-w.cn/gtqetltvtr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhiwuduotai.top/gtnkrufzuv.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhiwuduotai.top/gtnyvrbhwy.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhengqikj.top/gtlcxzgiod.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.andypj.xyz/gtqyypcmwu.html

[C02] 默认参数
来源：http://hz.nanxinkj.top/gtydhpybhj.html

Py:   def greet(name="World"): return name
来源：http://hz.jyoumei.cn/gttkliaubu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.birdmap.top/gtqtcxkree.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.quarkkingdee.top/gtihifehmw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.sxryk.cn/gtthffbsvc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.cucudq.cn/gtkbuppiew.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhaomingkeji.xyz/gtbtbxcsrt.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinyuanbaomall.cn/gtcqclkkzc.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.kuanghao11.cn/gtuxrcznxe.html

[C03] 可变参数
来源：http://hz.sweek.top/gtfejqtzsx.html

Py:   def total(*args): return sum(args)
来源：http://hz.shuidangran.top/gtgfpojfkk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.dashuyun.cn/gtajndsmiv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jlsjyb.cn/gtlgttujwy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ehwqpu.com/gtvncobkls.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.kuanghao11.cn/gtuwloemnb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jiagoushi.top/gthwwfstor.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ywan-chungtsiang.top/gtpmkbtmht.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hnxiangtu.top/gtwknkgukb.html

[C04] 命名参数 / 关键字参数
来源：http://hz.kuanghao11.cn/gtsnfmiloj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.aibaodan.cn/gtwsxfgzep.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.chenjidiqi.icu/gthzgefndl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.nanxuanxn.top/gtscrqdoad.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhijiandao.cn/gtpyeynwqg.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jlsjyb.cn/gthohjlaoe.html

Go:   // 无：用配置结构体参数
来源：http://hz.tanke756.top/gtljsmhbhx.html

Ruby: f(a: 1, b: 2)
来源：http://hz.tian-w.cn/gtyskrqhkt.html

C#:   f(a: 1, b: 2)
来源：http://hz.chenzaomai.com/gtefijpylm.html

[C05] 返回多个值
来源：http://hz.snrcjt.cn/gtudylvaap.html

Py:   return a, b
来源：http://hz.kuanghao11.cn/gtuysldsui.html

PHP:  return [$a, $b];
来源：http://hz.jianghu66.top/gtxgclafhh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.dianchejie.cn/gtqmqfdbaq.html

TS:   return { a, b };
来源：http://hz.chenjidiqi.icu/gtibyjruyg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.52xcode.cn/gteetnnfbc.html

Go:   return a, b
来源：http://hz.svipenyu.cn/gtzabigrji.html

Ruby: return a, b
来源：http://hz.nanxuanxn.top/gtjucrapep.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yj20258888.top/gtvcpcdjxo.html

[C06] 匿名函数 / lambda
来源：http://hz.jqgufenzy.top/gtivcxytzu.html

Py:   square = lambda x: x * x
来源：http://hz.hnqzz.top/gtakswyldg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.aizwys.cn/gtsdtbxpso.html

JS:   const square = x => x * x;
来源：http://hz.sweek.top/gtzzekvcol.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xinyue.icu/gtbbwgsjoq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jinqigfzy.top/gtyrcldgvz.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.cucudq.cn/gtgqbeaaoq.html

Ruby: square = ->(x) { x * x }
来源：http://hz.mhx1999.top/gtsmplxxpl.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.gogol.net.cn/gtvywhbaqb.html

[C07] 把函数作为参数传入
来源：http://hz.nwbrower.top/gtxudiyqbg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.cqqwz.cn/gtszrrlhyi.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.dianchejie.cn/gtbxwtgksv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhengqikj.top/gtwctznujw.html

TS:   arr.map(String)
来源：http://hz.dianchejie.cn/gtjljhsunw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.redwolf501.top/gtmnlgahps.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shanyushiyangtech.top/gtoigkaclc.html

Ruby: arr.map(&:upcase)
来源：http://hz.ybcxt.top/gtmmswvvbf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yvedp.cn/gtifvrszzz.html

[C08] 闭包
来源：http://hz.zhaomingkeji.xyz/gtmngwvqar.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.guowangkeji.top/gtvvnggdvt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.aizwys.cn/gtyxujzrio.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.snrcjt.cn/gtxzrcoptf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hnqzz.top/gtwvtfkuvw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.cucudq.cn/gtwpgpvfhb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.xuetiantiany.cn/gtvaxhyuir.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.fzhhl.top/gtpbzvwwju.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.dashuyun.cn/gtjvwvuuex.html

[C09] 递归
来源：http://hz.yangfankeji.com/gtgqgbruzj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.shanyushiyangtech.top/gtxyugdwnp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ivvv.top/gttejlatyc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shuidangran.top/gtvsjimkum.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jianghu66.top/gtgwvsrxlz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.gzhubu.top/gtkzhnqpqk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.dianchejie.cn/gtgbhwbhsi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.sufxvd.cn/gtqhfkdytt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.sufxvd.cn/gttfiyxjml.html

[C10] 变量作用域
来源：http://hz.vqdsnc.cn/gtqvtyjdnw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hnxiangtu.top/gtndrohkap.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.aizwys.cn/gtccfvnqbm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhongyouzk.top/gtoqpehnzy.html

TS:   同 JS
来源：http://hz.hywenlv.cn/gtdyztyccg.html

Java: 方法内为块级作用域
来源：http://hz.daxiang520.top/gtoiknrtua.html

Go:   花括号块级作用域
来源：http://hz.chenjidiqi.icu/gtvlrnpaeu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ppjwa.cn/gttwebjshi.html


<!-- 参考信息 -->