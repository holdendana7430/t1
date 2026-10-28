代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://hz.cheryme.top/gtsddiobww.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.ivvv.top/gtusnljwhe.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.hywenlv.cn/gtcapmlsvp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.gogol.net.cn/gtjqxonbxj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.guowangkeji.top/gtzknurtgh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.sufxvd.cn/gtmuikovyc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.havefunace.top/gtozuupert.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.bjfxy.top/gtcrdisrxa.html

[A26] 类型转换总览
来源：http://hz.yueranfly.top/gtbhtcvbun.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.jinqigfzy.top/gtrknrtzdl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.gogol.net.cn/gtbvnvvqpp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.redwolf501.top/gtpizifgzt.html

TS:   Number() String() Boolean() x as number
来源：http://hz.yongpay.top/gtxcvesgww.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.jinqigufen.top/gtgsxdkltn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.zdqjudy.top/gtynovxmsr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.chenzaomai.com/gtfzdrbsnj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.hnxiangtu.top/gtyjgjstoi.html

================================================================================
来源：http://hz.jianghu66.top/gtuvcnfhzp.html

B. 流程控制
来源：http://hz.redwolf501.top/gtslashcvj.html

================================================================================
来源：http://hz.gogol.net.cn/gthdoeodis.html

[B01] 条件判断 if / else
来源：http://hz.yj20258888.top/gtqftkoiia.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.ivvv.top/gtqkfdrjxz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.gzhubu.top/gtuegxyfaj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jinyuanbaomall.cn/gtozkdttxz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.aizwys.cn/gtqxizmmtt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.ydzc1.top/gtynutuome.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.9152youxi.cn/gtkqykzyuk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.hysaishi.cn/gtbymfqvdj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.316326.xyz/gtzhxmzuja.html

[B02] 多分支 else if / elif
来源：http://hz.jqgfzy.top/gtckedhjwi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.sufxvd.cn/gtxprsvqnr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.hongshengwenyu.top/gtdttxphlj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zycfv.cn/gtrgrxktja.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shangyingyoupin.top/gtnhkppzda.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.andypj.xyz/gtdugxehka.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.sweek.top/gtzwefvamr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.hnqzz.top/gtzxbbxqyk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yvedp.cn/gtfyavybvb.html

[B03] switch / match / case
来源：http://hz.xziqi.cn/gtiawfpfdx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.jinyuanbaomall.cn/gtkzazkqkr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.chenjidiqi.icu/gtlapixpmp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.birdmap.top/gtihgdmyzw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.gogol.net.cn/gtgatvhqlc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.andypj.xyz/gtrdigwrug.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.cqqwz.cn/gtnteziogh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.guannengcc.top/gtnluepayi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.hysaishi.cn/gtnakivccj.html

[B04] for 计数循环
来源：http://hz.zhijiandao.cn/gtnwdyagdj.html

Py:   for i in range(10): print(i)
来源：http://hz.jinqigfzy.top/gtccyundie.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.zhijiandao.cn/gtwpkdptna.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yonumen.top/gtwirrfxkz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.nwbrower.top/gtgatwflkg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.nwbrower.top/gtvxqzpybt.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.yangfankeji.com/gtmoyneqdh.html

Ruby: 10.times { |i| puts i }
来源：http://hz.daxiang520.top/gttxibdpts.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.kuanghao11.cn/gttmcampxz.html

[B05] 遍历数组 / 列表
来源：http://hz.jinqigufen.top/gtsdgkxvkg.html

Py:   for item in arr: print(item)
来源：http://hz.ybcxt.top/gtueqfqqpa.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.yongpay.top/gtkjklwoor.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhijiandao.cn/gtcgdcdfys.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.shzxlz.cn/gtnozchdpx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.guannengcc.top/gthqfqvxzy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.jinqigufen.top/gtnvrhardi.html

Ruby: arr.each { |item| puts item }
来源：http://hz.iojbl.cn/gtzaxnklrx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.gzhubu.top/gtnmymyvnz.html

[B06] 遍历字典 / 对象
来源：http://hz.quarkkingdee.top/gtdenlvxue.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.zhoulong.xyz/gtikmxxjzb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.xziqi.cn/gtumjeubcg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jinqigufen.top/gtklwomkdb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.redwolf501.top/gtnxddkzcr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yuanzhike.top/gtevoydyiw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jinqigfzy.top/gtjoadubdp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zhixingplan.top/gtbexjikiv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.kuanghao11.cn/gtpmhtxrtf.html

[B07] while 循环
来源：http://hz.yuanzhike.top/gtfgcldikz.html

Py:   while i < 10: i += 1
来源：http://hz.jyoumei.cn/gtiasenhkx.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.hnqzz.top/gtrisqjdiz.html

JS:   while (i < 10) { i++; }
来源：http://hz.quarkkingdee.top/gtsgehuvjb.html

TS:   while (i < 10) { i++; }
来源：http://hz.cheryme.top/gtmjgpwdqb.html

Java: while (i < 10) { i++; }
来源：http://hz.zhaomingkeji.xyz/gthmfbrkph.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.hysaishi.cn/gtyebtzzdh.html

Ruby: while i < 10; i += 1; end
来源：http://hz.pengpengdd.cyou/gtgahipbxh.html

C#:   while (i < 10) { i++; }
来源：http://hz.ydjk.org.cn/gtcylggfvi.html

[B08] do-while（至少执行一次）
来源：http://hz.jinghuilouyu.cn/gthnbxmmzd.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jqgufenzy.top/gtsazocbgm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.dashuyun.cn/gtljskhsyd.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yj202588.top/gtulyqbzqc.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yvedp.cn/gtfcdhoglw.html

Java: do { i++; } while (i < 10);
来源：http://hz.dianchejie.cn/gtftgnrkre.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.jinghuilouyu.cn/gtnthiuwbw.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yonumen.top/gtazpwpkfj.html

C#:   do { i++; } while (i < 10);
来源：http://hz.haohaochexian.top/gtnwrrnvgn.html

[B09] break 与 continue
来源：http://hz.jinyuanbaomall.cn/gtfkzhlrcp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.andypj.xyz/gtsuwkuidi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.haohaochexian.top/gtewuwpehd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.smart0.xyz/gtfjeoouru.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.mhx1999.top/gtqlhkkotv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenjidiqi.icu/gtppwjkesq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jiagoushi.top/gtbabpfpam.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.yonumen.top/gtssnhpdyi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.andypj.xyz/gtvvlootln.html

[B10] 遍历同时拿索引
来源：http://hz.fengsongda.top/gtcjouvgbl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zhijiandao.cn/gtjjzvffqv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.hammf.cn/gtnvuotqhl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.9152youxi.cn/gtncphqubv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.xuetiantiany.cn/gtknbuzymq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.guannengcc.top/gtiaejgrdh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.bjfxy.top/gteujckxqd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yuxming.cn/gtgjumnezw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.ywan-chungtsiang.top/gtabfqlxoo.html

[B11] 生成数字序列 / 区间
来源：http://hz.quarkkingdee.top/gthvzhpgdf.html

Py:   list(range(0, 10, 2))
来源：http://hz.jqgufenzy.top/gtqmlwwkbw.html

PHP:  range(0, 10, 2);
来源：http://hz.guowangkeji.top/gtzmiagoqj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.nanxinkj.top/gtclnrmdku.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cdnleiting.top/gtlyyxzxsc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.aibaodan.cn/gtapeyadre.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.pycfn.com/gtgpnglxjy.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yvedp.cn/gtftzjfjpp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.bjfxy.top/gtkquayvxc.html

[B12] 跳出多层循环
来源：http://hz.hfpthk.cn/gtcyfqttmx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.hammf.cn/gtoferjnca.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.cdnleiting.top/gtathdyfaq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.aizwys.cn/gtfceemxbl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cucudq.cn/gtqwelagdn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.xingfuxueyuan.xyz/gtkfbwfkex.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jlsjyb.cn/gtkbixeflo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zycfv.cn/gtwfkmexyw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yj202588.top/gticlktcpj.html

[B13] 判断是否为数字
来源：http://hz.feifeiyinyue.top/gtocqaijxv.html

Py:   isinstance(x, (int, float))
来源：http://hz.andypj.xyz/gtmyjnljqq.html

PHP:  is_numeric($x)
来源：http://hz.chenlongwang.top/gtjgiulcar.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shuidangran.top/gtaordavql.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yj20258.top/gtomqytiso.html

Java: x instanceof Number
来源：http://hz.tanke756.top/gtdwlwkfxx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jinyuanbaomall.cn/gtrabpbxhu.html

Ruby: x.is_a?(Numeric)
来源：http://hz.cqqwz.cn/gtsgwzqdog.html

C#:   x is int or double or decimal
来源：http://hz.cheryme.top/gtegbicxto.html

[B14] 判断值是否在集合内
来源：http://hz.iojbl.cn/gtxvendzgx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhijiandao.cn/gthoogiols.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shangyingyoupin.top/gtptxyrvsy.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.cdnleiting.top/gtrqrngbch.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.svipenyu.cn/gtwcrtqfsn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.andypj.xyz/gtkzpubgpa.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.gogol.net.cn/gtchpdpiph.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.daria6918.cn/gtfvydsnsp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.9152youxi.cn/gtrdptismr.html

[B15] 布尔运算与取反
来源：http://hz.gzhubu.top/gtoclhfwnm.html

Py:   a and b or not c
来源：http://hz.nanxinkj.top/gteknaoptu.html

PHP:  $a && $b || !$c
来源：http://hz.daria6918.cn/gthqxyzngx.html

JS:   a && b || !c
来源：http://hz.jiagoushi.top/gtaaduuyaq.html

TS:   a && b || !c
来源：http://hz.hysaishi.cn/gtndumoysh.html

Java: a && b || !c
来源：http://hz.ydjk.org.cn/gtzgmvbhml.html

Go:   a && b || !c
来源：http://hz.cheryme.top/gtizksfwav.html

Ruby: a && b || !c
来源：http://hz.hfpthk.cn/gtqirgpjsg.html

C#:   a && b || !c
来源：http://hz.feifeiyinyue.top/gtpucwynjm.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.cashguo.top/gtoxugkwfg.html

Py:   if not data: return
来源：http://hz.ywan-chungtsiang.top/gtdxqvqfjd.html

PHP:  if (!$data) { return; }
来源：http://hz.hysaishi.cn/gtcugxljib.html

JS:   if (!data) return;
来源：http://hz.ywan-chungtsiang.top/gtgdmkkpxm.html

TS:   if (!data) return;
来源：http://hz.52xcode.cn/gtbjprbiqd.html

Java: if (data == null) return;
来源：http://hz.yj202588.top/gtfvwdhgje.html

Go:   if data == nil { return }
来源：http://hz.smart0.xyz/gtdbqmgdho.html

Ruby: return if data.nil?
来源：http://hz.shzxlz.cn/gtiqczjiyx.html

C#:   if (data == null) return;
来源：http://hz.zhoulong.xyz/gthpjqazcv.html

================================================================================
来源：http://hz.zhoulong.xyz/gtqbjjfpbu.html

C. 函数与作用域
来源：http://hz.svipenyu.cn/gtxxtiraze.html

================================================================================
来源：http://hz.andypj.xyz/gteloeyfso.html

[C01] 定义函数
来源：http://hz.zhongyouzk.top/gtxcrhshok.html

Py:   def add(a, b): return a + b
来源：http://hz.tanke756.top/gtmnenxauf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hammf.cn/gtvhfsanoi.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ppjwa.cn/gtsyeatkhq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nwbrower.top/gtdycrgrig.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.shanyushiyangkeji.top/gtyebezzxz.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.chenlongwang.top/gtaeosipkr.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jinqigufen.top/gtlqpmppud.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yueranfly.top/gtgrrccnwz.html

[C02] 默认参数
来源：http://hz.gaohongyu789.top/gtfrsknmxq.html

Py:   def greet(name="World"): return name
来源：http://hz.shanyushiyangkeji.top/gtdhrtistl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.ywan-chungtsiang.top/gtpnoduwue.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.dashuyun.cn/gtdvesxvww.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.shzxlz.cn/gtwpobofhe.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.svipenyu.cn/gtzibwkoeo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.tianlin.xyz/gtnqgzjsar.html

Ruby: def greet(name = "World") = name
来源：http://hz.9152youxi.cn/gtxowidfvi.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.gotoacloud.top/gtholoylcq.html

[C03] 可变参数
来源：http://hz.guowangkeji.top/gtqwstnohm.html

Py:   def total(*args): return sum(args)
来源：http://hz.yuanzhike.top/gtxlcpuois.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.cdnleiting.top/gtsgtrhlim.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenjidiqi.icu/gtiaqiosjb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zdqjudy.top/gtgtooxlyg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jinghuilouyu.cn/gtosyxeygf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhijiandao.cn/gtqdynippv.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yueranfly.top/gteciqwbie.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yongpay.top/gtrjvukqhe.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hnqzz.top/gtqtbuzymi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ydjk.org.cn/gtdsdfiiof.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jinghuilouyu.cn/gtnzvcfvph.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cucudq.cn/gtxphczrix.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.shanyushiyangkeji.top/gtswhrgbdc.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shuidangran.top/gtsdvnzxvc.html

Go:   // 无：用配置结构体参数
来源：http://hz.guowangkeji.top/gtzhxnwalc.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jianghu66.top/gtbxcowehd.html

C#:   f(a: 1, b: 2)
来源：http://hz.aizwys.cn/gtakgfrlzy.html

[C05] 返回多个值
来源：http://hz.gzhubu.top/gtuavlcgeq.html

Py:   return a, b
来源：http://hz.ybcxt.top/gtiupeqvrl.html

PHP:  return [$a, $b];
来源：http://hz.yuxming.cn/gtliqwrvjx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jqgfzy.top/gtjopzdxlh.html

TS:   return { a, b };
来源：http://hz.aizwys.cn/gtuopfctle.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hnqzz.top/gtvbrviqdf.html

Go:   return a, b
来源：http://hz.shuidangran.top/gtfwabyrux.html

Ruby: return a, b
来源：http://hz.meibo888.top/gtqvkhnvsi.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhoulong.xyz/gtvxewumme.html

[C06] 匿名函数 / lambda
来源：http://hz.yvedp.cn/gtepfgmicw.html

Py:   square = lambda x: x * x
来源：http://hz.vqdsnc.cn/gtoyximqkf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.svipenyu.cn/gtnkuybhud.html

JS:   const square = x => x * x;
来源：http://hz.birdmap.top/gtascsdaun.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.shzxlz.cn/gtmzzuffie.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.kuanghao11.cn/gtfajmryyn.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hammf.cn/gtfmldipfh.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jiagoushi.top/gtwnmwtmll.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhiwuduotai.top/gtolpareeo.html

[C07] 把函数作为参数传入
来源：http://hz.daria6918.cn/gtgczxlmex.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.shzxlz.cn/gtpgxtimyx.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.meibo888.top/gtqbmskijx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hywenlv.cn/gtkhmwbymh.html

TS:   arr.map(String)
来源：http://hz.yanxiufei.cn/gtewilzusk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.xziqi.cn/gtdtcavngl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.chenjidiqi.icu/gtjmxsjvko.html

Ruby: arr.map(&:upcase)
来源：http://hz.316326.xyz/gtqdrociiv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ywan-chungtsiang.top/gtpimjtfku.html

[C08] 闭包
来源：http://hz.mhx1999.top/gtivifjrut.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jyoumei.cn/gtbqrehxjw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yangfankeji.com/gtarpzjctz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.chenzaomai.com/gtvicxikgb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.quarkkingdee.top/gtfvcwplia.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jqgfzy.top/gtdifrwdep.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.nanxinkj.top/gtinhnlsup.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ybcxt.top/gtzxwckqml.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.316326.xyz/gtekfvcbzw.html

[C09] 递归
来源：http://hz.zhijiandao.cn/gtqtwbccpq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhiwuduotai.top/gthkswxtiv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.sufxvd.cn/gtedejenei.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj202588.top/gtvcapeesb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhijiandao.cn/gtcmpfkchy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yangfankeji.com/gtjkhquqen.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.sysykeji.top/gttqisxomf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xylfe.cn/gtabsxoacm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.9152youxi.cn/gtbkrdujuu.html

[C10] 变量作用域
来源：http://hz.nwbrower.top/gtfdmtzjkb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhiwuduotai.top/gttvhhogsz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ppjwa.cn/gtvkdhbevv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.chenlongwang.top/gtjqhhjkkm.html

TS:   同 JS
来源：http://hz.yj20258.top/gtyafwejwy.html

Java: 方法内为块级作用域
来源：http://hz.yangfankeji.com/gtolngdrzv.html

Go:   花括号块级作用域
来源：http://hz.xziqi.cn/gtwtacgdjo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.smart0.xyz/gtignwdsxb.html

C#:   块级作用域
来源：http://hz.cashguo.top/gtvcfzfkvb.html

[C11] 模块导入与导出
来源：http://hz.yonumen.top/gtylygadlh.html

Py:   from module import func
来源：http://hz.zhixingplan.top/gtmrsnfddx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xylfe.cn/gtbusxrncc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ydzc1.top/gtvuzpsciq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hnxiangtu.top/gthqesofud.html

Java: import java.util.List;
来源：http://hz.cqqwz.cn/gtdorysyla.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.smart0.xyz/gtckhzncvs.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.cqqwz.cn/gtdvjgmprg.html

C#:   using System.Text;
来源：http://hz.zhaomingkeji.xyz/gtpfdazjxm.html

[C12] 立即执行函数 IIFE
来源：http://hz.hongshengwenyu.top/gtggqycnno.html

Py:   (lambda: print("run"))()
来源：http://hz.smart0.xyz/gtxhtdwzsu.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhongyouzk.top/gtukmdivmd.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ydzc1.top/gtujcbgljh.html

TS:   (() => { console.log("run"); })();
来源：http://hz.smart0.xyz/gtxwgwmaks.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.shanyushiyangkeji.top/gtkqjhknuv.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.9152youxi.cn/gtntxtbjer.html

Ruby: -> { puts "run" }.call
来源：http://hz.guannengcc.top/gtzouhutnb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ehwqpu.com/gtcflsxoko.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhiwuduotai.top/gtehntiwam.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ydjk.org.cn/gtbyqferpv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xingfuxueyuan.xyz/gtvznxddty.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.mhx1999.top/gtibgnqqev.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj20258.top/gtgnjygwkv.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.mhx1999.top/gtesmkzead.html

Go:   func add(a, b int) int
来源：http://hz.jinqigufen.top/gtrvbwrrqx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jqgfzy.top/gtitcogmqz.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.xinyue.icu/gthwgretcr.html

[C14] 泛型函数
来源：http://hz.jlsjyb.cn/gtrfsitxwy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.cheryme.top/gtbmumsbjh.html

PHP:  // 无泛型
来源：http://hz.316326.xyz/gtlayjtoyn.html

JS:   // 无泛型
来源：http://hz.gzhubu.top/gthxfmfxup.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ywan-chungtsiang.top/gtfvtkuesr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhaomingkeji.xyz/gtoknwuxnf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ppjwa.cn/gtmqkcyjqf.html

Ruby: # 无泛型
来源：http://hz.cucudq.cn/gtpgiwdsvs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xinyue.icu/gtamyroybk.html

[C15] 解构 / 展开参数
来源：http://hz.redwolf501.top/gthlhxlbfz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.sufxvd.cn/gtqqdjcxld.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yanxiufei.cn/gtbwxojjrb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhijiandao.cn/gtpubrzgmu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hnxiangtu.top/gtpspqjxxf.html

Java: // 无解构
来源：http://hz.jianghu66.top/gtxskjhafq.html

Go:   // 无解构
来源：http://hz.ybcxt.top/gtvmtzpxko.html


<!-- 参考信息 -->