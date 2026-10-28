代发 wailian999

C#:   list.Reverse();
来源：http://hz.yj20258.top/gtrrtkjjto.html

[D12] 查找元素下标
来源：http://hz.jianghu66.top/gtpryrxnoa.html

Py:   arr.index(x);  x in arr
来源：http://hz.gogol.net.cn/gtyzvpecse.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.cucudq.cn/gtzkynhugg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.mhx1999.top/gtalcvodrf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shangyingyoupin.top/gtcvgswzdh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.nanxuanxn.top/gtqibjtpyj.html

Go:   slices.Index(arr, x)
来源：http://hz.meibo888.top/gtgbnlmfjl.html

Ruby: arr.index(x)
来源：http://hz.0kj1m.cn/gtccrwsxco.html

C#:   list.IndexOf(x);
来源：http://hz.aizwys.cn/gtqsgjfuab.html

[D13] 过滤（保留满足条件的）
来源：http://hz.vqdsnc.cn/gtlopbiusi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jiagoushi.top/gtqwwnyozt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xingfuxueyuan.xyz/gtwjdtterz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.snrcjt.cn/gtvyebuypr.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jiagoushi.top/gtgovadoic.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.iojbl.cn/gtptcbcaaz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.gaohongyu789.top/gtxacotony.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yongpay.top/gthcjlaawz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jianghu66.top/gtanousjrj.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jiagoushi.top/gtlsfqxxyr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zycfv.cn/gtsqxleyhu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zycfv.cn/gtugvixzhk.html

JS:   arr.map(x => x * 2)
来源：http://hz.hammf.cn/gtbajidbbx.html

TS:   arr.map(x => x * 2)
来源：http://hz.ehwqpu.com/gtfbvudull.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.sysykeji.top/gtoxdsqojs.html

Go:   // 手写循环
来源：http://hz.gogol.net.cn/gtrdxsmzdg.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.snrcjt.cn/gtqkdyvizu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.feifeiyinyue.top/gtsuntnpqa.html

[D15] 去重
来源：http://hz.aibaodan.cn/gtshfewmmq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.bjfxy.top/gtmdlxlshp.html

PHP:  array_unique($arr);
来源：http://hz.daxiang520.top/gthvjkdloa.html

JS:   [...new Set(arr)]
来源：http://hz.zhiwuduotai.top/gtzqakyrlw.html

TS:   [...new Set(arr)]
来源：http://hz.pycfn.com/gtkvuujpwx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jianghu66.top/gtpnywelmb.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.tian-w.cn/gtlbaojrmi.html

Ruby: arr.uniq
来源：http://hz.xylfe.cn/gtbstpxcrj.html

C#:   list.Distinct().ToList()
来源：http://hz.nwbrower.top/gtahfriuns.html

[D16] 求和与平均值
来源：http://hz.52xcode.cn/gtmolouxiz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.fzhhl.top/gtpxucfaro.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.fzhhl.top/gtikdbggig.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jlsjyb.cn/gtfilgwtyn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zycfv.cn/gtkcngbqqv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ydzc1.top/gtvwhlkedc.html

Go:   // 手写循环累加
来源：http://hz.iojbl.cn/gtgddfwxue.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ydzc1.top/gtkhhdsbnn.html

C#:   list.Sum();  list.Average()
来源：http://hz.yj202588.top/gthrocefes.html

[D17] 最大值与最小值
来源：http://hz.xinyue.icu/gttxzhgkct.html

Py:   max(arr);  min(arr)
来源：http://hz.havefunace.top/gtzkfuhdrt.html

PHP:  max($arr);  min($arr);
来源：http://hz.guowangkeji.top/gtzifriysp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zdqjudy.top/gtqzetjfrn.html

TS:   Math.max(...arr);
来源：http://hz.hysaishi.cn/gtezrfiajs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jianghu66.top/gtyabwflhh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zdqjudy.top/gtnforuqrj.html

Ruby: arr.max;  arr.min
来源：http://hz.svipenyu.cn/gtebhghjmg.html

C#:   list.Max();  list.Min()
来源：http://hz.jinqigfzy.top/gtrhfeqryu.html

[D18] 扁平化嵌套数组
来源：http://hz.nwbrower.top/gtvvekfhfl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hysaishi.cn/gtaqfoplrc.html

PHP:  array_merge(...$nested);
来源：http://hz.xylfe.cn/gttxlwgoxx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhongyouzk.top/gtuoazfboo.html

TS:   nested.flat();
来源：http://hz.dianchejie.cn/gtmuxyviiw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.tianlin.xyz/gtvshbjofy.html

Go:   // 手写双层循环
来源：http://hz.jianghu66.top/gtskdjuyae.html

Ruby: nested.flatten
来源：http://hz.jqgufenzy.top/gtvpedovrn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.smart0.xyz/gtkijypddh.html

[D19] 按字段分组
来源：http://hz.yongpay.top/gtmkcavxxy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yuxming.cn/gthmtzxajr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hongshengwenyu.top/gtzvjxfhco.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhiwuduotai.top/gtpxksausj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cqqwz.cn/gtverzkmuf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhongyouzk.top/gtqyxkksll.html

Go:   // 手写 map[string][]T
来源：http://hz.fzhhl.top/gtiqikxhan.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yonumen.top/gtpkxacipr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jinqigufen.top/gtvofuoxsf.html

[D20] 统计每个元素出现次数
来源：http://hz.iojbl.cn/gtwxaslrdc.html

Py:   Counter(arr)
来源：http://hz.chenjidiqi.icu/gttgfpspgc.html

PHP:  array_count_values($arr);
来源：http://hz.mhx1999.top/gtprkqhpra.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgfzy.top/gtdpxlvmto.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangtech.top/gtcsjshiqq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.svipenyu.cn/gtefzolsvu.html

Go:   // 手写 map[T]int
来源：http://hz.shanyushiyangtech.top/gtfabxgsiv.html

Ruby: arr.tally
来源：http://hz.yj202588.top/gtfeaonaqp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ydjk.org.cn/gtuldpmyzm.html

[D21] 判断是否包含某元素
来源：http://hz.chenjidiqi.icu/gtwgrvdvie.html

Py:   x in arr
来源：http://hz.redwolf501.top/gtpybukhfw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.sysykeji.top/gtqqegjcpr.html

JS:   arr.includes(x)
来源：http://hz.smart0.xyz/gttafoaulm.html

TS:   arr.includes(x)
来源：http://hz.0kj1m.cn/gtmdrcqrmk.html

Java: list.contains(x)
来源：http://hz.aizwys.cn/gtzmmgxvfg.html

Go:   slices.Contains(arr, x)
来源：http://hz.fengsongda.top/gtglhplanc.html

Ruby: arr.include?(x)
来源：http://hz.redwolf501.top/gtsfckzfxr.html

C#:   list.Contains(x)
来源：http://hz.yanxiufei.cn/gtvyfovvgq.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhaomingkeji.xyz/gtzfqdtlvd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xuanzx.com/gtsefecsyh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhengqikj.top/gtkdkuakzl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yvedp.cn/gtplxjdzhj.html

TS:   [...arr];
来源：http://hz.snrcjt.cn/gtxdtdplwv.html

Java: new ArrayList<>(list);
来源：http://hz.snrcjt.cn/gtiuzlgsnr.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinqigfzy.top/gtzzrmbsvh.html

Ruby: arr.dup;  arr.clone
来源：http://hz.shangyingyoupin.top/gtcmbqjton.html

C#:   new List<int>(list);
来源：http://hz.dashuyun.cn/gtkpnrtmeq.html

[D23] reduce 累积计算
来源：http://hz.tian-w.cn/gtgatohdle.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yonumen.top/gtuehufafv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.aibaodan.cn/gtvcwkgmik.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jianghu66.top/gtkiffqvxo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ywan-chungtsiang.top/gtosmbqjix.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.gaohongyu789.top/gtxxiagejz.html

Go:   // 手写循环
来源：http://hz.fengsongda.top/gtfvemzeju.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cqqwz.cn/gtwgdxtncv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ehwqpu.com/gtzmwolizm.html

[D24] 字典 / Map 基本操作
来源：http://hz.hongshengwenyu.top/gtbzevhmaj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xinyue.icu/gtujsfrmvh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xingfuxueyuan.xyz/gtdokdfywq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.guannengcc.top/gtuddambau.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.wangshuangyany.cn/gtxsfexydv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.andypj.xyz/gthevajlzg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shzxlz.cn/gtrswqbhgz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.sweek.top/gtqmivuycr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.sweek.top/gtxpgowgeh.html

[D25] Set 集合去重与交并差
来源：http://hz.jiagoushi.top/gtraozqofp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ehwqpu.com/gtzayajsaj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yuanzhike.top/gtvnnvajrh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.fzhhl.top/gttajukuwo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jqgufenzy.top/gtgrzgqvua.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.gogol.net.cn/gtsoyytzdc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.dianchejie.cn/gtfkcfsnpy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.gogol.net.cn/gtdsivzsdi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.dianchejie.cn/gthofyhepf.html

[D26] 数组转字符串
来源：http://hz.daxiang520.top/gtmjltbnzq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhiwuduotai.top/gtpermszxj.html

PHP:  implode(", ", $arr);
来源：http://hz.zhongyouzk.top/gtxxaylnrf.html

JS:   arr.join(", ")
来源：http://hz.pengpengdd.cyou/gtwjugvvud.html

TS:   arr.join(", ")
来源：http://hz.jlsjyb.cn/gtvykvuhmb.html

Java: String.join(", ", list)
来源：http://hz.birdmap.top/gtyjbdcxax.html

Go:   strings.Join(strs, ", ")
来源：http://hz.chenzaomai.com/gtllogzvcm.html

Ruby: arr.join(", ")
来源：http://hz.gotoacloud.top/gtwnahrtlm.html

C#:   string.Join(", ", list)
来源：http://hz.chenlongwang.top/gtwtyaxquu.html

================================================================================
来源：http://hz.yj20258.top/gtxkgqijvw.html

E. 字符串处理
来源：http://hz.sufxvd.cn/gtsctefpgr.html

================================================================================
来源：http://hz.tianlin.xyz/gttlncuxtv.html

[E01] 拼接字符串
来源：http://hz.hnxiangtu.top/gtjbeanjjd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.kuanghao11.cn/gtuhmrrvte.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhongyouzk.top/gtlkvjyqzo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.9152youxi.cn/gtasoqbwvf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.svipenyu.cn/gtoebmemcd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hysaishi.cn/gthcmdypxh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.snrcjt.cn/gtuqftgere.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.wangdashe.top/gtrmlnibrl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yangfankeji.com/gtlrcnyazf.html

[E02] 重复字符串
来源：http://hz.daxiang520.top/gtdjeulojv.html

Py:   "ab" * 3
来源：http://hz.ydzc1.top/gtgzettjcm.html

PHP:  str_repeat("ab", 3);
来源：http://hz.dianchejie.cn/gtndmjcirq.html

JS:   "ab".repeat(3)
来源：http://hz.ivvv.top/gttawhhswy.html

TS:   "ab".repeat(3)
来源：http://hz.redwolf501.top/gtxdkaknas.html

Java: "ab".repeat(3)
来源：http://hz.pycfn.com/gtbdvngswy.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.wangshuangyany.cn/gttxpjjlxq.html

Ruby: "ab" * 3
来源：http://hz.shangyingyoupin.top/gtqkmdlgaz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.gotoacloud.top/gtylzqvjmb.html

[E03] 截取子串
来源：http://hz.mhx1999.top/gthrkwvueq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ywan-chungtsiang.top/gtajmbcssk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xziqi.cn/gtuuxcmnii.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.hnqzz.top/gtkoshqhpq.html

TS:   s.slice(1, 4)
来源：http://hz.nwbrower.top/gtujydgkbm.html

Java: s.substring(1, 4)
来源：http://hz.sweek.top/gtxpprjcly.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.chenzaomai.com/gtrsfyvfpm.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zdqjudy.top/gtpmhwhgsz.html

C#:   s.Substring(1, 3)
来源：http://hz.yj202588.top/gtpjmxkjfd.html

[E04] 查找子串位置
来源：http://hz.gaohongyu789.top/gtqhohnwoy.html

Py:   s.find("x");  s.index("x")
来源：http://hz.havefunace.top/gtsktpgqwj.html

PHP:  strpos($s, "x");
来源：http://hz.shanyushiyangtech.top/gtwdrswovh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yangfankeji.com/gtvuholfgz.html

TS:   s.indexOf("x")
来源：http://hz.gaohongyu789.top/gtfhwevovq.html

Java: s.indexOf("x")
来源：http://hz.yj202588.top/gthuthjnay.html

Go:   strings.Index(s, "x")
来源：http://hz.sufxvd.cn/gtluqjgwvj.html

Ruby: s.index("x")
来源：http://hz.cqqwz.cn/gttohycxzm.html

C#:   s.IndexOf("x")
来源：http://hz.nanxuanxn.top/gtsaogehcd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yonumen.top/gtggbyubnm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yuanzhike.top/gtcuvpjsws.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.shanyushiyangkeji.top/gtoimmilxx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tanke756.top/gtrdmzknqt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ppjwa.cn/gtmgbtrtsy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xingfuxueyuan.xyz/gtqtbxwskc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xziqi.cn/gtjhqqamvn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jqgufenzy.top/gtirqgawsy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ydzc1.top/gtxzquihfb.html

[E06] 替换子串
来源：http://hz.gzhubu.top/gtjaurmfxw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jinyuanbaomall.cn/gtkssganzn.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.cashguo.top/gtafvpctwv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zycfv.cn/gthxmffrst.html

TS:   s.replaceAll("a", "b")
来源：http://hz.xylfe.cn/gtvroiuhpg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yuanzhike.top/gtbmumafpa.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.feifeiyinyue.top/gtiuygjayg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhiwuduotai.top/gtsadmmhju.html

C#:   s.Replace("a", "b")
来源：http://hz.meibo888.top/gtaibmndsu.html

[E07] 按分隔符拆分
来源：http://hz.jyoumei.cn/gtktzzghrk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.c1oappe.top/gtvinagcjl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yj20258888.top/gtzyomtskh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cashguo.top/gtkpvcgihs.html

TS:   s.split(",")
来源：http://hz.gotoacloud.top/gtclucyhxs.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ppjwa.cn/gtzkbuyilh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.gotoacloud.top/gtpaltvnov.html

Ruby: s.split(",");  s.split
来源：http://hz.cdnleiting.top/gthkanlvun.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhengqikj.top/gtkraarqsk.html

[E08] 数组按分隔符合并
来源：http://hz.gotoacloud.top/gtjozqqjum.html

Py:   ",".join(items)
来源：http://hz.aibaodan.cn/gtizzymbvf.html

PHP:  implode(",", $items);
来源：http://hz.pycfn.com/gthtesjjkp.html

JS:   items.join(",")
来源：http://hz.guowangkeji.top/gtvzjlpaai.html

TS:   items.join(",")
来源：http://hz.fzhhl.top/gtbteinixj.html

Java: String.join(",", items)
来源：http://hz.cdnleiting.top/gtcswsvkqb.html

Go:   strings.Join(items, ",")
来源：http://hz.hammf.cn/gtylikyuzp.html

Ruby: items.join(",")
来源：http://hz.wangshuangyany.cn/gthdgsxulv.html

C#:   string.Join(",", items)
来源：http://hz.ppjwa.cn/gtpakpzmfn.html

[E09] 去除所有空白字符
来源：http://hz.gotoacloud.top/gtyemdftwt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.pycfn.com/gthdcugotv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ivvv.top/gtugafgvyl.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.meibo888.top/gtdxpmpvor.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ydzc1.top/gtvsiciuqx.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.cdnleiting.top/gtsfljkfjj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jiagoushi.top/gtqrfgqyyr.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.cdnleiting.top/gtfhweyxpy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jqgufenzy.top/gtismsrulf.html

[E10] 左侧补零 / 定长填充
来源：http://hz.aizwys.cn/gthrkhgnoi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.gaohongyu789.top/gtwfojbrev.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hnxiangtu.top/gtshvxgmuv.html

JS:   "7".padStart(3, "0")
来源：http://hz.jinqigufen.top/gtcxvihgsf.html

TS:   "7".padStart(3, "0")
来源：http://hz.sysykeji.top/gtvuecfzeq.html

Java: String.format("%03d", 7)
来源：http://hz.zdqjudy.top/gtiacveabx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shuidangran.top/gtoyufxpau.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.chenjidiqi.icu/gtmwsxeicp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.guowangkeji.top/gthjaeangk.html

[E11] 反转字符串
来源：http://hz.hongshengwenyu.top/gtgwxefsxh.html

Py:   s[::-1]
来源：http://hz.daxiang520.top/gtdufdjkmu.html

PHP:  strrev($s);
来源：http://hz.tanke756.top/gtkyoghwly.html

JS:   [...s].reverse().join("")
来源：http://hz.cashguo.top/gtyhcxtimk.html

TS:   [...s].reverse().join("")
来源：http://hz.c1oappe.top/gtvljmnxos.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xylfe.cn/gtgfiedklu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhixingplan.top/gtrpkdyojx.html

Ruby: s.reverse
来源：http://hz.gaohongyu789.top/gthazkrcey.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hnxiangtu.top/gtbgkhfjzs.html

[E12] 统计某字符出现次数
来源：http://hz.c1oappe.top/gttxeckfnq.html

Py:   s.count("a")
来源：http://hz.hnxiangtu.top/gtrmtkuybb.html

PHP:  substr_count($s, "a");
来源：http://hz.dashuyun.cn/gtmftvmrpq.html

JS:   s.split("a").length - 1
来源：http://hz.bjfxy.top/gtsqbcnuuc.html

TS:   s.split("a").length - 1
来源：http://hz.smart0.xyz/gtiqbzheml.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jqgufenzy.top/gtfiyjdsos.html

Go:   strings.Count(s, "a")
来源：http://hz.xuetiantiany.cn/gtuqhyecvp.html

Ruby: s.count("a")
来源：http://hz.shanyushiyangtech.top/gtyhxrwcsp.html

C#:   s.Count(c => c == 'a')
来源：http://hz.gotoacloud.top/gtuwphpnap.html

[E13] 逐字符遍历
来源：http://hz.jyoumei.cn/gtcbjhhqqr.html

Py:   for ch in s: print(ch)
来源：http://hz.chenzaomai.com/gtyqbdbarv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.fengsongda.top/gtszhmejxi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.redwolf501.top/gtctwiiqsg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.haohaochexian.top/gtknbwpegq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yongpay.top/gtqfhjyfvk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hnxiangtu.top/gtsqtknrxl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.meibo888.top/gtjnhcjrct.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yonumen.top/gtdwphtxiz.html

[E14] URL 编码与 Base64
来源：http://hz.nanxuanxn.top/gtsueqdnar.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhiwuduotai.top/gtcifegkaw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.gzhubu.top/gtujgaauiv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shuidangran.top/gtvbaulwmc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jqgufenzy.top/gtzvftzzfh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hammf.cn/gtgsqdmyxn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.chenjidiqi.icu/gtixfjplxj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ivvv.top/gtehczsuqc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cashguo.top/gtbqwihrjo.html

[E15] HTML 转义 / 反转义
来源：http://hz.tanke756.top/gtehluuhzy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ybcxt.top/gtplqqudjx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yj20258888.top/gtqklwxorb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.iojbl.cn/gtedinzvjh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.daria6918.cn/gtaucqwbjy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.cucudq.cn/gtbrpvfefq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.pengpengdd.cyou/gturdzbhyt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.snrcjt.cn/gtbndcnbhh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.pengpengdd.cyou/gtimwpcwtv.html

[E16] 数字千分位
来源：http://hz.yonumen.top/gtlbpkndya.html

Py:   f"{1234567:,}"
来源：http://hz.guannengcc.top/gtpghinpko.html

PHP:  number_format(1234567);
来源：http://hz.yangfankeji.com/gtyayuuxtr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuanzhike.top/gtvwkkujle.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.c1oappe.top/gtgaknllqr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hysaishi.cn/gtsjxhvoza.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yj20258888.top/gtfembwdje.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jqgfzy.top/gtobhwguad.html

C#:   1234567.ToString("N0")
来源：http://hz.mhx1999.top/gtmuabphnz.html

[E17] 首字母大写
来源：http://hz.ywan-chungtsiang.top/gtktgoskca.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.9152youxi.cn/gtzzfygekq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.aibaodan.cn/gtgncvcpwd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenlongwang.top/gtejgpafoh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gzhubu.top/gteqsqxbxa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ppjwa.cn/gtmpwnrver.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yuxming.cn/gteoufpcgb.html

Ruby: s.capitalize
来源：http://hz.hnxiangtu.top/gtrzmlntgp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.chenjidiqi.icu/gtklmzwhnx.html

[E18] 模板占位符替换
来源：http://hz.yvedp.cn/gtvgaarhab.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xingfuxueyuan.xyz/gtkbjjkfjo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jiagoushi.top/gtykztrwrb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.dashuyun.cn/gttsrykygk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xingfuxueyuan.xyz/gtznbthrtz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.nwbrower.top/gtpzyqlzsv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.c1oappe.top/gtkhfozlro.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.chenlongwang.top/gtzofoexqv.html


<!-- 参考信息 -->