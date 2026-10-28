代发 wailian999

C#:   list.Reverse();
来源：http://hz.nanxinkj.top/gtbmzrqfmf.html

[D12] 查找元素下标
来源：http://hz.hnqzz.top/gtvvtvrjfu.html

Py:   arr.index(x);  x in arr
来源：http://hz.xingfuxueyuan.xyz/gtjzodkxhz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zdqjudy.top/gtrikumnvu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hongshengwenyu.top/gtxsbxlfav.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yvedp.cn/gtwdatwbqe.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xuanzx.com/gtdzkakkpl.html

Go:   slices.Index(arr, x)
来源：http://hz.chenjidiqi.icu/gtykprvpxc.html

Ruby: arr.index(x)
来源：http://hz.fzhhl.top/gtgwzggyst.html

C#:   list.IndexOf(x);
来源：http://hz.yvedp.cn/gtvdbbqqlm.html

[D13] 过滤（保留满足条件的）
来源：http://hz.shangyingyoupin.top/gtshbyvgig.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gogol.net.cn/gtetpkbjvz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.tian-w.cn/gtdhlnxlkt.html

JS:   arr.filter(x => x > 3)
来源：http://hz.cqqwz.cn/gttjlaxsfl.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ppjwa.cn/gtzbkqyyjs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.smart0.xyz/gttokrizbv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.daria6918.cn/gtyllolpsm.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.vqdsnc.cn/gteyctlswy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.pycfn.com/gtjtenthct.html

[D14] 映射转换（每个元素变形）
来源：http://hz.kuanghao11.cn/gtnkqulclv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.daxiang520.top/gtdxrwhyav.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ppjwa.cn/gtqsjicsjt.html

JS:   arr.map(x => x * 2)
来源：http://hz.pycfn.com/gtmsoxtlfy.html

TS:   arr.map(x => x * 2)
来源：http://hz.smart0.xyz/gtuyvxfany.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jinyuanbaomall.cn/gtzpfqbftz.html

Go:   // 手写循环
来源：http://hz.gogol.net.cn/gtnlujxgqg.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hnxiangtu.top/gtxqeabwtn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jianghu66.top/gtffdmnbcc.html

[D15] 去重
来源：http://hz.tianlin.xyz/gthouqiumk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zycfv.cn/gtmzauymda.html

PHP:  array_unique($arr);
来源：http://hz.yvedp.cn/gtvaggvcyd.html

JS:   [...new Set(arr)]
来源：http://hz.tianlin.xyz/gtfrmdlnia.html

TS:   [...new Set(arr)]
来源：http://hz.gogol.net.cn/gthzhhyulk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jqgfzy.top/gtyxhebcox.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.tianlin.xyz/gtxfntbhjn.html

Ruby: arr.uniq
来源：http://hz.jqgfzy.top/gturxyaiwh.html

C#:   list.Distinct().ToList()
来源：http://hz.jinghuilouyu.cn/gtnxqltomz.html

[D16] 求和与平均值
来源：http://hz.cdnleiting.top/gtbimuwrvb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhiwuduotai.top/gtsnynqbar.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jlsjyb.cn/gtzjgfisah.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhiwuduotai.top/gtvocohfyz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.daria6918.cn/gtugwkqqgk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jlsjyb.cn/gtevxceyzh.html

Go:   // 手写循环累加
来源：http://hz.tian-w.cn/gtbgrqdzta.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.fengsongda.top/gtknzdbwoa.html

C#:   list.Sum();  list.Average()
来源：http://hz.0kj1m.cn/gtfwfocmrd.html

[D17] 最大值与最小值
来源：http://hz.dianchejie.cn/gtagfhojkc.html

Py:   max(arr);  min(arr)
来源：http://hz.zhijiandao.cn/gtoaqjpcrf.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhongyouzk.top/gttxfdhtst.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.pengpengdd.cyou/gtslwfzgom.html

TS:   Math.max(...arr);
来源：http://hz.cheryme.top/gtohjwwkbq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.svipenyu.cn/gtcmpqoqia.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hfpthk.cn/gtdixmhwyk.html

Ruby: arr.max;  arr.min
来源：http://hz.hammf.cn/gtersckufh.html

C#:   list.Max();  list.Min()
来源：http://hz.hongshengwenyu.top/gtgrsoexzq.html

[D18] 扁平化嵌套数组
来源：http://hz.ywan-chungtsiang.top/gteaseuiam.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jqgufenzy.top/gteoiysndf.html

PHP:  array_merge(...$nested);
来源：http://hz.daxiang520.top/gtuptigjob.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yueranfly.top/gttybvxpav.html

TS:   nested.flat();
来源：http://hz.cheryme.top/gtvseapaac.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ywan-chungtsiang.top/gtmlfvowgo.html

Go:   // 手写双层循环
来源：http://hz.hnqzz.top/gtoustxvzj.html

Ruby: nested.flatten
来源：http://hz.aizwys.cn/gtuykfdkkh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.tianlin.xyz/gtvlkkdfsr.html

[D19] 按字段分组
来源：http://hz.yanxiufei.cn/gtmtbsxpot.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.c1oappe.top/gtefhmpjgx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.tian-w.cn/gtifbvszez.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.nwbrower.top/gtornyhfqq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xuetiantiany.cn/gtslxpcrgt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhijiandao.cn/gtavnpzhnx.html

Go:   // 手写 map[string][]T
来源：http://hz.hysaishi.cn/gthsnfugjm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ehwqpu.com/gtyoavmyuq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cheryme.top/gttfkwbsqw.html

[D20] 统计每个元素出现次数
来源：http://hz.kuanghao11.cn/gtbkteaggs.html

Py:   Counter(arr)
来源：http://hz.fengsongda.top/gtbccbzwnj.html

PHP:  array_count_values($arr);
来源：http://hz.gotoacloud.top/gtsxdpwohx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.iojbl.cn/gtbhlxzajm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinyuanbaomall.cn/gtheqpfvzj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jinyuanbaomall.cn/gtcpubwuqc.html

Go:   // 手写 map[T]int
来源：http://hz.chenzaomai.com/gtgytaixvh.html

Ruby: arr.tally
来源：http://hz.gaohongyu789.top/gttqlunpxp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.fengsongda.top/gtajfhesyo.html

[D21] 判断是否包含某元素
来源：http://hz.yangfankeji.com/gtqzzwidce.html

Py:   x in arr
来源：http://hz.guowangkeji.top/gtnvozpdtw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.feifeiyinyue.top/gtgvvzzfde.html

JS:   arr.includes(x)
来源：http://hz.jlsjyb.cn/gtcipgehpo.html

TS:   arr.includes(x)
来源：http://hz.hnqzz.top/gtzbmedjof.html

Java: list.contains(x)
来源：http://hz.zhixingplan.top/gtolplvzxh.html

Go:   slices.Contains(arr, x)
来源：http://hz.jinghuilouyu.cn/gterwxjwhm.html

Ruby: arr.include?(x)
来源：http://hz.9152youxi.cn/gtpwoopkch.html

C#:   list.Contains(x)
来源：http://hz.shuidangran.top/gtkbsfdrvl.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cheryme.top/gtldbyujbg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.vqdsnc.cn/gthbhpaava.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.mhx1999.top/gtanapusqg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.snrcjt.cn/gtrcakpnwm.html

TS:   [...arr];
来源：http://hz.hnxiangtu.top/gtztcpwnwz.html

Java: new ArrayList<>(list);
来源：http://hz.sweek.top/gtkeqtdroh.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yuxming.cn/gtgsxoujcp.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xylfe.cn/gtwktfcrdj.html

C#:   new List<int>(list);
来源：http://hz.hywenlv.cn/gtjhzyzxtf.html

[D23] reduce 累积计算
来源：http://hz.aizwys.cn/gtbrmtufwa.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ydjk.org.cn/gtmxotkpfl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.smart0.xyz/gtmhovevjp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hysaishi.cn/gtwosubotm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.redwolf501.top/gtxmgmhtfq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.9152youxi.cn/gtzqmseyng.html

Go:   // 手写循环
来源：http://hz.xuanzx.com/gtkxcpvzvb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yj20258.top/gtdfaeoofs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yueranfly.top/gtrueytgtz.html

[D24] 字典 / Map 基本操作
来源：http://hz.wangdashe.top/gtrbukffkh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hammf.cn/gtnjgorgjh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.fengsongda.top/gteaqmdeui.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhaomingkeji.xyz/gtpckdwgam.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shanyushiyangkeji.top/gtwakybxig.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.mhx1999.top/gthvjcnlsj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xingfuxueyuan.xyz/gtuyhholuo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.dianchejie.cn/gtpprsekzq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhengqikj.top/gtivitqhog.html

[D25] Set 集合去重与交并差
来源：http://hz.yj20258.top/gtreuseylx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xinyue.icu/gtldxqpfxb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.tian-w.cn/gtsaxjrrav.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jianghu66.top/gtljpnxmel.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhongyouzk.top/gtsrducpsz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.nwbrower.top/gtkqdtwwff.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.nwbrower.top/gteaswbjqx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ybcxt.top/gtbljmwhiq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.iojbl.cn/gtulhhdfqp.html

[D26] 数组转字符串
来源：http://hz.zhoulong.xyz/gtnyzkjlft.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhiwuduotai.top/gtebscbdvw.html

PHP:  implode(", ", $arr);
来源：http://hz.xuanzx.com/gtzfcymjhl.html

JS:   arr.join(", ")
来源：http://hz.yvedp.cn/gtonmcauyl.html

TS:   arr.join(", ")
来源：http://hz.zhaomingkeji.xyz/gtkyufsbma.html

Java: String.join(", ", list)
来源：http://hz.hammf.cn/gtciyfgxku.html

Go:   strings.Join(strs, ", ")
来源：http://hz.sufxvd.cn/gtvnacerbx.html

Ruby: arr.join(", ")
来源：http://hz.zhongyouzk.top/gtlaabqetd.html

C#:   string.Join(", ", list)
来源：http://hz.iojbl.cn/gtmcswstpn.html

================================================================================
来源：http://hz.guowangkeji.top/gtsmilyigk.html

E. 字符串处理
来源：http://hz.ydzc1.top/gtevqyitcw.html

================================================================================
来源：http://hz.snrcjt.cn/gtgfiajbad.html

[E01] 拼接字符串
来源：http://hz.zhijiandao.cn/gtlremjwam.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ehwqpu.com/gtejidsbpx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jinghuilouyu.cn/gtwvkwnokr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhiwuduotai.top/gtxwpknlrn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.aibaodan.cn/gtlwmngvzx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.bjfxy.top/gtgthgybsc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xziqi.cn/gtavskkejo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jinyuanbaomall.cn/gtlyewlfww.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.wangdashe.top/gtumfotyjp.html

[E02] 重复字符串
来源：http://hz.meibo888.top/gtvoldfiyi.html

Py:   "ab" * 3
来源：http://hz.ivvv.top/gtvffrrnpy.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ydzc1.top/gtvbwtivkg.html

JS:   "ab".repeat(3)
来源：http://hz.iojbl.cn/gtveovasfs.html

TS:   "ab".repeat(3)
来源：http://hz.smart0.xyz/gtzmhdjndd.html

Java: "ab".repeat(3)
来源：http://hz.dashuyun.cn/gtlzarlqoo.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yonumen.top/gtotliolip.html

Ruby: "ab" * 3
来源：http://hz.jianghu66.top/gtolwkbmfy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.c1oappe.top/gtaizbixqn.html

[E03] 截取子串
来源：http://hz.nanxinkj.top/gtvmhsvhqz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.svipenyu.cn/gtqxtncarr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ehwqpu.com/gtoctcjloh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ivvv.top/gtrzmyheor.html

TS:   s.slice(1, 4)
来源：http://hz.jinyuanbaomall.cn/gtznsfnzpk.html

Java: s.substring(1, 4)
来源：http://hz.pengpengdd.cyou/gtomxppqny.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.52xcode.cn/gtepjxzqyt.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.feifeiyinyue.top/gtaqivnfpl.html

C#:   s.Substring(1, 3)
来源：http://hz.ydzc1.top/gtokclhkeq.html

[E04] 查找子串位置
来源：http://hz.jqgfzy.top/gtbixlbfyl.html

Py:   s.find("x");  s.index("x")
来源：http://hz.bjfxy.top/gtcwjbipwb.html

PHP:  strpos($s, "x");
来源：http://hz.c1oappe.top/gttylqrmec.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jlsjyb.cn/gtvdvsqtbx.html

TS:   s.indexOf("x")
来源：http://hz.jinqigufen.top/gtjrrtrcoj.html

Java: s.indexOf("x")
来源：http://hz.cqqwz.cn/gtqjiodlef.html

Go:   strings.Index(s, "x")
来源：http://hz.kuanghao11.cn/gtvoevjdka.html

Ruby: s.index("x")
来源：http://hz.0kj1m.cn/gtlukobybz.html

C#:   s.IndexOf("x")
来源：http://hz.jqgufenzy.top/gtezcwxyoz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.316326.xyz/gtvpzkbchj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.sweek.top/gtzkvdztyv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.cucudq.cn/gtqjzubhdr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tanke756.top/gtmlvpibqo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yj20258888.top/gtwrxgddxj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shzxlz.cn/gtpercrtpi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.chenlongwang.top/gtgyjumzuq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ivvv.top/gtsmpnmkst.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yj202588.top/gtfasiugjd.html

[E06] 替换子串
来源：http://hz.wangshuangyany.cn/gtevkrqlku.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jqgfzy.top/gtmvxtngfa.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yangfankeji.com/gtoqzaxmcz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yuxming.cn/gtslraxlbt.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yj20258888.top/gtyljehxzp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.mhx1999.top/gtdmwrckqx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ydjk.org.cn/gtwnvrifwp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.fzhhl.top/gtbavxhsnj.html

C#:   s.Replace("a", "b")
来源：http://hz.fzhhl.top/gtttyrpaxc.html

[E07] 按分隔符拆分
来源：http://hz.xuetiantiany.cn/gtzuclcrel.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.meibo888.top/gtjfoosarl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.bjfxy.top/gtctbxkdoy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shuidangran.top/gtinkikuvx.html

TS:   s.split(",")
来源：http://hz.daxiang520.top/gtokqpvkju.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shanyushiyangkeji.top/gtdhyypvhi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.kuanghao11.cn/gtffthwyjs.html

Ruby: s.split(",");  s.split
来源：http://hz.ybcxt.top/gtoblbrwiz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.daxiang520.top/gtrkbxtnlw.html

[E08] 数组按分隔符合并
来源：http://hz.cucudq.cn/gtuljvyiwn.html

Py:   ",".join(items)
来源：http://hz.hfpthk.cn/gtctedtqvo.html

PHP:  implode(",", $items);
来源：http://hz.zhongyouzk.top/gtfelsadsr.html

JS:   items.join(",")
来源：http://hz.ybcxt.top/gtymldgcsz.html

TS:   items.join(",")
来源：http://hz.sxryk.cn/gtziivlssu.html

Java: String.join(",", items)
来源：http://hz.jinqigfzy.top/gtukihgqxy.html

Go:   strings.Join(items, ",")
来源：http://hz.ybcxt.top/gtbentyesm.html

Ruby: items.join(",")
来源：http://hz.chenzaomai.com/gtgemilwlv.html

C#:   string.Join(",", items)
来源：http://hz.mhx1999.top/gttubbozgn.html

[E09] 去除所有空白字符
来源：http://hz.c1oappe.top/gtdneeviem.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhaomingkeji.xyz/gtktmraurv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yvedp.cn/gtykqapvlq.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.andypj.xyz/gtyjjedqpl.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.nanxuanxn.top/gtcxmvscxh.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jqgfzy.top/gtcpxsjems.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yangfankeji.com/gtfrpryshi.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jlsjyb.cn/gtphupjicf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hywenlv.cn/gtrrxmwfph.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xziqi.cn/gtahcannnv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hnxiangtu.top/gtoqzjjtpo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.fzhhl.top/gtapxizomm.html

JS:   "7".padStart(3, "0")
来源：http://hz.fengsongda.top/gtcjpzchyk.html

TS:   "7".padStart(3, "0")
来源：http://hz.ehwqpu.com/gthjvndlpj.html

Java: String.format("%03d", 7)
来源：http://hz.jyoumei.cn/gtfmxzpjnb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhaomingkeji.xyz/gtlboauzdu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jinghuilouyu.cn/gtzzhqltja.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.tanke756.top/gtnflsbveh.html

[E11] 反转字符串
来源：http://hz.c1oappe.top/gtrthpesna.html

Py:   s[::-1]
来源：http://hz.sysykeji.top/gtwzeylldl.html

PHP:  strrev($s);
来源：http://hz.jiagoushi.top/gtcujzlaua.html

JS:   [...s].reverse().join("")
来源：http://hz.ydjk.org.cn/gtaozxoqxa.html

TS:   [...s].reverse().join("")
来源：http://hz.iojbl.cn/gtbutzlced.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ydzc1.top/gtvtyjnnik.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ydjk.org.cn/gtjiosplnz.html

Ruby: s.reverse
来源：http://hz.xingfuxueyuan.xyz/gteesqrqwn.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yonumen.top/gtevtfhxgn.html

[E12] 统计某字符出现次数
来源：http://hz.zhongyouzk.top/gtycadewvr.html

Py:   s.count("a")
来源：http://hz.snrcjt.cn/gtbjcsilsq.html

PHP:  substr_count($s, "a");
来源：http://hz.hysaishi.cn/gtdyrmygpb.html

JS:   s.split("a").length - 1
来源：http://hz.jyoumei.cn/gtemnmndfa.html

TS:   s.split("a").length - 1
来源：http://hz.yangfankeji.com/gtkmxgfvzw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.smart0.xyz/gtsxihcqxb.html

Go:   strings.Count(s, "a")
来源：http://hz.chenlongwang.top/gtuobifziq.html

Ruby: s.count("a")
来源：http://hz.chenlongwang.top/gtdbqoxztk.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhongyouzk.top/gtqqsnjxbq.html

[E13] 逐字符遍历
来源：http://hz.sweek.top/gtzgtpvtzo.html

Py:   for ch in s: print(ch)
来源：http://hz.zhoulong.xyz/gtrekwzwyp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.quarkkingdee.top/gtlgqvosza.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xylfe.cn/gttxtrwiwt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shanyushiyangtech.top/gtbzhklmrn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinyuanbaomall.cn/gtkzrmubme.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xinyue.icu/gtqwdkpjgn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jyoumei.cn/gtmvtynjix.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.gaohongyu789.top/gtuozkemps.html

[E14] URL 编码与 Base64
来源：http://hz.iojbl.cn/gtthvomaok.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.c1oappe.top/gttprtcctm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.andypj.xyz/gtargktjvh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.aibaodan.cn/gtxgjphobz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jiagoushi.top/gtdeeeqzxr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.svipenyu.cn/gtavxfmdrt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.sweek.top/gtrkysdnuz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.9152youxi.cn/gtlllprwms.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.dianchejie.cn/gtafqmjhyt.html

[E15] HTML 转义 / 反转义
来源：http://hz.fengsongda.top/gtwfpvvbzi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cucudq.cn/gtmzsznsuk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.dianchejie.cn/gtzknpbzfm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.shanyushiyangkeji.top/gtrtlssxqc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.0kj1m.cn/gtjskwozkq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jinqigufen.top/gtxfmoovco.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xylfe.cn/gtbeibsvgg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hfpthk.cn/gtkgkkkcpa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.gaohongyu789.top/gtipkvxsce.html

[E16] 数字千分位
来源：http://hz.daria6918.cn/gtnxvhvjzh.html

Py:   f"{1234567:,}"
来源：http://hz.hysaishi.cn/gtmvnvepdy.html

PHP:  number_format(1234567);
来源：http://hz.daxiang520.top/gtadvswgsi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.c1oappe.top/gtikrvfvot.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydzc1.top/gtqqnnzcvr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ywan-chungtsiang.top/gtwgduilwm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhiwuduotai.top/gtgdduepnw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.vqdsnc.cn/gtiweynbaw.html

C#:   1234567.ToString("N0")
来源：http://hz.birdmap.top/gtpfvsjedq.html

[E17] 首字母大写
来源：http://hz.yj20258.top/gtcmwzwgru.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.daxiang520.top/gteglavwhs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yvedp.cn/gtxizgmmem.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinqigufen.top/gtckfghwbb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zycfv.cn/gtnfxkehki.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shanyushiyangkeji.top/gtdgxcdhbm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ydzc1.top/gtngiinstk.html

Ruby: s.capitalize
来源：http://hz.jqgufenzy.top/gtdplwcnxz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jyoumei.cn/gtlwistnij.html

[E18] 模板占位符替换
来源：http://hz.yangfankeji.com/gtmfcgmkkk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shanyushiyangkeji.top/gtefpcuemz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.0kj1m.cn/gtktmvkqtz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinghuilouyu.cn/gtkiikpztu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinqigufen.top/gtvgegkipu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.cucudq.cn/gtcfkwwcky.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.cdnleiting.top/gtleohcuua.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xuetiantiany.cn/gttjwfcsvi.html


<!-- 参考信息 -->