代发 wailian999

TS:   [...new Set(arr)]
来源：http://hz.zhixingplan.top/gtsumlvccn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jyoumei.cn/gtilwbnbfi.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shzxlz.cn/gtawqyzamy.html

Ruby: arr.uniq
来源：http://hz.vqdsnc.cn/gtgsiubzbl.html

C#:   list.Distinct().ToList()
来源：http://hz.chenzaomai.com/gtudrhxtyg.html

[D16] 求和与平均值
来源：http://hz.zhijiandao.cn/gtcfuoyqqv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.c1oappe.top/gtnzbsncoh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jianghu66.top/gtybgaazsc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yanxiufei.cn/gthcfitria.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ywan-chungtsiang.top/gtlwgqhjuq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ybcxt.top/gtxmwuvaqb.html

Go:   // 手写循环累加
来源：http://hz.zhaomingkeji.xyz/gtqzguoeqt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.dianchejie.cn/gtznbboyaq.html

C#:   list.Sum();  list.Average()
来源：http://hz.quarkkingdee.top/gtglkmrwxe.html

[D17] 最大值与最小值
来源：http://hz.shangyingyoupin.top/gtbxmfjxab.html

Py:   max(arr);  min(arr)
来源：http://hz.jianghu66.top/gtreqgisnh.html

PHP:  max($arr);  min($arr);
来源：http://hz.cucudq.cn/gtrifbthgw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.dianchejie.cn/gtdvhpxtfr.html

TS:   Math.max(...arr);
来源：http://hz.xingfuxueyuan.xyz/gtcslcpquq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yuxming.cn/gtwcpufdam.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yj202588.top/gtgrdjxonf.html

Ruby: arr.max;  arr.min
来源：http://hz.yueranfly.top/gtxldgqhgi.html

C#:   list.Max();  list.Min()
来源：http://hz.sweek.top/gtsgqmyswx.html

[D18] 扁平化嵌套数组
来源：http://hz.ydzc1.top/gtzxxwytzm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ehwqpu.com/gtnilmpqve.html

PHP:  array_merge(...$nested);
来源：http://hz.iojbl.cn/gtqwelivpd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.nanxinkj.top/gtozuyhscf.html

TS:   nested.flat();
来源：http://hz.hnqzz.top/gtbcnhbnmp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.chenzaomai.com/gtwaixwmuj.html

Go:   // 手写双层循环
来源：http://hz.shuidangran.top/gtsrfcicuj.html

Ruby: nested.flatten
来源：http://hz.ywan-chungtsiang.top/gthbrwjtrw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xziqi.cn/gtikvcaijj.html

[D19] 按字段分组
来源：http://hz.gogol.net.cn/gtxefdrrju.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cqqwz.cn/gtwdkvxbdm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.aibaodan.cn/gtqxaxuacs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.haohaochexian.top/gtpmyxlnxm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhiwuduotai.top/gtlrbgxqxb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yuxming.cn/gtgyuwslxf.html

Go:   // 手写 map[string][]T
来源：http://hz.yj202588.top/gtfyhglqcv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yangfankeji.com/gtvoiwqzmi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zycfv.cn/gtwbyjuokh.html

[D20] 统计每个元素出现次数
来源：http://hz.dashuyun.cn/gtahixgnad.html

Py:   Counter(arr)
来源：http://hz.jlsjyb.cn/gtyngvydha.html

PHP:  array_count_values($arr);
来源：http://hz.jqgufenzy.top/gtnbbfswfe.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.vqdsnc.cn/gtiqoxptgq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nanxuanxn.top/gtorrrkjbo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.mhx1999.top/gtmxaajecj.html

Go:   // 手写 map[T]int
来源：http://hz.chenlongwang.top/gtznxqyxio.html

Ruby: arr.tally
来源：http://hz.bjfxy.top/gtrvktgley.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.sufxvd.cn/gtukkvoxcp.html

[D21] 判断是否包含某元素
来源：http://hz.shanyushiyangtech.top/gtkfrhpant.html

Py:   x in arr
来源：http://hz.tian-w.cn/gtbdhmcyim.html

PHP:  in_array($x, $arr, true);
来源：http://hz.wangdashe.top/gtzrlybclc.html

JS:   arr.includes(x)
来源：http://hz.wangshuangyany.cn/gtdgwecpkn.html

TS:   arr.includes(x)
来源：http://hz.aizwys.cn/gtsskdgaxh.html

Java: list.contains(x)
来源：http://hz.zhiwuduotai.top/gtgfsfnjtj.html

Go:   slices.Contains(arr, x)
来源：http://hz.daxiang520.top/gtfhavxzig.html

Ruby: arr.include?(x)
来源：http://hz.ppjwa.cn/gtfaqlceyp.html

C#:   list.Contains(x)
来源：http://hz.cheryme.top/gtftcmofqu.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jyoumei.cn/gtcvkuoxwc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yueranfly.top/gtvrvuguwt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yj20258.top/gtunxlszgu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jinghuilouyu.cn/gtjmygrdrd.html

TS:   [...arr];
来源：http://hz.jinqigufen.top/gthffsjmzn.html

Java: new ArrayList<>(list);
来源：http://hz.ydzc1.top/gtapoytida.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.tianlin.xyz/gtyygsmdon.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhongyouzk.top/gtrtebqfrz.html

C#:   new List<int>(list);
来源：http://hz.jlsjyb.cn/gthmgugttg.html

[D23] reduce 累积计算
来源：http://hz.zhiwuduotai.top/gtqcqzhlge.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hysaishi.cn/gtcnyqiheh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jinghuilouyu.cn/gtkrnvrcci.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.wangdashe.top/gtcsgcwqvj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shzxlz.cn/gtmtpolzdy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.gotoacloud.top/gtfmwluvvg.html

Go:   // 手写循环
来源：http://hz.xylfe.cn/gteoudlhmt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hfpthk.cn/gtvrakzbcr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhiwuduotai.top/gtybxocbgt.html

[D24] 字典 / Map 基本操作
来源：http://hz.yongpay.top/gtpqpltpiv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhongyouzk.top/gtifyceaxb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jqgfzy.top/gtlditenml.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gotoacloud.top/gtkatklivg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jqgfzy.top/gtxziyffvh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.fzhhl.top/gtpxscrxsx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yongpay.top/gttcsgwycl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shangyingyoupin.top/gtdetjqgej.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.svipenyu.cn/gtxkoktyxr.html

[D25] Set 集合去重与交并差
来源：http://hz.shzxlz.cn/gtgduydhnd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.dashuyun.cn/gtzxlrtejs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jianghu66.top/gtzxvvxnrq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.aibaodan.cn/gtsnkmkarq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jqgfzy.top/gthynjfycf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.kuanghao11.cn/gtcpuklgku.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ehwqpu.com/gtsoeydlee.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhoulong.xyz/gthmoddexi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.shanyushiyangkeji.top/gtubokxbhj.html

[D26] 数组转字符串
来源：http://hz.dashuyun.cn/gtuhmfldcu.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hfpthk.cn/gtmlfaoimg.html

PHP:  implode(", ", $arr);
来源：http://hz.hnqzz.top/gtjutppzyd.html

JS:   arr.join(", ")
来源：http://hz.gotoacloud.top/gtijnrzump.html

TS:   arr.join(", ")
来源：http://hz.tianlin.xyz/gtjgkvogxy.html

Java: String.join(", ", list)
来源：http://hz.shanyushiyangtech.top/gtryesgwhc.html

Go:   strings.Join(strs, ", ")
来源：http://hz.aizwys.cn/gtfyfhdawa.html

Ruby: arr.join(", ")
来源：http://hz.wangdashe.top/gtkaabgrzn.html

C#:   string.Join(", ", list)
来源：http://hz.pengpengdd.cyou/gtagrelrqv.html

================================================================================
来源：http://hz.chenzaomai.com/gtkalijibr.html

E. 字符串处理
来源：http://hz.xinyue.icu/gtbdujqewz.html

================================================================================
来源：http://hz.ppjwa.cn/gtkjfcnzcx.html

[E01] 拼接字符串
来源：http://hz.zhengqikj.top/gtbldatmcy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.dianchejie.cn/gtdxzrubna.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ybcxt.top/gtmogerxqw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.0kj1m.cn/gtowpflseh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinyuanbaomall.cn/gtpxlkdxqv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yonumen.top/gttsqdozjx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yuanzhike.top/gtslrwmupj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yonumen.top/gtpaxeozuj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.nanxinkj.top/gtpralbrwr.html

[E02] 重复字符串
来源：http://hz.hnqzz.top/gtfsyrobda.html

Py:   "ab" * 3
来源：http://hz.zhongyouzk.top/gtuwciotfy.html

PHP:  str_repeat("ab", 3);
来源：http://hz.nanxinkj.top/gttrjeuzgv.html

JS:   "ab".repeat(3)
来源：http://hz.daxiang520.top/gtzwhynaeh.html

TS:   "ab".repeat(3)
来源：http://hz.ydzc1.top/gtwtwtwftd.html

Java: "ab".repeat(3)
来源：http://hz.tian-w.cn/gtdgstsbfs.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.aibaodan.cn/gtvokaezys.html

Ruby: "ab" * 3
来源：http://hz.guowangkeji.top/gtixgvdarj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhoulong.xyz/gtdkflhoww.html

[E03] 截取子串
来源：http://hz.shanyushiyangkeji.top/gtbioimobx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.gzhubu.top/gtnfopdfln.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.vqdsnc.cn/gtemghdwaq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.sweek.top/gtveewafra.html

TS:   s.slice(1, 4)
来源：http://hz.ydjk.org.cn/gtxqpydonj.html

Java: s.substring(1, 4)
来源：http://hz.shangyingyoupin.top/gtknnhlihi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hfpthk.cn/gtxeorauek.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jinyuanbaomall.cn/gtalrpfmhx.html

C#:   s.Substring(1, 3)
来源：http://hz.316326.xyz/gtadnhwiye.html

[E04] 查找子串位置
来源：http://hz.dashuyun.cn/gtgpbkgnaz.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jinqigufen.top/gtjcyglugg.html

PHP:  strpos($s, "x");
来源：http://hz.feifeiyinyue.top/gttyqrzxmj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zdqjudy.top/gtlhmcjvnt.html

TS:   s.indexOf("x")
来源：http://hz.pycfn.com/gtwuefholl.html

Java: s.indexOf("x")
来源：http://hz.zhaomingkeji.xyz/gtgddyyzmw.html

Go:   strings.Index(s, "x")
来源：http://hz.sweek.top/gtvyhgsgoz.html

Ruby: s.index("x")
来源：http://hz.xingfuxueyuan.xyz/gtzxiqqrlq.html

C#:   s.IndexOf("x")
来源：http://hz.c1oappe.top/gtzzrisbbv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jqgfzy.top/gtjxmnyool.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhiwuduotai.top/gtsxbzevof.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.haohaochexian.top/gtnzxaqpkl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.andypj.xyz/gthxqiufia.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.svipenyu.cn/gtbbxrbfzg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ydzc1.top/gtggtecrgz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.mhx1999.top/gtzosqdiqr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.andypj.xyz/gtaenusbek.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hnxiangtu.top/gtdlpeocnr.html

[E06] 替换子串
来源：http://hz.zhiwuduotai.top/gttcnaxphi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.tanke756.top/gtshzojnme.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.nwbrower.top/gtneyrxiud.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jiagoushi.top/gtwetkxayy.html

TS:   s.replaceAll("a", "b")
来源：http://hz.tanke756.top/gtjnzqmdtj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenzaomai.com/gtkyjiemip.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.nanxinkj.top/gtjadoxzqv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.52xcode.cn/gtcomfwkaa.html

C#:   s.Replace("a", "b")
来源：http://hz.zycfv.cn/gtekgzdyhp.html

[E07] 按分隔符拆分
来源：http://hz.redwolf501.top/gtmchmrjda.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.snrcjt.cn/gtcfesrxkb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.wangshuangyany.cn/gtmgknjsmb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hnxiangtu.top/gtewjismze.html

TS:   s.split(",")
来源：http://hz.shuidangran.top/gtqlrbfzqp.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.wangdashe.top/gtttwtyaok.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.kuanghao11.cn/gtmjbjxnfk.html

Ruby: s.split(",");  s.split
来源：http://hz.9152youxi.cn/gtbgzxqknp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.cqqwz.cn/gtzddpubkf.html

[E08] 数组按分隔符合并
来源：http://hz.yuanzhike.top/gtxygiyfkt.html

Py:   ",".join(items)
来源：http://hz.aibaodan.cn/gtwhqfitju.html

PHP:  implode(",", $items);
来源：http://hz.gzhubu.top/gtugnxwwcf.html

JS:   items.join(",")
来源：http://hz.zhongyouzk.top/gtxvvdberc.html

TS:   items.join(",")
来源：http://hz.andypj.xyz/gtgtdwhoga.html

Java: String.join(",", items)
来源：http://hz.xuetiantiany.cn/gtqkrfczjn.html

Go:   strings.Join(items, ",")
来源：http://hz.jianghu66.top/gtlwjcpaoa.html

Ruby: items.join(",")
来源：http://hz.nanxuanxn.top/gtjceywaau.html

C#:   string.Join(",", items)
来源：http://hz.zycfv.cn/gtobzlfoun.html

[E09] 去除所有空白字符
来源：http://hz.zdqjudy.top/gtccinktge.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.shuidangran.top/gtrbdvpmjb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jqgufenzy.top/gtlvgkgpgr.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.birdmap.top/gtaxmvygwz.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.snrcjt.cn/gtvpkleryj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xziqi.cn/gtufrzryku.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.nwbrower.top/gtxtpepppy.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hnqzz.top/gtalmjcsjm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xylfe.cn/gtcttjquua.html

[E10] 左侧补零 / 定长填充
来源：http://hz.guannengcc.top/gtdzplinyh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.iojbl.cn/gtorfjehrb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhaomingkeji.xyz/gtrliabkkr.html

JS:   "7".padStart(3, "0")
来源：http://hz.ehwqpu.com/gttnjfxleq.html

TS:   "7".padStart(3, "0")
来源：http://hz.cdnleiting.top/gtoabijavf.html

Java: String.format("%03d", 7)
来源：http://hz.tanke756.top/gtxzffbqje.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shanyushiyangtech.top/gtvyilcwsz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hammf.cn/gtxyvojmuu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cashguo.top/gtmwgbdjwu.html

[E11] 反转字符串
来源：http://hz.dashuyun.cn/gtghbdegyp.html

Py:   s[::-1]
来源：http://hz.jinghuilouyu.cn/gtszzyvtov.html

PHP:  strrev($s);
来源：http://hz.ydjk.org.cn/gteyvdmzqt.html

JS:   [...s].reverse().join("")
来源：http://hz.cashguo.top/gtaydxxdpc.html

TS:   [...s].reverse().join("")
来源：http://hz.yuxming.cn/gtubnvteyd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yj202588.top/gtcbbbujur.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hnxiangtu.top/gtqjqgejbb.html

Ruby: s.reverse
来源：http://hz.svipenyu.cn/gtvuzbdqhm.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.nwbrower.top/gtubjxijvf.html

[E12] 统计某字符出现次数
来源：http://hz.fzhhl.top/gtxnjukgfo.html

Py:   s.count("a")
来源：http://hz.aibaodan.cn/gtuptjepkl.html

PHP:  substr_count($s, "a");
来源：http://hz.zycfv.cn/gtjtktufzf.html

JS:   s.split("a").length - 1
来源：http://hz.snrcjt.cn/gtuapdpdxv.html

TS:   s.split("a").length - 1
来源：http://hz.pengpengdd.cyou/gtjouzycsw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.vqdsnc.cn/gthmfvqyjj.html

Go:   strings.Count(s, "a")
来源：http://hz.c1oappe.top/gtaitpvxmm.html

Ruby: s.count("a")
来源：http://hz.yuxming.cn/gtbczzkeju.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ydjk.org.cn/gtzcxklsij.html

[E13] 逐字符遍历
来源：http://hz.mhx1999.top/gtnmujbldw.html

Py:   for ch in s: print(ch)
来源：http://hz.birdmap.top/gtrgmlgoei.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.svipenyu.cn/gtpjmjkdwr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinqigufen.top/gttrokmzdn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.52xcode.cn/gtpapwqreo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.gotoacloud.top/gtjwsucwpj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cdnleiting.top/gtlsgirjyk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.9152youxi.cn/gtusrhmkds.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ehwqpu.com/gtghebwxsz.html

[E14] URL 编码与 Base64
来源：http://hz.ehwqpu.com/gttggskhuf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.andypj.xyz/gtbdsxniqo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.aibaodan.cn/gthqjobrds.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shangyingyoupin.top/gtxynorlbz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.redwolf501.top/gtsjjihpcx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.sxryk.cn/gtgtoawjps.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shanyushiyangkeji.top/gtkjujjsvn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xinyue.icu/gtcwjlhajw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yangfankeji.com/gtpwxnstzb.html

[E15] HTML 转义 / 反转义
来源：http://hz.ydzc1.top/gtqholvgap.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.daxiang520.top/gtytofwqzp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hywenlv.cn/gtmpkfgevr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.guannengcc.top/gtvyndiulh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.316326.xyz/gtszemglft.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jinghuilouyu.cn/gtpepoxufj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ydjk.org.cn/gtxdsnrzvt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jqgfzy.top/gtnclhzwuk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.tanke756.top/gtmfqvcxxh.html

[E16] 数字千分位
来源：http://hz.aizwys.cn/gttehlaeyr.html

Py:   f"{1234567:,}"
来源：http://hz.havefunace.top/gtroqruxql.html

PHP:  number_format(1234567);
来源：http://hz.nanxuanxn.top/gtcfbalqsj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.nwbrower.top/gtohopqorp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydjk.org.cn/gtqclehgau.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.wangshuangyany.cn/gtrwfmtfum.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hongshengwenyu.top/gtnpsinjwh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.fengsongda.top/gtbyqrwfuj.html

C#:   1234567.ToString("N0")
来源：http://hz.shzxlz.cn/gtfrfwdsro.html

[E17] 首字母大写
来源：http://hz.cheryme.top/gtkhhqmhla.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xuetiantiany.cn/gtglzzdxaw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xingfuxueyuan.xyz/gtwrtjbbim.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydzc1.top/gtjjwgzkbi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinghuilouyu.cn/gttcdsrxyk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jianghu66.top/gtvlubrihc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xingfuxueyuan.xyz/gtszlshhdv.html

Ruby: s.capitalize
来源：http://hz.cheryme.top/gtkzmcbxqf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xylfe.cn/gtnvepagos.html

[E18] 模板占位符替换
来源：http://hz.wangdashe.top/gtzxtadtmf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.andypj.xyz/gtvrlbvvbv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.gogol.net.cn/gtepxptjzq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenlongwang.top/gtnrmindbq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hywenlv.cn/gtooozspng.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.haohaochexian.top/gtgllrvynf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.meibo888.top/gtvbwtfaso.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hywenlv.cn/gtxmiygjyv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.meibo888.top/gtnhzikpqv.html

[E19] 多行文本按行拆分
来源：http://hz.feifeiyinyue.top/gtrkfrpzxc.html

Py:   s.splitlines()
来源：http://hz.daxiang520.top/gtwdzifece.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jinghuilouyu.cn/gtjmeclouc.html

JS:   s.split(/\r?\n/)
来源：http://hz.hywenlv.cn/gtvquxgjji.html

TS:   s.split(/\r?\n/)
来源：http://hz.gogol.net.cn/gtfrxwxtpg.html

Java: s.lines().toList()
来源：http://hz.cheryme.top/gtrmsoaece.html

Go:   strings.Split(s, "\n")
来源：http://hz.guannengcc.top/gtafjitcvs.html

Ruby: s.lines
来源：http://hz.gzhubu.top/gtlpoqlfcr.html

C#:   s.Split('\n')
来源：http://hz.gzhubu.top/gtipapacju.html

[E20] 判断字符串是否为空
来源：http://hz.tanke756.top/gtwvupdmvq.html

Py:   if not s:
来源：http://hz.ybcxt.top/gtdapmlniu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jqgfzy.top/gtqckmwqnj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jqgufenzy.top/gtsyeltgsl.html

TS:   if (s === "") {}
来源：http://hz.hammf.cn/gtqomqzvpx.html

Java: if (s.isEmpty()) {}
来源：http://hz.iojbl.cn/gtnbuvyewj.html

Go:   if s == "" {}
来源：http://hz.zhongyouzk.top/gtbwazegib.html

Ruby: if s.empty?
来源：http://hz.tanke756.top/gtbacdiwzd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jinyuanbaomall.cn/gtzelgxppk.html

[E21] 超长截断加省略号
来源：http://hz.shanyushiyangtech.top/gtobiqsuub.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hongshengwenyu.top/gtanvsafaw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jinqigufen.top/gtsmwiqqoq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yvedp.cn/gtvtsncijo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhiwuduotai.top/gtshibtufa.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cashguo.top/gteybeeqrr.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.daria6918.cn/gtpardxyea.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shangyingyoupin.top/gtqzpjcqgt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.snrcjt.cn/gtadwjtdqx.html

[E22] 字节长度与字符长度
来源：http://hz.snrcjt.cn/gttnjfhgyl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.sysykeji.top/gtyemlrfxe.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gotoacloud.top/gtjnucbkjh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinghuilouyu.cn/gtzzwfgfhr.html


<!-- 参考信息 -->