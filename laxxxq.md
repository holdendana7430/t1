代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.gogol.net.cn/gtxjaegmxs.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.zhaomingkeji.xyz/gtenqugpyg.html

TS:   // Node.js：readline 模块
来源：http://hz.9152youxi.cn/gtybofjeup.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.nanxuanxn.top/gtfcaotcot.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.vqdsnc.cn/gtmzrsdghn.html

Ruby: gets.chomp
来源：http://hz.guannengcc.top/gttzozcnhw.html

C#:   Console.ReadLine();
来源：http://hz.yanxiufei.cn/gtbexcqirc.html

[A21] 保留指定小数位输出
来源：http://hz.tian-w.cn/gtgtiahqht.html

Py:   f"{3.14159:.2f}"
来源：http://hz.ydjk.org.cn/gtvbavwhls.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.cdnleiting.top/gtslompniq.html

JS:   (3.14159).toFixed(2)
来源：http://hz.sysykeji.top/gtrmsggtjx.html

TS:   (3.14159).toFixed(2)
来源：http://hz.haohaochexian.top/gtorqfawyz.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.hysaishi.cn/gtincnjnus.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.zhijiandao.cn/gttsjybmgv.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.sysykeji.top/gtsseyzhtb.html

C#:   3.14159.ToString("F2")
来源：http://hz.hysaishi.cn/gtwljqefpy.html

[A22] 获取字符串长度
来源：http://hz.tianlin.xyz/gtrcpvtcwk.html

Py:   len(s)
来源：http://hz.316326.xyz/gthhjbqwuv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.pycfn.com/gtjvwjxrcw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.ivvv.top/gtszagfsov.html

TS:   s.length
来源：http://hz.zhengqikj.top/gtofoqtaqq.html

Java: s.length()
来源：http://hz.shzxlz.cn/gthvddfofc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.gzhubu.top/gtlethyhyn.html

Ruby: s.length
来源：http://hz.haohaochexian.top/gtelhrtexi.html

C#:   s.Length
来源：http://hz.shzxlz.cn/gtmonlhhom.html

[A23] 大小写转换
来源：http://hz.shuidangran.top/gtlahkbrtx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.zhongyouzk.top/gtyospzqti.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.yj20258888.top/gtvbljdjgs.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.sufxvd.cn/gtydwaqvoq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.xziqi.cn/gtdavjxkiy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.zhiwuduotai.top/gtldcladaf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.gzhubu.top/gtcongfoqh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.sweek.top/gtohlmmsbz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.redwolf501.top/gtlikluicw.html

[A24] 去除首尾空白
来源：http://hz.hnqzz.top/gtylhbakan.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.jqgfzy.top/gtnvzugwue.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.jinqigfzy.top/gtgjaldqpb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yueranfly.top/gtkksdwwnf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.316326.xyz/gtdembdbdo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.pengpengdd.cyou/gtcycwzkjj.html

Go:   strings.TrimSpace(s)
来源：http://hz.chenjidiqi.icu/gtssfeirlp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.yj20258.top/gtaddcbtxi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.jinqigufen.top/gtpipfufix.html

[A25] 字符串比较
来源：http://hz.hfpthk.cn/gtcsbxgwdp.html

Py:   s1 == s2; s1 != s2
来源：http://hz.hnxiangtu.top/gtzaaweamg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.ydzc1.top/gtzlrlsvwx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.ybcxt.top/gtgkrljhdd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.cheryme.top/gtmcdeecbk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.aibaodan.cn/gtotzjzusx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.jyoumei.cn/gtlikcywdd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.hfpthk.cn/gttdehcvqm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.ydzc1.top/gtaekfuydk.html

[A26] 类型转换总览
来源：http://hz.hnxiangtu.top/gtoxnuabpe.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.jyoumei.cn/gtscxywytc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.jianghu66.top/gtuoshdeem.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.jinqigufen.top/gtvfptfahw.html

TS:   Number() String() Boolean() x as number
来源：http://hz.guowangkeji.top/gtkazgcarr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.316326.xyz/gtkzkutzda.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.ivvv.top/gttoqljyxi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.jinyuanbaomall.cn/gtusutqvwv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.zhixingplan.top/gtahwrflwa.html

================================================================================
来源：http://hz.zhengqikj.top/gtcpwvqxjr.html

B. 流程控制
来源：http://hz.cucudq.cn/gtofupjdfo.html

================================================================================
来源：http://hz.shzxlz.cn/gthxozenif.html

[B01] 条件判断 if / else
来源：http://hz.pycfn.com/gtosshbpyu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.feifeiyinyue.top/gtcjahwrir.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.guannengcc.top/gthsgfbxuu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.tanke756.top/gtzzcuocvv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.vqdsnc.cn/gthedupxan.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.hfpthk.cn/gtjfewdtfd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.hammf.cn/gtlinosqmg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.zhongyouzk.top/gtzuqtznnu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.gotoacloud.top/gtaugwwrer.html

[B02] 多分支 else if / elif
来源：http://hz.cdnleiting.top/gtioheywgy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.dianchejie.cn/gtvhoiyppr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.gzhubu.top/gtdbpttpao.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.andypj.xyz/gtldqeuplz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shuidangran.top/gtwzxvynvh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jlsjyb.cn/gtldnvcedo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.zhengqikj.top/gtxdaiyfyy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.xuetiantiany.cn/gtfcwzcima.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhiwuduotai.top/gtuewybjry.html

[B03] switch / match / case
来源：http://hz.jqgufenzy.top/gtfvtfxgqy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.kuanghao11.cn/gtaycwmwsm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.ybcxt.top/gtehdknbyu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.iojbl.cn/gtjuwedjcw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.bjfxy.top/gthftztxfx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.yj20258.top/gtrsushqxv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.hnqzz.top/gtwnytpkcn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.kuanghao11.cn/gtgbypname.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.bjfxy.top/gtbnoacsyx.html

[B04] for 计数循环
来源：http://hz.zhoulong.xyz/gtbqjuahod.html

Py:   for i in range(10): print(i)
来源：http://hz.fengsongda.top/gttgnfvrxd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.meibo888.top/gtepafzkzt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yueranfly.top/gtwekfczqs.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.meibo888.top/gtnhenrahq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.mhx1999.top/gtzhytazux.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.zhoulong.xyz/gtosiyvgmo.html

Ruby: 10.times { |i| puts i }
来源：http://hz.shzxlz.cn/gtieuxatng.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.guannengcc.top/gtftswbuop.html

[B05] 遍历数组 / 列表
来源：http://hz.zhaomingkeji.xyz/gtpzvowrij.html

Py:   for item in arr: print(item)
来源：http://hz.zdqjudy.top/gtaxrocntc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.sxryk.cn/gtiagdfhta.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.gaohongyu789.top/gtuolkrwus.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yj202588.top/gtqizthmdl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.zhijiandao.cn/gtgzggdwgz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.ivvv.top/gtmskwfgon.html

Ruby: arr.each { |item| puts item }
来源：http://hz.tian-w.cn/gtbdmdjeuh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.hnxiangtu.top/gtsqvbazqg.html

[B06] 遍历字典 / 对象
来源：http://hz.0kj1m.cn/gtvmqajmfa.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.nwbrower.top/gtcpedmnjv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.vqdsnc.cn/gtwnxkewxu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.feifeiyinyue.top/gtfcapfzok.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yanxiufei.cn/gtywhxybkr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.sysykeji.top/gtsizstezs.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.zhiwuduotai.top/gtqglxmzwi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.yvedp.cn/gtkobprsek.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.ydzc1.top/gtsoeiearu.html

[B07] while 循环
来源：http://hz.yangfankeji.com/gtowdzoywj.html

Py:   while i < 10: i += 1
来源：http://hz.shzxlz.cn/gtjuqjboww.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.zhijiandao.cn/gtttuohivn.html

JS:   while (i < 10) { i++; }
来源：http://hz.tanke756.top/gthohtpuhc.html

TS:   while (i < 10) { i++; }
来源：http://hz.yanxiufei.cn/gtelmhnics.html

Java: while (i < 10) { i++; }
来源：http://hz.meibo888.top/gtamenmeqy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yanxiufei.cn/gtmcmeswwe.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jlsjyb.cn/gtkjwetruf.html

C#:   while (i < 10) { i++; }
来源：http://hz.gaohongyu789.top/gtdmtawlgt.html

[B08] do-while（至少执行一次）
来源：http://hz.havefunace.top/gtbcybvwmp.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.gotoacloud.top/gtipnhtvbx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.fzhhl.top/gtxfkfgaeg.html

JS:   do { i++; } while (i < 10);
来源：http://hz.sweek.top/gtwejrbdik.html

TS:   do { i++; } while (i < 10);
来源：http://hz.bjfxy.top/gtpnibkmid.html

Java: do { i++; } while (i < 10);
来源：http://hz.meibo888.top/gtomhozvxf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.kuanghao11.cn/gtyguaeqnz.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hnxiangtu.top/gtfrcjerhw.html

C#:   do { i++; } while (i < 10);
来源：http://hz.guowangkeji.top/gtkhaqgfje.html

[B09] break 与 continue
来源：http://hz.chenlongwang.top/gtcxgkoemi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.hnqzz.top/gtamrnhywk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yanxiufei.cn/gtpvgjyfxz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinqigfzy.top/gtnegavxsw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.havefunace.top/gtcbsxekkv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhongyouzk.top/gtcquagemn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zhijiandao.cn/gtlweynres.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.zhijiandao.cn/gtzmasljth.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenzaomai.com/gtlnwjjoku.html

[B10] 遍历同时拿索引
来源：http://hz.jinqigufen.top/gtrzwdzzbw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.chenzaomai.com/gtuhssbukc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.aizwys.cn/gtxoeapkxh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jinyuanbaomall.cn/gtrzybremc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.smart0.xyz/gtfqbienlo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zycfv.cn/gtzhwlgpml.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yvedp.cn/gtrvgyirfi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.chenzaomai.com/gtjilyvilv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jianghu66.top/gtigvruhed.html

[B11] 生成数字序列 / 区间
来源：http://hz.daria6918.cn/gtoapieafk.html

Py:   list(range(0, 10, 2))
来源：http://hz.daria6918.cn/gtlcplmxnv.html

PHP:  range(0, 10, 2);
来源：http://hz.yanxiufei.cn/gtrrdlrnhl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gaohongyu789.top/gtgwoonjij.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.chenzaomai.com/gtercrfizr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yj20258888.top/gtrnsjidwr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.birdmap.top/gtrhfzohlr.html

Ruby: (0...10).step(2).to_a
来源：http://hz.daria6918.cn/gtmumxrpbx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.hongshengwenyu.top/gtbwshgxgb.html

[B12] 跳出多层循环
来源：http://hz.0kj1m.cn/gtgucfwnpm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.tanke756.top/gtkvnlfihd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.xinyue.icu/gtrrwqaeko.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.andypj.xyz/gtznxvswlr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ywan-chungtsiang.top/gtofeuoclg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.9152youxi.cn/gtltmwbisc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.chenlongwang.top/gtubmfvgvh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.0kj1m.cn/gtqywmghic.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ydzc1.top/gtrnlevtfb.html

[B13] 判断是否为数字
来源：http://hz.nanxuanxn.top/gtrxeifnpm.html

Py:   isinstance(x, (int, float))
来源：http://hz.jlsjyb.cn/gtnjynatcy.html

PHP:  is_numeric($x)
来源：http://hz.aibaodan.cn/gtppntpuaj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yj20258.top/gtjrwowfly.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.nwbrower.top/gtplabpcxb.html

Java: x instanceof Number
来源：http://hz.c1oappe.top/gtpazigdxv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.snrcjt.cn/gtstkjasuv.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jiagoushi.top/gtzbwzntbk.html

C#:   x is int or double or decimal
来源：http://hz.tianlin.xyz/gtzoumgdge.html

[B14] 判断值是否在集合内
来源：http://hz.zycfv.cn/gtlebstaeu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhiwuduotai.top/gtpuzzfwkd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.kuanghao11.cn/gtgwxmewar.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.birdmap.top/gtjwzgksaf.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yuanzhike.top/gtkxyriowz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yuxming.cn/gtcabjtnwz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hysaishi.cn/gtveitpaxs.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.haohaochexian.top/gtsqkthvzn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.chenlongwang.top/gtaehgudjv.html

[B15] 布尔运算与取反
来源：http://hz.yanxiufei.cn/gtxjrkvthy.html

Py:   a and b or not c
来源：http://hz.yongpay.top/gtrradnvzs.html

PHP:  $a && $b || !$c
来源：http://hz.zycfv.cn/gtzjebljqr.html

JS:   a && b || !c
来源：http://hz.xinyue.icu/gtrfgzsvlr.html

TS:   a && b || !c
来源：http://hz.jianghu66.top/gtpvcyupki.html

Java: a && b || !c
来源：http://hz.dianchejie.cn/gtlipjbeaa.html

Go:   a && b || !c
来源：http://hz.svipenyu.cn/gtkvfasxji.html

Ruby: a && b || !c
来源：http://hz.gaohongyu789.top/gtuxbmnheq.html

C#:   a && b || !c
来源：http://hz.chenjidiqi.icu/gtckfayamg.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ivvv.top/gtswrzovne.html

Py:   if not data: return
来源：http://hz.xylfe.cn/gtpnhkdwjw.html

PHP:  if (!$data) { return; }
来源：http://hz.sysykeji.top/gtwajwiyoc.html

JS:   if (!data) return;
来源：http://hz.kuanghao11.cn/gtjuxeuhrb.html

TS:   if (!data) return;
来源：http://hz.meibo888.top/gtofciusjj.html

Java: if (data == null) return;
来源：http://hz.svipenyu.cn/gtsyebyros.html

Go:   if data == nil { return }
来源：http://hz.iojbl.cn/gtotllrosq.html

Ruby: return if data.nil?
来源：http://hz.hywenlv.cn/gtohdanblc.html

C#:   if (data == null) return;
来源：http://hz.xuetiantiany.cn/gtmyfqevge.html

================================================================================
来源：http://hz.zhoulong.xyz/gtjxlnblnm.html

C. 函数与作用域
来源：http://hz.andypj.xyz/gthibscnlw.html

================================================================================
来源：http://hz.chenlongwang.top/gtrljxhtlc.html

[C01] 定义函数
来源：http://hz.hysaishi.cn/gtdsdjputn.html

Py:   def add(a, b): return a + b
来源：http://hz.nanxuanxn.top/gtoahlsopj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xuetiantiany.cn/gtdoyrmmfw.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhijiandao.cn/gtscuikcqy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.wangdashe.top/gtmjtybwio.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xuanzx.com/gtyqukqphy.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.wangshuangyany.cn/gtxetiojzy.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hongshengwenyu.top/gtxjplxhir.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.daria6918.cn/gtrygrldwq.html

[C02] 默认参数
来源：http://hz.shzxlz.cn/gtfmqqrvtt.html

Py:   def greet(name="World"): return name
来源：http://hz.xylfe.cn/gtzthmqaqm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hfpthk.cn/gtnyvlghnq.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.fzhhl.top/gtxfwtmrxf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.vqdsnc.cn/gtcwrtkxea.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ydzc1.top/gtrpnxjhbo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhiwuduotai.top/gtaumlhsqp.html

Ruby: def greet(name = "World") = name
来源：http://hz.hfpthk.cn/gtcckpiycx.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.haohaochexian.top/gtdlkhfwfi.html

[C03] 可变参数
来源：http://hz.yuxming.cn/gtwvpxtwqr.html

Py:   def total(*args): return sum(args)
来源：http://hz.iojbl.cn/gtqrutpwac.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.dashuyun.cn/gtprgkckhv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.vqdsnc.cn/gtbrpvkllh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hnxiangtu.top/gtamcksjzj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.haohaochexian.top/gtqaxdpsan.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hysaishi.cn/gtosyfnmgm.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.316326.xyz/gtodkwvsln.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhijiandao.cn/gtsfukkbze.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yuxming.cn/gtyywfvnth.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.quarkkingdee.top/gtpixvcued.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.9152youxi.cn/gtbdlesauv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jyoumei.cn/gtkiwohdyk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.kuanghao11.cn/gtujcmjnph.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.52xcode.cn/gtykmohtba.html

Go:   // 无：用配置结构体参数
来源：http://hz.snrcjt.cn/gtkpbbpfqh.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hnqzz.top/gtetzqvgrn.html

C#:   f(a: 1, b: 2)
来源：http://hz.ydjk.org.cn/gtyhwwfwkz.html

[C05] 返回多个值
来源：http://hz.pycfn.com/gtzchjhmjk.html

Py:   return a, b
来源：http://hz.svipenyu.cn/gtirjivvuh.html

PHP:  return [$a, $b];
来源：http://hz.jianghu66.top/gtgcdopzyo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jiagoushi.top/gtoihwvmgo.html

TS:   return { a, b };
来源：http://hz.shanyushiyangtech.top/gtqlscuihq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xuetiantiany.cn/gtchlcjjxn.html

Go:   return a, b
来源：http://hz.xingfuxueyuan.xyz/gtbmmwuohz.html

Ruby: return a, b
来源：http://hz.gogol.net.cn/gtjlikvika.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhongyouzk.top/gtlylvurgd.html

[C06] 匿名函数 / lambda
来源：http://hz.wangdashe.top/gtxxxbsbfz.html

Py:   square = lambda x: x * x
来源：http://hz.bjfxy.top/gtjlhmhrqy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.pengpengdd.cyou/gtyozooawu.html

JS:   const square = x => x * x;
来源：http://hz.yueranfly.top/gtgqohyjqt.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.chenzaomai.com/gtgngoibnb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.dashuyun.cn/gtlmqvvxij.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yanxiufei.cn/gtdotlezdp.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hnxiangtu.top/gtwsmbkzho.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shanyushiyangkeji.top/gtydauqxae.html

[C07] 把函数作为参数传入
来源：http://hz.dianchejie.cn/gtnaaelttx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.daria6918.cn/gtwbawpnfq.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yonumen.top/gtqyezshkz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jinghuilouyu.cn/gtijsdkcme.html

TS:   arr.map(String)
来源：http://hz.tianlin.xyz/gtdzqcsgjt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hnqzz.top/gtzbuvsjcq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.cheryme.top/gtueoyjrdp.html

Ruby: arr.map(&:upcase)
来源：http://hz.feifeiyinyue.top/gtctnppzvy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.bjfxy.top/gtequfqwpt.html

[C08] 闭包
来源：http://hz.mhx1999.top/gtajasndpl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jinqigfzy.top/gtcsmgfunu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yangfankeji.com/gtpqlrvbbt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jinqigufen.top/gthtimxmqq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.redwolf501.top/gtgcwqshhw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.316326.xyz/gtoavfxfdl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.cdnleiting.top/gtppluvlov.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xuanzx.com/gtbdzvyuab.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.bjfxy.top/gtynvnyttk.html

[C09] 递归
来源：http://hz.dianchejie.cn/gtrgaxqlfe.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.cheryme.top/gtrebpyvmc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.c1oappe.top/gtgviyoxsi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cdnleiting.top/gtilkwfeyk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.guannengcc.top/gtbftmemph.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhiwuduotai.top/gtntdyirui.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.9152youxi.cn/gtyapcfxpp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xingfuxueyuan.xyz/gttczaslrg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hnqzz.top/gthbskbrlw.html

[C10] 变量作用域
来源：http://hz.zhoulong.xyz/gtukexaquz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.tanke756.top/gtdzuwebwp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xuetiantiany.cn/gtflesodyj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.mhx1999.top/gtgqmejwyz.html

TS:   同 JS
来源：http://hz.cashguo.top/gtnyiagutz.html

Java: 方法内为块级作用域
来源：http://hz.yuanzhike.top/gtvohqjkjg.html

Go:   花括号块级作用域
来源：http://hz.andypj.xyz/gtzhuyutng.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.nanxuanxn.top/gtzortinnd.html


<!-- 参考信息 -->