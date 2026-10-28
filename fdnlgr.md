代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.jianghu66.top/gtqsvbmoso.html

Ruby: gets.chomp
来源：http://hz.hongshengwenyu.top/gtqnylncno.html

C#:   Console.ReadLine();
来源：http://hz.0kj1m.cn/gtmdxwxsbc.html

[A21] 保留指定小数位输出
来源：http://hz.zhoulong.xyz/gtbqvannvr.html

Py:   f"{3.14159:.2f}"
来源：http://hz.dashuyun.cn/gtlivwdkyq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.bjfxy.top/gtuhuxfils.html

JS:   (3.14159).toFixed(2)
来源：http://hz.yj202588.top/gtwsrkeotd.html

TS:   (3.14159).toFixed(2)
来源：http://hz.sweek.top/gtocbacrcq.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.xziqi.cn/gtfewpnbia.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.cqqwz.cn/gtksafsjjw.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.hfpthk.cn/gtgtjmvjbm.html

C#:   3.14159.ToString("F2")
来源：http://hz.c1oappe.top/gtltfchogn.html

[A22] 获取字符串长度
来源：http://hz.xingfuxueyuan.xyz/gtuagsagwi.html

Py:   len(s)
来源：http://hz.xuanzx.com/gtzdpuswsd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.yueranfly.top/gtqfmogbqt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.jiagoushi.top/gtxaspqcjy.html

TS:   s.length
来源：http://hz.yueranfly.top/gtivvkxfju.html

Java: s.length()
来源：http://hz.hfpthk.cn/gtawyjtgeq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.zhaomingkeji.xyz/gtvurqwkmm.html

Ruby: s.length
来源：http://hz.ybcxt.top/gttmpldydj.html

C#:   s.Length
来源：http://hz.xziqi.cn/gtoaqffboj.html

[A23] 大小写转换
来源：http://hz.chenlongwang.top/gthoyketuo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.hywenlv.cn/gtyqsxfytn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.zhoulong.xyz/gtzmoourmo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.xylfe.cn/gtkyjgumbb.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yj20258888.top/gtyrhlprlw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.pycfn.com/gtrdiwghtr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.zycfv.cn/gtucfydxoc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.haohaochexian.top/gtguxddlzt.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.redwolf501.top/gtafaelxcm.html

[A24] 去除首尾空白
来源：http://hz.gzhubu.top/gtyoyxsgxg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.chenlongwang.top/gtuusjiiye.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.haohaochexian.top/gtxmzorwdf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.cqqwz.cn/gtwgppdisy.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.aizwys.cn/gtouymjxbj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.ydjk.org.cn/gtomjzheci.html

Go:   strings.TrimSpace(s)
来源：http://hz.vqdsnc.cn/gtjmseqonr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.316326.xyz/gtfpbubrlf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.hysaishi.cn/gtjqvuiuzz.html

[A25] 字符串比较
来源：http://hz.mhx1999.top/gtricwyhjc.html

Py:   s1 == s2; s1 != s2
来源：http://hz.fengsongda.top/gtfxllcohs.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.iojbl.cn/gtkclaneni.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.wangshuangyany.cn/gtifsymzes.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.sysykeji.top/gtjgalzxxt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.svipenyu.cn/gtksyudwzk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.shuidangran.top/gtvjovugxf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.xuanzx.com/gthvyuokuj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.pycfn.com/gtljospiuc.html

[A26] 类型转换总览
来源：http://hz.sysykeji.top/gtbstgabqd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.pengpengdd.cyou/gthkdgwkzr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.vqdsnc.cn/gtmeuzcdky.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.aibaodan.cn/gtyebafuep.html

TS:   Number() String() Boolean() x as number
来源：http://hz.pengpengdd.cyou/gtrwzbsnrz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.xziqi.cn/gtetmytyfj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.hnxiangtu.top/gtnfvlntig.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.dianchejie.cn/gtvtcqbcjc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.9152youxi.cn/gtqoyvkcrk.html

================================================================================
来源：http://hz.guannengcc.top/gtljvoknll.html

B. 流程控制
来源：http://hz.ivvv.top/gtdwkhpbax.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gttgduafny.html

[B01] 条件判断 if / else
来源：http://hz.shuidangran.top/gtukjpurpa.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.yangfankeji.com/gtqslroxpg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.ehwqpu.com/gttsbgtdtm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.xziqi.cn/gtdxriiqkq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yuxming.cn/gtwajzzbhn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.zhengqikj.top/gtyakyswrf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.hnxiangtu.top/gtbxadvygd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.andypj.xyz/gtvxlulgax.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.andypj.xyz/gtshrvufwu.html

[B02] 多分支 else if / elif
来源：http://hz.sysykeji.top/gtocxuiiuw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zhongyouzk.top/gtureibpht.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.yj202588.top/gtuyoyumfg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jlsjyb.cn/gtbaltgreq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.tian-w.cn/gtysnkaohq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zdqjudy.top/gttfrgrtid.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.kuanghao11.cn/gtrrmlmywn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.gzhubu.top/gtwanurufa.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cdnleiting.top/gtoumzfjrv.html

[B03] switch / match / case
来源：http://hz.jinqigufen.top/gtrpggdhdn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.pengpengdd.cyou/gtdkwxnulh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.fzhhl.top/gtachtgjni.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.cucudq.cn/gtchsoqszz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.mhx1999.top/gthbvodyoh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.smart0.xyz/gtysdbbcdc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.jyoumei.cn/gtidodvohf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.ehwqpu.com/gtcpwxbnaj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.cqqwz.cn/gtmgflvvkv.html

[B04] for 计数循环
来源：http://hz.dashuyun.cn/gtuahdlibj.html

Py:   for i in range(10): print(i)
来源：http://hz.pycfn.com/gtjpcullvz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.jlsjyb.cn/gtobwqmhha.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.haohaochexian.top/gtfzyffkmf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zhiwuduotai.top/gtwcnvzydt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.sweek.top/gtlnfktyea.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.0kj1m.cn/gtincclucn.html

Ruby: 10.times { |i| puts i }
来源：http://hz.0kj1m.cn/gttvapzsqx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.daxiang520.top/gtngrdbczi.html

[B05] 遍历数组 / 列表
来源：http://hz.hfpthk.cn/gtbpezgiik.html

Py:   for item in arr: print(item)
来源：http://hz.cheryme.top/gtzymrkzog.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.hongshengwenyu.top/gtaehajate.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.sysykeji.top/gtwmfpwwvi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.wangshuangyany.cn/gtamothdxz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.jlsjyb.cn/gtbyctagle.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.jiagoushi.top/gtgymyzcga.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yanxiufei.cn/gtjsehhzch.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.haohaochexian.top/gthogniyyq.html

[B06] 遍历字典 / 对象
来源：http://hz.nanxuanxn.top/gtahpzoqow.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.sxryk.cn/gtfqgidjca.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.dianchejie.cn/gtjpqfmdvf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.svipenyu.cn/gtakpxomeg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.aizwys.cn/gtetwlbtje.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.shzxlz.cn/gtjxlekqkg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.yuanzhike.top/gtmcgqvuri.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zhoulong.xyz/gtraxabmuj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.cashguo.top/gtkwlllvgr.html

[B07] while 循环
来源：http://hz.meibo888.top/gtosxbsdnw.html

Py:   while i < 10: i += 1
来源：http://hz.snrcjt.cn/gtxaarjgvr.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.kuanghao11.cn/gtfsbhumdj.html

JS:   while (i < 10) { i++; }
来源：http://hz.jianghu66.top/gtnhnqdqhq.html

TS:   while (i < 10) { i++; }
来源：http://hz.iojbl.cn/gtzotiwobm.html

Java: while (i < 10) { i++; }
来源：http://hz.nanxinkj.top/gtedeztguo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.mhx1999.top/gtawhcxpne.html

Ruby: while i < 10; i += 1; end
来源：http://hz.guannengcc.top/gtlpvqhqzf.html

C#:   while (i < 10) { i++; }
来源：http://hz.xylfe.cn/gtstewvozz.html

[B08] do-while（至少执行一次）
来源：http://hz.yanxiufei.cn/gtnszonlsl.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.chenjidiqi.icu/gtjqrvvqfr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.ybcxt.top/gtvcgvrkfu.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jinqigufen.top/gtbfbelwmv.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yj20258888.top/gtqimnsapb.html

Java: do { i++; } while (i < 10);
来源：http://hz.quarkkingdee.top/gtdgobwhok.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.wangshuangyany.cn/gthdifefmk.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.tianlin.xyz/gtbtfjtbez.html

C#:   do { i++; } while (i < 10);
来源：http://hz.cucudq.cn/gtdhchxudt.html

[B09] break 与 continue
来源：http://hz.52xcode.cn/gtvedsbzlm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.haohaochexian.top/gtjjcjtsig.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.sysykeji.top/gttuatrzkw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gotoacloud.top/gtypcgfubx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhengqikj.top/gtkjwqzdqn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hongshengwenyu.top/gtmxixkkez.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.chenjidiqi.icu/gtsqviejpt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.shzxlz.cn/gtedhvqmaz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuetiantiany.cn/gtpgavfapf.html

[B10] 遍历同时拿索引
来源：http://hz.gotoacloud.top/gtjuauubtg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.ybcxt.top/gtwrbqehxf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.316326.xyz/gtpniqhrqp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.meibo888.top/gtryopuopw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.tianlin.xyz/gtcrmqaycy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zhijiandao.cn/gtqtgqzete.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.aibaodan.cn/gtzkdyujxc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.havefunace.top/gtvakxxjst.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.snrcjt.cn/gtzdglhowv.html

[B11] 生成数字序列 / 区间
来源：http://hz.fzhhl.top/gtuhdilxdv.html

Py:   list(range(0, 10, 2))
来源：http://hz.tanke756.top/gtphdlkuvh.html

PHP:  range(0, 10, 2);
来源：http://hz.xinyue.icu/gtlwdlsjvu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yuxming.cn/gtzzrsrvqq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhoulong.xyz/gtpgxbngps.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.quarkkingdee.top/gthjrqikia.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yj20258.top/gtaqphjodk.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jianghu66.top/gtcizoasku.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.ivvv.top/gtuojeinva.html

[B12] 跳出多层循环
来源：http://hz.tanke756.top/gtpnywbhlf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.xuanzx.com/gtucoyhihl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.dianchejie.cn/gtacbhzzql.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.redwolf501.top/gtcuhqdmpf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.nanxuanxn.top/gtevwyijhx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.tian-w.cn/gtjvjghviy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.gaohongyu789.top/gtpfotcpzt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.daria6918.cn/gtufijzthi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.sweek.top/gtfjochovp.html

[B13] 判断是否为数字
来源：http://hz.ydjk.org.cn/gtyphurdff.html

Py:   isinstance(x, (int, float))
来源：http://hz.chenlongwang.top/gtnrdgxzab.html

PHP:  is_numeric($x)
来源：http://hz.aizwys.cn/gtenxhuhns.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhengqikj.top/gtameqqbwz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.pengpengdd.cyou/gtmuhpofsb.html

Java: x instanceof Number
来源：http://hz.hnxiangtu.top/gtcirtgzdz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jlsjyb.cn/gttebawmdt.html

Ruby: x.is_a?(Numeric)
来源：http://hz.shanyushiyangtech.top/gtyfdqwspg.html

C#:   x is int or double or decimal
来源：http://hz.dashuyun.cn/gtkyikyxpd.html

[B14] 判断值是否在集合内
来源：http://hz.yueranfly.top/gtimqdumey.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.aizwys.cn/gtwurrswnf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.wangdashe.top/gtnsxaxyyj.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.iojbl.cn/gtmzyqxoxb.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.xuanzx.com/gtptvikjqd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yangfankeji.com/gtkwxryhry.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yuanzhike.top/gtkbgzilpu.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.pengpengdd.cyou/gtowlbsigp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yj20258.top/gtpkdcpcjg.html

[B15] 布尔运算与取反
来源：http://hz.sxryk.cn/gtrfwbsokk.html

Py:   a and b or not c
来源：http://hz.xziqi.cn/gtrcoepghc.html

PHP:  $a && $b || !$c
来源：http://hz.hfpthk.cn/gtqtrgvjfy.html

JS:   a && b || !c
来源：http://hz.zhiwuduotai.top/gtnioympox.html

TS:   a && b || !c
来源：http://hz.gzhubu.top/gtcaewfdup.html

Java: a && b || !c
来源：http://hz.zhijiandao.cn/gtqktrbcjv.html

Go:   a && b || !c
来源：http://hz.jiagoushi.top/gtmomwbygu.html

Ruby: a && b || !c
来源：http://hz.ivvv.top/gtwtmbijfh.html

C#:   a && b || !c
来源：http://hz.wangshuangyany.cn/gttyougabx.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yuxming.cn/gtggwfmxvo.html

Py:   if not data: return
来源：http://hz.yangfankeji.com/gtgvtqkyci.html

PHP:  if (!$data) { return; }
来源：http://hz.jiagoushi.top/gtpcfhsdzk.html

JS:   if (!data) return;
来源：http://hz.xylfe.cn/gtssbiuylg.html

TS:   if (!data) return;
来源：http://hz.shanyushiyangkeji.top/gtiwkvrlwn.html

Java: if (data == null) return;
来源：http://hz.316326.xyz/gtiqsrmpkc.html

Go:   if data == nil { return }
来源：http://hz.sxryk.cn/gtpnjtghrj.html

Ruby: return if data.nil?
来源：http://hz.andypj.xyz/gtgamuesxr.html

C#:   if (data == null) return;
来源：http://hz.ydzc1.top/gtkotsnjmq.html

================================================================================
来源：http://hz.guowangkeji.top/gtehvkibjq.html

C. 函数与作用域
来源：http://hz.jinyuanbaomall.cn/gtgtpwqrak.html

================================================================================
来源：http://hz.xziqi.cn/gtlixcmeqe.html

[C01] 定义函数
来源：http://hz.0kj1m.cn/gtvegrvhxp.html

Py:   def add(a, b): return a + b
来源：http://hz.yongpay.top/gtzwhyqbro.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hysaishi.cn/gtdyuaudox.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.316326.xyz/gtuytdmnso.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cdnleiting.top/gtvgrllggp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.ppjwa.cn/gtyjzthrxp.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jinyuanbaomall.cn/gtifetrgwr.html

Ruby: def add(a, b); a + b; end
来源：http://hz.feifeiyinyue.top/gtfhoabboj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yongpay.top/gtuurjucqp.html

[C02] 默认参数
来源：http://hz.daxiang520.top/gthqybzobb.html

Py:   def greet(name="World"): return name
来源：http://hz.jinqigfzy.top/gtrptzfwuu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.shanyushiyangtech.top/gtchivbzoq.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.xziqi.cn/gtqeklpmmm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ehwqpu.com/gtwjcupacy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.wangdashe.top/gtnkishxyj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.andypj.xyz/gtuairvywh.html

Ruby: def greet(name = "World") = name
来源：http://hz.xylfe.cn/gtnmdivfqi.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.gzhubu.top/gtbczjkgga.html

[C03] 可变参数
来源：http://hz.yvedp.cn/gtuqwyjrjf.html

Py:   def total(*args): return sum(args)
来源：http://hz.zdqjudy.top/gtuhjrejfr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.52xcode.cn/gtwwlmntep.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.havefunace.top/gtfscmrene.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ywan-chungtsiang.top/gtwgyxeigq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.gotoacloud.top/gtacyuuwcp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hywenlv.cn/gtamjffrhp.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ybcxt.top/gthhrksbke.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jiagoushi.top/gtibwqgxoq.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yj20258.top/gtamgdjcmg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jqgufenzy.top/gtgysxpjuw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.pengpengdd.cyou/gtxiytuxmu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jlsjyb.cn/gtvwgeqavq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.sxryk.cn/gtsilacycf.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yuxming.cn/gthdvmljgu.html

Go:   // 无：用配置结构体参数
来源：http://hz.0kj1m.cn/gtoisjtqww.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yj202588.top/gtbgvqdmaw.html

C#:   f(a: 1, b: 2)
来源：http://hz.cashguo.top/gtxewccgak.html

[C05] 返回多个值
来源：http://hz.iojbl.cn/gthexvjpjs.html

Py:   return a, b
来源：http://hz.nanxuanxn.top/gtekxoxhuz.html

PHP:  return [$a, $b];
来源：http://hz.cucudq.cn/gtgqgyardc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yangfankeji.com/gtggnizmaj.html

TS:   return { a, b };
来源：http://hz.9152youxi.cn/gtpbiuojmy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hfpthk.cn/gthkddmvii.html

Go:   return a, b
来源：http://hz.sweek.top/gtofufuich.html

Ruby: return a, b
来源：http://hz.ydzc1.top/gtptmwjcag.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jinghuilouyu.cn/gtmbfnzqsq.html

[C06] 匿名函数 / lambda
来源：http://hz.xinyue.icu/gtifjftrpo.html

Py:   square = lambda x: x * x
来源：http://hz.cashguo.top/gtairopcxp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.pycfn.com/gtfvbzspgo.html

JS:   const square = x => x * x;
来源：http://hz.yj20258888.top/gtjkfhdfsz.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ybcxt.top/gtyyxkqvto.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.nanxuanxn.top/gtguyvrujc.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.chenlongwang.top/gtwrnqscby.html

Ruby: square = ->(x) { x * x }
来源：http://hz.tanke756.top/gtcczfxqnh.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.snrcjt.cn/gtcklcnzff.html

[C07] 把函数作为参数传入
来源：http://hz.shanyushiyangtech.top/gthzweesli.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hysaishi.cn/gtraoutisu.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jianghu66.top/gtpzdhvwfa.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yvedp.cn/gtygatdfjv.html

TS:   arr.map(String)
来源：http://hz.cheryme.top/gtttlyznvf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.dashuyun.cn/gtqgdhtlwb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hongshengwenyu.top/gtyvrybxch.html

Ruby: arr.map(&:upcase)
来源：http://hz.fzhhl.top/gtnxkqhlof.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.daxiang520.top/gtfbzfwpgl.html

[C08] 闭包
来源：http://hz.shzxlz.cn/gtrsivrbtd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yj20258888.top/gtajxhkuiq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.nwbrower.top/gtdhimtgif.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.guowangkeji.top/gtlvnaaffm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.chenzaomai.com/gticjiufyf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.andypj.xyz/gtpdhgfwvb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.guowangkeji.top/gtsfwkgury.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.wangshuangyany.cn/gtiffapjfi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yueranfly.top/gtnxivagix.html

[C09] 递归
来源：http://hz.nwbrower.top/gtmywjqaga.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.gaohongyu789.top/gtooqktdld.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ehwqpu.com/gtpqrrzoko.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gzhubu.top/gtdbsgrios.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.dianchejie.cn/gtniweqzsl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yonumen.top/gtfgkpniuy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.shanyushiyangtech.top/gtjfzaurim.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.meibo888.top/gtfmbunzxm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.nanxuanxn.top/gtvhzeosqq.html

[C10] 变量作用域
来源：http://hz.hfpthk.cn/gtehrdjkzx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.cucudq.cn/gtteirfokk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.aibaodan.cn/gtlxqtwxby.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.chenjidiqi.icu/gtjxvlevyd.html

TS:   同 JS
来源：http://hz.guannengcc.top/gtrdickfuy.html

Java: 方法内为块级作用域
来源：http://hz.zycfv.cn/gtnquwsyqt.html

Go:   花括号块级作用域
来源：http://hz.shanyushiyangtech.top/gtuifvsuqt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yj202588.top/gtffsnolcb.html

C#:   块级作用域
来源：http://hz.hfpthk.cn/gtsnzbhsgk.html

[C11] 模块导入与导出
来源：http://hz.zdqjudy.top/gtespmapgn.html

Py:   from module import func
来源：http://hz.sxryk.cn/gtswohlemo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xuanzx.com/gtggpnaqqe.html


<!-- 参考信息 -->