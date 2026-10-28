代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.svipenyu.cn/gtpiqurgip.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ivvv.top/gthyxffsyh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xinyue.icu/gtrpgytjrh.html

Go:   // 手写循环累加
来源：http://hz.nwbrower.top/gtqurljnri.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.andypj.xyz/gtjxtgxkte.html

C#:   list.Sum();  list.Average()
来源：http://hz.hysaishi.cn/gtiajspwli.html

[D17] 最大值与最小值
来源：http://hz.ydzc1.top/gtvantnprh.html

Py:   max(arr);  min(arr)
来源：http://hz.tanke756.top/gtekacywgz.html

PHP:  max($arr);  min($arr);
来源：http://hz.0kj1m.cn/gtzfymlbqe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.meibo888.top/gtpgwegadu.html

TS:   Math.max(...arr);
来源：http://hz.wangdashe.top/gtokevwdlb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ydzc1.top/gtxeisojro.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yanxiufei.cn/gtmrjpwudp.html

Ruby: arr.max;  arr.min
来源：http://hz.yangfankeji.com/gthdzrueuj.html

C#:   list.Max();  list.Min()
来源：http://hz.yanxiufei.cn/gtoaaqifgd.html

[D18] 扁平化嵌套数组
来源：http://hz.svipenyu.cn/gtnfjoufqt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.tianlin.xyz/gteemhumkn.html

PHP:  array_merge(...$nested);
来源：http://hz.cheryme.top/gthrertdml.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.shanyushiyangkeji.top/gtlvxcdrwo.html

TS:   nested.flat();
来源：http://hz.feifeiyinyue.top/gtfobslamx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.iojbl.cn/gtsvxnxdsv.html

Go:   // 手写双层循环
来源：http://hz.jinyuanbaomall.cn/gtsmmqscoo.html

Ruby: nested.flatten
来源：http://hz.fzhhl.top/gtrwijucut.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.mhx1999.top/gtvtlobpkj.html

[D19] 按字段分组
来源：http://hz.ywan-chungtsiang.top/gtpyyduboh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.sysykeji.top/gtuuxlcsvt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.guowangkeji.top/gtfamdiecf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hnxiangtu.top/gtfsccrsut.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.dashuyun.cn/gttdlgpngd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.gotoacloud.top/gtigoduvdu.html

Go:   // 手写 map[string][]T
来源：http://hz.hammf.cn/gteyaeqhyp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jqgufenzy.top/gtlwzitoph.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.dashuyun.cn/gtyytqadcs.html

[D20] 统计每个元素出现次数
来源：http://hz.daria6918.cn/gtstqaenny.html

Py:   Counter(arr)
来源：http://hz.meibo888.top/gtelfzxnds.html

PHP:  array_count_values($arr);
来源：http://hz.shanyushiyangtech.top/gtjtujculy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.iojbl.cn/gtlmlssgff.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.dashuyun.cn/gtwjrwhuou.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhiwuduotai.top/gtegswvavw.html

Go:   // 手写 map[T]int
来源：http://hz.fengsongda.top/gtchqieqvj.html

Ruby: arr.tally
来源：http://hz.xylfe.cn/gtguithvye.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.xingfuxueyuan.xyz/gtywxwnvbe.html

[D21] 判断是否包含某元素
来源：http://hz.kuanghao11.cn/gtjqgvaslv.html

Py:   x in arr
来源：http://hz.bjfxy.top/gtngvkxjwl.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cdnleiting.top/gtszsencxj.html

JS:   arr.includes(x)
来源：http://hz.zdqjudy.top/gtobxjhiku.html

TS:   arr.includes(x)
来源：http://hz.hfpthk.cn/gtpujsuhtv.html

Java: list.contains(x)
来源：http://hz.yj20258.top/gtweqoziqn.html

Go:   slices.Contains(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtmrhvtrjo.html

Ruby: arr.include?(x)
来源：http://hz.xylfe.cn/gtsiatlbns.html

C#:   list.Contains(x)
来源：http://hz.xziqi.cn/gttzvkoair.html

[D22] 复制数组（避免共享引用）
来源：http://hz.gzhubu.top/gtiftsuboo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ydzc1.top/gtixemujgq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jinghuilouyu.cn/gtmjqsrkgb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.snrcjt.cn/gtsghfgebp.html

TS:   [...arr];
来源：http://hz.yj202588.top/gtieoonscs.html

Java: new ArrayList<>(list);
来源：http://hz.yj202588.top/gtxijasqmm.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yuxming.cn/gtmesukirv.html

Ruby: arr.dup;  arr.clone
来源：http://hz.cdnleiting.top/gtobvmoqey.html

C#:   new List<int>(list);
来源：http://hz.smart0.xyz/gtadzlpyig.html

[D23] reduce 累积计算
来源：http://hz.pycfn.com/gtaxqzevwt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.aibaodan.cn/gtizthqvjg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.xuetiantiany.cn/gtzyhzoqig.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhoulong.xyz/gtuoldkuok.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cheryme.top/gtmeshxtnm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinqigufen.top/gtatbexmsq.html

Go:   // 手写循环
来源：http://hz.ydzc1.top/gtouxsfrjd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.sxryk.cn/gtpzppvqrz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.bjfxy.top/gtowfhmumy.html

[D24] 字典 / Map 基本操作
来源：http://hz.smart0.xyz/gtcgaumwmv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shanyushiyangtech.top/gtdbqbxsuh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ywan-chungtsiang.top/gtsdkpaaht.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xingfuxueyuan.xyz/gtzuwseiwz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hnxiangtu.top/gthgelvzti.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.daxiang520.top/gttndzwqnp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jyoumei.cn/gtasvubqsd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jyoumei.cn/gtkgmvloya.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.meibo888.top/gtjgonugmh.html

[D25] Set 集合去重与交并差
来源：http://hz.guowangkeji.top/gtrasbjyxj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jinqigufen.top/gtauqnazme.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.gotoacloud.top/gtrggzabll.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.pycfn.com/gtwrvvdqbc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.snrcjt.cn/gtyotfeksf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.quarkkingdee.top/gtskkbytoi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.tianlin.xyz/gtaflgcuwt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhiwuduotai.top/gttikhfsmb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yangfankeji.com/gtrwywmdlx.html

[D26] 数组转字符串
来源：http://hz.tanke756.top/gtklhxzqnn.html

Py:   ", ".join(map(str, arr))
来源：http://hz.aibaodan.cn/gtdphhctzj.html

PHP:  implode(", ", $arr);
来源：http://hz.tanke756.top/gtqwhnqkzn.html

JS:   arr.join(", ")
来源：http://hz.tanke756.top/gtmcwwprkh.html

TS:   arr.join(", ")
来源：http://hz.quarkkingdee.top/gtzsguzvhu.html

Java: String.join(", ", list)
来源：http://hz.jianghu66.top/gtpnevbdud.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jinyuanbaomall.cn/gttdnkqnen.html

Ruby: arr.join(", ")
来源：http://hz.sufxvd.cn/gtszksmpqz.html

C#:   string.Join(", ", list)
来源：http://hz.xingfuxueyuan.xyz/gtntglwypd.html

================================================================================
来源：http://hz.yj20258.top/gtqoydvgbp.html

E. 字符串处理
来源：http://hz.c1oappe.top/gtdserkfix.html

================================================================================
来源：http://hz.havefunace.top/gtgarxkyqa.html

[E01] 拼接字符串
来源：http://hz.meibo888.top/gtusqdtvat.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.svipenyu.cn/gtqxzlvkcf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.316326.xyz/gthzlvzadl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.havefunace.top/gtjzvbfvah.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.9152youxi.cn/gtfeodiifw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zdqjudy.top/gtdeabjwjl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hnqzz.top/gtezkthvop.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shanyushiyangtech.top/gtcsyezpsr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhiwuduotai.top/gtpztgdpjd.html

[E02] 重复字符串
来源：http://hz.feifeiyinyue.top/gtijjblwmj.html

Py:   "ab" * 3
来源：http://hz.zhijiandao.cn/gtsnuipqyw.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jqgufenzy.top/gtqjdyuvub.html

JS:   "ab".repeat(3)
来源：http://hz.jianghu66.top/gthstlyscg.html

TS:   "ab".repeat(3)
来源：http://hz.yangfankeji.com/gtdrlqpbzb.html

Java: "ab".repeat(3)
来源：http://hz.wangdashe.top/gtacjwlcga.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hysaishi.cn/gtyvbdmpgf.html

Ruby: "ab" * 3
来源：http://hz.hnxiangtu.top/gtijqthzxv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.iojbl.cn/gtypnqewop.html

[E03] 截取子串
来源：http://hz.yuanzhike.top/gttzwiupyr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.wangdashe.top/gtzcadfqqc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.nwbrower.top/gtwophhabp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.c1oappe.top/gtktbmxacs.html

TS:   s.slice(1, 4)
来源：http://hz.jinyuanbaomall.cn/gtlnzxphsa.html

Java: s.substring(1, 4)
来源：http://hz.chenzaomai.com/gtzwrqqlaa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yuanzhike.top/gttlpbbent.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hywenlv.cn/gtuchchngb.html

C#:   s.Substring(1, 3)
来源：http://hz.chenzaomai.com/gtkitvzndj.html

[E04] 查找子串位置
来源：http://hz.hammf.cn/gtwckdvjrv.html

Py:   s.find("x");  s.index("x")
来源：http://hz.fengsongda.top/gtypxmfnst.html

PHP:  strpos($s, "x");
来源：http://hz.yj20258.top/gtibhcrngj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hammf.cn/gtrrwzzurb.html

TS:   s.indexOf("x")
来源：http://hz.pengpengdd.cyou/gtiyafkdhz.html

Java: s.indexOf("x")
来源：http://hz.ybcxt.top/gtugqwrelj.html

Go:   strings.Index(s, "x")
来源：http://hz.yuanzhike.top/gtlkdsvilg.html

Ruby: s.index("x")
来源：http://hz.yj202588.top/gtzhmpoeaz.html

C#:   s.IndexOf("x")
来源：http://hz.iojbl.cn/gthkjgncps.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhaomingkeji.xyz/gttdpqijhw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.kuanghao11.cn/gtsvmfeuwo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.xylfe.cn/gtyyjaxtzw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tian-w.cn/gtfaqpqrhh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.feifeiyinyue.top/gthtwylobc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhaomingkeji.xyz/gtdgkhcdeh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cdnleiting.top/gtnifrgfba.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.kuanghao11.cn/gtexyfolyx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.cashguo.top/gtoylztxok.html

[E06] 替换子串
来源：http://hz.wangshuangyany.cn/gtkopqtmnf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yueranfly.top/gtpbsvjbhi.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ivvv.top/gtqjkgbaim.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xuetiantiany.cn/gtlbmiknnq.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jyoumei.cn/gtatobwuvq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhixingplan.top/gtaidsghvn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yuanzhike.top/gtqvfczrra.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.pengpengdd.cyou/gtzojkmjgm.html

C#:   s.Replace("a", "b")
来源：http://hz.shanyushiyangtech.top/gtjttncjak.html

[E07] 按分隔符拆分
来源：http://hz.tian-w.cn/gtcaxjbmpx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.gotoacloud.top/gtnjrnkciv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.gzhubu.top/gtrmhrxjgt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shuidangran.top/gtpfvvvxiq.html

TS:   s.split(",")
来源：http://hz.shanyushiyangtech.top/gtawfwhwji.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhijiandao.cn/gtlxwrclnd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.havefunace.top/gtsibwocua.html

Ruby: s.split(",");  s.split
来源：http://hz.hongshengwenyu.top/gtrflsstet.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jinghuilouyu.cn/gtdryuocyy.html

[E08] 数组按分隔符合并
来源：http://hz.ehwqpu.com/gtxjojluqx.html

Py:   ",".join(items)
来源：http://hz.zhijiandao.cn/gtkichayps.html

PHP:  implode(",", $items);
来源：http://hz.yvedp.cn/gtoflftano.html

JS:   items.join(",")
来源：http://hz.cucudq.cn/gtrifwharf.html

TS:   items.join(",")
来源：http://hz.zhengqikj.top/gtqkoxongw.html

Java: String.join(",", items)
来源：http://hz.zhaomingkeji.xyz/gtuievmjbp.html

Go:   strings.Join(items, ",")
来源：http://hz.yangfankeji.com/gtmttpoupn.html

Ruby: items.join(",")
来源：http://hz.yongpay.top/gtsvunodsb.html

C#:   string.Join(",", items)
来源：http://hz.pengpengdd.cyou/gtesgsgmsv.html

[E09] 去除所有空白字符
来源：http://hz.yj202588.top/gtodedzcvn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.meibo888.top/gtihgaiako.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jinqigufen.top/gtobywddbn.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ydjk.org.cn/gtxhnnutav.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhengqikj.top/gtrcsqltyb.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.meibo888.top/gtyeiwcttw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.snrcjt.cn/gtxprjftic.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhengqikj.top/gtxnmrtmjw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.chenjidiqi.icu/gtbnfitdan.html

[E10] 左侧补零 / 定长填充
来源：http://hz.gzhubu.top/gtdjyufwdp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.havefunace.top/gttcqtmmbm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.sxryk.cn/gtepzhzhij.html

JS:   "7".padStart(3, "0")
来源：http://hz.yanxiufei.cn/gtmizzwoui.html

TS:   "7".padStart(3, "0")
来源：http://hz.haohaochexian.top/gtlsgrhwfj.html

Java: String.format("%03d", 7)
来源：http://hz.yvedp.cn/gtsireeuqn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yuxming.cn/gtyqetwoeo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.svipenyu.cn/gtokfoefwp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hysaishi.cn/gtixesdjdd.html

[E11] 反转字符串
来源：http://hz.xuanzx.com/gtpqpbaaym.html

Py:   s[::-1]
来源：http://hz.jiagoushi.top/gtxrfidhqi.html

PHP:  strrev($s);
来源：http://hz.hnqzz.top/gtrdkfmcop.html

JS:   [...s].reverse().join("")
来源：http://hz.cdnleiting.top/gtxmlleqdx.html

TS:   [...s].reverse().join("")
来源：http://hz.gogol.net.cn/gtpgltnnec.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ywan-chungtsiang.top/gtknuvtgjg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.snrcjt.cn/gtmxdibeau.html

Ruby: s.reverse
来源：http://hz.shangyingyoupin.top/gtjuqlrlnv.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jqgfzy.top/gtvqkyicds.html

[E12] 统计某字符出现次数
来源：http://hz.haohaochexian.top/gtdzdtblzt.html

Py:   s.count("a")
来源：http://hz.yonumen.top/gtdcotqqmb.html

PHP:  substr_count($s, "a");
来源：http://hz.aibaodan.cn/gtwqiyanan.html

JS:   s.split("a").length - 1
来源：http://hz.jqgfzy.top/gtvcbpthgp.html

TS:   s.split("a").length - 1
来源：http://hz.tian-w.cn/gtorgmclon.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhixingplan.top/gtebufejad.html

Go:   strings.Count(s, "a")
来源：http://hz.wangshuangyany.cn/gtbclnglxv.html

Ruby: s.count("a")
来源：http://hz.jinqigufen.top/gtttmivugq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cheryme.top/gtnekvuogt.html

[E13] 逐字符遍历
来源：http://hz.c1oappe.top/gtafzwtrrh.html

Py:   for ch in s: print(ch)
来源：http://hz.aibaodan.cn/gtqmkqudky.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jiagoushi.top/gteinnnexb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sysykeji.top/gtcqcesbfm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sxryk.cn/gtjiubxtlp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jiagoushi.top/gtoiezkgdh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.pycfn.com/gtvtxiowum.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.daxiang520.top/gtnyuazolt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xziqi.cn/gthqticseu.html

[E14] URL 编码与 Base64
来源：http://hz.hongshengwenyu.top/gtmxxalpuu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zycfv.cn/gtlgbpbuef.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hnxiangtu.top/gtebsgjemr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.nwbrower.top/gtisowdffy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.52xcode.cn/gtbqohydjj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.tanke756.top/gtosbugqbp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shuidangran.top/gtfwicydcy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.c1oappe.top/gtrbcpevsn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.9152youxi.cn/gtaqqzvmzm.html

[E15] HTML 转义 / 反转义
来源：http://hz.nanxinkj.top/gtezxgiajz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yanxiufei.cn/gtghfaidit.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.sysykeji.top/gtmnmsmjna.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ydjk.org.cn/gtwdqgnodt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yj20258.top/gtclvcsxvl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.fzhhl.top/gtfvbftseo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.gogol.net.cn/gttiflsswl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hysaishi.cn/gtpbqyshjl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yangfankeji.com/gthzaqhmvm.html

[E16] 数字千分位
来源：http://hz.havefunace.top/gtgzqcbajk.html

Py:   f"{1234567:,}"
来源：http://hz.c1oappe.top/gtubvuguhi.html

PHP:  number_format(1234567);
来源：http://hz.jianghu66.top/gteviukhkp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ivvv.top/gtkxitdwzd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuxming.cn/gtezjomzbh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.andypj.xyz/gtphwlwspp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.pengpengdd.cyou/gtnhvkpjnx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.52xcode.cn/gtixkrfetm.html

C#:   1234567.ToString("N0")
来源：http://hz.hnqzz.top/gtbvtegidy.html

[E17] 首字母大写
来源：http://hz.xylfe.cn/gtfnflwtzi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yonumen.top/gtkxjooqny.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jqgufenzy.top/gtcenoivdm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.dashuyun.cn/gtswpiqwtc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ppjwa.cn/gtwouhazte.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.daxiang520.top/gtkbabrqjt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xylfe.cn/gtwzktkqng.html

Ruby: s.capitalize
来源：http://hz.jyoumei.cn/gtbkntdsuh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.9152youxi.cn/gtyjezcnlg.html

[E18] 模板占位符替换
来源：http://hz.yj20258888.top/gtjvszdsxb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.guannengcc.top/gtycjrmlne.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xuetiantiany.cn/gtpwwjjdup.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hongshengwenyu.top/gtgemurjvc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.sweek.top/gtksklcsbu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.gaohongyu789.top/gtldkhzdcw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhongyouzk.top/gtmhpozqid.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.sxryk.cn/gtunukuqox.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.316326.xyz/gtxlgobrkn.html

[E19] 多行文本按行拆分
来源：http://hz.gzhubu.top/gtiyvkywkw.html

Py:   s.splitlines()
来源：http://hz.ywan-chungtsiang.top/gtsdvbejuw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.snrcjt.cn/gtszfbvahf.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhiwuduotai.top/gtrcalcdwe.html

TS:   s.split(/\r?\n/)
来源：http://hz.guannengcc.top/gtqfmyueyt.html

Java: s.lines().toList()
来源：http://hz.ivvv.top/gtnwswrrlb.html

Go:   strings.Split(s, "\n")
来源：http://hz.gogol.net.cn/gtfuexlzip.html

Ruby: s.lines
来源：http://hz.zhiwuduotai.top/gtoiynugji.html

C#:   s.Split('\n')
来源：http://hz.hfpthk.cn/gtunnvwuli.html

[E20] 判断字符串是否为空
来源：http://hz.xylfe.cn/gtqdupyedv.html

Py:   if not s:
来源：http://hz.tian-w.cn/gtytfopdhj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jlsjyb.cn/gtkdofbtgi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hnqzz.top/gtueuvpdgs.html

TS:   if (s === "") {}
来源：http://hz.zhijiandao.cn/gttnoxpbrj.html

Java: if (s.isEmpty()) {}
来源：http://hz.0kj1m.cn/gtcvjjyffr.html

Go:   if s == "" {}
来源：http://hz.sweek.top/gttkespvzu.html

Ruby: if s.empty?
来源：http://hz.hongshengwenyu.top/gtlyjcwicr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.haohaochexian.top/gtymxekjfh.html

[E21] 超长截断加省略号
来源：http://hz.daxiang520.top/gtuvaukqon.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.dianchejie.cn/gtvvjkftbe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.nwbrower.top/gtqelgnpqt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gotoacloud.top/gtzupcqtdv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhixingplan.top/gtdlhoiecr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yuxming.cn/gttytuknqe.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.chenjidiqi.icu/gttifstlvu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.tianlin.xyz/gtywximtpn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhijiandao.cn/gtehqkfjcs.html

[E22] 字节长度与字符长度
来源：http://hz.sweek.top/gtgeutiymx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.guannengcc.top/gtjyrfxiuz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhixingplan.top/gtitqekaop.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.redwolf501.top/gtymfxbgwu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yvedp.cn/gtodmivlhv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hnqzz.top/gtupbklxqs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yueranfly.top/gtgbxesbcc.html

Ruby: s.bytesize;  s.length
来源：http://hz.jlsjyb.cn/gtshtmtxxn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yj202588.top/gtmwlpxmtq.html

================================================================================
来源：http://hz.cqqwz.cn/gtmgehjmbr.html

F. 文件与目录
来源：http://hz.chenjidiqi.icu/gtuirecdfb.html

================================================================================
来源：http://hz.tianlin.xyz/gtwwuokwxx.html


<!-- 参考信息 -->