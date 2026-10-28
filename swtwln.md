代发 wailian999

C#:   (int)'A'; (char)65
来源：http://hz.xinyue.icu/gtghvagsac.html

[A19] 交换两个变量
来源：http://hz.52xcode.cn/gtjkasjdiw.html

Py:   a, b = b, a
来源：http://hz.zhijiandao.cn/gtcttvlphz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.jianghu66.top/gtnoxzjhdf.html

JS:   [a, b] = [b, a];
来源：http://hz.quarkkingdee.top/gtnmpiqccw.html

TS:   [a, b] = [b, a];
来源：http://hz.52xcode.cn/gttssrieek.html

Java: int t = a; a = b; b = t;
来源：http://hz.dianchejie.cn/gtlvktbmac.html

Go:   a, b = b, a
来源：http://hz.aizwys.cn/gtgtxogjkw.html

Ruby: a, b = b, a
来源：http://hz.zycfv.cn/gthqsuxach.html

C#:   (a, b) = (b, a);
来源：http://hz.zdqjudy.top/gtksiveiax.html

[A20] 读取标准输入
来源：http://hz.zhengqikj.top/gtxlftjkvp.html

Py:   name = input("请输入：")
来源：http://hz.zycfv.cn/gtgbuqhmsl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.havefunace.top/gtgyrdfsms.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.yangfankeji.com/gtqglyvnjy.html

TS:   // Node.js：readline 模块
来源：http://hz.yuanzhike.top/gtqcerwczw.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.kuanghao11.cn/gtnphsdxif.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.zycfv.cn/gtilnsvphg.html

Ruby: gets.chomp
来源：http://hz.pengpengdd.cyou/gtkckamcxy.html

C#:   Console.ReadLine();
来源：http://hz.jinqigfzy.top/gthxexfkrb.html

[A21] 保留指定小数位输出
来源：http://hz.jiagoushi.top/gtvxmvzdab.html

Py:   f"{3.14159:.2f}"
来源：http://hz.xylfe.cn/gthrusayhy.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.smart0.xyz/gtcvekbztw.html

JS:   (3.14159).toFixed(2)
来源：http://hz.xinyue.icu/gtkvdviavz.html

TS:   (3.14159).toFixed(2)
来源：http://hz.shuidangran.top/gtbeufxadn.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.jyoumei.cn/gtcjlqlxzb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.xuetiantiany.cn/gtaktoalut.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.jinqigfzy.top/gtrlmaajgr.html

C#:   3.14159.ToString("F2")
来源：http://hz.hnxiangtu.top/gtjbmfcnmh.html

[A22] 获取字符串长度
来源：http://hz.cqqwz.cn/gtsdqgyihl.html

Py:   len(s)
来源：http://hz.xylfe.cn/gtqzcgljox.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.shzxlz.cn/gtedzjybef.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.svipenyu.cn/gtyliukyqs.html

TS:   s.length
来源：http://hz.zhoulong.xyz/gtosvrheea.html

Java: s.length()
来源：http://hz.redwolf501.top/gtzymfwjog.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.feifeiyinyue.top/gtgcsylbdv.html

Ruby: s.length
来源：http://hz.kuanghao11.cn/gtzqfhyvpj.html

C#:   s.Length
来源：http://hz.0kj1m.cn/gtbjgjusib.html

[A23] 大小写转换
来源：http://hz.shuidangran.top/gtfeqlzamp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.zdqjudy.top/gtuxcfwjiy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.dashuyun.cn/gtrxviouka.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.iojbl.cn/gtgbfrwozl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.hnqzz.top/gtrtdpogyp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.jqgfzy.top/gtmplvjybf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.chenlongwang.top/gthhswlbom.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.zycfv.cn/gtzixlfzah.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.jqgfzy.top/gtcocjnumf.html

[A24] 去除首尾空白
来源：http://hz.xinyue.icu/gtpxyicmbb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.yuanzhike.top/gtujdmvjri.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.hnxiangtu.top/gtesrexalj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.nanxuanxn.top/gttbcgmsoo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yj20258.top/gtmwdgtrrx.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.jianghu66.top/gtfvchvbef.html

Go:   strings.TrimSpace(s)
来源：http://hz.gaohongyu789.top/gtanmvtwwt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.zhoulong.xyz/gtkpwxufvv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.fzhhl.top/gtrkupdhmc.html

[A25] 字符串比较
来源：http://hz.svipenyu.cn/gtjhopcvqi.html

Py:   s1 == s2; s1 != s2
来源：http://hz.52xcode.cn/gtenrikzwa.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.gogol.net.cn/gthrjeahsu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yuxming.cn/gtlpuspytc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.zdqjudy.top/gtmcbhzaad.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.0kj1m.cn/gthuracwgw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.gogol.net.cn/gtfggquexi.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.ydzc1.top/gtllnwqsog.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.svipenyu.cn/gtlrsvajil.html

[A26] 类型转换总览
来源：http://hz.jinghuilouyu.cn/gtvnxyjuum.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.sufxvd.cn/gtrywlftsx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.fengsongda.top/gtoxrnlabq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.hongshengwenyu.top/gthabehxhd.html

TS:   Number() String() Boolean() x as number
来源：http://hz.birdmap.top/gtsbswmlyp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.yueranfly.top/gtfnndojtl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.bjfxy.top/gtcodhmikd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.tianlin.xyz/gtloddrzlm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.cheryme.top/gteoyjpssk.html

================================================================================
来源：http://hz.zhixingplan.top/gtjcbdnkqc.html

B. 流程控制
来源：http://hz.bjfxy.top/gtsvfdcgia.html

================================================================================
来源：http://hz.zhengqikj.top/gtzmcnkxox.html

[B01] 条件判断 if / else
来源：http://hz.shanyushiyangkeji.top/gtogffgxjs.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.cucudq.cn/gtcifcyenr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.shzxlz.cn/gtbavitylp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.shanyushiyangtech.top/gtmnbzkopp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.gotoacloud.top/gtemkkkhlc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.jqgufenzy.top/gtllyfctoo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.ydzc1.top/gtctcjovyq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.gotoacloud.top/gtshakjkql.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.jianghu66.top/gtvsfdmukf.html

[B02] 多分支 else if / elif
来源：http://hz.xinyue.icu/gtknlfpkgx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.yuxming.cn/gthhbozvwt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.jqgufenzy.top/gtmzsakbay.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhoulong.xyz/gtjwitavpp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.dianchejie.cn/gtabdoaskx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yongpay.top/gtutrwdrzs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.fengsongda.top/gtmfgeprog.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.iojbl.cn/gtatncbohq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xziqi.cn/gttmzkgcrx.html

[B03] switch / match / case
来源：http://hz.zhaomingkeji.xyz/gtlvykilhl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.chenlongwang.top/gtsbqjrjrl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.daria6918.cn/gtjycjfful.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.xylfe.cn/gtajlzjmtv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.gzhubu.top/gtgmpjhaac.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.chenjidiqi.icu/gtjxptvlfb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.yuanzhike.top/gtvkjxxfur.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.hysaishi.cn/gtizvfxizv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.haohaochexian.top/gturgvgafc.html

[B04] for 计数循环
来源：http://hz.sxryk.cn/gtkwigqidc.html

Py:   for i in range(10): print(i)
来源：http://hz.zhongyouzk.top/gtmsinbonc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.52xcode.cn/gtcmnadglu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jinyuanbaomall.cn/gtcbyzfjsc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zhixingplan.top/gthpcrgeqq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.jinqigfzy.top/gtjbcptqle.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.jinqigufen.top/gtfsfkmqsj.html

Ruby: 10.times { |i| puts i }
来源：http://hz.zhixingplan.top/gtpmhnyccl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.0kj1m.cn/gtimqqiaak.html

[B05] 遍历数组 / 列表
来源：http://hz.tian-w.cn/gtouqlyeof.html

Py:   for item in arr: print(item)
来源：http://hz.dianchejie.cn/gthfbmomvw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.xingfuxueyuan.xyz/gtzianhlwc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.52xcode.cn/gtdzgicijl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhongyouzk.top/gtapangsnk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.iojbl.cn/gtdjbfaexj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.guowangkeji.top/gtzymzneas.html

Ruby: arr.each { |item| puts item }
来源：http://hz.cashguo.top/gtluxxktzo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.dianchejie.cn/gthlnymxxt.html

[B06] 遍历字典 / 对象
来源：http://hz.zhixingplan.top/gtoqihvyhe.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.hnxiangtu.top/gtivemarbs.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.vqdsnc.cn/gtqazvnmvj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.fengsongda.top/gtgogmispt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ydjk.org.cn/gtlzpmmqpb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.ydjk.org.cn/gtoczfdbql.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.kuanghao11.cn/gthmsjextf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.nanxuanxn.top/gtockrcovb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.yanxiufei.cn/gtqpgwtoxn.html

[B07] while 循环
来源：http://hz.dianchejie.cn/gtnzstkovy.html

Py:   while i < 10: i += 1
来源：http://hz.yj20258888.top/gtaanxdclx.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.meibo888.top/gtrknmwffu.html

JS:   while (i < 10) { i++; }
来源：http://hz.zycfv.cn/gtgkghguto.html

TS:   while (i < 10) { i++; }
来源：http://hz.hfpthk.cn/gtmszqappe.html

Java: while (i < 10) { i++; }
来源：http://hz.shanyushiyangtech.top/gtnyydphsv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.sweek.top/gtykathpdp.html

Ruby: while i < 10; i += 1; end
来源：http://hz.smart0.xyz/gtukfkeovm.html

C#:   while (i < 10) { i++; }
来源：http://hz.gogol.net.cn/gtapjrihvp.html

[B08] do-while（至少执行一次）
来源：http://hz.hongshengwenyu.top/gtaxingykb.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.andypj.xyz/gtetlsggub.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.yj20258888.top/gtqvmtmcgc.html

JS:   do { i++; } while (i < 10);
来源：http://hz.cashguo.top/gtwouqiaog.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jianghu66.top/gtxdeoayqv.html

Java: do { i++; } while (i < 10);
来源：http://hz.hywenlv.cn/gtcmowmqfr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.sxryk.cn/gtmeesgouq.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.andypj.xyz/gtegyrhkop.html

C#:   do { i++; } while (i < 10);
来源：http://hz.zhijiandao.cn/gtrivpdgzs.html

[B09] break 与 continue
来源：http://hz.gaohongyu789.top/gtvihpslaj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.hywenlv.cn/gtykwgizsx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.ydzc1.top/gtveyinoka.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sysykeji.top/gtammyoabf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yuxming.cn/gtaidcmqqc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shangyingyoupin.top/gtgcmduaue.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yongpay.top/gtkhindwiv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.xylfe.cn/gtbddmhfmx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.smart0.xyz/gtvgmmnyly.html

[B10] 遍历同时拿索引
来源：http://hz.xuanzx.com/gtgtcmmliy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zhaomingkeji.xyz/gtskivssks.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.fengsongda.top/gtflgebwig.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.wangdashe.top/gttzjojebk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.pycfn.com/gtuzjdbdho.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.mhx1999.top/gtsumdzvjk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.zycfv.cn/gtktcicwzg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.xuetiantiany.cn/gtzhpqubwx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.gzhubu.top/gtrshhuvxx.html

[B11] 生成数字序列 / 区间
来源：http://hz.andypj.xyz/gtdbnkphdn.html

Py:   list(range(0, 10, 2))
来源：http://hz.shzxlz.cn/gtbiwrrnrp.html

PHP:  range(0, 10, 2);
来源：http://hz.xylfe.cn/gtbkdwalwc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.redwolf501.top/gtokexzzfz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ppjwa.cn/gtnbsknynm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jinyuanbaomall.cn/gtnjaczyru.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hfpthk.cn/gtiosbshhu.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yj20258.top/gtsomhlrms.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.ydjk.org.cn/gtoyxnpwah.html

[B12] 跳出多层循环
来源：http://hz.fzhhl.top/gtcsckenea.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.aizwys.cn/gtziivoyrv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhongyouzk.top/gtlywxbeso.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.quarkkingdee.top/gtqlyqgodm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yueranfly.top/gtnhrpwnff.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.xylfe.cn/gtavjsmxwj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yuanzhike.top/gtjhitcact.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.ivvv.top/gtvfhiswxg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.jinyuanbaomall.cn/gtvnvuossp.html

[B13] 判断是否为数字
来源：http://hz.dianchejie.cn/gtjutvoevj.html

Py:   isinstance(x, (int, float))
来源：http://hz.hnxiangtu.top/gtedjvjzkg.html

PHP:  is_numeric($x)
来源：http://hz.yongpay.top/gtbaacqkzt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cashguo.top/gthlpsrieu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhengqikj.top/gtnidafciw.html

Java: x instanceof Number
来源：http://hz.gaohongyu789.top/gtnkmdpwez.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yvedp.cn/gtlubhcbgw.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yongpay.top/gtxnscfowm.html

C#:   x is int or double or decimal
来源：http://hz.wangdashe.top/gtwqipmyiz.html

[B14] 判断值是否在集合内
来源：http://hz.andypj.xyz/gtunedbrxv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jinqigufen.top/gtawcyaqoo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yj202588.top/gtzkkxzmve.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.guowangkeji.top/gtlnuyaqcy.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jinqigufen.top/gtywzdrbmh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jinqigfzy.top/gtjeorytcp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.nanxuanxn.top/gtkyccwoty.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xuetiantiany.cn/gtvtkaqmvc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jyoumei.cn/gtlyyxmive.html

[B15] 布尔运算与取反
来源：http://hz.yj20258888.top/gtzuhzkxor.html

Py:   a and b or not c
来源：http://hz.52xcode.cn/gtcshbczyu.html

PHP:  $a && $b || !$c
来源：http://hz.cashguo.top/gttmibrnpo.html

JS:   a && b || !c
来源：http://hz.ydjk.org.cn/gtggbsbyhp.html

TS:   a && b || !c
来源：http://hz.jinqigfzy.top/gttkqicbok.html

Java: a && b || !c
来源：http://hz.nanxuanxn.top/gtuoixyiwp.html

Go:   a && b || !c
来源：http://hz.zhengqikj.top/gtohhiitvr.html

Ruby: a && b || !c
来源：http://hz.pengpengdd.cyou/gtpxvexkun.html

C#:   a && b || !c
来源：http://hz.yvedp.cn/gtvheftgzi.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.xinyue.icu/gtqodvocyd.html

Py:   if not data: return
来源：http://hz.jyoumei.cn/gtxwpxdrzu.html

PHP:  if (!$data) { return; }
来源：http://hz.xziqi.cn/gtfacqupya.html

JS:   if (!data) return;
来源：http://hz.hfpthk.cn/gtjhedhdxo.html

TS:   if (!data) return;
来源：http://hz.wangshuangyany.cn/gtyfsutyqc.html

Java: if (data == null) return;
来源：http://hz.yanxiufei.cn/gtxosuwjex.html

Go:   if data == nil { return }
来源：http://hz.nanxuanxn.top/gtsecghdkd.html

Ruby: return if data.nil?
来源：http://hz.sufxvd.cn/gtdunvnatz.html

C#:   if (data == null) return;
来源：http://hz.chenzaomai.com/gtfetohkac.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtacwnfoms.html

C. 函数与作用域
来源：http://hz.yueranfly.top/gttfjikpfb.html

================================================================================
来源：http://hz.chenzaomai.com/gtnpzbszvb.html

[C01] 定义函数
来源：http://hz.zhongyouzk.top/gtuuegioii.html

Py:   def add(a, b): return a + b
来源：http://hz.zhoulong.xyz/gtcnkmhzra.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.meibo888.top/gthodkegff.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhengqikj.top/gtkgctihuz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nanxinkj.top/gtfamyzoch.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xuetiantiany.cn/gtpqjtwsgj.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.gotoacloud.top/gtuerrmoqa.html

Ruby: def add(a, b); a + b; end
来源：http://hz.chenjidiqi.icu/gtpdudwhxl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.mhx1999.top/gtiimrebks.html

[C02] 默认参数
来源：http://hz.jinghuilouyu.cn/gtdygivnss.html

Py:   def greet(name="World"): return name
来源：http://hz.zhiwuduotai.top/gtuuyfdtwo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jinyuanbaomall.cn/gtjhirgtvb.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hnqzz.top/gtcirxauag.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.9152youxi.cn/gtzuccvdbe.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.aibaodan.cn/gtqmuehfqx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jinghuilouyu.cn/gtrutswknw.html

Ruby: def greet(name = "World") = name
来源：http://hz.nanxuanxn.top/gtboyfigwb.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhaomingkeji.xyz/gtpwrugvjf.html

[C03] 可变参数
来源：http://hz.birdmap.top/gtbilyapgj.html

Py:   def total(*args): return sum(args)
来源：http://hz.bjfxy.top/gtivsqbxln.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hysaishi.cn/gtlgozjzsd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ydjk.org.cn/gtrjgvwwwm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xuanzx.com/gtfmzazwcn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.dianchejie.cn/gtglupvjpg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yuanzhike.top/gtpfbeuwba.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xingfuxueyuan.xyz/gtbyprkcpb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xziqi.cn/gtpuyqhkxl.html

[C04] 命名参数 / 关键字参数
来源：http://hz.sweek.top/gtkbxadqai.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ywan-chungtsiang.top/gtvugvpwrr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.gaohongyu789.top/gtbkunkpdq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zhijiandao.cn/gtqyzsmnag.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zdqjudy.top/gtzzzzuiso.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.tian-w.cn/gtcfowxrst.html

Go:   // 无：用配置结构体参数
来源：http://hz.ehwqpu.com/gtzpedoxxj.html

Ruby: f(a: 1, b: 2)
来源：http://hz.iojbl.cn/gtyuwhiwkl.html

C#:   f(a: 1, b: 2)
来源：http://hz.yongpay.top/gtvmeujlll.html

[C05] 返回多个值
来源：http://hz.haohaochexian.top/gthiqrkheo.html

Py:   return a, b
来源：http://hz.bjfxy.top/gtizcyjmps.html

PHP:  return [$a, $b];
来源：http://hz.yvedp.cn/gtqlahcelo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jiagoushi.top/gtzceplvun.html

TS:   return { a, b };
来源：http://hz.kuanghao11.cn/gtnzahrqok.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.fzhhl.top/gtcvlftpnb.html

Go:   return a, b
来源：http://hz.haohaochexian.top/gtwavpseyi.html

Ruby: return a, b
来源：http://hz.ydjk.org.cn/gthyrizytu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.sweek.top/gtrokhfnws.html

[C06] 匿名函数 / lambda
来源：http://hz.gzhubu.top/gteakpqlzm.html

Py:   square = lambda x: x * x
来源：http://hz.jiagoushi.top/gtongxjsmz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jinqigufen.top/gtopgfzlxh.html

JS:   const square = x => x * x;
来源：http://hz.shuidangran.top/gtbniwpuyl.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yongpay.top/gtvuzencsy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jyoumei.cn/gtbbldlaad.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.pycfn.com/gtrbvhjubg.html

Ruby: square = ->(x) { x * x }
来源：http://hz.chenlongwang.top/gtspjorvgi.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.52xcode.cn/gtvhpthmva.html

[C07] 把函数作为参数传入
来源：http://hz.hfpthk.cn/gtyratzivt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jinghuilouyu.cn/gtaiicvbgj.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.dashuyun.cn/gtodrwgzac.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhijiandao.cn/gtrvgszpab.html

TS:   arr.map(String)
来源：http://hz.tian-w.cn/gtupxqxjgw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yangfankeji.com/gtopycpgpk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yj20258888.top/gtdkfsfrek.html

Ruby: arr.map(&:upcase)
来源：http://hz.zycfv.cn/gtmcqxjwyp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jinqigufen.top/gtpbcchfyw.html

[C08] 闭包
来源：http://hz.hammf.cn/gtyjywntxv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhixingplan.top/gtsnigvkrp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.xuanzx.com/gtfnigkfxz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.redwolf501.top/gtkdsqdovm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.guowangkeji.top/gtwlvshmzm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhengqikj.top/gtjcjbmpyk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhijiandao.cn/gtbvrzxwkh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.shanyushiyangkeji.top/gtdrrnshga.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhaomingkeji.xyz/gtaoueinke.html

[C09] 递归
来源：http://hz.quarkkingdee.top/gtzzuhijmt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xingfuxueyuan.xyz/gtemrfwxxd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yonumen.top/gtvtafvpct.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.feifeiyinyue.top/gtpzxtvwwd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xingfuxueyuan.xyz/gtrlnykhrc.html


<!-- 参考信息 -->