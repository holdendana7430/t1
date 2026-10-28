代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.jiagoushi.top/gtythebpar.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.yuxming.cn/gtdbowxatd.html

TS:   // Node.js：readline 模块
来源：http://hz.52xcode.cn/gtyebbevnc.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.jyoumei.cn/gtdqposkdz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.xinyue.icu/gtbpybvkgn.html

Ruby: gets.chomp
来源：http://hz.ivvv.top/gtqynfclgo.html

C#:   Console.ReadLine();
来源：http://hz.vqdsnc.cn/gtngjntqhj.html

[A21] 保留指定小数位输出
来源：http://hz.xuanzx.com/gtyevprabx.html

Py:   f"{3.14159:.2f}"
来源：http://hz.jianghu66.top/gtorkzqpco.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.jianghu66.top/gtbujxjnek.html

JS:   (3.14159).toFixed(2)
来源：http://hz.sysykeji.top/gtgddofgdz.html

TS:   (3.14159).toFixed(2)
来源：http://hz.sxryk.cn/gttyyvpwjy.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.xuetiantiany.cn/gthyuqrsds.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.hysaishi.cn/gtnrxwczlh.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.shanyushiyangtech.top/gtebdmgmoa.html

C#:   3.14159.ToString("F2")
来源：http://hz.haohaochexian.top/gtqathtbfp.html

[A22] 获取字符串长度
来源：http://hz.kuanghao11.cn/gtexveekrb.html

Py:   len(s)
来源：http://hz.cqqwz.cn/gtvxcugpwg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.havefunace.top/gtmjjpwjzm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.jinqigufen.top/gtntdkpoos.html

TS:   s.length
来源：http://hz.yvedp.cn/gtqymrbqwf.html

Java: s.length()
来源：http://hz.316326.xyz/gtgmzhmaem.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.316326.xyz/gtzhmmjpix.html

Ruby: s.length
来源：http://hz.cdnleiting.top/gthozbweut.html

C#:   s.Length
来源：http://hz.gogol.net.cn/gtmffxgwcy.html

[A23] 大小写转换
来源：http://hz.zhoulong.xyz/gtgarginba.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.jinghuilouyu.cn/gtapbjdrsf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.wangdashe.top/gtlngroson.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.bjfxy.top/gtuopbtwqp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.vqdsnc.cn/gtlmtwdxwg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.guannengcc.top/gtsxikruvv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.zhoulong.xyz/gtmkqqfnas.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.52xcode.cn/gtumjyknvr.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.hongshengwenyu.top/gthuuylcoy.html

[A24] 去除首尾空白
来源：http://hz.zycfv.cn/gthsjxqqax.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.zhixingplan.top/gtucdeatnd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.ppjwa.cn/gtqnlotdxw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zycfv.cn/gtcmlzdfjr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.chenzaomai.com/gtciipazta.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.nanxuanxn.top/gtssviqhwk.html

Go:   strings.TrimSpace(s)
来源：http://hz.yonumen.top/gtqcpdjvtu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.zhixingplan.top/gtifnmjmsi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.jianghu66.top/gtvgldthcg.html

[A25] 字符串比较
来源：http://hz.guannengcc.top/gtibarcrtp.html

Py:   s1 == s2; s1 != s2
来源：http://hz.ivvv.top/gthpmlphjd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.jyoumei.cn/gtypvipuid.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yonumen.top/gtyniipeqj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.cucudq.cn/gttrboejai.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.wangdashe.top/gtshldhzef.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.dianchejie.cn/gtdiqptrjs.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.gaohongyu789.top/gtfxndbvyd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.zhixingplan.top/gtpfooonrd.html

[A26] 类型转换总览
来源：http://hz.jinqigufen.top/gthkwrslmk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.havefunace.top/gtxvqdlylk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.jinyuanbaomall.cn/gtdurbfuly.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.snrcjt.cn/gtnyxvgvsh.html

TS:   Number() String() Boolean() x as number
来源：http://hz.zhixingplan.top/gtsjytvugv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.chenlongwang.top/gtjovuwxtf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.xuanzx.com/gtwejmlfuv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.cashguo.top/gtinvcqtti.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.ivvv.top/gtpprkxyjg.html

================================================================================
来源：http://hz.jlsjyb.cn/gtbaotmnel.html

B. 流程控制
来源：http://hz.snrcjt.cn/gtclxlundv.html

================================================================================
来源：http://hz.fengsongda.top/gtmfrmwyte.html

[B01] 条件判断 if / else
来源：http://hz.zhixingplan.top/gtihzkyxfp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.yj202588.top/gtpofglitc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.redwolf501.top/gtzcwsqeea.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.redwolf501.top/gttvsyrxun.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.fengsongda.top/gtpbpccqfn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.ywan-chungtsiang.top/gtqwjjyblw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.wangdashe.top/gtuxvsummn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.dianchejie.cn/gtyfikgkmy.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.yvedp.cn/gtbezsxasy.html

[B02] 多分支 else if / elif
来源：http://hz.guannengcc.top/gtjhrqnjga.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.yj20258888.top/gteiojjvfg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.yongpay.top/gtxkituecd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhengqikj.top/gtprtcaakz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jinqigfzy.top/gtpxnnmvtj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jinqigufen.top/gtuoqzktzo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.sweek.top/gtcmrairyx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.cheryme.top/gtzfwrerlf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.nwbrower.top/gtaxgeiouv.html

[B03] switch / match / case
来源：http://hz.ydzc1.top/gtcidnqarc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.jqgfzy.top/gtsyxskogt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.gotoacloud.top/gtsbziftmd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.sufxvd.cn/gtlbbngjsb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.nanxuanxn.top/gthhlucuwq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.jlsjyb.cn/gthuimhmow.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.52xcode.cn/gtqsuaavnf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.cashguo.top/gtauzpclnj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.cashguo.top/gtbbdummxa.html

[B04] for 计数循环
来源：http://hz.andypj.xyz/gteyiygaww.html

Py:   for i in range(10): print(i)
来源：http://hz.cashguo.top/gtfmsxxovp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.yanxiufei.cn/gtuxcwtvic.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.gotoacloud.top/gtgatfjhvb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zhiwuduotai.top/gtsnmlmkqx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.guowangkeji.top/gtswtecgwe.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.chenjidiqi.icu/gtnxxngies.html

Ruby: 10.times { |i| puts i }
来源：http://hz.quarkkingdee.top/gtyurxxlvu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.0kj1m.cn/gthjvhxpxf.html

[B05] 遍历数组 / 列表
来源：http://hz.yj20258888.top/gtmfjfdsun.html

Py:   for item in arr: print(item)
来源：http://hz.yanxiufei.cn/gtszgnryzl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.chenlongwang.top/gtdkpfgnsl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.cdnleiting.top/gtbtyyrjaw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.jianghu66.top/gtphmhdgii.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.hongshengwenyu.top/gtsmnovcuy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.gotoacloud.top/gtmqungdzf.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yj202588.top/gtiadeajtx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.zdqjudy.top/gtioswsqsa.html

[B06] 遍历字典 / 对象
来源：http://hz.bjfxy.top/gtdambemev.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.ybcxt.top/gtwekgyvaz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.zhiwuduotai.top/gtmkpmcyhw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.haohaochexian.top/gtnjzxqqve.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hnxiangtu.top/gtbqebwjio.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.fzhhl.top/gtnpmfzyvl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jlsjyb.cn/gtpcpcalyh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.ivvv.top/gtxpfpiwnj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jinqigufen.top/gttwkpixmi.html

[B07] while 循环
来源：http://hz.svipenyu.cn/gtfndlkhzr.html

Py:   while i < 10: i += 1
来源：http://hz.quarkkingdee.top/gthzhrwmzw.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jlsjyb.cn/gtjlzjstam.html

JS:   while (i < 10) { i++; }
来源：http://hz.gaohongyu789.top/gtbbxbzfyh.html

TS:   while (i < 10) { i++; }
来源：http://hz.cdnleiting.top/gtdovzdgog.html

Java: while (i < 10) { i++; }
来源：http://hz.316326.xyz/gtrjnslomh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yanxiufei.cn/gtypvgoiyg.html

Ruby: while i < 10; i += 1; end
来源：http://hz.tian-w.cn/gtjfngssur.html

C#:   while (i < 10) { i++; }
来源：http://hz.daxiang520.top/gtwlxvtnmk.html

[B08] do-while（至少执行一次）
来源：http://hz.yonumen.top/gtnpstavvo.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.yj20258.top/gttkwkeufn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.hywenlv.cn/gtmvoswwgt.html

JS:   do { i++; } while (i < 10);
来源：http://hz.havefunace.top/gttnpuzywz.html

TS:   do { i++; } while (i < 10);
来源：http://hz.shuidangran.top/gtkglrpuzc.html

Java: do { i++; } while (i < 10);
来源：http://hz.zhiwuduotai.top/gtfbvytzhr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.wangdashe.top/gtxmcwwdsd.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.0kj1m.cn/gtcxrvyzya.html

C#:   do { i++; } while (i < 10);
来源：http://hz.snrcjt.cn/gtyntjtpgn.html

[B09] break 与 continue
来源：http://hz.yj202588.top/gtmcvtizch.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.zhengqikj.top/gtfcrklsxx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hywenlv.cn/gtgfwquaca.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.c1oappe.top/gtgiwspake.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jqgfzy.top/gtwwldewll.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ydjk.org.cn/gthuymzgmq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jyoumei.cn/gtrmzvylbe.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.xylfe.cn/gtgntecndj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ehwqpu.com/gtlejroccq.html

[B10] 遍历同时拿索引
来源：http://hz.jlsjyb.cn/gtyhnmroly.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.xinyue.icu/gttryxjrbr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.jinqigfzy.top/gtlbcbswzt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.fzhhl.top/gtmcklzluv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.svipenyu.cn/gtbvqrglzj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.9152youxi.cn/gtgaznhsbl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.shzxlz.cn/gtcsncfavu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.c1oappe.top/gtknrjkuep.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jqgfzy.top/gtieftfmyp.html

[B11] 生成数字序列 / 区间
来源：http://hz.yueranfly.top/gtaopsuoiy.html

Py:   list(range(0, 10, 2))
来源：http://hz.hnqzz.top/gtvfxbnumg.html

PHP:  range(0, 10, 2);
来源：http://hz.dianchejie.cn/gtlvfmaqfz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.wangdashe.top/gtzrxhjdwb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gzhubu.top/gtdqqhzibg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.birdmap.top/gtxuefucjl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.ydjk.org.cn/gtwbprtvad.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jqgfzy.top/gthqyetnnc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.9152youxi.cn/gtfltaahfx.html

[B12] 跳出多层循环
来源：http://hz.tanke756.top/gtluqwukel.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zhixingplan.top/gtqxwblvvm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.nanxuanxn.top/gtorscprts.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.snrcjt.cn/gtyjbrkyjg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jiagoushi.top/gtnoamvbqm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yonumen.top/gtsqzdfljv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.0kj1m.cn/gtiudmlwvq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.ybcxt.top/gtagmspgrg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.xylfe.cn/gtackjzllx.html

[B13] 判断是否为数字
来源：http://hz.sxryk.cn/gtmtehpbsz.html

Py:   isinstance(x, (int, float))
来源：http://hz.9152youxi.cn/gtfiebeucy.html

PHP:  is_numeric($x)
来源：http://hz.fengsongda.top/gthqyhsyto.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shangyingyoupin.top/gtzqixrtha.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.mhx1999.top/gtxotznfck.html

Java: x instanceof Number
来源：http://hz.guannengcc.top/gtbqdoxdig.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.dashuyun.cn/gtrxfbziaq.html

Ruby: x.is_a?(Numeric)
来源：http://hz.iojbl.cn/gtpoltxqfm.html

C#:   x is int or double or decimal
来源：http://hz.shangyingyoupin.top/gtlvmzbhbw.html

[B14] 判断值是否在集合内
来源：http://hz.ivvv.top/gtsjqfvldj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.nanxuanxn.top/gttdecofxd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.c1oappe.top/gtribfyquc.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.wangshuangyany.cn/gtihbsktrt.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.andypj.xyz/gtexvymexa.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.sysykeji.top/gtvofnhhrl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.sweek.top/gtmclgnvjw.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.meibo888.top/gtcypiembr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.ydjk.org.cn/gtcktzjprb.html

[B15] 布尔运算与取反
来源：http://hz.xingfuxueyuan.xyz/gtxzdeduka.html

Py:   a and b or not c
来源：http://hz.cdnleiting.top/gteagfnwqm.html

PHP:  $a && $b || !$c
来源：http://hz.316326.xyz/gtqyxlejtu.html

JS:   a && b || !c
来源：http://hz.iojbl.cn/gtjhjuwwni.html

TS:   a && b || !c
来源：http://hz.yanxiufei.cn/gtvqyjdqtx.html

Java: a && b || !c
来源：http://hz.aizwys.cn/gtlyzngwjy.html

Go:   a && b || !c
来源：http://hz.gotoacloud.top/gthioupmpf.html

Ruby: a && b || !c
来源：http://hz.yj20258888.top/gtnorikgek.html

C#:   a && b || !c
来源：http://hz.jinghuilouyu.cn/gtlqjmgozb.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.feifeiyinyue.top/gtrocploxg.html

Py:   if not data: return
来源：http://hz.wangdashe.top/gtkhjclfio.html

PHP:  if (!$data) { return; }
来源：http://hz.kuanghao11.cn/gtivzenbpg.html

JS:   if (!data) return;
来源：http://hz.hfpthk.cn/gtowvebzch.html

TS:   if (!data) return;
来源：http://hz.ybcxt.top/gtahaazmnd.html

Java: if (data == null) return;
来源：http://hz.snrcjt.cn/gtnxhhsmwm.html

Go:   if data == nil { return }
来源：http://hz.shanyushiyangkeji.top/gtgtxpyfgb.html

Ruby: return if data.nil?
来源：http://hz.jinyuanbaomall.cn/gtnmizletm.html

C#:   if (data == null) return;
来源：http://hz.ppjwa.cn/gtubpwfpoq.html

================================================================================
来源：http://hz.yj20258.top/gtvaxjflxn.html

C. 函数与作用域
来源：http://hz.52xcode.cn/gtpziyjazg.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gthkslvgfe.html

[C01] 定义函数
来源：http://hz.feifeiyinyue.top/gtsozptljn.html

Py:   def add(a, b): return a + b
来源：http://hz.jianghu66.top/gtlidqudcz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gotoacloud.top/gtfhimtgha.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.wangshuangyany.cn/gtzcbathdd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.chenzaomai.com/gtjlusxdyd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zycfv.cn/gtuoigevst.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.hnxiangtu.top/gtwmhuuars.html

Ruby: def add(a, b); a + b; end
来源：http://hz.sweek.top/gtlrvskekh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.sxryk.cn/gtobpidwzz.html

[C02] 默认参数
来源：http://hz.hnxiangtu.top/gtfjehlfkp.html

Py:   def greet(name="World"): return name
来源：http://hz.cdnleiting.top/gtxqurxtdz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.kuanghao11.cn/gtgurqxbja.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.birdmap.top/gtmljfauhy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.guannengcc.top/gtwnszksqf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhixingplan.top/gtodjksusl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jlsjyb.cn/gtgdapylun.html

Ruby: def greet(name = "World") = name
来源：http://hz.nwbrower.top/gtfzmofuqk.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.aizwys.cn/gttuiqwgvp.html

[C03] 可变参数
来源：http://hz.vqdsnc.cn/gttdlxknrr.html

Py:   def total(*args): return sum(args)
来源：http://hz.aizwys.cn/gtxoqriuhz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ppjwa.cn/gtmfkzqldt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shanyushiyangkeji.top/gtjjlrndgf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jianghu66.top/gtcfduwaws.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.xingfuxueyuan.xyz/gtfsortgon.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jianghu66.top/gtjbnnjqwp.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xuanzx.com/gtvxqcvyno.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yuxming.cn/gtnftauimb.html

[C04] 命名参数 / 关键字参数
来源：http://hz.iojbl.cn/gttvivdmvi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhongyouzk.top/gtsnkmpint.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.chenlongwang.top/gtqtjlqgyb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.ywan-chungtsiang.top/gtcykitsvm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.kuanghao11.cn/gtycyaomdc.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jiagoushi.top/gttaocryxk.html

Go:   // 无：用配置结构体参数
来源：http://hz.ehwqpu.com/gtxpqebwgx.html

Ruby: f(a: 1, b: 2)
来源：http://hz.gaohongyu789.top/gtcxlkzrti.html

C#:   f(a: 1, b: 2)
来源：http://hz.gogol.net.cn/gtjsfqcbwq.html

[C05] 返回多个值
来源：http://hz.daxiang520.top/gtjsjwnpxj.html

Py:   return a, b
来源：http://hz.sxryk.cn/gtaqqvzjny.html

PHP:  return [$a, $b];
来源：http://hz.guannengcc.top/gtyyywlokn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.shzxlz.cn/gtkgqccvdw.html

TS:   return { a, b };
来源：http://hz.shzxlz.cn/gtopopgxvc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhongyouzk.top/gtpkdbgtuy.html

Go:   return a, b
来源：http://hz.jianghu66.top/gthvhduudu.html

Ruby: return a, b
来源：http://hz.quarkkingdee.top/gtybeztrls.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ivvv.top/gtweepbgwh.html

[C06] 匿名函数 / lambda
来源：http://hz.zdqjudy.top/gtqcqvgroq.html

Py:   square = lambda x: x * x
来源：http://hz.ydjk.org.cn/gthohldzpu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.cashguo.top/gtkgdhebhx.html

JS:   const square = x => x * x;
来源：http://hz.chenlongwang.top/gtedgmrcrj.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.birdmap.top/gtrqwqfldj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.xziqi.cn/gtwhuybvge.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.xinyue.icu/gthvblmkig.html

Ruby: square = ->(x) { x * x }
来源：http://hz.tanke756.top/gtdkrideky.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.cqqwz.cn/gtphedebsg.html

[C07] 把函数作为参数传入
来源：http://hz.yonumen.top/gtmbxeshjf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.guannengcc.top/gtmrucpzbt.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.bjfxy.top/gtcqqutnak.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yangfankeji.com/gteeepktoi.html

TS:   arr.map(String)
来源：http://hz.pengpengdd.cyou/gthnrhbzby.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.c1oappe.top/gtcgmafrsl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.wangdashe.top/gtefpftozi.html

Ruby: arr.map(&:upcase)
来源：http://hz.shanyushiyangtech.top/gtkqbomncl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.sxryk.cn/gtdwoilrat.html

[C08] 闭包
来源：http://hz.jlsjyb.cn/gtjtqkwkvx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hywenlv.cn/gtjhtaubae.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.hammf.cn/gtbcukudvh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.pengpengdd.cyou/gtyocmuhgh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.52xcode.cn/gtgdptbrlh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.redwolf501.top/gtugyssvne.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.0kj1m.cn/gtmbqogood.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.tianlin.xyz/gtfqadaneo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.guannengcc.top/gtwutjbgtd.html

[C09] 递归
来源：http://hz.feifeiyinyue.top/gtpkfjdoam.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yonumen.top/gtwxblkrhu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yvedp.cn/gtbjbrexrd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jlsjyb.cn/gtbbtiysav.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.andypj.xyz/gtlghlcvhd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.mhx1999.top/gtbuwyowwg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.ppjwa.cn/gteatrmsgf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hysaishi.cn/gtamfmsvqs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jianghu66.top/gtwhmcmpqj.html

[C10] 变量作用域
来源：http://hz.yuxming.cn/gtujpzqowr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.shanyushiyangtech.top/gtjjdisqvf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.havefunace.top/gtckfuypgr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.nanxinkj.top/gtacpsvqfe.html

TS:   同 JS
来源：http://hz.316326.xyz/gtvqcdtohg.html

Java: 方法内为块级作用域
来源：http://hz.shanyushiyangtech.top/gtyqhparqr.html

Go:   花括号块级作用域
来源：http://hz.jqgufenzy.top/gtxlueonwp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.chenzaomai.com/gtqyuwvrol.html


<!-- 参考信息 -->