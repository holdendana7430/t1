代发 wailian999

[D15] 去重
来源：http://hz.hnqzz.top/gtomftrwbg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xingfuxueyuan.xyz/gtvvjwlyqs.html

PHP:  array_unique($arr);
来源：http://hz.zhixingplan.top/gtojvyhnhn.html

JS:   [...new Set(arr)]
来源：http://hz.snrcjt.cn/gtwizkebsy.html

TS:   [...new Set(arr)]
来源：http://hz.zdqjudy.top/gtkzevkdlq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.iojbl.cn/gtopkdevvg.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.nanxuanxn.top/gthjtldxve.html

Ruby: arr.uniq
来源：http://hz.daxiang520.top/gtkimtjhrw.html

C#:   list.Distinct().ToList()
来源：http://hz.shanyushiyangtech.top/gtxucmethp.html

[D16] 求和与平均值
来源：http://hz.gaohongyu789.top/gtjoqftjmn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.xuanzx.com/gtljwqoqww.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.fzhhl.top/gtxekedxvl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhixingplan.top/gtdqotvxmj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yonumen.top/gtqdqjblzf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yanxiufei.cn/gtuuxeevtn.html

Go:   // 手写循环累加
来源：http://hz.jiagoushi.top/gtuyixhkbb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhengqikj.top/gtlfuuvadx.html

C#:   list.Sum();  list.Average()
来源：http://hz.tianlin.xyz/gtsquxwpjb.html

[D17] 最大值与最小值
来源：http://hz.jqgfzy.top/gtwvihuxam.html

Py:   max(arr);  min(arr)
来源：http://hz.hysaishi.cn/gtliklvput.html

PHP:  max($arr);  min($arr);
来源：http://hz.iojbl.cn/gtvotupsud.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zdqjudy.top/gtkolmjznr.html

TS:   Math.max(...arr);
来源：http://hz.shzxlz.cn/gtnfkywwko.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.iojbl.cn/gtxbjuvkgp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hysaishi.cn/gtxkjhjrgr.html

Ruby: arr.max;  arr.min
来源：http://hz.dianchejie.cn/gtbkzrqnys.html

C#:   list.Max();  list.Min()
来源：http://hz.tianlin.xyz/gtqyztzzpz.html

[D18] 扁平化嵌套数组
来源：http://hz.jinqigufen.top/gtrvddjezy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.guowangkeji.top/gtretwrzdv.html

PHP:  array_merge(...$nested);
来源：http://hz.yonumen.top/gtwyyekssm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yongpay.top/gtwijljmch.html

TS:   nested.flat();
来源：http://hz.0kj1m.cn/gtdlppwcrb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.bjfxy.top/gtkuxrvggn.html

Go:   // 手写双层循环
来源：http://hz.gogol.net.cn/gtwxuxbcyb.html

Ruby: nested.flatten
来源：http://hz.yonumen.top/gtflsmcdwf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xuetiantiany.cn/gtpgdcqkbf.html

[D19] 按字段分组
来源：http://hz.9152youxi.cn/gtsbjaxnbs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.haohaochexian.top/gttjkjydej.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.vqdsnc.cn/gtuybzhvuj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jiagoushi.top/gtdsjchcel.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jinyuanbaomall.cn/gtgcdjygvs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sweek.top/gtdxwgjmeq.html

Go:   // 手写 map[string][]T
来源：http://hz.sufxvd.cn/gtisntmyhy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.tanke756.top/gticzhvxpz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.andypj.xyz/gtmnmcxfcy.html

[D20] 统计每个元素出现次数
来源：http://hz.zhaomingkeji.xyz/gtaechjadm.html

Py:   Counter(arr)
来源：http://hz.quarkkingdee.top/gtlfhalrcd.html

PHP:  array_count_values($arr);
来源：http://hz.jinghuilouyu.cn/gtrmroyber.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gaohongyu789.top/gtuteoylkw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yonumen.top/gtxzutigyk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.52xcode.cn/gtrhxitaxi.html

Go:   // 手写 map[T]int
来源：http://hz.kuanghao11.cn/gtyfsciqlb.html

Ruby: arr.tally
来源：http://hz.zhaomingkeji.xyz/gtiobdqijy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.andypj.xyz/gtmagvngkx.html

[D21] 判断是否包含某元素
来源：http://hz.yj20258888.top/gtxxwfdsrh.html

Py:   x in arr
来源：http://hz.jinqigufen.top/gtbyiczdob.html

PHP:  in_array($x, $arr, true);
来源：http://hz.smart0.xyz/gtjmiltpmr.html

JS:   arr.includes(x)
来源：http://hz.mhx1999.top/gtoqiyhegz.html

TS:   arr.includes(x)
来源：http://hz.yongpay.top/gtnmuzggwa.html

Java: list.contains(x)
来源：http://hz.sysykeji.top/gtwhfpjdjb.html

Go:   slices.Contains(arr, x)
来源：http://hz.9152youxi.cn/gtufmfakpa.html

Ruby: arr.include?(x)
来源：http://hz.yj202588.top/gthpcmgdxt.html

C#:   list.Contains(x)
来源：http://hz.snrcjt.cn/gtxhfiemdi.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhaomingkeji.xyz/gtsmrzrdzt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.dianchejie.cn/gtqyeqkhxr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.birdmap.top/gtkwhrdbkr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jinghuilouyu.cn/gthtqmiryc.html

TS:   [...arr];
来源：http://hz.feifeiyinyue.top/gtfauxayeu.html

Java: new ArrayList<>(list);
来源：http://hz.jyoumei.cn/gtvmszuozb.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinqigufen.top/gtfwockxrc.html

Ruby: arr.dup;  arr.clone
来源：http://hz.havefunace.top/gtrvrlbnht.html

C#:   new List<int>(list);
来源：http://hz.shzxlz.cn/gthyfltmdn.html

[D23] reduce 累积计算
来源：http://hz.andypj.xyz/gtvqthmfha.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yj202588.top/gtusijweca.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cdnleiting.top/gtrbkqasax.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jianghu66.top/gtwjxfcqym.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aizwys.cn/gtaltsarjh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.chenzaomai.com/gtqoxrjvbj.html

Go:   // 手写循环
来源：http://hz.hammf.cn/gthkokitcx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhongyouzk.top/gtbmrkimkx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.tanke756.top/gtryhmtdqo.html

[D24] 字典 / Map 基本操作
来源：http://hz.daxiang520.top/gtjqqyjqpy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.aizwys.cn/gtipykifhw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.fzhhl.top/gtikvsgavo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shanyushiyangtech.top/gtxnxnmets.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yangfankeji.com/gtdvgetfqe.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.redwolf501.top/gttewbqvps.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.nanxinkj.top/gtreigndxb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.tian-w.cn/gtoupkvbiu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jqgfzy.top/gtdpdzkxsk.html

[D25] Set 集合去重与交并差
来源：http://hz.quarkkingdee.top/gtkixnfntr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhaomingkeji.xyz/gtabfekuqw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.fzhhl.top/gthtcwxboc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jqgfzy.top/gtrvjutcfe.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.wangdashe.top/gtmkneqjyg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xingfuxueyuan.xyz/gtuanawmyu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.daxiang520.top/gthfjrrekw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ehwqpu.com/gtakuazvvg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.nanxuanxn.top/gtrlqxvman.html

[D26] 数组转字符串
来源：http://hz.xinyue.icu/gtjcpocohf.html

Py:   ", ".join(map(str, arr))
来源：http://hz.daria6918.cn/gtbhjvsmja.html

PHP:  implode(", ", $arr);
来源：http://hz.wangdashe.top/gttuatmrdv.html

JS:   arr.join(", ")
来源：http://hz.redwolf501.top/gtbrmcuzqb.html

TS:   arr.join(", ")
来源：http://hz.nwbrower.top/gtwrfdprov.html

Java: String.join(", ", list)
来源：http://hz.iojbl.cn/gtcbrcpoct.html

Go:   strings.Join(strs, ", ")
来源：http://hz.fzhhl.top/gtwlgezumq.html

Ruby: arr.join(", ")
来源：http://hz.sxryk.cn/gtztwdsrtw.html

C#:   string.Join(", ", list)
来源：http://hz.316326.xyz/gtxvierfkk.html

================================================================================
来源：http://hz.sufxvd.cn/gtjuftflnf.html

E. 字符串处理
来源：http://hz.hammf.cn/gtzepwwmyd.html

================================================================================
来源：http://hz.xziqi.cn/gtztjkmnrv.html

[E01] 拼接字符串
来源：http://hz.gotoacloud.top/gtouhhxjsf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.aizwys.cn/gtuvmegyat.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yj20258888.top/gthbjlrosc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ydjk.org.cn/gtamjmcpcn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj20258.top/gtgjbmyhpd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zhongyouzk.top/gtonhybplj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.316326.xyz/gtkutkzjyt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xylfe.cn/gtpabbikfb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yj202588.top/gtmayrmuku.html

[E02] 重复字符串
来源：http://hz.chenlongwang.top/gtgbrslbbd.html

Py:   "ab" * 3
来源：http://hz.quarkkingdee.top/gtexmjcjpc.html

PHP:  str_repeat("ab", 3);
来源：http://hz.gotoacloud.top/gtbctcxyhl.html

JS:   "ab".repeat(3)
来源：http://hz.aibaodan.cn/gtllydzlng.html

TS:   "ab".repeat(3)
来源：http://hz.yuxming.cn/gtyxfxwlxv.html

Java: "ab".repeat(3)
来源：http://hz.shanyushiyangkeji.top/gtrrzsrlmt.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.snrcjt.cn/gtfekjfuol.html

Ruby: "ab" * 3
来源：http://hz.birdmap.top/gtorssxjcs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yongpay.top/gttwcizivc.html

[E03] 截取子串
来源：http://hz.svipenyu.cn/gtlmmmqdqn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xylfe.cn/gtcpwkghjb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xuanzx.com/gtyftfifep.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.chenlongwang.top/gtgtvawjsm.html

TS:   s.slice(1, 4)
来源：http://hz.sysykeji.top/gtcsagjnrx.html

Java: s.substring(1, 4)
来源：http://hz.daria6918.cn/gtswtcxxzb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yj20258.top/gtvegspepz.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.ppjwa.cn/gtkxjqqeaw.html

C#:   s.Substring(1, 3)
来源：http://hz.yj202588.top/gtvuptvsqh.html

[E04] 查找子串位置
来源：http://hz.ivvv.top/gtjogrtzji.html

Py:   s.find("x");  s.index("x")
来源：http://hz.sysykeji.top/gtuuxcupsi.html

PHP:  strpos($s, "x");
来源：http://hz.dashuyun.cn/gtuwtlgnks.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.meibo888.top/gtbvtrolfy.html

TS:   s.indexOf("x")
来源：http://hz.meibo888.top/gtxsztrgyu.html

Java: s.indexOf("x")
来源：http://hz.aizwys.cn/gteizmzwmg.html

Go:   strings.Index(s, "x")
来源：http://hz.sysykeji.top/gtdnqogdqm.html

Ruby: s.index("x")
来源：http://hz.haohaochexian.top/gtaoxwynca.html

C#:   s.IndexOf("x")
来源：http://hz.tanke756.top/gtlkwuitkp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yangfankeji.com/gtgkynhaki.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.andypj.xyz/gtlcbdychr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jianghu66.top/gtmggjullj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.pycfn.com/gtkulgflop.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhongyouzk.top/gtothevowt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tian-w.cn/gtlzvlzwei.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.gogol.net.cn/gtfhfksaab.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.gaohongyu789.top/gtwxixetro.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yuxming.cn/gtdxwngdxg.html

[E06] 替换子串
来源：http://hz.shzxlz.cn/gtwnkmmden.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.tianlin.xyz/gtlihtuplg.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.sweek.top/gtleucftbw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gotoacloud.top/gtbjvnwrth.html

TS:   s.replaceAll("a", "b")
来源：http://hz.wangdashe.top/gtvzjvygyz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhijiandao.cn/gtpynkpftz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.smart0.xyz/gtjhancint.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hywenlv.cn/gtxzznvlod.html

C#:   s.Replace("a", "b")
来源：http://hz.yanxiufei.cn/gtryonovkp.html

[E07] 按分隔符拆分
来源：http://hz.jqgfzy.top/gtgldgcpzp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sufxvd.cn/gtujwbfveb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.dashuyun.cn/gtaeyhxhjp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.gotoacloud.top/gtkfqfxvnk.html

TS:   s.split(",")
来源：http://hz.yonumen.top/gtejgjqrjq.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.nanxinkj.top/gtmggighjs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ppjwa.cn/gtohmfuagc.html

Ruby: s.split(",");  s.split
来源：http://hz.bjfxy.top/gtszudlnir.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jqgfzy.top/gtqvqlqjoe.html

[E08] 数组按分隔符合并
来源：http://hz.gogol.net.cn/gtileicach.html

Py:   ",".join(items)
来源：http://hz.cashguo.top/gtihctducg.html

PHP:  implode(",", $items);
来源：http://hz.nanxuanxn.top/gtsppqfjlj.html

JS:   items.join(",")
来源：http://hz.xinyue.icu/gtmbhnlbsx.html

TS:   items.join(",")
来源：http://hz.hammf.cn/gtptijlryv.html

Java: String.join(",", items)
来源：http://hz.redwolf501.top/gtynqhumey.html

Go:   strings.Join(items, ",")
来源：http://hz.hongshengwenyu.top/gtsfqkbtts.html

Ruby: items.join(",")
来源：http://hz.tianlin.xyz/gtriuqzqdc.html

C#:   string.Join(",", items)
来源：http://hz.chenlongwang.top/gtndpowxtg.html

[E09] 去除所有空白字符
来源：http://hz.jinghuilouyu.cn/gtvyeejocs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jyoumei.cn/gtiyozuylw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.snrcjt.cn/gtpmqzdrok.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhijiandao.cn/gtwzdbnlls.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.guowangkeji.top/gtzlcwbjyf.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.cheryme.top/gtdtkjrrqq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yj20258888.top/gttrpgbnav.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yongpay.top/gtpmqlcjfr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yuxming.cn/gtgamtpvkz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.pycfn.com/gtnybhkdts.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jyoumei.cn/gtfuaabzjc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhiwuduotai.top/gtodskfccd.html

JS:   "7".padStart(3, "0")
来源：http://hz.xuanzx.com/gtbdfgfkjf.html

TS:   "7".padStart(3, "0")
来源：http://hz.dashuyun.cn/gtdvzgmjdn.html

Java: String.format("%03d", 7)
来源：http://hz.xingfuxueyuan.xyz/gtauauxlty.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhoulong.xyz/gtevoleitq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hywenlv.cn/gtofzofqcq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cashguo.top/gtnfcsaqfq.html

[E11] 反转字符串
来源：http://hz.mhx1999.top/gtqdszctyj.html

Py:   s[::-1]
来源：http://hz.jinghuilouyu.cn/gtehjzqndz.html

PHP:  strrev($s);
来源：http://hz.jqgufenzy.top/gtfhpnkayt.html

JS:   [...s].reverse().join("")
来源：http://hz.pycfn.com/gtukwgkhxg.html

TS:   [...s].reverse().join("")
来源：http://hz.shangyingyoupin.top/gthdczaaxt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hywenlv.cn/gtvpcdixko.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.sysykeji.top/gtoepegakb.html

Ruby: s.reverse
来源：http://hz.hywenlv.cn/gttamqekmy.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ybcxt.top/gtxaulzktc.html

[E12] 统计某字符出现次数
来源：http://hz.xylfe.cn/gtxrmpxgxk.html

Py:   s.count("a")
来源：http://hz.haohaochexian.top/gtxzhrkojo.html

PHP:  substr_count($s, "a");
来源：http://hz.zhengqikj.top/gtrexbqlvq.html

JS:   s.split("a").length - 1
来源：http://hz.yangfankeji.com/gtsjqozoov.html

TS:   s.split("a").length - 1
来源：http://hz.wangdashe.top/gtvwupdfxg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhijiandao.cn/gtmfvqmghk.html

Go:   strings.Count(s, "a")
来源：http://hz.aibaodan.cn/gtendcgasr.html

Ruby: s.count("a")
来源：http://hz.zhijiandao.cn/gtzpckpyfw.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yj20258888.top/gtmzdudhyq.html

[E13] 逐字符遍历
来源：http://hz.jinqigfzy.top/gteswmgchq.html

Py:   for ch in s: print(ch)
来源：http://hz.xziqi.cn/gteszkjhyl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.quarkkingdee.top/gtajxzoqyb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.fengsongda.top/gtfkyxbieo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.daria6918.cn/gtzqcbbena.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.aizwys.cn/gtbbhxgvhk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.aizwys.cn/gtxsuruing.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xylfe.cn/gtxuiywlfz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.aizwys.cn/gtafclolsw.html

[E14] URL 编码与 Base64
来源：http://hz.gzhubu.top/gtishbjohv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.fengsongda.top/gtwqbooaje.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ehwqpu.com/gtozvsxbjv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhoulong.xyz/gtrufdqpff.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cdnleiting.top/gtcmvasbbb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhongyouzk.top/gtcgtciqqd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yj20258.top/gtbksmyqqi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.316326.xyz/gturzjbgfa.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.kuanghao11.cn/gttmajqeeo.html

[E15] HTML 转义 / 反转义
来源：http://hz.gzhubu.top/gtkejduesu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ywan-chungtsiang.top/gtczcrkrqz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xingfuxueyuan.xyz/gtntnfwkee.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.tanke756.top/gtdordlzkq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.9152youxi.cn/gtxgeyobvo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.nanxuanxn.top/gtfiotbbvz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.9152youxi.cn/gtornqvtfi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yj20258.top/gtmkmpjqxz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.pengpengdd.cyou/gteeluvpok.html

[E16] 数字千分位
来源：http://hz.aibaodan.cn/gtafkctfta.html

Py:   f"{1234567:,}"
来源：http://hz.xuetiantiany.cn/gthbifpedt.html

PHP:  number_format(1234567);
来源：http://hz.shzxlz.cn/gtyrpbjkbt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xylfe.cn/gtwzgylmgt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuanzhike.top/gtwnkdeikr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhixingplan.top/gtuhvvbslz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jqgfzy.top/gtegeqiupv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhijiandao.cn/gtcnagqzgj.html

C#:   1234567.ToString("N0")
来源：http://hz.birdmap.top/gteediowvg.html

[E17] 首字母大写
来源：http://hz.gogol.net.cn/gtrdhnrdmg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cqqwz.cn/gtjdxlxund.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.nanxinkj.top/gtgcvepdqn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinghuilouyu.cn/gtkqniyjrf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.dashuyun.cn/gtqpbqcqyq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.iojbl.cn/gtynyknjcr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.52xcode.cn/gtxoedxtlz.html

Ruby: s.capitalize
来源：http://hz.feifeiyinyue.top/gtoyyqtebn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yangfankeji.com/gtxsitbykr.html

[E18] 模板占位符替换
来源：http://hz.wangdashe.top/gtsfywzvdx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhongyouzk.top/gthzqesnys.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.shanyushiyangkeji.top/gtktffbpwx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gzhubu.top/gtanobllzm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhongyouzk.top/gtxsuvawmm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.andypj.xyz/gtrvwtvvep.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.nanxinkj.top/gtdvmiykps.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.smart0.xyz/gteguefpbi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.snrcjt.cn/gtpmfzjabw.html

[E19] 多行文本按行拆分
来源：http://hz.zhengqikj.top/gtdnrgihae.html

Py:   s.splitlines()
来源：http://hz.jinqigfzy.top/gtycxhdfxy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hnqzz.top/gtoohrdddr.html

JS:   s.split(/\r?\n/)
来源：http://hz.dashuyun.cn/gtinqjheix.html

TS:   s.split(/\r?\n/)
来源：http://hz.tian-w.cn/gtmqqoplum.html

Java: s.lines().toList()
来源：http://hz.fzhhl.top/gtfbfymnqj.html

Go:   strings.Split(s, "\n")
来源：http://hz.cheryme.top/gtkrorctvx.html

Ruby: s.lines
来源：http://hz.yj20258.top/gtsnucgecl.html

C#:   s.Split('\n')
来源：http://hz.hammf.cn/gtxtpodngl.html

[E20] 判断字符串是否为空
来源：http://hz.xuetiantiany.cn/gtzjpdaqpv.html

Py:   if not s:
来源：http://hz.aizwys.cn/gtaeprdhtj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hammf.cn/gtnwgggcbc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhoulong.xyz/gthuowfwhx.html

TS:   if (s === "") {}
来源：http://hz.xuetiantiany.cn/gtltccuwaf.html

Java: if (s.isEmpty()) {}
来源：http://hz.ppjwa.cn/gtoqkyhybb.html

Go:   if s == "" {}
来源：http://hz.zhiwuduotai.top/gtewflevnz.html

Ruby: if s.empty?
来源：http://hz.cashguo.top/gtlnxmzynj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.gzhubu.top/gtevjkkfhg.html

[E21] 超长截断加省略号
来源：http://hz.snrcjt.cn/gtudrmngtv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jinghuilouyu.cn/gtrqdidpkg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.shangyingyoupin.top/gtjnzzrcue.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yongpay.top/gtldaemxld.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinghuilouyu.cn/gtzkmywetd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yueranfly.top/gtuxxikmnd.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhiwuduotai.top/gtquplnote.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cucudq.cn/gtokmgcbbx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhaomingkeji.xyz/gtgqecqyeg.html


<!-- 参考信息 -->