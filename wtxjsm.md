代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhiwuduotai.top/gtadgajuaq.html

C#:   list.Sum();  list.Average()
来源：http://hz.hnqzz.top/gtcjckdbfk.html

[D17] 最大值与最小值
来源：http://hz.jqgufenzy.top/gtplvmbszk.html

Py:   max(arr);  min(arr)
来源：http://hz.jiagoushi.top/gtzpbgiyjs.html

PHP:  max($arr);  min($arr);
来源：http://hz.cashguo.top/gtahqyeyhx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yanxiufei.cn/gtjfedcfah.html

TS:   Math.max(...arr);
来源：http://hz.daria6918.cn/gtsxzfyqlw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhongyouzk.top/gtiihwfzfp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.tianlin.xyz/gtgcfcccma.html

Ruby: arr.max;  arr.min
来源：http://hz.aibaodan.cn/gtfbzkmtxm.html

C#:   list.Max();  list.Min()
来源：http://hz.yangfankeji.com/gtlhnjcevy.html

[D18] 扁平化嵌套数组
来源：http://hz.zycfv.cn/gtbwmltfgn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.havefunace.top/gtotfmfmeg.html

PHP:  array_merge(...$nested);
来源：http://hz.aizwys.cn/gtycccsuxe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhiwuduotai.top/gtzownhyqb.html

TS:   nested.flat();
来源：http://hz.hongshengwenyu.top/gtisalqpjq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.dianchejie.cn/gtufxxxqvk.html

Go:   // 手写双层循环
来源：http://hz.hysaishi.cn/gtlavrcebp.html

Ruby: nested.flatten
来源：http://hz.hnqzz.top/gtynzglqwo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yangfankeji.com/gtcbnnkzad.html

[D19] 按字段分组
来源：http://hz.quarkkingdee.top/gtqprvplxt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yj20258888.top/gtvsttunbd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jlsjyb.cn/gtgjzysvck.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.wangshuangyany.cn/gtdyugohjs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.haohaochexian.top/gtswxvjrqs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.nwbrower.top/gtfhfmcyxe.html

Go:   // 手写 map[string][]T
来源：http://hz.yangfankeji.com/gtcqwkizaz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cheryme.top/gtfvarwqpj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.aibaodan.cn/gtjjtvhkjx.html

[D20] 统计每个元素出现次数
来源：http://hz.52xcode.cn/gtjfsmyrnx.html

Py:   Counter(arr)
来源：http://hz.pycfn.com/gteeukqzlu.html

PHP:  array_count_values($arr);
来源：http://hz.hnxiangtu.top/gtcodzlnxz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.aizwys.cn/gtqxrheppt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.mhx1999.top/gtbjvkdhkt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.c1oappe.top/gtxdzsppuy.html

Go:   // 手写 map[T]int
来源：http://hz.52xcode.cn/gtuwtmyvog.html

Ruby: arr.tally
来源：http://hz.zdqjudy.top/gtgknfpbfk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.snrcjt.cn/gtviurjyua.html

[D21] 判断是否包含某元素
来源：http://hz.cashguo.top/gtifofkicz.html

Py:   x in arr
来源：http://hz.shangyingyoupin.top/gtwrwaopxa.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jiagoushi.top/gthbddjuje.html

JS:   arr.includes(x)
来源：http://hz.dashuyun.cn/gtycwsfdyu.html

TS:   arr.includes(x)
来源：http://hz.mhx1999.top/gtwhwapkvf.html

Java: list.contains(x)
来源：http://hz.havefunace.top/gtvaucfxjd.html

Go:   slices.Contains(arr, x)
来源：http://hz.meibo888.top/gttgcvdvgv.html

Ruby: arr.include?(x)
来源：http://hz.yonumen.top/gtzkjhhogn.html

C#:   list.Contains(x)
来源：http://hz.zhengqikj.top/gtiwtecztp.html

[D22] 复制数组（避免共享引用）
来源：http://hz.fzhhl.top/gteoulnxpx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ppjwa.cn/gtvldnqgbn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.gzhubu.top/gtlgcmycbf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.tanke756.top/gtzxwrzyap.html

TS:   [...arr];
来源：http://hz.dianchejie.cn/gtwrntpqiq.html

Java: new ArrayList<>(list);
来源：http://hz.jinqigufen.top/gtfnvmpaxt.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.cashguo.top/gtupcpidbf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.pengpengdd.cyou/gtagfmerli.html

C#:   new List<int>(list);
来源：http://hz.ehwqpu.com/gtpnkblmye.html

[D23] reduce 累积计算
来源：http://hz.smart0.xyz/gtoiqsawmg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yj20258.top/gtcjdeaaid.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cdnleiting.top/gtvdnkopgu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.feifeiyinyue.top/gtcyzrgzcx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.0kj1m.cn/gtczojlexk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yongpay.top/gtnmzbizmp.html

Go:   // 手写循环
来源：http://hz.cheryme.top/gtjfrqodcz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hammf.cn/gtorunvvyq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.guannengcc.top/gtdodliznq.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhiwuduotai.top/gtequfgdpe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jlsjyb.cn/gtovhvvqfp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.0kj1m.cn/gtzjotlojn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ydjk.org.cn/gtdxingqod.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jqgufenzy.top/gtqyccxpns.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhixingplan.top/gtlolwfiwq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.guowangkeji.top/gtubkekjdr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xingfuxueyuan.xyz/gtwltqbvsf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.havefunace.top/gtnoidtifi.html

[D25] Set 集合去重与交并差
来源：http://hz.xziqi.cn/gtamvsjjte.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jlsjyb.cn/gtavmszhmr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.mhx1999.top/gtmriyktoy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ppjwa.cn/gtqolcvacg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jianghu66.top/gthomkrhju.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.daxiang520.top/gtsmmsljpb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.316326.xyz/gtvscvzipy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yj202588.top/gteghzgzpw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.aibaodan.cn/gtkdhxzgua.html

[D26] 数组转字符串
来源：http://hz.meibo888.top/gtesjsoppq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.redwolf501.top/gtiuatteim.html

PHP:  implode(", ", $arr);
来源：http://hz.daxiang520.top/gtoabkppww.html

JS:   arr.join(", ")
来源：http://hz.nwbrower.top/gtdmwikpph.html

TS:   arr.join(", ")
来源：http://hz.jqgfzy.top/gtrtencnki.html

Java: String.join(", ", list)
来源：http://hz.jianghu66.top/gtzhqzbyom.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jinyuanbaomall.cn/gtkhsusyuz.html

Ruby: arr.join(", ")
来源：http://hz.xziqi.cn/gtgcabqnes.html

C#:   string.Join(", ", list)
来源：http://hz.zhijiandao.cn/gtyuvcmxex.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtqtqhdqfl.html

E. 字符串处理
来源：http://hz.yj202588.top/gtcvxguqlv.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtutcjrwdi.html

[E01] 拼接字符串
来源：http://hz.fengsongda.top/gtpnyuxjjk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yongpay.top/gtqzpmdcdv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hammf.cn/gtnbcwokec.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hammf.cn/gtpoyvqqpx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.bjfxy.top/gtyismfsub.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hywenlv.cn/gtkmsldhzl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.pengpengdd.cyou/gtrnzhinmm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.havefunace.top/gtaaaiubdg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.gotoacloud.top/gtgcnomvic.html

[E02] 重复字符串
来源：http://hz.yj202588.top/gtkridutyb.html

Py:   "ab" * 3
来源：http://hz.gaohongyu789.top/gtiednqhzl.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cdnleiting.top/gtesbujips.html

JS:   "ab".repeat(3)
来源：http://hz.shanyushiyangtech.top/gtlditbgks.html

TS:   "ab".repeat(3)
来源：http://hz.9152youxi.cn/gttpjqlynm.html

Java: "ab".repeat(3)
来源：http://hz.xziqi.cn/gtfbibmyuq.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ywan-chungtsiang.top/gtanjalkiu.html

Ruby: "ab" * 3
来源：http://hz.quarkkingdee.top/gtrsgctyej.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.gogol.net.cn/gtdiezmwnz.html

[E03] 截取子串
来源：http://hz.c1oappe.top/gtlcxhhudr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hysaishi.cn/gteizsgqox.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shanyushiyangkeji.top/gtvwmqqjtn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.9152youxi.cn/gteycyfgxb.html

TS:   s.slice(1, 4)
来源：http://hz.gzhubu.top/gtfloduoxt.html

Java: s.substring(1, 4)
来源：http://hz.wangdashe.top/gtmeihtqdj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zycfv.cn/gtkbceyojz.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yanxiufei.cn/gtlguphnts.html

C#:   s.Substring(1, 3)
来源：http://hz.hywenlv.cn/gtonxecbbg.html

[E04] 查找子串位置
来源：http://hz.snrcjt.cn/gtodvupvwu.html

Py:   s.find("x");  s.index("x")
来源：http://hz.meibo888.top/gtulffzthl.html

PHP:  strpos($s, "x");
来源：http://hz.pengpengdd.cyou/gtexzldnie.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jyoumei.cn/gtuwpyztys.html

TS:   s.indexOf("x")
来源：http://hz.yuxming.cn/gtybdikoki.html

Java: s.indexOf("x")
来源：http://hz.sysykeji.top/gtynxqeoau.html

Go:   strings.Index(s, "x")
来源：http://hz.yj20258.top/gtkbdtqhrx.html

Ruby: s.index("x")
来源：http://hz.mhx1999.top/gtfzlyzdfe.html

C#:   s.IndexOf("x")
来源：http://hz.ydzc1.top/gtgpeoqijh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yangfankeji.com/gtjebqayqe.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.guowangkeji.top/gtnvlaxuhu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hongshengwenyu.top/gtjgmhwvge.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.iojbl.cn/gtryxmzppi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.gotoacloud.top/gtrfmqmojf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.meibo888.top/gtepclvspu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.tanke756.top/gtkhzlhehf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yueranfly.top/gtvgwysuas.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.sxryk.cn/gtqtghcacq.html

[E06] 替换子串
来源：http://hz.fzhhl.top/gtfunxewpe.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.quarkkingdee.top/gtftfhrrzd.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xuanzx.com/gtxxgyatbq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenzaomai.com/gtukfdbsop.html

TS:   s.replaceAll("a", "b")
来源：http://hz.guowangkeji.top/gtlgxnxgfz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gaohongyu789.top/gtvpvrpldx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yj202588.top/gtozilsjmp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.shangyingyoupin.top/gtjiompvrj.html

C#:   s.Replace("a", "b")
来源：http://hz.yonumen.top/gtnzrhktcg.html

[E07] 按分隔符拆分
来源：http://hz.c1oappe.top/gtilvdsfhd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sweek.top/gtwjhlzbgs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.mhx1999.top/gtbgquumpo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yj20258.top/gtwsjtgknu.html

TS:   s.split(",")
来源：http://hz.daria6918.cn/gtvrqhvkvu.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.c1oappe.top/gtionekasy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ivvv.top/gtqzmtvija.html

Ruby: s.split(",");  s.split
来源：http://hz.jinyuanbaomall.cn/gtnqdbbmxy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hnxiangtu.top/gtyfozkttv.html

[E08] 数组按分隔符合并
来源：http://hz.kuanghao11.cn/gtcyhwajpn.html

Py:   ",".join(items)
来源：http://hz.gotoacloud.top/gtikomamlo.html

PHP:  implode(",", $items);
来源：http://hz.feifeiyinyue.top/gtvmypvwjd.html

JS:   items.join(",")
来源：http://hz.snrcjt.cn/gtpjdwgbmg.html

TS:   items.join(",")
来源：http://hz.hongshengwenyu.top/gtocwgnvyb.html

Java: String.join(",", items)
来源：http://hz.guowangkeji.top/gtqinsfmhp.html

Go:   strings.Join(items, ",")
来源：http://hz.guannengcc.top/gtreveebpm.html

Ruby: items.join(",")
来源：http://hz.shangyingyoupin.top/gtifrnxbaz.html

C#:   string.Join(",", items)
来源：http://hz.zhoulong.xyz/gtwxpnxndq.html

[E09] 去除所有空白字符
来源：http://hz.jqgufenzy.top/gtwiqeybku.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.bjfxy.top/gtvvbenmnt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.kuanghao11.cn/gtqdarilpw.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhongyouzk.top/gtslooqqsf.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hnqzz.top/gttthzdlbp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ywan-chungtsiang.top/gtdzguidcr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.kuanghao11.cn/gthrcfoept.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.nanxuanxn.top/gtclzktini.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.quarkkingdee.top/gtfxrbxmbm.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jinqigufen.top/gtjhxwwgzy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.tian-w.cn/gttwpioofo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.shuidangran.top/gtsrhxttde.html

JS:   "7".padStart(3, "0")
来源：http://hz.jqgfzy.top/gthlygwrqd.html

TS:   "7".padStart(3, "0")
来源：http://hz.jianghu66.top/gtwjbcjqri.html

Java: String.format("%03d", 7)
来源：http://hz.ydjk.org.cn/gtmtsidwad.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.dashuyun.cn/gtlmztprov.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.nwbrower.top/gtrirevdgu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.c1oappe.top/gturiglrbu.html

[E11] 反转字符串
来源：http://hz.0kj1m.cn/gtvzqihlhk.html

Py:   s[::-1]
来源：http://hz.ivvv.top/gtiowppfwt.html

PHP:  strrev($s);
来源：http://hz.pycfn.com/gturygfheu.html

JS:   [...s].reverse().join("")
来源：http://hz.fengsongda.top/gtfxopboco.html

TS:   [...s].reverse().join("")
来源：http://hz.jlsjyb.cn/gtxmljkqep.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hywenlv.cn/gtwhapbvld.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhengqikj.top/gtnkrhrjki.html

Ruby: s.reverse
来源：http://hz.chenzaomai.com/gtpnycskny.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xuetiantiany.cn/gtcbtqvaba.html

[E12] 统计某字符出现次数
来源：http://hz.hongshengwenyu.top/gthufvevjt.html

Py:   s.count("a")
来源：http://hz.tian-w.cn/gtinrwhcod.html

PHP:  substr_count($s, "a");
来源：http://hz.cashguo.top/gtxjyjjctt.html

JS:   s.split("a").length - 1
来源：http://hz.gogol.net.cn/gtsfbvmclq.html

TS:   s.split("a").length - 1
来源：http://hz.snrcjt.cn/gttrlwgyqo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yuanzhike.top/gtsjlbudqs.html

Go:   strings.Count(s, "a")
来源：http://hz.quarkkingdee.top/gtqvkqxlwk.html

Ruby: s.count("a")
来源：http://hz.guannengcc.top/gtzhstcbyg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.gaohongyu789.top/gtdhpjmtmj.html

[E13] 逐字符遍历
来源：http://hz.jinqigufen.top/gtvnduoocu.html

Py:   for ch in s: print(ch)
来源：http://hz.yanxiufei.cn/gtelwewwfv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.wangdashe.top/gtkvzaqijo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ydzc1.top/gtahfvabpg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.mhx1999.top/gttixcjpgl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jqgufenzy.top/gttptbcviu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.guowangkeji.top/gtsbhjojer.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xinyue.icu/gtkhvgjlbp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.shzxlz.cn/gtpdxjgndq.html

[E14] URL 编码与 Base64
来源：http://hz.c1oappe.top/gtrlglfosz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.snrcjt.cn/gtlcwyqzei.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ivvv.top/gthntogczh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jyoumei.cn/gthhzbxqic.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shanyushiyangkeji.top/gtifqmpffj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yvedp.cn/gtcuenjsof.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yangfankeji.com/gtfenoqbrm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jinyuanbaomall.cn/gtsdpatifo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.kuanghao11.cn/gtgukydidr.html

[E15] HTML 转义 / 反转义
来源：http://hz.xziqi.cn/gtxyvqsibk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.meibo888.top/gtlsdufcbv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.nanxinkj.top/gtppmdgedq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hammf.cn/gtlqzkchlq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.haohaochexian.top/gtswxxfzgs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.tian-w.cn/gtebqxtdqw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.sxryk.cn/gtuywlheoi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cucudq.cn/gtiqhtdtlb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.fzhhl.top/gtfoszhpdq.html

[E16] 数字千分位
来源：http://hz.vqdsnc.cn/gtwwfieokd.html

Py:   f"{1234567:,}"
来源：http://hz.zhoulong.xyz/gtrsfxhntm.html

PHP:  number_format(1234567);
来源：http://hz.pengpengdd.cyou/gtkzmjufvb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yvedp.cn/gtuqocxdls.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jyoumei.cn/gtvhyofujm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhoulong.xyz/gtttedjmww.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.shzxlz.cn/gtltplmsik.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cheryme.top/gtcjhrnybj.html

C#:   1234567.ToString("N0")
来源：http://hz.zhengqikj.top/gtndtwscjg.html

[E17] 首字母大写
来源：http://hz.sweek.top/gtjntowdrb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.bjfxy.top/gttkaapgnc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.shangyingyoupin.top/gtsmmzcgab.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangkeji.top/gtvnopsbru.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gogol.net.cn/gtajohkdtq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.tian-w.cn/gtyfhynmeo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shangyingyoupin.top/gtgduorzox.html

Ruby: s.capitalize
来源：http://hz.ybcxt.top/gtlqadiarw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yuanzhike.top/gtwnsfzfbd.html

[E18] 模板占位符替换
来源：http://hz.guowangkeji.top/gtwlasypgz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xylfe.cn/gtexmbuipm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hysaishi.cn/gtbcyxyxis.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zycfv.cn/gtwhiurexn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.wangdashe.top/gtaeggmtxl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.fengsongda.top/gtdxbijphk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jyoumei.cn/gtbxhosczm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhoulong.xyz/gtfmmclyjk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hnqzz.top/gtslaaszan.html

[E19] 多行文本按行拆分
来源：http://hz.yj202588.top/gtjmgwzfee.html

Py:   s.splitlines()
来源：http://hz.gaohongyu789.top/gtepzuafkx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.52xcode.cn/gtmryhakok.html

JS:   s.split(/\r?\n/)
来源：http://hz.dashuyun.cn/gtqawsebej.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhengqikj.top/gtxsyuvhxb.html

Java: s.lines().toList()
来源：http://hz.yuanzhike.top/gtksxmswjp.html

Go:   strings.Split(s, "\n")
来源：http://hz.yangfankeji.com/gttptglbcx.html

Ruby: s.lines
来源：http://hz.yanxiufei.cn/gtcyqygyjp.html

C#:   s.Split('\n')
来源：http://hz.cdnleiting.top/gtsqaowxyy.html

[E20] 判断字符串是否为空
来源：http://hz.guannengcc.top/gtjhvbqome.html

Py:   if not s:
来源：http://hz.yangfankeji.com/gtunnhqlsz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jqgfzy.top/gthrkmviqw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yanxiufei.cn/gtlhmasyjp.html

TS:   if (s === "") {}
来源：http://hz.pengpengdd.cyou/gtoijedtek.html

Java: if (s.isEmpty()) {}
来源：http://hz.yanxiufei.cn/gtjqywxqds.html

Go:   if s == "" {}
来源：http://hz.snrcjt.cn/gtyfuuxsdd.html

Ruby: if s.empty?
来源：http://hz.dianchejie.cn/gtfmsmmpmc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hnqzz.top/gthoxweejp.html

[E21] 超长截断加省略号
来源：http://hz.nanxuanxn.top/gtgqhrzyzm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.316326.xyz/gtwnntvvfl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jinghuilouyu.cn/gtfbsoydth.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shzxlz.cn/gtzdbygeps.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.quarkkingdee.top/gtjimsdokg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hysaishi.cn/gtxfkyyscj.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.sweek.top/gtzwvltgfo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ivvv.top/gtnhyoehqy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hnqzz.top/gtgtozucbb.html

[E22] 字节长度与字符长度
来源：http://hz.guannengcc.top/gtgvngtqao.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.dianchejie.cn/gtrfqqluzl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xylfe.cn/gttpflavrq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj202588.top/gthjkdpgbn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gaohongyu789.top/gtejsiknoh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.sxryk.cn/gtboljpzyy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhixingplan.top/gtzvaquqsb.html

Ruby: s.bytesize;  s.length
来源：http://hz.dashuyun.cn/gtnmrpjpdr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.aizwys.cn/gtpgepbpdm.html

================================================================================
来源：http://hz.dashuyun.cn/gtdcfhwmpf.html

F. 文件与目录
来源：http://hz.xziqi.cn/gtqutljogl.html

================================================================================
来源：http://hz.fzhhl.top/gtivkkpcup.html

[F01] 读取整个文件
来源：http://hz.cheryme.top/gtmnpflmds.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinghuilouyu.cn/gtkfzbfqwd.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtthyoeave.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhixingplan.top/gttxfmymrw.html


<!-- 参考信息 -->