代发 wailian999

Ruby: arr.index(x)
来源：http://hz.andypj.xyz/gtkpqjfixe.html

C#:   list.IndexOf(x);
来源：http://hz.xziqi.cn/gtemtwghsa.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xziqi.cn/gtjcvgzsqw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.0kj1m.cn/gtvrstlvsf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zycfv.cn/gtbtuykuee.html

JS:   arr.filter(x => x > 3)
来源：http://hz.chenjidiqi.icu/gtdhsppdot.html

TS:   arr.filter(x => x > 3)
来源：http://hz.guannengcc.top/gtnkthuppe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.0kj1m.cn/gtmovkrcds.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.gogol.net.cn/gtufnnqzpj.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.xuanzx.com/gtuffetutz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shanyushiyangkeji.top/gtxcjulzcy.html

[D14] 映射转换（每个元素变形）
来源：http://hz.aibaodan.cn/gtfnsmpemx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yanxiufei.cn/gtgjwzhvgu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jinqigufen.top/gthoatalaj.html

JS:   arr.map(x => x * 2)
来源：http://hz.hnqzz.top/gtqkyncnog.html

TS:   arr.map(x => x * 2)
来源：http://hz.iojbl.cn/gtzgfbrmhw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.feifeiyinyue.top/gtyuiornmy.html

Go:   // 手写循环
来源：http://hz.wangshuangyany.cn/gtshoudbgs.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhixingplan.top/gtyiqeucfc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.pycfn.com/gtyognvcld.html

[D15] 去重
来源：http://hz.vqdsnc.cn/gtoevjvxie.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.gotoacloud.top/gtunjojdch.html

PHP:  array_unique($arr);
来源：http://hz.0kj1m.cn/gtvovlhkge.html

JS:   [...new Set(arr)]
来源：http://hz.yanxiufei.cn/gtsyblhfsv.html

TS:   [...new Set(arr)]
来源：http://hz.xuanzx.com/gtckxffjpj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.fzhhl.top/gtmbowbkjx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.gogol.net.cn/gtgeeaomen.html

Ruby: arr.uniq
来源：http://hz.shzxlz.cn/gtatdpqtwf.html

C#:   list.Distinct().ToList()
来源：http://hz.jinqigfzy.top/gtsvwwojvu.html

[D16] 求和与平均值
来源：http://hz.zhoulong.xyz/gtrnvbtjic.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhaomingkeji.xyz/gtbwiktwqh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ywan-chungtsiang.top/gtqjiiywlg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.meibo888.top/gtrouynfbq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ydjk.org.cn/gttoovppsl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yj20258.top/gtdgkbwwps.html

Go:   // 手写循环累加
来源：http://hz.shuidangran.top/gtaoppxlnx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.chenzaomai.com/gthhpsjlll.html

C#:   list.Sum();  list.Average()
来源：http://hz.mhx1999.top/gtvafzfudn.html

[D17] 最大值与最小值
来源：http://hz.yueranfly.top/gtvmvfzzco.html

Py:   max(arr);  min(arr)
来源：http://hz.xziqi.cn/gtjxhrtstr.html

PHP:  max($arr);  min($arr);
来源：http://hz.316326.xyz/gtrzwbrorf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yangfankeji.com/gtvegxykeu.html

TS:   Math.max(...arr);
来源：http://hz.gotoacloud.top/gtqfzutrwx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hnqzz.top/gtjximpubq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhiwuduotai.top/gtthmawoih.html

Ruby: arr.max;  arr.min
来源：http://hz.yanxiufei.cn/gthmxktyhs.html

C#:   list.Max();  list.Min()
来源：http://hz.ybcxt.top/gtmyprrqep.html

[D18] 扁平化嵌套数组
来源：http://hz.zhaomingkeji.xyz/gtpgayqhqw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ybcxt.top/gtfqbywcfy.html

PHP:  array_merge(...$nested);
来源：http://hz.dashuyun.cn/gtkknymgrn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.quarkkingdee.top/gtybaeqdhq.html

TS:   nested.flat();
来源：http://hz.shangyingyoupin.top/gtujnsuoqd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.haohaochexian.top/gtgnzqqjov.html

Go:   // 手写双层循环
来源：http://hz.yuxming.cn/gtytruditl.html

Ruby: nested.flatten
来源：http://hz.zhoulong.xyz/gtixheeymo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.chenlongwang.top/gtcljuudjp.html

[D19] 按字段分组
来源：http://hz.hywenlv.cn/gtzdjftjou.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yvedp.cn/gtndpnkgtc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yj20258.top/gtaqetrneu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.nanxinkj.top/gtnirocoxu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xingfuxueyuan.xyz/gtxcadbccq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.hongshengwenyu.top/gtxedbjwms.html

Go:   // 手写 map[string][]T
来源：http://hz.zhongyouzk.top/gtrkqqtcro.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cashguo.top/gtdgndqerm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gaohongyu789.top/gtafdazhek.html

[D20] 统计每个元素出现次数
来源：http://hz.haohaochexian.top/gtfcfrrgfe.html

Py:   Counter(arr)
来源：http://hz.zycfv.cn/gthzteirnx.html

PHP:  array_count_values($arr);
来源：http://hz.jiagoushi.top/gtpgkaavnj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgufenzy.top/gtlcxqzxuz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenlongwang.top/gtwluxuzuh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.cheryme.top/gtqqwcskmp.html

Go:   // 手写 map[T]int
来源：http://hz.xuanzx.com/gtwltpinjc.html

Ruby: arr.tally
来源：http://hz.yj202588.top/gtmnqxwhdq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.daria6918.cn/gtrzdywwvh.html

[D21] 判断是否包含某元素
来源：http://hz.zhoulong.xyz/gtzbsbuujf.html

Py:   x in arr
来源：http://hz.smart0.xyz/gttvyiazvu.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jiagoushi.top/gttuhfadqt.html

JS:   arr.includes(x)
来源：http://hz.hywenlv.cn/gtbrwtsvlu.html

TS:   arr.includes(x)
来源：http://hz.sysykeji.top/gtxvawpjjc.html

Java: list.contains(x)
来源：http://hz.ivvv.top/gtemztkpyz.html

Go:   slices.Contains(arr, x)
来源：http://hz.gogol.net.cn/gtaznazder.html

Ruby: arr.include?(x)
来源：http://hz.nwbrower.top/gtpiitvjls.html

C#:   list.Contains(x)
来源：http://hz.havefunace.top/gthpoehdrf.html

[D22] 复制数组（避免共享引用）
来源：http://hz.nanxuanxn.top/gtywosaafq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.feifeiyinyue.top/gtavgnfvxb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xingfuxueyuan.xyz/gtqplnwedg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.smart0.xyz/gtzfjdsgku.html

TS:   [...arr];
来源：http://hz.gotoacloud.top/gtskfthiqg.html

Java: new ArrayList<>(list);
来源：http://hz.shuidangran.top/gtpsvlvvrj.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yangfankeji.com/gtjemejgcr.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jinqigfzy.top/gtlakuaqwt.html

C#:   new List<int>(list);
来源：http://hz.jinghuilouyu.cn/gtlrvvpxpu.html

[D23] reduce 累积计算
来源：http://hz.jianghu66.top/gtkrvyvxzy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yonumen.top/gtotfmecwt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sufxvd.cn/gtrdefxfin.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jyoumei.cn/gtirlxwjbz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ydzc1.top/gtcoonwhbq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yuanzhike.top/gtmwbpjiua.html

Go:   // 手写循环
来源：http://hz.xingfuxueyuan.xyz/gttejnnzeb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.316326.xyz/gtootgzgfq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenlongwang.top/gtfosyynzp.html

[D24] 字典 / Map 基本操作
来源：http://hz.52xcode.cn/gtmupdkpwj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zdqjudy.top/gtnyignfib.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cucudq.cn/gttntffsea.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xziqi.cn/gtkrvdqfzt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jianghu66.top/gtdjgwbcaf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.shanyushiyangkeji.top/gtdpvgswwb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.nanxuanxn.top/gtpzkemjcs.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zycfv.cn/gtrrbxxdkk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hywenlv.cn/gtimhdyeyf.html

[D25] Set 集合去重与交并差
来源：http://hz.xziqi.cn/gtpmdczljo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.dianchejie.cn/gtlycouemr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jqgfzy.top/gtrsxkqkwu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.cdnleiting.top/gtcwgmaadq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hnqzz.top/gtvkcvjbzu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.bjfxy.top/gtmihjymcc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.meibo888.top/gtcyfdhgbg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jlsjyb.cn/gturmomdzj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hfpthk.cn/gtwqpsrwiu.html

[D26] 数组转字符串
来源：http://hz.gotoacloud.top/gtihsptcuo.html

Py:   ", ".join(map(str, arr))
来源：http://hz.guowangkeji.top/gtscmnwywj.html

PHP:  implode(", ", $arr);
来源：http://hz.havefunace.top/gtbdnksbzn.html

JS:   arr.join(", ")
来源：http://hz.bjfxy.top/gtumijshap.html

TS:   arr.join(", ")
来源：http://hz.nanxinkj.top/gtyqoamzrm.html

Java: String.join(", ", list)
来源：http://hz.yj202588.top/gtvggogcpk.html

Go:   strings.Join(strs, ", ")
来源：http://hz.chenzaomai.com/gtvaubczvf.html

Ruby: arr.join(", ")
来源：http://hz.gogol.net.cn/gtphqdcnnd.html

C#:   string.Join(", ", list)
来源：http://hz.haohaochexian.top/gtuumuaaza.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtfgfipoqd.html

E. 字符串处理
来源：http://hz.jyoumei.cn/gtcpzpwmmm.html

================================================================================
来源：http://hz.ppjwa.cn/gtawakvuar.html

[E01] 拼接字符串
来源：http://hz.yj20258.top/gtbwtykcjq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.aibaodan.cn/gtxzlytcit.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ydzc1.top/gtcykebdfn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj202588.top/gtkypyohah.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ehwqpu.com/gtprojoirn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.tian-w.cn/gtlfdzlpyg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jianghu66.top/gtmynkbqms.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.cashguo.top/gthzghjtyu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hnqzz.top/gtblqrytny.html

[E02] 重复字符串
来源：http://hz.gzhubu.top/gtrxtnnxvs.html

Py:   "ab" * 3
来源：http://hz.ppjwa.cn/gtlzqactkw.html

PHP:  str_repeat("ab", 3);
来源：http://hz.sysykeji.top/gtorkqurvu.html

JS:   "ab".repeat(3)
来源：http://hz.zhongyouzk.top/gtzqoxbaut.html

TS:   "ab".repeat(3)
来源：http://hz.dianchejie.cn/gtbkwkheok.html

Java: "ab".repeat(3)
来源：http://hz.dashuyun.cn/gtphotcfjr.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.nanxinkj.top/gtldysuoyx.html

Ruby: "ab" * 3
来源：http://hz.yuxming.cn/gtfspomtln.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xingfuxueyuan.xyz/gtqwfnijzq.html

[E03] 截取子串
来源：http://hz.yueranfly.top/gthgswcccs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.kuanghao11.cn/gtoyoenyta.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.gzhubu.top/gthrapbmkn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.c1oappe.top/gtlgkaxecc.html

TS:   s.slice(1, 4)
来源：http://hz.cqqwz.cn/gtwujnytxz.html

Java: s.substring(1, 4)
来源：http://hz.guannengcc.top/gtwxmywpla.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.nanxuanxn.top/gtltgnesbt.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shanyushiyangtech.top/gtskqgfdfi.html

C#:   s.Substring(1, 3)
来源：http://hz.ybcxt.top/gtmdyzzxmb.html

[E04] 查找子串位置
来源：http://hz.yj20258.top/gtmglrmavp.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhijiandao.cn/gtxtaprqxq.html

PHP:  strpos($s, "x");
来源：http://hz.yongpay.top/gtvbwbcwns.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ybcxt.top/gtmlsjramf.html

TS:   s.indexOf("x")
来源：http://hz.xingfuxueyuan.xyz/gttttfhatx.html

Java: s.indexOf("x")
来源：http://hz.sxryk.cn/gtbwbcqifr.html

Go:   strings.Index(s, "x")
来源：http://hz.xuetiantiany.cn/gttzpwewtp.html

Ruby: s.index("x")
来源：http://hz.shuidangran.top/gttfqjreni.html

C#:   s.IndexOf("x")
来源：http://hz.wangshuangyany.cn/gtudpjonqc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.aizwys.cn/gtxtstqtqx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xuetiantiany.cn/gtrygvsose.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jyoumei.cn/gtscsktutd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shanyushiyangtech.top/gtvmlumnob.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.smart0.xyz/gtzlhdwxgp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.quarkkingdee.top/gtwzarvyha.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cashguo.top/gtmetxkstn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhixingplan.top/gteisffzkj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.smart0.xyz/gtnlvzygba.html

[E06] 替换子串
来源：http://hz.9152youxi.cn/gtfqbzpdez.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jianghu66.top/gtcnkmtocc.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ydjk.org.cn/gtzsotsjpv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sxryk.cn/gtyrlaizrf.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cheryme.top/gtezmzasll.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.vqdsnc.cn/gtmpbepxvh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jlsjyb.cn/gtlpznmprd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.wangdashe.top/gtdkwxkluz.html

C#:   s.Replace("a", "b")
来源：http://hz.zhengqikj.top/gtxzyoqxlb.html

[E07] 按分隔符拆分
来源：http://hz.smart0.xyz/gtnqphtpsw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhijiandao.cn/gtmljoluzk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hammf.cn/gtlcbfoshp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hongshengwenyu.top/gtbhdxlrvv.html

TS:   s.split(",")
来源：http://hz.shzxlz.cn/gtzfulnnha.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhaomingkeji.xyz/gtcrxvyaig.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.fengsongda.top/gtlvccozkh.html

Ruby: s.split(",");  s.split
来源：http://hz.redwolf501.top/gtbkpqtuvm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.0kj1m.cn/gtuvxmfioa.html

[E08] 数组按分隔符合并
来源：http://hz.aizwys.cn/gtqnmjwihv.html

Py:   ",".join(items)
来源：http://hz.zycfv.cn/gtmgjetero.html

PHP:  implode(",", $items);
来源：http://hz.birdmap.top/gtwejmjatp.html

JS:   items.join(",")
来源：http://hz.snrcjt.cn/gtmewlpujo.html

TS:   items.join(",")
来源：http://hz.shanyushiyangtech.top/gtyrzvmcvf.html

Java: String.join(",", items)
来源：http://hz.zhongyouzk.top/gttxpeqmlr.html

Go:   strings.Join(items, ",")
来源：http://hz.birdmap.top/gtmdmvbpim.html

Ruby: items.join(",")
来源：http://hz.zhoulong.xyz/gtiqppxjqn.html

C#:   string.Join(",", items)
来源：http://hz.yj20258888.top/gtwcsxwlus.html

[E09] 去除所有空白字符
来源：http://hz.cqqwz.cn/gtrgkciisn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jinyuanbaomall.cn/gtpfelatqv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zycfv.cn/gtfjggxlri.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.dashuyun.cn/gthdvzecba.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.c1oappe.top/gtnhgzfqxq.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.cashguo.top/gtymaxzpcp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.aibaodan.cn/gtxqbwzqlz.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yj20258888.top/gtlwsskxvy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.gogol.net.cn/gtlmhwcrhs.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhengqikj.top/gtcjiblxbn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhaomingkeji.xyz/gtaervmbmc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhengqikj.top/gtlxyzlysf.html

JS:   "7".padStart(3, "0")
来源：http://hz.guannengcc.top/gtyzbybcgg.html

TS:   "7".padStart(3, "0")
来源：http://hz.cashguo.top/gtxpolonua.html

Java: String.format("%03d", 7)
来源：http://hz.gotoacloud.top/gthxterdau.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.wangshuangyany.cn/gtegiaqwsp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.iojbl.cn/gtsywyaeeq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zdqjudy.top/gthkedviuo.html

[E11] 反转字符串
来源：http://hz.0kj1m.cn/gtbcxncioy.html

Py:   s[::-1]
来源：http://hz.andypj.xyz/gticsncznh.html

PHP:  strrev($s);
来源：http://hz.tanke756.top/gtyaflpaci.html

JS:   [...s].reverse().join("")
来源：http://hz.ydjk.org.cn/gtgcaismyo.html

TS:   [...s].reverse().join("")
来源：http://hz.aibaodan.cn/gtbanwzfch.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.sweek.top/gtyrvlvzau.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.daria6918.cn/gtjzdmxhwj.html

Ruby: s.reverse
来源：http://hz.shzxlz.cn/gtktdrbvpu.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.tanke756.top/gtxgcxzydw.html

[E12] 统计某字符出现次数
来源：http://hz.feifeiyinyue.top/gtpfvotqux.html

Py:   s.count("a")
来源：http://hz.dashuyun.cn/gtucpduxrc.html

PHP:  substr_count($s, "a");
来源：http://hz.xingfuxueyuan.xyz/gtwcvvmmgl.html

JS:   s.split("a").length - 1
来源：http://hz.jyoumei.cn/gtmnttijoh.html

TS:   s.split("a").length - 1
来源：http://hz.hnxiangtu.top/gtzzjnjvfj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.tanke756.top/gtrjxuxkee.html

Go:   strings.Count(s, "a")
来源：http://hz.yj20258.top/gtvrwyeqnk.html

Ruby: s.count("a")
来源：http://hz.ppjwa.cn/gtqmtmydoe.html

C#:   s.Count(c => c == 'a')
来源：http://hz.kuanghao11.cn/gtleoghusu.html

[E13] 逐字符遍历
来源：http://hz.cqqwz.cn/gthkbnihgi.html

Py:   for ch in s: print(ch)
来源：http://hz.tian-w.cn/gtdyrounry.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ydjk.org.cn/gtwojnpmyu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tianlin.xyz/gtskzgckut.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nwbrower.top/gtibgomkgm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yj20258.top/gtxodpijdf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hongshengwenyu.top/gtfmltjjkq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jinghuilouyu.cn/gtxzqcvhmv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.dianchejie.cn/gtnkvqvxag.html

[E14] URL 编码与 Base64
来源：http://hz.hammf.cn/gtzmlyoqod.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yanxiufei.cn/gtkfczijwm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.svipenyu.cn/gtsgmznqyc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yj20258888.top/gttevozxtq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.meibo888.top/gtrwbygxrp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cucudq.cn/gtrrnskhqu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shangyingyoupin.top/gtwdbuhimy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.chenjidiqi.icu/gtbcfvwpvi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jqgufenzy.top/gtolknqzpv.html

[E15] HTML 转义 / 反转义
来源：http://hz.birdmap.top/gtfmcbsjvh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.wangshuangyany.cn/gtqtivmzgk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ehwqpu.com/gtkqhparvi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.mhx1999.top/gtifzqgnmo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.chenzaomai.com/gtypithucc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yvedp.cn/gtuseznlfc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.shanyushiyangkeji.top/gtlpirxjhg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.birdmap.top/gtxaduwtos.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yj20258888.top/gtkhbxilcb.html

[E16] 数字千分位
来源：http://hz.aizwys.cn/gtinethrur.html

Py:   f"{1234567:,}"
来源：http://hz.yj20258.top/gtcdjscevf.html

PHP:  number_format(1234567);
来源：http://hz.hnxiangtu.top/gtcoscybta.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinyuanbaomall.cn/gtgpcdngkb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinghuilouyu.cn/gtussfozls.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.kuanghao11.cn/gtjzrcevcy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.fzhhl.top/gthxsndpmt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.iojbl.cn/gtpbyngcmh.html

C#:   1234567.ToString("N0")
来源：http://hz.xinyue.icu/gthfkyuyra.html

[E17] 首字母大写
来源：http://hz.haohaochexian.top/gtfjhmzvmf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cqqwz.cn/gtwuhrudxh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jinqigufen.top/gtpugyiiew.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hnxiangtu.top/gtjhtcoieq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xuetiantiany.cn/gtmipitviq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhijiandao.cn/gtbdybuzln.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinqigfzy.top/gtmijkhmog.html

Ruby: s.capitalize
来源：http://hz.zdqjudy.top/gtdyxexywp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yvedp.cn/gtznqrypeg.html

[E18] 模板占位符替换
来源：http://hz.xuetiantiany.cn/gtajciytcu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jyoumei.cn/gtdpnsdyaq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ydjk.org.cn/gtynpyqqhx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.c1oappe.top/gtgwzkkvoy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xuetiantiany.cn/gtehmcnugy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.cheryme.top/gttboyoqio.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shanyushiyangtech.top/gtrbcebaky.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jianghu66.top/gtnvoibfuo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hfpthk.cn/gtwjadoctz.html

[E19] 多行文本按行拆分
来源：http://hz.52xcode.cn/gtqffsizot.html

Py:   s.splitlines()
来源：http://hz.zdqjudy.top/gtkywcvoti.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhijiandao.cn/gtdwereymc.html

JS:   s.split(/\r?\n/)
来源：http://hz.yongpay.top/gtdpkwgkjx.html

TS:   s.split(/\r?\n/)
来源：http://hz.nanxinkj.top/gtioehbnsg.html

Java: s.lines().toList()
来源：http://hz.ydjk.org.cn/gtiukjcntl.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhixingplan.top/gtxkntngzb.html


<!-- 参考信息 -->