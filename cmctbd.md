代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.kuanghao11.cn/gtppugikfd.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xingfuxueyuan.xyz/gtkqseugig.html

TS:   arr.filter(x => x > 3)
来源：http://hz.gaohongyu789.top/gtbbdqwcqn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.wangdashe.top/gthfdxoypz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.fengsongda.top/gtnbkqusja.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.chenzaomai.com/gtqmcotaov.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.birdmap.top/gtobhkubxd.html

[D14] 映射转换（每个元素变形）
来源：http://hz.guannengcc.top/gtmswznzwl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.andypj.xyz/gttbdgwnjo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.wangdashe.top/gtmqdgvagi.html

JS:   arr.map(x => x * 2)
来源：http://hz.shzxlz.cn/gtnhfovtgg.html

TS:   arr.map(x => x * 2)
来源：http://hz.ydjk.org.cn/gtblrcnjyg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jyoumei.cn/gtmjhixdwx.html

Go:   // 手写循环
来源：http://hz.shuidangran.top/gtstcmeqho.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gotoacloud.top/gtvfwnzcrb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.aibaodan.cn/gtmxlksdai.html

[D15] 去重
来源：http://hz.ppjwa.cn/gtxdnrbpyn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xuanzx.com/gtevdoteko.html

PHP:  array_unique($arr);
来源：http://hz.iojbl.cn/gtlcpodfgz.html

JS:   [...new Set(arr)]
来源：http://hz.ydjk.org.cn/gtlaymtxmz.html

TS:   [...new Set(arr)]
来源：http://hz.hfpthk.cn/gtchmeflje.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yangfankeji.com/gtjvtztrcj.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.bjfxy.top/gtdivoonrv.html

Ruby: arr.uniq
来源：http://hz.zhijiandao.cn/gtmoifreag.html

C#:   list.Distinct().ToList()
来源：http://hz.aibaodan.cn/gtmsvmjdfi.html

[D16] 求和与平均值
来源：http://hz.hfpthk.cn/gtpxranjcy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhijiandao.cn/gtztooixvl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ydzc1.top/gtmncuxnbx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tianlin.xyz/gtvibcwmxh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinyuanbaomall.cn/gtkivqmpmm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yj20258888.top/gtkoedjqda.html

Go:   // 手写循环累加
来源：http://hz.jqgfzy.top/gtgholewrj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.0kj1m.cn/gtcnyvtgzl.html

C#:   list.Sum();  list.Average()
来源：http://hz.cheryme.top/gtmvdgnndx.html

[D17] 最大值与最小值
来源：http://hz.chenlongwang.top/gtydxlflum.html

Py:   max(arr);  min(arr)
来源：http://hz.tianlin.xyz/gtcijllqvh.html

PHP:  max($arr);  min($arr);
来源：http://hz.mhx1999.top/gtquhhzzkm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.kuanghao11.cn/gtmudckefe.html

TS:   Math.max(...arr);
来源：http://hz.yuanzhike.top/gtgzcvmiul.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yj20258.top/gtykhbugjo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jianghu66.top/gttkegosmv.html

Ruby: arr.max;  arr.min
来源：http://hz.iojbl.cn/gtbqolzjfu.html

C#:   list.Max();  list.Min()
来源：http://hz.xylfe.cn/gtiaomhvsi.html

[D18] 扁平化嵌套数组
来源：http://hz.pycfn.com/gtgwlltceb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhengqikj.top/gtvspdohxw.html

PHP:  array_merge(...$nested);
来源：http://hz.fzhhl.top/gtxiqwjiej.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jqgfzy.top/gtgiwctrkl.html

TS:   nested.flat();
来源：http://hz.daria6918.cn/gtlbpnlupu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.kuanghao11.cn/gtstzoskyl.html

Go:   // 手写双层循环
来源：http://hz.hnqzz.top/gtrzklhrww.html

Ruby: nested.flatten
来源：http://hz.aibaodan.cn/gtwcfhtxmq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yueranfly.top/gtnlrjcvhs.html

[D19] 按字段分组
来源：http://hz.chenzaomai.com/gtmizwvlzj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hysaishi.cn/gtrmymrvlc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.quarkkingdee.top/gtttwccrkj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.haohaochexian.top/gtxdhtupju.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yangfankeji.com/gtedfkhbwh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.smart0.xyz/gtjklqlcqv.html

Go:   // 手写 map[string][]T
来源：http://hz.aibaodan.cn/gtprptdaue.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.daria6918.cn/gtlinqypqh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yangfankeji.com/gtwdbcliet.html

[D20] 统计每个元素出现次数
来源：http://hz.tanke756.top/gtzhcqxjxw.html

Py:   Counter(arr)
来源：http://hz.cqqwz.cn/gtihfyoite.html

PHP:  array_count_values($arr);
来源：http://hz.hnqzz.top/gtorbdxlsn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shzxlz.cn/gttdhtyheh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangtech.top/gtddubnwpr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jiagoushi.top/gtcimtqizs.html

Go:   // 手写 map[T]int
来源：http://hz.meibo888.top/gtrbzzqafl.html

Ruby: arr.tally
来源：http://hz.tian-w.cn/gtuqpuhazh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhixingplan.top/gtqxiojsuz.html

[D21] 判断是否包含某元素
来源：http://hz.52xcode.cn/gtbflsvfro.html

Py:   x in arr
来源：http://hz.guannengcc.top/gtahfcvgzo.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ydzc1.top/gtxwxdjtyc.html

JS:   arr.includes(x)
来源：http://hz.jinqigufen.top/gtnrtsoplm.html

TS:   arr.includes(x)
来源：http://hz.sufxvd.cn/gtkjpowugs.html

Java: list.contains(x)
来源：http://hz.jqgfzy.top/gtcluarzkv.html

Go:   slices.Contains(arr, x)
来源：http://hz.xziqi.cn/gtkemtqrdu.html

Ruby: arr.include?(x)
来源：http://hz.zhaomingkeji.xyz/gtzhypiemj.html

C#:   list.Contains(x)
来源：http://hz.mhx1999.top/gtgalngonb.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shangyingyoupin.top/gtrhadbpuv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.snrcjt.cn/gtfgcfghdv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.redwolf501.top/gtfghwspph.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.svipenyu.cn/gtglzuymrp.html

TS:   [...arr];
来源：http://hz.dianchejie.cn/gtpswijttr.html

Java: new ArrayList<>(list);
来源：http://hz.jinghuilouyu.cn/gtspsypiwe.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zdqjudy.top/gtseswtvkq.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hysaishi.cn/gtakigyefb.html

C#:   new List<int>(list);
来源：http://hz.wangshuangyany.cn/gtyxonurye.html

[D23] reduce 累积计算
来源：http://hz.jqgufenzy.top/gtliegdqot.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.daxiang520.top/gtywaubusy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhoulong.xyz/gtcgkhqlsj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhoulong.xyz/gteyswnnnk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gaohongyu789.top/gtmsvjtswm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhaomingkeji.xyz/gteasdhlnx.html

Go:   // 手写循环
来源：http://hz.shanyushiyangtech.top/gthtsjdxix.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.sysykeji.top/gtnjngxdnz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.shuidangran.top/gthhrhzyli.html

[D24] 字典 / Map 基本操作
来源：http://hz.daxiang520.top/gtzvkfrzcj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.iojbl.cn/gthocerugl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jqgfzy.top/gtftitbgzl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gotoacloud.top/gtdeztwrhi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.pengpengdd.cyou/gtxaujvbit.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.pengpengdd.cyou/gtvqlatrci.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shzxlz.cn/gtpyawyfzx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.kuanghao11.cn/gttalnrgjj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gzhubu.top/gtkaymzibc.html

[D25] Set 集合去重与交并差
来源：http://hz.feifeiyinyue.top/gtijsqtmsl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zycfv.cn/gtfafyyznm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.aizwys.cn/gtcimhvpif.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.nanxuanxn.top/gtgdwwkuuv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xylfe.cn/gtmzwgtdri.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jinyuanbaomall.cn/gtnursgcdf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.0kj1m.cn/gtlmvvtkov.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhixingplan.top/gtftpdmnvd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.tian-w.cn/gtpypxbtaj.html

[D26] 数组转字符串
来源：http://hz.iojbl.cn/gtxpdcnizt.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhijiandao.cn/gtgxqhmdxw.html

PHP:  implode(", ", $arr);
来源：http://hz.cashguo.top/gtzqfrltsp.html

JS:   arr.join(", ")
来源：http://hz.316326.xyz/gthwulohxl.html

TS:   arr.join(", ")
来源：http://hz.zhiwuduotai.top/gtmvehevny.html

Java: String.join(", ", list)
来源：http://hz.sxryk.cn/gtcmxsoftu.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yanxiufei.cn/gthbdkcqux.html

Ruby: arr.join(", ")
来源：http://hz.aizwys.cn/gtfhhckjpd.html

C#:   string.Join(", ", list)
来源：http://hz.gotoacloud.top/gtsnxbqzde.html

================================================================================
来源：http://hz.sxryk.cn/gtdzwwnxaw.html

E. 字符串处理
来源：http://hz.yangfankeji.com/gtesmarhmh.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtganmkvyf.html

[E01] 拼接字符串
来源：http://hz.zhoulong.xyz/gtecmdpikh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jiagoushi.top/gtcddfdtta.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hnxiangtu.top/gtmzkllftl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.meibo888.top/gtjkelvawz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ydjk.org.cn/gtstlimhtr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shanyushiyangtech.top/gtdmcndmre.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.ehwqpu.com/gtrhfgrjci.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.gzhubu.top/gtnnwwjdgl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.havefunace.top/gturdsrmaj.html

[E02] 重复字符串
来源：http://hz.jqgfzy.top/gtvhqldatg.html

Py:   "ab" * 3
来源：http://hz.xuetiantiany.cn/gtvzxhrhdd.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yueranfly.top/gttsudgfhx.html

JS:   "ab".repeat(3)
来源：http://hz.yuxming.cn/gttvosyyrh.html

TS:   "ab".repeat(3)
来源：http://hz.jinghuilouyu.cn/gtbbvyhuwm.html

Java: "ab".repeat(3)
来源：http://hz.sweek.top/gtdphmtiqy.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.pycfn.com/gtamnqedfn.html

Ruby: "ab" * 3
来源：http://hz.smart0.xyz/gtiqsvalmj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yj20258888.top/gtsrsycpgb.html

[E03] 截取子串
来源：http://hz.fzhhl.top/gtcmuffgmj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ydjk.org.cn/gtakboclpm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hywenlv.cn/gteyzqxrpf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhoulong.xyz/gtghlwpvtg.html

TS:   s.slice(1, 4)
来源：http://hz.feifeiyinyue.top/gtkvykkewf.html

Java: s.substring(1, 4)
来源：http://hz.gogol.net.cn/gtcqvxfvxd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.shangyingyoupin.top/gtkfptsmse.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cashguo.top/gturqjcnjw.html

C#:   s.Substring(1, 3)
来源：http://hz.snrcjt.cn/gtbrpbxyxy.html

[E04] 查找子串位置
来源：http://hz.zhoulong.xyz/gtavdneuob.html

Py:   s.find("x");  s.index("x")
来源：http://hz.haohaochexian.top/gtrbmytgjj.html

PHP:  strpos($s, "x");
来源：http://hz.cucudq.cn/gtmhagtfxu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yonumen.top/gtamqwbpbr.html

TS:   s.indexOf("x")
来源：http://hz.zdqjudy.top/gtegfhapps.html

Java: s.indexOf("x")
来源：http://hz.pycfn.com/gtdeontbew.html

Go:   strings.Index(s, "x")
来源：http://hz.ybcxt.top/gtprcybxyn.html

Ruby: s.index("x")
来源：http://hz.sysykeji.top/gtyuwmszke.html

C#:   s.IndexOf("x")
来源：http://hz.zhaomingkeji.xyz/gtyfpdtptw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.9152youxi.cn/gtcopxdopb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.snrcjt.cn/gtytbizhbg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.aibaodan.cn/gtizhexdoe.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sufxvd.cn/gtvwetcpgh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yj202588.top/gtgmflcpep.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yuxming.cn/gterdwveyk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zhijiandao.cn/gtjtkyxkdg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.haohaochexian.top/gtmtqwuwkp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ydjk.org.cn/gtnzmdixbb.html

[E06] 替换子串
来源：http://hz.ehwqpu.com/gttdtjiabb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ybcxt.top/gtwkklmjvu.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.tanke756.top/gtqiiqkydk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.daxiang520.top/gtlafdrpbv.html

TS:   s.replaceAll("a", "b")
来源：http://hz.quarkkingdee.top/gtujwvvdrk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jlsjyb.cn/gtvyciaolc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhengqikj.top/gtusygdwlw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jiagoushi.top/gtpqheryjh.html

C#:   s.Replace("a", "b")
来源：http://hz.jinqigfzy.top/gtlehfgmpw.html

[E07] 按分隔符拆分
来源：http://hz.cashguo.top/gtpjvpiwsd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.shzxlz.cn/gtaiyagutv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cucudq.cn/gtzrtnsuce.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cdnleiting.top/gthrwpquaq.html

TS:   s.split(",")
来源：http://hz.yvedp.cn/gtlumcuylj.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.havefunace.top/gthwljlvqr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.wangshuangyany.cn/gtxcaxtiqo.html

Ruby: s.split(",");  s.split
来源：http://hz.shanyushiyangkeji.top/gtkfiwdzqd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yj202588.top/gtwopidhzu.html

[E08] 数组按分隔符合并
来源：http://hz.zhongyouzk.top/gtcechetad.html

Py:   ",".join(items)
来源：http://hz.tian-w.cn/gtaispxgoy.html

PHP:  implode(",", $items);
来源：http://hz.havefunace.top/gtzvbctekc.html

JS:   items.join(",")
来源：http://hz.ybcxt.top/gtxljfpkss.html

TS:   items.join(",")
来源：http://hz.yvedp.cn/gtrpxdacrx.html

Java: String.join(",", items)
来源：http://hz.cheryme.top/gtcaqeivku.html

Go:   strings.Join(items, ",")
来源：http://hz.yuxming.cn/gtarcofytc.html

Ruby: items.join(",")
来源：http://hz.yj202588.top/gtteywkomu.html

C#:   string.Join(",", items)
来源：http://hz.yj20258.top/gtcpupxlgd.html

[E09] 去除所有空白字符
来源：http://hz.guannengcc.top/gthxxqrqbp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.52xcode.cn/gtokuycjnc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.wangshuangyany.cn/gtdfhytgxe.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.fzhhl.top/gtcotckgje.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cashguo.top/gtjrmwpprn.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.guannengcc.top/gtggskgjmq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xylfe.cn/gtucrsfilo.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hammf.cn/gtqmzgsmie.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.sufxvd.cn/gtkvwzcksp.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hywenlv.cn/gtpjpondar.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.tianlin.xyz/gtqnqecvnc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.bjfxy.top/gtnhvuaiis.html

JS:   "7".padStart(3, "0")
来源：http://hz.yangfankeji.com/gteyqytyrh.html

TS:   "7".padStart(3, "0")
来源：http://hz.bjfxy.top/gtruiqtsxb.html

Java: String.format("%03d", 7)
来源：http://hz.hongshengwenyu.top/gtfzehvxxg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shzxlz.cn/gtgwisssml.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.sufxvd.cn/gtysvvprhw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.svipenyu.cn/gtoijxcprc.html

[E11] 反转字符串
来源：http://hz.sysykeji.top/gtxcixncip.html

Py:   s[::-1]
来源：http://hz.bjfxy.top/gtfismqkpu.html

PHP:  strrev($s);
来源：http://hz.meibo888.top/gthzgdcbji.html

JS:   [...s].reverse().join("")
来源：http://hz.feifeiyinyue.top/gtvektsbsu.html

TS:   [...s].reverse().join("")
来源：http://hz.zhijiandao.cn/gtqckuhihk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.cucudq.cn/gtnpyqcigd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yongpay.top/gtxqqncqbq.html

Ruby: s.reverse
来源：http://hz.mhx1999.top/gtydapqajz.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.dashuyun.cn/gttzxidczt.html

[E12] 统计某字符出现次数
来源：http://hz.tianlin.xyz/gtzvssimdi.html

Py:   s.count("a")
来源：http://hz.hnqzz.top/gtberlkkil.html

PHP:  substr_count($s, "a");
来源：http://hz.snrcjt.cn/gtgxllvxhq.html

JS:   s.split("a").length - 1
来源：http://hz.gzhubu.top/gtojokedbk.html

TS:   s.split("a").length - 1
来源：http://hz.ybcxt.top/gtziayynox.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.quarkkingdee.top/gtztybohub.html

Go:   strings.Count(s, "a")
来源：http://hz.dianchejie.cn/gtjgfciggu.html

Ruby: s.count("a")
来源：http://hz.ywan-chungtsiang.top/gtkrnmyvlx.html

C#:   s.Count(c => c == 'a')
来源：http://hz.tanke756.top/gtwycsovsh.html

[E13] 逐字符遍历
来源：http://hz.hywenlv.cn/gtafpbiuhd.html

Py:   for ch in s: print(ch)
来源：http://hz.yj20258888.top/gtmjwyqxfy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shuidangran.top/gtlkirotzl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nwbrower.top/gthnuqfshu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jqgfzy.top/gtrlkxuubt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xylfe.cn/gtmfhotmoy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ppjwa.cn/gtbgnbuqkg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.cqqwz.cn/gtzapyevkq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhoulong.xyz/gtqetzmice.html

[E14] URL 编码与 Base64
来源：http://hz.aizwys.cn/gtfehvlubg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yanxiufei.cn/gtxfkiggts.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.daxiang520.top/gtjbjfggtn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.aizwys.cn/gtsbarduob.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.daria6918.cn/gtbrdjdmjl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.chenlongwang.top/gtkmymugod.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hysaishi.cn/gtxwywkwbd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ywan-chungtsiang.top/gtwenpgqdu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yongpay.top/gtuakrisjc.html

[E15] HTML 转义 / 反转义
来源：http://hz.redwolf501.top/gtgipnkfnk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.sxryk.cn/gtkoubxuzw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.feifeiyinyue.top/gtioimkwhc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.guowangkeji.top/gtllambspv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xziqi.cn/gtksxbdayd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhaomingkeji.xyz/gtyvnbyhts.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.gzhubu.top/gtjqkcvtpk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhengqikj.top/gthujwaafc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinyuanbaomall.cn/gtcbuftyal.html

[E16] 数字千分位
来源：http://hz.birdmap.top/gtfhhrpxsy.html

Py:   f"{1234567:,}"
来源：http://hz.yangfankeji.com/gtrvdeqkcj.html

PHP:  number_format(1234567);
来源：http://hz.chenzaomai.com/gttwbxlbvh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.quarkkingdee.top/gtknlclkub.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.kuanghao11.cn/gtccjdwuvi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.bjfxy.top/gtxaynuvpn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jiagoushi.top/gtlanssdmv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.fzhhl.top/gtkqgzoqny.html

C#:   1234567.ToString("N0")
来源：http://hz.ppjwa.cn/gtfmwsdzvu.html

[E17] 首字母大写
来源：http://hz.pycfn.com/gtfomnnlec.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ydjk.org.cn/gtlduzvucm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yvedp.cn/gtvaaqtvja.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shuidangran.top/gtscniucjc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gogol.net.cn/gtjyklmpol.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.cqqwz.cn/gtkxhpfgbi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.daxiang520.top/gtqkziprfd.html

Ruby: s.capitalize
来源：http://hz.gzhubu.top/gtpwexwtgu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.smart0.xyz/gtvhbcwgnh.html

[E18] 模板占位符替换
来源：http://hz.feifeiyinyue.top/gtfffitrhu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ywan-chungtsiang.top/gtzxpowmvm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.tianlin.xyz/gtbvryqlab.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.vqdsnc.cn/gtkcdruhwh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.dashuyun.cn/gtmitcnnix.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.fengsongda.top/gtolkrqprz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ydjk.org.cn/gtkbtsilsd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.pengpengdd.cyou/gtqiqgmezr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ehwqpu.com/gtdujnxksg.html

[E19] 多行文本按行拆分
来源：http://hz.hysaishi.cn/gtkjojyifa.html

Py:   s.splitlines()
来源：http://hz.xziqi.cn/gtpyxnporr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.shanyushiyangkeji.top/gtmlblkome.html

JS:   s.split(/\r?\n/)
来源：http://hz.mhx1999.top/gtbdojpjmk.html

TS:   s.split(/\r?\n/)
来源：http://hz.hysaishi.cn/gttywcjvxr.html

Java: s.lines().toList()
来源：http://hz.sxryk.cn/gtpoiwzpef.html

Go:   strings.Split(s, "\n")
来源：http://hz.vqdsnc.cn/gthtcolbgy.html

Ruby: s.lines
来源：http://hz.daxiang520.top/gtjiflmxra.html

C#:   s.Split('\n')
来源：http://hz.yj20258.top/gtgbkllngs.html

[E20] 判断字符串是否为空
来源：http://hz.hywenlv.cn/gtxynlorhs.html

Py:   if not s:
来源：http://hz.zhoulong.xyz/gtapsvjoqu.html


<!-- 参考信息 -->