代发 wailian999

Ruby: arr.index(x)
来源：http://hz.c1oappe.top/gtzizperal.html

C#:   list.IndexOf(x);
来源：http://hz.yuanzhike.top/gtqajakogr.html

[D13] 过滤（保留满足条件的）
来源：http://hz.tianlin.xyz/gtvzkpaweg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.52xcode.cn/gtosqqqszo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.tian-w.cn/gtdejelnvz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xinyue.icu/gtuyhoqhzq.html

TS:   arr.filter(x => x > 3)
来源：http://hz.dashuyun.cn/gtqitirrap.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.guowangkeji.top/gtmjnobmfu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zycfv.cn/gtrxipwult.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ydzc1.top/gtkceuqfzk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yj20258.top/gtzzpchgsv.html

[D14] 映射转换（每个元素变形）
来源：http://hz.birdmap.top/gtirotcfok.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jinqigufen.top/gtzcecxxec.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.sweek.top/gtylgxdssn.html

JS:   arr.map(x => x * 2)
来源：http://hz.chenzaomai.com/gtuagjivji.html

TS:   arr.map(x => x * 2)
来源：http://hz.pycfn.com/gtbbyjfqpv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.sufxvd.cn/gtamejaztr.html

Go:   // 手写循环
来源：http://hz.wangdashe.top/gtjriqkheb.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jiagoushi.top/gtfqhqvsza.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hnqzz.top/gtzbrlwwec.html

[D15] 去重
来源：http://hz.cucudq.cn/gtgujiwytr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.redwolf501.top/gtqpjbkcsu.html

PHP:  array_unique($arr);
来源：http://hz.kuanghao11.cn/gtaivzcbvk.html

JS:   [...new Set(arr)]
来源：http://hz.sweek.top/gtrzucnenc.html

TS:   [...new Set(arr)]
来源：http://hz.yj20258.top/gtjeqciwsy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.daxiang520.top/gtogdsruvp.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hywenlv.cn/gttlwnxpwj.html

Ruby: arr.uniq
来源：http://hz.zhoulong.xyz/gteaycxhio.html

C#:   list.Distinct().ToList()
来源：http://hz.hongshengwenyu.top/gteswucotp.html

[D16] 求和与平均值
来源：http://hz.tian-w.cn/gtorvcmqsz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.cheryme.top/gtfyybwvxg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.aizwys.cn/gtkhqunzxm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.havefunace.top/gtmoldbkhc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shuidangran.top/gtzdgrglqy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jiagoushi.top/gtfeevlskd.html

Go:   // 手写循环累加
来源：http://hz.gaohongyu789.top/gtrekgmuzc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yangfankeji.com/gtgrvfcvce.html

C#:   list.Sum();  list.Average()
来源：http://hz.xylfe.cn/gtmigpoqse.html

[D17] 最大值与最小值
来源：http://hz.tian-w.cn/gtcweetufv.html

Py:   max(arr);  min(arr)
来源：http://hz.0kj1m.cn/gtwojjafke.html

PHP:  max($arr);  min($arr);
来源：http://hz.xylfe.cn/gtjeouvcza.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.dianchejie.cn/gtipyibgjw.html

TS:   Math.max(...arr);
来源：http://hz.yongpay.top/gtipvkbgua.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.smart0.xyz/gtrhnumdyb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhengqikj.top/gtmxevwnjw.html

Ruby: arr.max;  arr.min
来源：http://hz.zhengqikj.top/gtytvszukv.html

C#:   list.Max();  list.Min()
来源：http://hz.sweek.top/gtesgedjmk.html

[D18] 扁平化嵌套数组
来源：http://hz.yj20258888.top/gtujidpnbx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhijiandao.cn/gtiwtoqhkl.html

PHP:  array_merge(...$nested);
来源：http://hz.yonumen.top/gtknbwxwhy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.redwolf501.top/gthheytfpd.html

TS:   nested.flat();
来源：http://hz.gaohongyu789.top/gtogrhddnx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.xziqi.cn/gtrlfeycvp.html

Go:   // 手写双层循环
来源：http://hz.ehwqpu.com/gtciofvvvg.html

Ruby: nested.flatten
来源：http://hz.quarkkingdee.top/gtdrnzqhrj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yongpay.top/gtrglyyjnj.html

[D19] 按字段分组
来源：http://hz.hammf.cn/gtmuzkdizv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cucudq.cn/gtyvkypdgb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.sxryk.cn/gtlzioglrn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xylfe.cn/gtgvribawb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.c1oappe.top/gtjvnnvmpu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.daxiang520.top/gtylrhlwly.html

Go:   // 手写 map[string][]T
来源：http://hz.zhiwuduotai.top/gtpqkxjqml.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhijiandao.cn/gtbjqlqqqy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ivvv.top/gtfostjriw.html

[D20] 统计每个元素出现次数
来源：http://hz.tanke756.top/gthvewmtwm.html

Py:   Counter(arr)
来源：http://hz.wangdashe.top/gtqurfkhpc.html

PHP:  array_count_values($arr);
来源：http://hz.zhengqikj.top/gtrefaeacl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.iojbl.cn/gtzihefsuj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj20258888.top/gtcpjwdjny.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.316326.xyz/gtenhbhama.html

Go:   // 手写 map[T]int
来源：http://hz.vqdsnc.cn/gtybksmicw.html

Ruby: arr.tally
来源：http://hz.pycfn.com/gtslvdiztz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ywan-chungtsiang.top/gtozxcrgia.html

[D21] 判断是否包含某元素
来源：http://hz.birdmap.top/gtoofvzpay.html

Py:   x in arr
来源：http://hz.yueranfly.top/gtpqqdevqw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.bjfxy.top/gtedzcklzm.html

JS:   arr.includes(x)
来源：http://hz.gotoacloud.top/gtkqbjtlqz.html

TS:   arr.includes(x)
来源：http://hz.jiagoushi.top/gtkybhdvxo.html

Java: list.contains(x)
来源：http://hz.jianghu66.top/gtsumfaoor.html

Go:   slices.Contains(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtsnscbami.html

Ruby: arr.include?(x)
来源：http://hz.daria6918.cn/gtdtvnswjo.html

C#:   list.Contains(x)
来源：http://hz.iojbl.cn/gtweqcqijh.html

[D22] 复制数组（避免共享引用）
来源：http://hz.tanke756.top/gtrxyctxol.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xinyue.icu/gtrjwppopi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.aizwys.cn/gtbdsbivul.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gaohongyu789.top/gttaqurboh.html

TS:   [...arr];
来源：http://hz.vqdsnc.cn/gtjvokxggk.html

Java: new ArrayList<>(list);
来源：http://hz.hnxiangtu.top/gtnypmzntu.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hnxiangtu.top/gtdocadjaa.html

Ruby: arr.dup;  arr.clone
来源：http://hz.c1oappe.top/gtufzvwtlm.html

C#:   new List<int>(list);
来源：http://hz.zhaomingkeji.xyz/gtxfhhkkew.html

[D23] reduce 累积计算
来源：http://hz.xuetiantiany.cn/gtzunwndux.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.daxiang520.top/gthjckzqie.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jinyuanbaomall.cn/gtkaubldfb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guowangkeji.top/gtnmcmgcgj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ivvv.top/gtxrkujflj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.cheryme.top/gtkiuahcgf.html

Go:   // 手写循环
来源：http://hz.hywenlv.cn/gtbnwggxcx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.dianchejie.cn/gtakzrdaxr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.kuanghao11.cn/gtoidctdcs.html

[D24] 字典 / Map 基本操作
来源：http://hz.fzhhl.top/gtuzooxzhu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yj20258888.top/gtohhrmqmp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.snrcjt.cn/gtbwjyibrb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.daria6918.cn/gtkzejheuj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.guannengcc.top/gtunqzwewy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hysaishi.cn/gtsykcdbww.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yanxiufei.cn/gtdggjbmnv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.wangshuangyany.cn/gtapkhzjqy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xuetiantiany.cn/gtbeefeucc.html

[D25] Set 集合去重与交并差
来源：http://hz.xuanzx.com/gtyahywqqo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jinqigfzy.top/gtzvxrcgvu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.guannengcc.top/gtuteffwjb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.9152youxi.cn/gtijkrqxai.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ppjwa.cn/gtqyqoyznj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hammf.cn/gtafyfvuqk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.sweek.top/gttqjyvvdn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhixingplan.top/gtqcxllinp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.wangshuangyany.cn/gtyqvyzenr.html

[D26] 数组转字符串
来源：http://hz.tanke756.top/gtkbrgzlwh.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shuidangran.top/gtmrqdvjtl.html

PHP:  implode(", ", $arr);
来源：http://hz.hammf.cn/gtnfzwexqf.html

JS:   arr.join(", ")
来源：http://hz.9152youxi.cn/gtqliwkvuw.html

TS:   arr.join(", ")
来源：http://hz.zhongyouzk.top/gtevxipuxm.html

Java: String.join(", ", list)
来源：http://hz.guannengcc.top/gtqynevuqn.html

Go:   strings.Join(strs, ", ")
来源：http://hz.birdmap.top/gtisrsqucb.html

Ruby: arr.join(", ")
来源：http://hz.xuanzx.com/gtvjptybvf.html

C#:   string.Join(", ", list)
来源：http://hz.zhijiandao.cn/gtaydvleds.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtchzdjnjb.html

E. 字符串处理
来源：http://hz.0kj1m.cn/gtfngsixnx.html

================================================================================
来源：http://hz.zhixingplan.top/gtbohidtpf.html

[E01] 拼接字符串
来源：http://hz.chenjidiqi.icu/gtvcxmwofl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xuanzx.com/gtksrdfxvb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ydjk.org.cn/gtwrmuubcl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.redwolf501.top/gthdsghjaa.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gogol.net.cn/gtenjyjueg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.nanxuanxn.top/gtxgvamdya.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yj20258.top/gtrcjvzgip.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhengqikj.top/gtyxliygqj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jlsjyb.cn/gtdmkaklsq.html

[E02] 重复字符串
来源：http://hz.xziqi.cn/gtnejyfpsx.html

Py:   "ab" * 3
来源：http://hz.yongpay.top/gtchesqhya.html

PHP:  str_repeat("ab", 3);
来源：http://hz.fzhhl.top/gtijpjjflo.html

JS:   "ab".repeat(3)
来源：http://hz.aizwys.cn/gtsebquaok.html

TS:   "ab".repeat(3)
来源：http://hz.0kj1m.cn/gtdvmoblva.html

Java: "ab".repeat(3)
来源：http://hz.shuidangran.top/gtspabpycz.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zdqjudy.top/gtzuvrdped.html

Ruby: "ab" * 3
来源：http://hz.daxiang520.top/gtyryhlhgp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhoulong.xyz/gteqvvgfmm.html

[E03] 截取子串
来源：http://hz.zycfv.cn/gtybyzgalu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.shanyushiyangkeji.top/gttjjeowcw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zycfv.cn/gtznjigtqs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jlsjyb.cn/gtkjutpwey.html

TS:   s.slice(1, 4)
来源：http://hz.hywenlv.cn/gtdthtdcev.html

Java: s.substring(1, 4)
来源：http://hz.yvedp.cn/gtsegamgfn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.0kj1m.cn/gtlonpomfo.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.wangdashe.top/gtztsnwggw.html

C#:   s.Substring(1, 3)
来源：http://hz.gotoacloud.top/gtcwhnxxxh.html

[E04] 查找子串位置
来源：http://hz.cheryme.top/gtmkokwgcs.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jinqigufen.top/gtzpdpdofx.html

PHP:  strpos($s, "x");
来源：http://hz.yueranfly.top/gtlhvlnqvy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ehwqpu.com/gtsowebbzo.html

TS:   s.indexOf("x")
来源：http://hz.gogol.net.cn/gtobrnmukg.html

Java: s.indexOf("x")
来源：http://hz.0kj1m.cn/gtlodtnvyt.html

Go:   strings.Index(s, "x")
来源：http://hz.pycfn.com/gtoacdkvlf.html

Ruby: s.index("x")
来源：http://hz.dianchejie.cn/gtyeuncgwe.html

C#:   s.IndexOf("x")
来源：http://hz.sweek.top/gtsedxurpy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hongshengwenyu.top/gtjojddjvv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yueranfly.top/gtxwinhlxt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.aizwys.cn/gtnhsqpbrr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jianghu66.top/gthdzcnpuk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.guannengcc.top/gtmujysvnq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinghuilouyu.cn/gtugaujeka.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ehwqpu.com/gtrcjiwtak.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.sxryk.cn/gtjkddbtee.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yonumen.top/gtvfjisyhj.html

[E06] 替换子串
来源：http://hz.snrcjt.cn/gtmhdttkew.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.dianchejie.cn/gtufsaefte.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.dianchejie.cn/gtbocayawk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.feifeiyinyue.top/gtboawyvub.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cashguo.top/gtopssreym.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sufxvd.cn/gteaojwoie.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.hfpthk.cn/gtmtkxjymv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hammf.cn/gtkriruymt.html

C#:   s.Replace("a", "b")
来源：http://hz.0kj1m.cn/gtdsxatsog.html

[E07] 按分隔符拆分
来源：http://hz.jinqigufen.top/gtgrujgskh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yj20258.top/gtforvbiwv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jinqigfzy.top/gtlkrpyzgj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.52xcode.cn/gtqwvrvgrp.html

TS:   s.split(",")
来源：http://hz.wangshuangyany.cn/gtctvcvnvl.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jinyuanbaomall.cn/gtbslmtmxh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.gzhubu.top/gtwykmhhoi.html

Ruby: s.split(",");  s.split
来源：http://hz.pycfn.com/gteljegyso.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.chenzaomai.com/gtinmodvzl.html

[E08] 数组按分隔符合并
来源：http://hz.meibo888.top/gthwhrrugw.html

Py:   ",".join(items)
来源：http://hz.zhaomingkeji.xyz/gtrrdgmrly.html

PHP:  implode(",", $items);
来源：http://hz.wangshuangyany.cn/gtytxtuuna.html

JS:   items.join(",")
来源：http://hz.gotoacloud.top/gtxjmljwtc.html

TS:   items.join(",")
来源：http://hz.yonumen.top/gtpjuhuxhw.html

Java: String.join(",", items)
来源：http://hz.jqgfzy.top/gtyzfolgpz.html

Go:   strings.Join(items, ",")
来源：http://hz.316326.xyz/gtfsmqzbxi.html

Ruby: items.join(",")
来源：http://hz.tian-w.cn/gttwvlulut.html

C#:   string.Join(",", items)
来源：http://hz.nanxinkj.top/gtoerbymvu.html

[E09] 去除所有空白字符
来源：http://hz.tanke756.top/gtkzcrsuvm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.52xcode.cn/gtzqnojgey.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhijiandao.cn/gtyziquukx.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenjidiqi.icu/gtqukdfkaj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yuanzhike.top/gtpjrpcagu.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.gaohongyu789.top/gtmtbtacdv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.daxiang520.top/gtklclxhwd.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jqgufenzy.top/gtectfjhqv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jinghuilouyu.cn/gtvnflnmkb.html

[E10] 左侧补零 / 定长填充
来源：http://hz.fengsongda.top/gtmuvtxyjv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ydjk.org.cn/gtfdgtjivn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yueranfly.top/gtgvzduuvj.html

JS:   "7".padStart(3, "0")
来源：http://hz.shanyushiyangtech.top/gtbcbpdlke.html

TS:   "7".padStart(3, "0")
来源：http://hz.yj202588.top/gtfnvbbwpm.html

Java: String.format("%03d", 7)
来源：http://hz.tanke756.top/gtvctxdnyq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hnqzz.top/gtnwlewvkn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.nanxinkj.top/gtfqlegepn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hywenlv.cn/gtbycsarfx.html

[E11] 反转字符串
来源：http://hz.ppjwa.cn/gtwsxlmiyy.html

Py:   s[::-1]
来源：http://hz.mhx1999.top/gtytbfclme.html

PHP:  strrev($s);
来源：http://hz.yj202588.top/gtesqtklwp.html

JS:   [...s].reverse().join("")
来源：http://hz.jianghu66.top/gtwwllnyvh.html

TS:   [...s].reverse().join("")
来源：http://hz.chenjidiqi.icu/gtwanubsoc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xziqi.cn/gtberagrzg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jyoumei.cn/gtftuvqwge.html

Ruby: s.reverse
来源：http://hz.wangshuangyany.cn/gtwwxqhich.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.chenzaomai.com/gtppclucow.html

[E12] 统计某字符出现次数
来源：http://hz.jyoumei.cn/gtnhampxgy.html

Py:   s.count("a")
来源：http://hz.jiagoushi.top/gtfqmqzvwp.html

PHP:  substr_count($s, "a");
来源：http://hz.hywenlv.cn/gtrzfosbgy.html

JS:   s.split("a").length - 1
来源：http://hz.jinqigufen.top/gtjqepniht.html

TS:   s.split("a").length - 1
来源：http://hz.guowangkeji.top/gtolylafoq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinyuanbaomall.cn/gtqjcavgrv.html

Go:   strings.Count(s, "a")
来源：http://hz.pengpengdd.cyou/gtxqnuxulb.html

Ruby: s.count("a")
来源：http://hz.zhoulong.xyz/gtdhkfcuqc.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yangfankeji.com/gtddntycdz.html

[E13] 逐字符遍历
来源：http://hz.xylfe.cn/gtnlgzbxtb.html

Py:   for ch in s: print(ch)
来源：http://hz.ydjk.org.cn/gtsjdfccpy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hnxiangtu.top/gtsgffjcoc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ehwqpu.com/gtlwlsmwex.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yuxming.cn/gtcuyimdyc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.pengpengdd.cyou/gtvkaxatmb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.guowangkeji.top/gtfyvodooy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.sweek.top/gtwjrgmwim.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.daria6918.cn/gtblqsfnan.html

[E14] URL 编码与 Base64
来源：http://hz.zhaomingkeji.xyz/gtwcxdngqo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.gotoacloud.top/gtgnvebdtu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinqigfzy.top/gtmgfmjoau.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.aizwys.cn/gtavmzhkww.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.iojbl.cn/gtqezhgdzu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.redwolf501.top/gttmwmragd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.aizwys.cn/gtdnmgcbet.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.52xcode.cn/gtiemdyiwq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.chenjidiqi.icu/gtjsflvtow.html

[E15] HTML 转义 / 反转义
来源：http://hz.jiagoushi.top/gtnmalytrs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ivvv.top/gtdnfhluuo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hfpthk.cn/gtvgxmhprj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ivvv.top/gtdgowqlsu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.vqdsnc.cn/gtbhzwokwn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zycfv.cn/gtmquvazlg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.redwolf501.top/gtqdbgolmq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yuanzhike.top/gtwdrgccrp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yonumen.top/gtigrwbayq.html

[E16] 数字千分位
来源：http://hz.cucudq.cn/gtwmhmdqjk.html

Py:   f"{1234567:,}"
来源：http://hz.svipenyu.cn/gtwvxygwdv.html

PHP:  number_format(1234567);
来源：http://hz.jiagoushi.top/gtywuxahod.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.tianlin.xyz/gtazldbgki.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.vqdsnc.cn/gtecasslhy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.dashuyun.cn/gtnyhespng.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.wangdashe.top/gtohwpsdti.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hywenlv.cn/gtlpzatykz.html

C#:   1234567.ToString("N0")
来源：http://hz.jyoumei.cn/gtximptclk.html

[E17] 首字母大写
来源：http://hz.cqqwz.cn/gttgrjaabv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.aizwys.cn/gtyxaffdla.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ehwqpu.com/gtuiaqgnpu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.daxiang520.top/gtgjlmtivm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhaomingkeji.xyz/gtjdgsnoun.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.gzhubu.top/gtjmqsdbpf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.gaohongyu789.top/gtkfgrsepo.html

Ruby: s.capitalize
来源：http://hz.havefunace.top/gtlpeyawjb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.snrcjt.cn/gtezzucrfd.html

[E18] 模板占位符替换
来源：http://hz.guowangkeji.top/gtlfkkilwe.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ehwqpu.com/gtatswfswt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.quarkkingdee.top/gtjuoqcbtk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.aibaodan.cn/gtgulyjrgj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.tianlin.xyz/gtfreyeoet.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.kuanghao11.cn/gtvmjgjafz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hnxiangtu.top/gtlidmkyqw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jiagoushi.top/gtktttmphj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.shangyingyoupin.top/gtyrtfapuz.html

[E19] 多行文本按行拆分
来源：http://hz.cheryme.top/gtrzjbxmas.html

Py:   s.splitlines()
来源：http://hz.pycfn.com/gttmnksqrj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yonumen.top/gtqisexppb.html

JS:   s.split(/\r?\n/)
来源：http://hz.shanyushiyangkeji.top/gtrsnvqzdj.html

TS:   s.split(/\r?\n/)
来源：http://hz.52xcode.cn/gtshhzcalq.html

Java: s.lines().toList()
来源：http://hz.gogol.net.cn/gtdjuejbfu.html

Go:   strings.Split(s, "\n")
来源：http://hz.yonumen.top/gtirrbnsre.html


<!-- 参考信息 -->