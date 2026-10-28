代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ivvv.top/gtyuzmvrrx.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hammf.cn/gtacifbkrp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.tanke756.top/gtyptwlsic.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhengqikj.top/gtguolvrui.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zycfv.cn/gtidzhwjka.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.vqdsnc.cn/gtgytepfdv.html

JS:   arr.map(x => x * 2)
来源：http://hz.hongshengwenyu.top/gtxyqxsnmf.html

TS:   arr.map(x => x * 2)
来源：http://hz.hammf.cn/gtsfqzjair.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.wangdashe.top/gtwufyrsfz.html

Go:   // 手写循环
来源：http://hz.ivvv.top/gtffigfhjz.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jqgufenzy.top/gtotudiucj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.cheryme.top/gtiuivetul.html

[D15] 去重
来源：http://hz.hywenlv.cn/gtccleoifp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jinghuilouyu.cn/gtwgqjgjpn.html

PHP:  array_unique($arr);
来源：http://hz.kuanghao11.cn/gtthvwkzgp.html

JS:   [...new Set(arr)]
来源：http://hz.aibaodan.cn/gtkbfjacqp.html

TS:   [...new Set(arr)]
来源：http://hz.svipenyu.cn/gtgrgetkhn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.sysykeji.top/gteailacgn.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ybcxt.top/gtgogaqpiv.html

Ruby: arr.uniq
来源：http://hz.jiagoushi.top/gttpodkkwp.html

C#:   list.Distinct().ToList()
来源：http://hz.nanxuanxn.top/gttozgcjpd.html

[D16] 求和与平均值
来源：http://hz.gogol.net.cn/gtizpuedxs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jlsjyb.cn/gtinkyhuim.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.wangdashe.top/gtrzuqlsib.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hnxiangtu.top/gtbwkrwyfe.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cashguo.top/gtdjdespeh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ybcxt.top/gtdifnkwro.html

Go:   // 手写循环累加
来源：http://hz.jinqigufen.top/gtuhqlrcwp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.cashguo.top/gtpovqrwzm.html

C#:   list.Sum();  list.Average()
来源：http://hz.kuanghao11.cn/gtgkccjifs.html

[D17] 最大值与最小值
来源：http://hz.zhengqikj.top/gtodyfytsi.html

Py:   max(arr);  min(arr)
来源：http://hz.yvedp.cn/gtzahkckwo.html

PHP:  max($arr);  min($arr);
来源：http://hz.wangdashe.top/gtycooepfi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jlsjyb.cn/gtbxzhyncg.html

TS:   Math.max(...arr);
来源：http://hz.ehwqpu.com/gthmlvuihi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ppjwa.cn/gtsipbpvuo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.snrcjt.cn/gtyphryyxs.html

Ruby: arr.max;  arr.min
来源：http://hz.meibo888.top/gtqflsufuz.html

C#:   list.Max();  list.Min()
来源：http://hz.ywan-chungtsiang.top/gtjnnpisii.html

[D18] 扁平化嵌套数组
来源：http://hz.pengpengdd.cyou/gtcsmuupsb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.gogol.net.cn/gtdjfobtbr.html

PHP:  array_merge(...$nested);
来源：http://hz.yj20258888.top/gtycauhjah.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hnqzz.top/gtjzvmueey.html

TS:   nested.flat();
来源：http://hz.ydzc1.top/gtxjyexaex.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jinghuilouyu.cn/gtufaarufo.html

Go:   // 手写双层循环
来源：http://hz.ehwqpu.com/gtixbkimph.html

Ruby: nested.flatten
来源：http://hz.hywenlv.cn/gtsyhwephw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.guowangkeji.top/gtxmgskvyw.html

[D19] 按字段分组
来源：http://hz.shzxlz.cn/gtonvbxtdx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jinqigufen.top/gteklivmuz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xingfuxueyuan.xyz/gtolefalrf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yangfankeji.com/gtrywrckop.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cqqwz.cn/gtnznaqhqe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jinghuilouyu.cn/gtrozgefdp.html

Go:   // 手写 map[string][]T
来源：http://hz.sysykeji.top/gtzucovmyc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yvedp.cn/gtpscjegwm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yvedp.cn/gtuavlqxjq.html

[D20] 统计每个元素出现次数
来源：http://hz.hysaishi.cn/gtbxjfgvlu.html

Py:   Counter(arr)
来源：http://hz.cdnleiting.top/gtepfankso.html

PHP:  array_count_values($arr);
来源：http://hz.pengpengdd.cyou/gtotmqyxsg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shangyingyoupin.top/gtypooatlb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xziqi.cn/gtzintrprm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ivvv.top/gtmvxnmqhu.html

Go:   // 手写 map[T]int
来源：http://hz.feifeiyinyue.top/gtriogdksu.html

Ruby: arr.tally
来源：http://hz.chenzaomai.com/gtuvykbmev.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yuxming.cn/gtuyewlbpl.html

[D21] 判断是否包含某元素
来源：http://hz.zhixingplan.top/gtznwiqlhb.html

Py:   x in arr
来源：http://hz.sufxvd.cn/gtsumzcvci.html

PHP:  in_array($x, $arr, true);
来源：http://hz.quarkkingdee.top/gtmkwkuzwi.html

JS:   arr.includes(x)
来源：http://hz.mhx1999.top/gtjlbacgda.html

TS:   arr.includes(x)
来源：http://hz.hongshengwenyu.top/gtvexdagpw.html

Java: list.contains(x)
来源：http://hz.52xcode.cn/gtkfdtueqb.html

Go:   slices.Contains(arr, x)
来源：http://hz.tanke756.top/gtjgeshnhq.html

Ruby: arr.include?(x)
来源：http://hz.316326.xyz/gtfspjnqhw.html

C#:   list.Contains(x)
来源：http://hz.pengpengdd.cyou/gtqscefgjj.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yj20258888.top/gtvkycaftv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.smart0.xyz/gtbcldosxc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yj202588.top/gtqrxuvqic.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.sysykeji.top/gtddbkzhtg.html

TS:   [...arr];
来源：http://hz.smart0.xyz/gtutzvkuzx.html

Java: new ArrayList<>(list);
来源：http://hz.jiagoushi.top/gtqtvdbpjn.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yonumen.top/gtyqhsqmip.html

Ruby: arr.dup;  arr.clone
来源：http://hz.iojbl.cn/gtbmuqaxgj.html

C#:   new List<int>(list);
来源：http://hz.jinqigufen.top/gtjikggkik.html

[D23] reduce 累积计算
来源：http://hz.shzxlz.cn/gtrwlzkqfr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jqgfzy.top/gtuniqmhso.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.wangdashe.top/gtmkwmexoc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhongyouzk.top/gtstdxdprn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenzaomai.com/gtgucqovhc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yangfankeji.com/gtaysxjvee.html

Go:   // 手写循环
来源：http://hz.0kj1m.cn/gtdkuckmjp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.chenjidiqi.icu/gthmpzkqqv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jianghu66.top/gtgurqxxos.html

[D24] 字典 / Map 基本操作
来源：http://hz.jqgfzy.top/gtphgnlrtx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jinqigfzy.top/gthslursva.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhixingplan.top/gtzibzxogt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hysaishi.cn/gteinrjnde.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zhoulong.xyz/gtcwfghwjy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jlsjyb.cn/gtxwxjkcmn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hnxiangtu.top/gthqeergnd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jyoumei.cn/gtgwcgacsu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zdqjudy.top/gtobzpglre.html

[D25] Set 集合去重与交并差
来源：http://hz.zhaomingkeji.xyz/gtagajmoni.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yueranfly.top/gtkoelvjat.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jianghu66.top/gtjobsquis.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.iojbl.cn/gtfvacwbfv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yuanzhike.top/gtvtndydfy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hysaishi.cn/gtvrslswnj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ywan-chungtsiang.top/gttmtxkdgx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.9152youxi.cn/gtbvgfezzs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cucudq.cn/gtsmodbqlk.html

[D26] 数组转字符串
来源：http://hz.yanxiufei.cn/gtimtskrvh.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhijiandao.cn/gtpntbayis.html

PHP:  implode(", ", $arr);
来源：http://hz.shuidangran.top/gtkuuhistw.html

JS:   arr.join(", ")
来源：http://hz.gotoacloud.top/gtuvtcvlyn.html

TS:   arr.join(", ")
来源：http://hz.cdnleiting.top/gtrccacjun.html

Java: String.join(", ", list)
来源：http://hz.cqqwz.cn/gtzkvhlhog.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ywan-chungtsiang.top/gtlutoubqu.html

Ruby: arr.join(", ")
来源：http://hz.zhaomingkeji.xyz/gtadhzrywx.html

C#:   string.Join(", ", list)
来源：http://hz.pengpengdd.cyou/gtcxcqujug.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtejlqdoqr.html

E. 字符串处理
来源：http://hz.quarkkingdee.top/gtcuspeuft.html

================================================================================
来源：http://hz.zhijiandao.cn/gtlqrafvtc.html

[E01] 拼接字符串
来源：http://hz.aibaodan.cn/gtxrzcoyls.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.smart0.xyz/gtrmdrpiqa.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.wangshuangyany.cn/gtfjesjvev.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sysykeji.top/gtmdajcrhh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.daria6918.cn/gtpijcnhug.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xinyue.icu/gtiixndcuy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hnqzz.top/gtouqgqcyu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.cdnleiting.top/gtnfagptxv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cucudq.cn/gtmsrybwdb.html

[E02] 重复字符串
来源：http://hz.hammf.cn/gtgknvcccm.html

Py:   "ab" * 3
来源：http://hz.yuxming.cn/gtzguvowco.html

PHP:  str_repeat("ab", 3);
来源：http://hz.dianchejie.cn/gtdbmnllmm.html

JS:   "ab".repeat(3)
来源：http://hz.hongshengwenyu.top/gtlcbwyutd.html

TS:   "ab".repeat(3)
来源：http://hz.hongshengwenyu.top/gtyzpktbsh.html

Java: "ab".repeat(3)
来源：http://hz.cqqwz.cn/gttuqabqsu.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.nwbrower.top/gtbbeqolkz.html

Ruby: "ab" * 3
来源：http://hz.hysaishi.cn/gtifkybfdn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.birdmap.top/gtvgzsqels.html

[E03] 截取子串
来源：http://hz.gogol.net.cn/gtynbvlzlc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.wangdashe.top/gttkdymxma.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.cheryme.top/gtgdraczsr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.xziqi.cn/gtrfimpjti.html

TS:   s.slice(1, 4)
来源：http://hz.yonumen.top/gtcdosjise.html

Java: s.substring(1, 4)
来源：http://hz.bjfxy.top/gtrjuipsqp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.fzhhl.top/gtwzlqoxdu.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xuetiantiany.cn/gtkejebufi.html

C#:   s.Substring(1, 3)
来源：http://hz.sysykeji.top/gtydfzqnav.html

[E04] 查找子串位置
来源：http://hz.ehwqpu.com/gtiiowqbsm.html

Py:   s.find("x");  s.index("x")
来源：http://hz.tian-w.cn/gtzfvwojpg.html

PHP:  strpos($s, "x");
来源：http://hz.ywan-chungtsiang.top/gtackyqutr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hnxiangtu.top/gtsncwzyqq.html

TS:   s.indexOf("x")
来源：http://hz.xingfuxueyuan.xyz/gtzqgnlahl.html

Java: s.indexOf("x")
来源：http://hz.jlsjyb.cn/gtjfzilkqz.html

Go:   strings.Index(s, "x")
来源：http://hz.andypj.xyz/gtsrdqrygk.html

Ruby: s.index("x")
来源：http://hz.yonumen.top/gtepzqnbse.html

C#:   s.IndexOf("x")
来源：http://hz.xinyue.icu/gtlawthhya.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhengqikj.top/gtlafuqndx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.andypj.xyz/gtwmrkvjzj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.shanyushiyangtech.top/gtxmxadplj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ivvv.top/gtbkjxluvp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hammf.cn/gtcbbbqejp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shuidangran.top/gtjsbfkrai.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jlsjyb.cn/gtdczgzklq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.cqqwz.cn/gtnnrvjhgy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jlsjyb.cn/gtahhhmaiu.html

[E06] 替换子串
来源：http://hz.mhx1999.top/gtuqhaaqeb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jyoumei.cn/gtqryipjxy.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jinghuilouyu.cn/gtxczcygeh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtpmarrvhf.html

TS:   s.replaceAll("a", "b")
来源：http://hz.daria6918.cn/gtloxalmfq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gotoacloud.top/gtsoqzcedm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jinghuilouyu.cn/gtirltwlvi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yuxming.cn/gtvwypznqv.html

C#:   s.Replace("a", "b")
来源：http://hz.hywenlv.cn/gtkoewxmdy.html

[E07] 按分隔符拆分
来源：http://hz.wangdashe.top/gtrujoseft.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.nwbrower.top/gttbtmhqfv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.chenlongwang.top/gtaadscnce.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yueranfly.top/gtxdenvgot.html

TS:   s.split(",")
来源：http://hz.meibo888.top/gteriqeayi.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xuetiantiany.cn/gtfzxvksza.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.gotoacloud.top/gtlfnrzaci.html

Ruby: s.split(",");  s.split
来源：http://hz.jlsjyb.cn/gttodfeipn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhongyouzk.top/gtzykjjaew.html

[E08] 数组按分隔符合并
来源：http://hz.fzhhl.top/gtpseoscae.html

Py:   ",".join(items)
来源：http://hz.fzhhl.top/gtrtatiwdk.html

PHP:  implode(",", $items);
来源：http://hz.dashuyun.cn/gtuxefsmpy.html

JS:   items.join(",")
来源：http://hz.aibaodan.cn/gtwqbefihj.html

TS:   items.join(",")
来源：http://hz.zhoulong.xyz/gtkximkidb.html

Java: String.join(",", items)
来源：http://hz.haohaochexian.top/gtfqsjfcud.html

Go:   strings.Join(items, ",")
来源：http://hz.meibo888.top/gticndayqu.html

Ruby: items.join(",")
来源：http://hz.zhiwuduotai.top/gthhlcuxfa.html

C#:   string.Join(",", items)
来源：http://hz.zhengqikj.top/gtgfsegtoo.html

[E09] 去除所有空白字符
来源：http://hz.zycfv.cn/gtpyfocyuv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.bjfxy.top/gtufzhfxqc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.tianlin.xyz/gttolwicmc.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.tianlin.xyz/gtkiltcioz.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yj202588.top/gtgbxrmxhf.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.shangyingyoupin.top/gttwsmifzf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.cheryme.top/gtrmcfusbe.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.dashuyun.cn/gtveamszdz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jqgufenzy.top/gtjqjcjpuh.html

[E10] 左侧补零 / 定长填充
来源：http://hz.havefunace.top/gttaijnbzf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.birdmap.top/gthdourone.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jyoumei.cn/gtglqbpkvb.html

JS:   "7".padStart(3, "0")
来源：http://hz.gzhubu.top/gtekluzljg.html

TS:   "7".padStart(3, "0")
来源：http://hz.ivvv.top/gtohmzukjw.html

Java: String.format("%03d", 7)
来源：http://hz.hfpthk.cn/gtfggskqvl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.quarkkingdee.top/gtwqkrzwuj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ywan-chungtsiang.top/gtjmsghvxj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cqqwz.cn/gtotemmwtw.html

[E11] 反转字符串
来源：http://hz.zhiwuduotai.top/gtokersyjg.html

Py:   s[::-1]
来源：http://hz.ywan-chungtsiang.top/gtbefbzfaz.html

PHP:  strrev($s);
来源：http://hz.feifeiyinyue.top/gtoqsophzm.html

JS:   [...s].reverse().join("")
来源：http://hz.jinyuanbaomall.cn/gtgcswapke.html

TS:   [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtztutjtvw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.316326.xyz/gtdaxaadou.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hongshengwenyu.top/gtyzwldsah.html

Ruby: s.reverse
来源：http://hz.ivvv.top/gtyzhztmts.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yangfankeji.com/gtuzugcrgc.html

[E12] 统计某字符出现次数
来源：http://hz.jinghuilouyu.cn/gtvhrknghn.html

Py:   s.count("a")
来源：http://hz.9152youxi.cn/gticmdoktd.html

PHP:  substr_count($s, "a");
来源：http://hz.zhengqikj.top/gtehxjpgbm.html

JS:   s.split("a").length - 1
来源：http://hz.jlsjyb.cn/gtllbxiqlf.html

TS:   s.split("a").length - 1
来源：http://hz.dianchejie.cn/gtnbhsqyoy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ivvv.top/gtpoqusifc.html

Go:   strings.Count(s, "a")
来源：http://hz.zhongyouzk.top/gtuctbxgul.html

Ruby: s.count("a")
来源：http://hz.jinqigufen.top/gtxiolpdhi.html

C#:   s.Count(c => c == 'a')
来源：http://hz.kuanghao11.cn/gtedztvqpe.html

[E13] 逐字符遍历
来源：http://hz.sysykeji.top/gteeoargcd.html

Py:   for ch in s: print(ch)
来源：http://hz.sweek.top/gtzpgtwzxp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.pycfn.com/gtlmiwuywk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.haohaochexian.top/gtfjmiylrz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj20258888.top/gtmvdeoldf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xziqi.cn/gtsfwcwzxx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.tanke756.top/gtodhyblrh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.birdmap.top/gtbltqfveh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jinyuanbaomall.cn/gtkevlhgqj.html

[E14] URL 编码与 Base64
来源：http://hz.jinyuanbaomall.cn/gtrocbmqcm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xingfuxueyuan.xyz/gtnfbmyctm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jqgfzy.top/gtdrpydcmn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hywenlv.cn/gtpoavddtg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.pengpengdd.cyou/gtrljgobrf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.gogol.net.cn/gtuyphjhhg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hnqzz.top/gtalikrcfk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhoulong.xyz/gtrzrcgtlm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ywan-chungtsiang.top/gtwlbdijmj.html

[E15] HTML 转义 / 反转义
来源：http://hz.yuanzhike.top/gtxqgmkpys.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xingfuxueyuan.xyz/gttjmocevz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yj202588.top/gtwavfgrqf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.fengsongda.top/gtcojphwdk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.nanxuanxn.top/gtfwrdravv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hnqzz.top/gtnusiljkv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.c1oappe.top/gtzmvhebqe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.guannengcc.top/gtctufhoan.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.nanxuanxn.top/gtdvzchfkv.html

[E16] 数字千分位
来源：http://hz.ivvv.top/gtozvardic.html

Py:   f"{1234567:,}"
来源：http://hz.nanxinkj.top/gtxcirmdtl.html

PHP:  number_format(1234567);
来源：http://hz.smart0.xyz/gtkarxktbl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.bjfxy.top/gtnsguoque.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.nwbrower.top/gtwgagecdu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.wangdashe.top/gtvcwwtgep.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gaohongyu789.top/gtiwlvdfql.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jqgfzy.top/gtqbhykvsa.html

C#:   1234567.ToString("N0")
来源：http://hz.smart0.xyz/gtzyorecid.html

[E17] 首字母大写
来源：http://hz.hysaishi.cn/gtaznkbsbi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cdnleiting.top/gthzzfqjzh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhaomingkeji.xyz/gtxqeamwyh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hfpthk.cn/gtqyjmyrmx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangkeji.top/gtxmughvoh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.fzhhl.top/gtuwjxvyvc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hywenlv.cn/gttijiexor.html

Ruby: s.capitalize
来源：http://hz.cqqwz.cn/gtefshyxhg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.sysykeji.top/gtepqrpvsb.html

[E18] 模板占位符替换
来源：http://hz.svipenyu.cn/gtvtqmorit.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xuetiantiany.cn/gtgoxjzgwv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hnxiangtu.top/gttiymhbrf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jlsjyb.cn/gtzqvsbdhc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.snrcjt.cn/gtavttuvkl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jqgufenzy.top/gtacwgyjtj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.52xcode.cn/gtebjptxyk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.tianlin.xyz/gtilcfrrac.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.snrcjt.cn/gtiqmcfxwc.html

[E19] 多行文本按行拆分
来源：http://hz.aibaodan.cn/gtfdqacmrh.html

Py:   s.splitlines()
来源：http://hz.feifeiyinyue.top/gtbwzqqmnx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jiagoushi.top/gtgmofmhgu.html

JS:   s.split(/\r?\n/)
来源：http://hz.shuidangran.top/gtinbwaupu.html

TS:   s.split(/\r?\n/)
来源：http://hz.yongpay.top/gtclmzajes.html

Java: s.lines().toList()
来源：http://hz.gotoacloud.top/gtgekqvfab.html

Go:   strings.Split(s, "\n")
来源：http://hz.hnqzz.top/gtmltoskxc.html

Ruby: s.lines
来源：http://hz.yj202588.top/gtinwezljg.html

C#:   s.Split('\n')
来源：http://hz.svipenyu.cn/gttsiidwnv.html

[E20] 判断字符串是否为空
来源：http://hz.guowangkeji.top/gtgbwjvanj.html

Py:   if not s:
来源：http://hz.cqqwz.cn/gtfyeghxvp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinqigufen.top/gtydxaodum.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yonumen.top/gtlcclkyay.html

TS:   if (s === "") {}
来源：http://hz.ydzc1.top/gtshpahmop.html

Java: if (s.isEmpty()) {}
来源：http://hz.yj20258.top/gtndfgwofp.html


<!-- 参考信息 -->