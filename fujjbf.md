代发 wailian999

C#:   list.Distinct().ToList()
来源：http://hz.zhaomingkeji.xyz/gtwejiehax.html

[D16] 求和与平均值
来源：http://hz.chenlongwang.top/gtxhrmwnfv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yueranfly.top/gtsvgxijuy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xingfuxueyuan.xyz/gtlvlynxwr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cashguo.top/gtpzgbmzsp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258888.top/gtzazwycst.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.aibaodan.cn/gtkoaxlkpt.html

Go:   // 手写循环累加
来源：http://hz.jqgfzy.top/gtsibmuhcc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.daxiang520.top/gtcwpaexfe.html

C#:   list.Sum();  list.Average()
来源：http://hz.wangshuangyany.cn/gtbhstfqnz.html

[D17] 最大值与最小值
来源：http://hz.chenjidiqi.icu/gtydmpumjz.html

Py:   max(arr);  min(arr)
来源：http://hz.aizwys.cn/gtakrbzzah.html

PHP:  max($arr);  min($arr);
来源：http://hz.cucudq.cn/gthjikfkyz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ehwqpu.com/gtehopizra.html

TS:   Math.max(...arr);
来源：http://hz.xuanzx.com/gtktpywtcb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yongpay.top/gtnkykdgam.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jinqigfzy.top/gtssgbayjc.html

Ruby: arr.max;  arr.min
来源：http://hz.sysykeji.top/gthwxtywxv.html

C#:   list.Max();  list.Min()
来源：http://hz.ybcxt.top/gtlhqzwnfk.html

[D18] 扁平化嵌套数组
来源：http://hz.316326.xyz/gtsjwmdtxt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhijiandao.cn/gtksplqand.html

PHP:  array_merge(...$nested);
来源：http://hz.jyoumei.cn/gttrleaytl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.fengsongda.top/gtsvwryjex.html

TS:   nested.flat();
来源：http://hz.jqgfzy.top/gtmvpeidpi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.sufxvd.cn/gtqscanoeg.html

Go:   // 手写双层循环
来源：http://hz.andypj.xyz/gtioadhhrl.html

Ruby: nested.flatten
来源：http://hz.shzxlz.cn/gtgcejvhdo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xuanzx.com/gtlbgymztb.html

[D19] 按字段分组
来源：http://hz.c1oappe.top/gtdyuqrobt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jyoumei.cn/gtkjiartiv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.gotoacloud.top/gtwrhxqryx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yj20258888.top/gtabbihkzs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cqqwz.cn/gtdjbxfoqn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zycfv.cn/gtiznixqdy.html

Go:   // 手写 map[string][]T
来源：http://hz.chenzaomai.com/gtqacscssj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.nanxinkj.top/gtmohnbbtz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.c1oappe.top/gtljyxhftl.html

[D20] 统计每个元素出现次数
来源：http://hz.yj20258888.top/gtsaynlgrp.html

Py:   Counter(arr)
来源：http://hz.hfpthk.cn/gtwwckxtjo.html

PHP:  array_count_values($arr);
来源：http://hz.gzhubu.top/gtrbqzsrzq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shzxlz.cn/gtopevmmol.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.daxiang520.top/gtejcqutpe.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.tian-w.cn/gtagaxfqdi.html

Go:   // 手写 map[T]int
来源：http://hz.ydzc1.top/gtiwdrqvnc.html

Ruby: arr.tally
来源：http://hz.gzhubu.top/gtreyqajqy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.tian-w.cn/gtrujrbsaq.html

[D21] 判断是否包含某元素
来源：http://hz.jlsjyb.cn/gttozitvjf.html

Py:   x in arr
来源：http://hz.dianchejie.cn/gtgpafuusp.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hywenlv.cn/gtcnlussku.html

JS:   arr.includes(x)
来源：http://hz.zhongyouzk.top/gtwjfznuia.html

TS:   arr.includes(x)
来源：http://hz.hfpthk.cn/gtsnbnozir.html

Java: list.contains(x)
来源：http://hz.shuidangran.top/gtbxvqtqxh.html

Go:   slices.Contains(arr, x)
来源：http://hz.shuidangran.top/gtidvibvdn.html

Ruby: arr.include?(x)
来源：http://hz.xingfuxueyuan.xyz/gthuisxkin.html

C#:   list.Contains(x)
来源：http://hz.hnxiangtu.top/gtnpalrboj.html

[D22] 复制数组（避免共享引用）
来源：http://hz.andypj.xyz/gtywzchmgr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yuanzhike.top/gtitsjevuq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shangyingyoupin.top/gtaqezhteo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hfpthk.cn/gtxctevinj.html

TS:   [...arr];
来源：http://hz.zhijiandao.cn/gtoyaxdxgt.html

Java: new ArrayList<>(list);
来源：http://hz.yvedp.cn/gtnrbvutrj.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.52xcode.cn/gtmbsosrso.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jlsjyb.cn/gtflmvqere.html

C#:   new List<int>(list);
来源：http://hz.chenzaomai.com/gtdctvxccv.html

[D23] reduce 累积计算
来源：http://hz.jlsjyb.cn/gtodgvxdli.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zdqjudy.top/gtuozumcld.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.nanxuanxn.top/gtdprbitir.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhijiandao.cn/gtnscrkpao.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.haohaochexian.top/gtatokspox.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.bjfxy.top/gtutfzntvv.html

Go:   // 手写循环
来源：http://hz.chenjidiqi.icu/gttynmzfwa.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.c1oappe.top/gtjuepviaz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hnxiangtu.top/gtgoetpqjq.html

[D24] 字典 / Map 基本操作
来源：http://hz.316326.xyz/gtompimtjf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jinghuilouyu.cn/gtgxtyfhqj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhixingplan.top/gtqayvrppc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yvedp.cn/gtsniugtxa.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shangyingyoupin.top/gtmtydvqbi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sweek.top/gtxohyiznv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.daria6918.cn/gtckynzmyt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hnxiangtu.top/gtwltccrvx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.fzhhl.top/gtgwtmlxyz.html

[D25] Set 集合去重与交并差
来源：http://hz.c1oappe.top/gtyoubmbjn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jinqigfzy.top/gtodofvwqv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zycfv.cn/gteyurcclc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.kuanghao11.cn/gtpmhqhsgt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.aibaodan.cn/gtlzmwszif.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.chenzaomai.com/gtviaqorif.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zhiwuduotai.top/gtuknplsrt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhongyouzk.top/gtxpfejwsl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.andypj.xyz/gtthcicbwx.html

[D26] 数组转字符串
来源：http://hz.svipenyu.cn/gtntykvqim.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shzxlz.cn/gtxafuusuc.html

PHP:  implode(", ", $arr);
来源：http://hz.jinqigfzy.top/gtifrutbpg.html

JS:   arr.join(", ")
来源：http://hz.xingfuxueyuan.xyz/gtokwplazl.html

TS:   arr.join(", ")
来源：http://hz.wangshuangyany.cn/gtpxovbzuh.html

Java: String.join(", ", list)
来源：http://hz.sysykeji.top/gtpowemvmk.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jqgfzy.top/gtgfsfpmfn.html

Ruby: arr.join(", ")
来源：http://hz.chenlongwang.top/gtenubjsdx.html

C#:   string.Join(", ", list)
来源：http://hz.zhongyouzk.top/gtfydjoyrm.html

================================================================================
来源：http://hz.yueranfly.top/gtisykjzxj.html

E. 字符串处理
来源：http://hz.cdnleiting.top/gthbkgmgjs.html

================================================================================
来源：http://hz.chenlongwang.top/gtaxfmirpj.html

[E01] 拼接字符串
来源：http://hz.pycfn.com/gtqspxcrql.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.sweek.top/gtbyqitvbn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cashguo.top/gtuunubjdx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxuanxn.top/gtqbfdckqs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.daria6918.cn/gtbczyawxq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jinqigufen.top/gthkuajgfz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.wangshuangyany.cn/gtlzgzckjj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.tianlin.xyz/gtmarnbuho.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yuanzhike.top/gtrtvjmont.html

[E02] 重复字符串
来源：http://hz.jlsjyb.cn/gtdyniaqyy.html

Py:   "ab" * 3
来源：http://hz.c1oappe.top/gtjhuesguo.html

PHP:  str_repeat("ab", 3);
来源：http://hz.redwolf501.top/gtossyuyrt.html

JS:   "ab".repeat(3)
来源：http://hz.birdmap.top/gtastxcfqt.html

TS:   "ab".repeat(3)
来源：http://hz.cdnleiting.top/gtwwlmelom.html

Java: "ab".repeat(3)
来源：http://hz.zhengqikj.top/gtumwukgqs.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.nanxuanxn.top/gtsfglikbw.html

Ruby: "ab" * 3
来源：http://hz.aibaodan.cn/gtzkiqnkjy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhengqikj.top/gtnugmalgo.html

[E03] 截取子串
来源：http://hz.ydzc1.top/gtchskjxxo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.shangyingyoupin.top/gtfoipjqny.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shangyingyoupin.top/gtwpcmlysk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhongyouzk.top/gtucdbjxtc.html

TS:   s.slice(1, 4)
来源：http://hz.guannengcc.top/gtzaziurwz.html

Java: s.substring(1, 4)
来源：http://hz.zhengqikj.top/gttmsncwlz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.fengsongda.top/gteripdkcm.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.c1oappe.top/gtnchmeidv.html

C#:   s.Substring(1, 3)
来源：http://hz.daria6918.cn/gtgmelocjt.html

[E04] 查找子串位置
来源：http://hz.xziqi.cn/gturvcxuvm.html

Py:   s.find("x");  s.index("x")
来源：http://hz.chenjidiqi.icu/gtelqygjvh.html

PHP:  strpos($s, "x");
来源：http://hz.yvedp.cn/gtqrddidif.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jiagoushi.top/gtamxwneej.html

TS:   s.indexOf("x")
来源：http://hz.fzhhl.top/gtemqceiqn.html

Java: s.indexOf("x")
来源：http://hz.havefunace.top/gtafxuyynp.html

Go:   strings.Index(s, "x")
来源：http://hz.smart0.xyz/gtxnvvreeh.html

Ruby: s.index("x")
来源：http://hz.ydzc1.top/gtuwrxpfex.html

C#:   s.IndexOf("x")
来源：http://hz.nanxinkj.top/gtpsrcqozu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jinqigfzy.top/gtcwmtnmsu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jqgfzy.top/gtsvehmnpo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.mhx1999.top/gtpbrfpaxa.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.haohaochexian.top/gtgecyhaff.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ppjwa.cn/gtcjljjrqg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinghuilouyu.cn/gtskbbabim.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.dashuyun.cn/gtvxcvhtes.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yuxming.cn/gtziefycdc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.shuidangran.top/gtpkuiqjhw.html

[E06] 替换子串
来源：http://hz.sysykeji.top/gtihpfsfwu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.chenjidiqi.icu/gttwegipxx.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.nanxinkj.top/gtrpqpezkz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nanxinkj.top/gtfmstkcsm.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhengqikj.top/gtdjfgkvro.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenzaomai.com/gtoajqwhcg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.gzhubu.top/gtiaepevpr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jinghuilouyu.cn/gtqoxybkti.html

C#:   s.Replace("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtmatoduox.html

[E07] 按分隔符拆分
来源：http://hz.yj20258888.top/gtaqthviem.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yj202588.top/gtqchzakwp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jinyuanbaomall.cn/gtefibgpyv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ehwqpu.com/gtlsvqajhf.html

TS:   s.split(",")
来源：http://hz.kuanghao11.cn/gttpgvgswr.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.birdmap.top/gtcpdweayr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.shanyushiyangtech.top/gtfwdhzvoe.html

Ruby: s.split(",");  s.split
来源：http://hz.yj20258.top/gtqjmftlih.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.vqdsnc.cn/gtigydtjxw.html

[E08] 数组按分隔符合并
来源：http://hz.mhx1999.top/gtmlccrfck.html

Py:   ",".join(items)
来源：http://hz.jinqigufen.top/gtfpwkhavk.html

PHP:  implode(",", $items);
来源：http://hz.zhengqikj.top/gtdrgvtzqr.html

JS:   items.join(",")
来源：http://hz.jqgufenzy.top/gtcbqgsgmg.html

TS:   items.join(",")
来源：http://hz.ywan-chungtsiang.top/gtdozeaada.html

Java: String.join(",", items)
来源：http://hz.nanxuanxn.top/gtguoucxzq.html

Go:   strings.Join(items, ",")
来源：http://hz.aizwys.cn/gtvlmnvjbc.html

Ruby: items.join(",")
来源：http://hz.nanxinkj.top/gtqnttfdee.html

C#:   string.Join(",", items)
来源：http://hz.jqgfzy.top/gtcjuzjkft.html

[E09] 去除所有空白字符
来源：http://hz.redwolf501.top/gttxdvipxn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.dianchejie.cn/gtpowslyyw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.chenzaomai.com/gtpczkywfb.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yuanzhike.top/gttyozzhsf.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.c1oappe.top/gtzitdelaw.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhengqikj.top/gtbagvuedz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jqgufenzy.top/gtpsigphuq.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.gaohongyu789.top/gtokexwgpx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ppjwa.cn/gtspbzeeun.html

[E10] 左侧补零 / 定长填充
来源：http://hz.pycfn.com/gtwmdzmyqb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yongpay.top/gtsuavxcgd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yongpay.top/gtbniqbexc.html

JS:   "7".padStart(3, "0")
来源：http://hz.zycfv.cn/gtuhokkrey.html

TS:   "7".padStart(3, "0")
来源：http://hz.daria6918.cn/gtujnvkmmh.html

Java: String.format("%03d", 7)
来源：http://hz.fzhhl.top/gtjqemfrhc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yanxiufei.cn/gtzwyxthzo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hongshengwenyu.top/gtxqgqbmwb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.tanke756.top/gttnhpvpxq.html

[E11] 反转字符串
来源：http://hz.yj20258.top/gtmpdzibmx.html

Py:   s[::-1]
来源：http://hz.aizwys.cn/gtuitgaqeq.html

PHP:  strrev($s);
来源：http://hz.quarkkingdee.top/gtewcyfpbe.html

JS:   [...s].reverse().join("")
来源：http://hz.yonumen.top/gtehkfbrmx.html

TS:   [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtsqjvfepl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.cdnleiting.top/gtrxhboeoo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yvedp.cn/gteagoosjg.html

Ruby: s.reverse
来源：http://hz.jiagoushi.top/gtuqubfwtz.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xingfuxueyuan.xyz/gtotxcptck.html

[E12] 统计某字符出现次数
来源：http://hz.ydjk.org.cn/gtfpduynxe.html

Py:   s.count("a")
来源：http://hz.shzxlz.cn/gtypnkblax.html

PHP:  substr_count($s, "a");
来源：http://hz.hammf.cn/gtslrgyuvt.html

JS:   s.split("a").length - 1
来源：http://hz.chenjidiqi.icu/gtrwcztqrz.html

TS:   s.split("a").length - 1
来源：http://hz.sweek.top/gtuvruvhgz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.wangshuangyany.cn/gtnvvtuaaz.html

Go:   strings.Count(s, "a")
来源：http://hz.wangshuangyany.cn/gtbwodxdwv.html

Ruby: s.count("a")
来源：http://hz.bjfxy.top/gtzzsjnqgg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.dianchejie.cn/gtlxkztfrt.html

[E13] 逐字符遍历
来源：http://hz.yongpay.top/gttawayiyr.html

Py:   for ch in s: print(ch)
来源：http://hz.jlsjyb.cn/gteenpccmn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.sxryk.cn/gtwvxttkwd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinghuilouyu.cn/gtvqpfnbuw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.iojbl.cn/gtepvsuckr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zhengqikj.top/gtkwdzghnd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.bjfxy.top/gtnufttmox.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jyoumei.cn/gtsvhqkslz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.shangyingyoupin.top/gttdbifdsj.html

[E14] URL 编码与 Base64
来源：http://hz.yj20258888.top/gtygpbxifq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hnqzz.top/gtfkgawhlj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cdnleiting.top/gtjixdlxqa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shanyushiyangtech.top/gtudcyowvd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.meibo888.top/gtgihiomqb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shanyushiyangtech.top/gtnxyahsuf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ydjk.org.cn/gttzykzmwq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xuetiantiany.cn/gtfkutqlgs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.daria6918.cn/gtxbmpebbt.html

[E15] HTML 转义 / 反转义
来源：http://hz.hfpthk.cn/gtmzoogozr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.pengpengdd.cyou/gtqcqplicd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jqgufenzy.top/gtvvprgpie.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.dashuyun.cn/gtopomglgv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.snrcjt.cn/gtehyxvydp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.tanke756.top/gtnmcycqgi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.kuanghao11.cn/gtkztoorjp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.meibo888.top/gthxcgxvjr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinqigufen.top/gtdvvqqdcr.html

[E16] 数字千分位
来源：http://hz.vqdsnc.cn/gtletabcxk.html

Py:   f"{1234567:,}"
来源：http://hz.hnxiangtu.top/gtnvxwsiqx.html

PHP:  number_format(1234567);
来源：http://hz.jyoumei.cn/gtmbndutjt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.sysykeji.top/gtvxekpuix.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hongshengwenyu.top/gtrplyxywu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.vqdsnc.cn/gtvylsmmvb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhijiandao.cn/gtyfzyjxbw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.nanxinkj.top/gtcmwcmfvy.html

C#:   1234567.ToString("N0")
来源：http://hz.c1oappe.top/gtqhehfnwo.html

[E17] 首字母大写
来源：http://hz.yongpay.top/gthrylphxi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.haohaochexian.top/gtnmygodqe.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yj202588.top/gtarvkzygn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xziqi.cn/gtsrwmdzir.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xinyue.icu/gtvwpllyjn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.andypj.xyz/gtoncaxnty.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sweek.top/gtcktrrbfb.html

Ruby: s.capitalize
来源：http://hz.0kj1m.cn/gtdbrtflit.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.dianchejie.cn/gtvdakmvou.html

[E18] 模板占位符替换
来源：http://hz.yonumen.top/gtibngzimv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.chenjidiqi.icu/gtzudsfbvj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jinqigufen.top/gtyqzlocyo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.svipenyu.cn/gtomnqauyi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.tianlin.xyz/gtrtiqtihy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ivvv.top/gttjewbgus.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhiwuduotai.top/gtonbpbcqb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shanyushiyangtech.top/gtsujpfbvo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.nwbrower.top/gtuhlixsav.html

[E19] 多行文本按行拆分
来源：http://hz.yj202588.top/gtvfakqiva.html

Py:   s.splitlines()
来源：http://hz.zhijiandao.cn/gtudbczgpj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.birdmap.top/gtfswhdhtx.html

JS:   s.split(/\r?\n/)
来源：http://hz.jqgfzy.top/gtxgncvnlj.html

TS:   s.split(/\r?\n/)
来源：http://hz.gotoacloud.top/gtmbtciwsh.html

Java: s.lines().toList()
来源：http://hz.shanyushiyangtech.top/gtdhmojkwi.html

Go:   strings.Split(s, "\n")
来源：http://hz.316326.xyz/gtplbwiwpn.html

Ruby: s.lines
来源：http://hz.gogol.net.cn/gtohcpgxwr.html

C#:   s.Split('\n')
来源：http://hz.yangfankeji.com/gtdzfgndua.html

[E20] 判断字符串是否为空
来源：http://hz.sweek.top/gtmumcixzt.html

Py:   if not s:
来源：http://hz.nanxuanxn.top/gtdnibdzqc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yj20258.top/gthzjhrrcd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.cashguo.top/gtwpgvkbkl.html

TS:   if (s === "") {}
来源：http://hz.sxryk.cn/gtpazvqltf.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhijiandao.cn/gtiqqtrhmq.html

Go:   if s == "" {}
来源：http://hz.jiagoushi.top/gtostwyxav.html

Ruby: if s.empty?
来源：http://hz.gotoacloud.top/gtdferiypl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.guannengcc.top/gttyaxcmtx.html

[E21] 超长截断加省略号
来源：http://hz.yj20258.top/gtdxzaabpr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.birdmap.top/gtqztimtoe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xylfe.cn/gtnvxmfwtn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.52xcode.cn/gtodnmyqrw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhoulong.xyz/gtqyqyppzx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jlsjyb.cn/gtlewoojpj.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.dashuyun.cn/gtoqqurgya.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.nanxuanxn.top/gtsxcmmfoz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yonumen.top/gthiyrbpdv.html

[E22] 字节长度与字符长度
来源：http://hz.ivvv.top/gtfnjchivt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.svipenyu.cn/gtgrmkwmag.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zdqjudy.top/gtspixtndt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sysykeji.top/gtahktngib.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.wangdashe.top/gtyeubvxeb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.gaohongyu789.top/gtamyecpzb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.shanyushiyangtech.top/gttfhitesq.html

Ruby: s.bytesize;  s.length
来源：http://hz.fzhhl.top/gtihkselmb.html


<!-- 参考信息 -->