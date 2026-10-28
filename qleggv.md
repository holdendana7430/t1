代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.redwolf501.top/gtbuibpnkm.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gogol.net.cn/gtpwuhcoyk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zdqjudy.top/gtvtmitbxi.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ydzc1.top/gtqvvbhajh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.quarkkingdee.top/gtantpmaaq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.daria6918.cn/gtibfsyedq.html

JS:   arr.map(x => x * 2)
来源：http://hz.daxiang520.top/gtjchixhfx.html

TS:   arr.map(x => x * 2)
来源：http://hz.daxiang520.top/gtasroizoi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zycfv.cn/gtrdvowqax.html

Go:   // 手写循环
来源：http://hz.zhijiandao.cn/gtnwjyepea.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yonumen.top/gtzjtfkccz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xinyue.icu/gtmxjuqorj.html

[D15] 去重
来源：http://hz.daxiang520.top/gtcazluade.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.chenlongwang.top/gtggncyzrw.html

PHP:  array_unique($arr);
来源：http://hz.jlsjyb.cn/gtocgowzqs.html

JS:   [...new Set(arr)]
来源：http://hz.zhongyouzk.top/gtzsyjvhpp.html

TS:   [...new Set(arr)]
来源：http://hz.316326.xyz/gttsynykjj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.sufxvd.cn/gtswwdvahb.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cqqwz.cn/gtfsqhllrl.html

Ruby: arr.uniq
来源：http://hz.zhengqikj.top/gtpuvpjwrj.html

C#:   list.Distinct().ToList()
来源：http://hz.haohaochexian.top/gtdrmdkwem.html

[D16] 求和与平均值
来源：http://hz.pycfn.com/gtcurottwy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.vqdsnc.cn/gtymrssynq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhoulong.xyz/gtaseserbl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yvedp.cn/gtcqspndwp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ehwqpu.com/gtxfloehqv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jinyuanbaomall.cn/gtzbxdidvd.html

Go:   // 手写循环累加
来源：http://hz.yangfankeji.com/gtzqzqhbht.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hysaishi.cn/gtwxltpisy.html

C#:   list.Sum();  list.Average()
来源：http://hz.svipenyu.cn/gtjakoezra.html

[D17] 最大值与最小值
来源：http://hz.cdnleiting.top/gtfvupdfwn.html

Py:   max(arr);  min(arr)
来源：http://hz.nwbrower.top/gtxgafopjr.html

PHP:  max($arr);  min($arr);
来源：http://hz.316326.xyz/gtyftpkdxo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.dianchejie.cn/gtewxdxjsx.html

TS:   Math.max(...arr);
来源：http://hz.yuxming.cn/gthluapiez.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hnxiangtu.top/gtpanqfprl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhoulong.xyz/gtxgnlltzw.html

Ruby: arr.max;  arr.min
来源：http://hz.jlsjyb.cn/gtbtiyaiux.html

C#:   list.Max();  list.Min()
来源：http://hz.fzhhl.top/gtglwnbvgc.html

[D18] 扁平化嵌套数组
来源：http://hz.yanxiufei.cn/gtvfagvmco.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.gogol.net.cn/gtldehfudl.html

PHP:  array_merge(...$nested);
来源：http://hz.shangyingyoupin.top/gtvogoukgl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.smart0.xyz/gttcvbaoac.html

TS:   nested.flat();
来源：http://hz.zycfv.cn/gthvxaahjj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shanyushiyangkeji.top/gtelyhuwwj.html

Go:   // 手写双层循环
来源：http://hz.gaohongyu789.top/gtxtbrqjwb.html

Ruby: nested.flatten
来源：http://hz.fzhhl.top/gtpxezhlaa.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.daxiang520.top/gtfctpgkmf.html

[D19] 按字段分组
来源：http://hz.yanxiufei.cn/gtjujwapyk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yj20258.top/gtrytqzfyi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hnxiangtu.top/gtdzsphkaf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yvedp.cn/gtmbgcgqwn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.kuanghao11.cn/gtasygtxwf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.dashuyun.cn/gtcxwwvlhe.html

Go:   // 手写 map[string][]T
来源：http://hz.52xcode.cn/gtbvviczio.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yangfankeji.com/gtgcjmpntg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhixingplan.top/gtfseofbwc.html

[D20] 统计每个元素出现次数
来源：http://hz.tanke756.top/gthkyrxinf.html

Py:   Counter(arr)
来源：http://hz.guowangkeji.top/gtsdepuech.html

PHP:  array_count_values($arr);
来源：http://hz.tanke756.top/gtprffosbb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cqqwz.cn/gtolyqjwzl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sufxvd.cn/gtfqtfkgdj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.daria6918.cn/gtcyxcmend.html

Go:   // 手写 map[T]int
来源：http://hz.kuanghao11.cn/gtduwpujys.html

Ruby: arr.tally
来源：http://hz.jianghu66.top/gtwykfrurx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jinqigufen.top/gtsoromhes.html

[D21] 判断是否包含某元素
来源：http://hz.316326.xyz/gtanacmyai.html

Py:   x in arr
来源：http://hz.jiagoushi.top/gtmdrbgsfn.html

PHP:  in_array($x, $arr, true);
来源：http://hz.vqdsnc.cn/gtyegqxlqr.html

JS:   arr.includes(x)
来源：http://hz.hnqzz.top/gthttzmxgc.html

TS:   arr.includes(x)
来源：http://hz.nwbrower.top/gtybblofzq.html

Java: list.contains(x)
来源：http://hz.fengsongda.top/gtgvzbrugh.html

Go:   slices.Contains(arr, x)
来源：http://hz.316326.xyz/gtqfuppyes.html

Ruby: arr.include?(x)
来源：http://hz.jqgufenzy.top/gtgetjoysg.html

C#:   list.Contains(x)
来源：http://hz.ydzc1.top/gtresvbwjg.html

[D22] 复制数组（避免共享引用）
来源：http://hz.tian-w.cn/gtzymujhco.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ydzc1.top/gtuouvwwki.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xylfe.cn/gtgjjtqjbd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.nanxinkj.top/gtzdqnegan.html

TS:   [...arr];
来源：http://hz.yanxiufei.cn/gtxcsglvra.html

Java: new ArrayList<>(list);
来源：http://hz.jyoumei.cn/gtwxkwliup.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.kuanghao11.cn/gtxqcckbya.html

Ruby: arr.dup;  arr.clone
来源：http://hz.pycfn.com/gtvibdybgy.html

C#:   new List<int>(list);
来源：http://hz.tanke756.top/gtfbyqeqab.html

[D23] reduce 累积计算
来源：http://hz.ywan-chungtsiang.top/gtjoowtbtz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yj20258.top/gtzszjqpmz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cdnleiting.top/gtwqemzfqo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shanyushiyangtech.top/gtkgwekruk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tian-w.cn/gtdbusybzj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhixingplan.top/gtcwxyxocc.html

Go:   // 手写循环
来源：http://hz.jyoumei.cn/gtufbrevzk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.sufxvd.cn/gtuhgpuase.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yonumen.top/gtsgqnppmp.html

[D24] 字典 / Map 基本操作
来源：http://hz.xingfuxueyuan.xyz/gttuogapsc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yuanzhike.top/gtozhrzhan.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.nwbrower.top/gtgfgdhyws.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yj202588.top/gtyhiuhwlp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ehwqpu.com/gtipywiutm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xylfe.cn/gtvaypjaml.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.nwbrower.top/gtbouvxopi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hnqzz.top/gtyeoylmxe.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.0kj1m.cn/gtlmkapukj.html

[D25] Set 集合去重与交并差
来源：http://hz.shanyushiyangtech.top/gtgkofeoky.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.smart0.xyz/gtrvgpdmnt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.quarkkingdee.top/gtunyobdzh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.andypj.xyz/gtcgzhyjix.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sufxvd.cn/gtoakgsqhj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.kuanghao11.cn/gtlbjyhxus.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.tian-w.cn/gttdfrbnve.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.mhx1999.top/gtbcfiuypw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.kuanghao11.cn/gteongsuor.html

[D26] 数组转字符串
来源：http://hz.cqqwz.cn/gtbbhgchlk.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shangyingyoupin.top/gtealfsnpn.html

PHP:  implode(", ", $arr);
来源：http://hz.snrcjt.cn/gtmgcfqwmf.html

JS:   arr.join(", ")
来源：http://hz.tanke756.top/gtqyymadyc.html

TS:   arr.join(", ")
来源：http://hz.gotoacloud.top/gtkdgqokaj.html

Java: String.join(", ", list)
来源：http://hz.gogol.net.cn/gtzliqssqa.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jqgufenzy.top/gtbjuhuxuf.html

Ruby: arr.join(", ")
来源：http://hz.jlsjyb.cn/gtksrmgsxw.html

C#:   string.Join(", ", list)
来源：http://hz.xylfe.cn/gtdnkcvqyi.html

================================================================================
来源：http://hz.ppjwa.cn/gtozcqoanr.html

E. 字符串处理
来源：http://hz.fengsongda.top/gtsfifdsdp.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtbuhxciyz.html

[E01] 拼接字符串
来源：http://hz.hywenlv.cn/gtcdvrgnlg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hfpthk.cn/gtkrxstynd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.birdmap.top/gtlaekxnyg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.pengpengdd.cyou/gtlnfelbbh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxinkj.top/gtoobdqupo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hongshengwenyu.top/gtpnkxarsv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yj20258888.top/gtzcvxjpev.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.gogol.net.cn/gtoyrfgcvh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.sxryk.cn/gtixrdcyiy.html

[E02] 重复字符串
来源：http://hz.yj20258.top/gtefejhtsc.html

Py:   "ab" * 3
来源：http://hz.haohaochexian.top/gtnlnkwewb.html

PHP:  str_repeat("ab", 3);
来源：http://hz.nanxinkj.top/gtytlyqahg.html

JS:   "ab".repeat(3)
来源：http://hz.gzhubu.top/gtuwnsjmte.html

TS:   "ab".repeat(3)
来源：http://hz.bjfxy.top/gtpetqmcdg.html

Java: "ab".repeat(3)
来源：http://hz.jiagoushi.top/gtvimtasvu.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hongshengwenyu.top/gtjdmcwzqe.html

Ruby: "ab" * 3
来源：http://hz.iojbl.cn/gthpdoyuao.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.cucudq.cn/gtcjqrryyt.html

[E03] 截取子串
来源：http://hz.yongpay.top/gtgqbsxkwt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.shanyushiyangtech.top/gtaecxdvre.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ppjwa.cn/gtnyrrjzuy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.chenzaomai.com/gtldrexxua.html

TS:   s.slice(1, 4)
来源：http://hz.smart0.xyz/gtocupxlcm.html

Java: s.substring(1, 4)
来源：http://hz.quarkkingdee.top/gtuqyvlvkq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhixingplan.top/gttqkqxjvu.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yangfankeji.com/gtyqvlduyb.html

C#:   s.Substring(1, 3)
来源：http://hz.yueranfly.top/gtzhwbhhjt.html

[E04] 查找子串位置
来源：http://hz.jiagoushi.top/gtunnvbstu.html

Py:   s.find("x");  s.index("x")
来源：http://hz.cucudq.cn/gtxtebrvky.html

PHP:  strpos($s, "x");
来源：http://hz.vqdsnc.cn/gtpgwjzhet.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.tian-w.cn/gtlprmjcia.html

TS:   s.indexOf("x")
来源：http://hz.yj20258888.top/gtxxrbooyg.html

Java: s.indexOf("x")
来源：http://hz.zhixingplan.top/gthxqmfaiw.html

Go:   strings.Index(s, "x")
来源：http://hz.birdmap.top/gtcxehfayf.html

Ruby: s.index("x")
来源：http://hz.jyoumei.cn/gtvjcwroou.html

C#:   s.IndexOf("x")
来源：http://hz.jyoumei.cn/gtrctqckfy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.guannengcc.top/gtohorizsy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhengqikj.top/gtliogvrgl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hfpthk.cn/gtvboizpjj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.aibaodan.cn/gtyhnsqpin.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.xziqi.cn/gtbdlqwcux.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ydjk.org.cn/gtncqrshlg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.meibo888.top/gtoudqtsvt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jqgfzy.top/gtuwvrlyoy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zhaomingkeji.xyz/gtncrjimxu.html

[E06] 替换子串
来源：http://hz.haohaochexian.top/gtincecpia.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.hammf.cn/gtaxhxlgvz.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.sxryk.cn/gtqzhxxbxi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj20258.top/gtygwvfdnl.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jinghuilouyu.cn/gtdslnfgtq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenzaomai.com/gttwrcaasj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jyoumei.cn/gtyfsvcgmv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ydzc1.top/gtkvfmesie.html

C#:   s.Replace("a", "b")
来源：http://hz.aizwys.cn/gtybzsyxmv.html

[E07] 按分隔符拆分
来源：http://hz.bjfxy.top/gtestfiwmk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yongpay.top/gtdpwhpcgx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zhongyouzk.top/gtzyogwchr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ybcxt.top/gtqrpbpejv.html

TS:   s.split(",")
来源：http://hz.bjfxy.top/gttnwwxkgb.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.smart0.xyz/gtryodeoxp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.hfpthk.cn/gtnvcyljez.html

Ruby: s.split(",");  s.split
来源：http://hz.jlsjyb.cn/gtftdixpmj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zycfv.cn/gtlgqspkpo.html

[E08] 数组按分隔符合并
来源：http://hz.xingfuxueyuan.xyz/gtnrxbfpvo.html

Py:   ",".join(items)
来源：http://hz.ivvv.top/gtbxnbggra.html

PHP:  implode(",", $items);
来源：http://hz.yj20258.top/gtwrvsxyiw.html

JS:   items.join(",")
来源：http://hz.aizwys.cn/gtidzjsvyh.html

TS:   items.join(",")
来源：http://hz.meibo888.top/gtbbupwsaz.html

Java: String.join(",", items)
来源：http://hz.jinqigfzy.top/gtsnadkiix.html

Go:   strings.Join(items, ",")
来源：http://hz.c1oappe.top/gtqlvowehr.html

Ruby: items.join(",")
来源：http://hz.9152youxi.cn/gtcibiwafd.html

C#:   string.Join(",", items)
来源：http://hz.pengpengdd.cyou/gtijwkdabe.html

[E09] 去除所有空白字符
来源：http://hz.tian-w.cn/gtcmzonqpv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xinyue.icu/gtaozgsslk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hnxiangtu.top/gtrpjowdrj.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zdqjudy.top/gtpnajsbpb.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ppjwa.cn/gthhreghht.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zdqjudy.top/gtbqhfthgp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sxryk.cn/gtcxgnlczj.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shanyushiyangtech.top/gteykmntdy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.fengsongda.top/gtfhtggwsm.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yongpay.top/gtsrfevinu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.52xcode.cn/gtcrfubbqz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.sweek.top/gtniolemzy.html

JS:   "7".padStart(3, "0")
来源：http://hz.birdmap.top/gtocqsxcvb.html

TS:   "7".padStart(3, "0")
来源：http://hz.sxryk.cn/gtjqiaxqrm.html

Java: String.format("%03d", 7)
来源：http://hz.dashuyun.cn/gtklnxvyuu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cqqwz.cn/gtapdiwyfu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.aizwys.cn/gtjynjnefo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yueranfly.top/gtjqxrcegv.html

[E11] 反转字符串
来源：http://hz.ydjk.org.cn/gtzdtyexch.html

Py:   s[::-1]
来源：http://hz.sysykeji.top/gtfsuwuoph.html

PHP:  strrev($s);
来源：http://hz.cqqwz.cn/gtnrinaavz.html

JS:   [...s].reverse().join("")
来源：http://hz.zhiwuduotai.top/gtdbuzkzvk.html

TS:   [...s].reverse().join("")
来源：http://hz.cdnleiting.top/gtojyagdbn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhaomingkeji.xyz/gtllphpdzi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.iojbl.cn/gtsdboyygz.html

Ruby: s.reverse
来源：http://hz.bjfxy.top/gtxsndkryo.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xuanzx.com/gttslxoycu.html

[E12] 统计某字符出现次数
来源：http://hz.jqgfzy.top/gtttqasklh.html

Py:   s.count("a")
来源：http://hz.zhijiandao.cn/gtlpevfzwl.html

PHP:  substr_count($s, "a");
来源：http://hz.hfpthk.cn/gtwmpbzcyp.html

JS:   s.split("a").length - 1
来源：http://hz.snrcjt.cn/gtvfvgsoaf.html

TS:   s.split("a").length - 1
来源：http://hz.yuanzhike.top/gtjgpfojxv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.aibaodan.cn/gtzjwuniup.html

Go:   strings.Count(s, "a")
来源：http://hz.gogol.net.cn/gtsnefbvcm.html

Ruby: s.count("a")
来源：http://hz.xuetiantiany.cn/gtvijgalkg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.sysykeji.top/gtwyhmwvis.html

[E13] 逐字符遍历
来源：http://hz.daria6918.cn/gtmdasryic.html

Py:   for ch in s: print(ch)
来源：http://hz.iojbl.cn/gtynnfsvgz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhoulong.xyz/gtscekxzqr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.daxiang520.top/gtcijzuuho.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.birdmap.top/gtewdzqvqq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xuetiantiany.cn/gtguqrjotk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xingfuxueyuan.xyz/gttutvhlnd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.pycfn.com/gtolvuzfrt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.gaohongyu789.top/gtnajuqlnf.html

[E14] URL 编码与 Base64
来源：http://hz.ybcxt.top/gttumxdoov.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shzxlz.cn/gtvxkigzlp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cdnleiting.top/gthgvxhpfx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hnqzz.top/gtpuwctpea.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ehwqpu.com/gtdiwoimmj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.haohaochexian.top/gthiccvndk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.gzhubu.top/gtetszujor.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhijiandao.cn/gtwuwqfafq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.iojbl.cn/gtswhsrhhe.html

[E15] HTML 转义 / 反转义
来源：http://hz.svipenyu.cn/gtcnvrpzel.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.dianchejie.cn/gtcnsegjgs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.redwolf501.top/gtofjfejdv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.guowangkeji.top/gtjelekavg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ybcxt.top/gtunkjdyjg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ywan-chungtsiang.top/gtilzpguzt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.redwolf501.top/gtifyiehua.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.smart0.xyz/gthqmtoxlj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.316326.xyz/gtbxfpdvcn.html

[E16] 数字千分位
来源：http://hz.hfpthk.cn/gtberskisq.html

Py:   f"{1234567:,}"
来源：http://hz.vqdsnc.cn/gtrxmgtpwh.html

PHP:  number_format(1234567);
来源：http://hz.zhixingplan.top/gtpnqupzls.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jyoumei.cn/gtmcdgxrhl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.aizwys.cn/gtbdgzduvg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xuanzx.com/gtclfvvjyw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yuanzhike.top/gtdfntshpq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hywenlv.cn/gtdxbdjuxr.html

C#:   1234567.ToString("N0")
来源：http://hz.jlsjyb.cn/gtnhhygzsh.html

[E17] 首字母大写
来源：http://hz.dianchejie.cn/gtsfowcrrw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.snrcjt.cn/gtqljcvvdl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.dianchejie.cn/gtdpyjqxmv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj20258.top/gtytnofxsm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nanxinkj.top/gtjtpvrvyi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.c1oappe.top/gtuvpqvmdf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ywan-chungtsiang.top/gtnymazktb.html

Ruby: s.capitalize
来源：http://hz.yuxming.cn/gtdsfpmmts.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.havefunace.top/gtitpdkdnl.html

[E18] 模板占位符替换
来源：http://hz.sysykeji.top/gtqenlmdwb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.guowangkeji.top/gthhmpyuyd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhijiandao.cn/gtkgcmotee.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zdqjudy.top/gtffgtwpzl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.gzhubu.top/gtexabtkhh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.nwbrower.top/gtsqdishfv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.9152youxi.cn/gttxtwejov.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xuetiantiany.cn/gtneiiekge.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.guowangkeji.top/gtpxgclgvm.html

[E19] 多行文本按行拆分
来源：http://hz.vqdsnc.cn/gtmbrlobmz.html

Py:   s.splitlines()
来源：http://hz.xuanzx.com/gtkxksjtxr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jyoumei.cn/gtfbbasbpp.html

JS:   s.split(/\r?\n/)
来源：http://hz.yuxming.cn/gtjudddpbv.html

TS:   s.split(/\r?\n/)
来源：http://hz.xuanzx.com/gtowciraxx.html

Java: s.lines().toList()
来源：http://hz.snrcjt.cn/gtphvracgl.html

Go:   strings.Split(s, "\n")
来源：http://hz.pengpengdd.cyou/gtflakblee.html

Ruby: s.lines
来源：http://hz.cucudq.cn/gtqplworvi.html

C#:   s.Split('\n')
来源：http://hz.ywan-chungtsiang.top/gtzwpsbzkq.html

[E20] 判断字符串是否为空
来源：http://hz.bjfxy.top/gtvadrsdzs.html

Py:   if not s:
来源：http://hz.tianlin.xyz/gtdoijiybd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.gogol.net.cn/gtscmliptr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.haohaochexian.top/gtteeycmyy.html

TS:   if (s === "") {}
来源：http://hz.havefunace.top/gtduplteqs.html

Java: if (s.isEmpty()) {}
来源：http://hz.aibaodan.cn/gtixefkwug.html


<!-- 参考信息 -->