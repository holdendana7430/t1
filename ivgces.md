代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2nrauwchy.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ftwmksyq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2mwgcauob.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2xcraggbk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jpbrjwgm.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2miiogrtg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2kgbikfum.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ttgokzmj.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2aszkdfzy.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2rmudselp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2xmmycisx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rjbfdfnh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2nyxscoqr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2najiojps.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rqpmucse.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2iarwetjy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ttdfxuqi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2gapetqxy.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2kdnqabbw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dqkpuiie.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fkwsdrvw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bgzssena.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2maleczrr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2zjittfmg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ovwvpfyr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bbyhvwdk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gzxvyjsz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ryrpqdls.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gptjiywa.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2dlvbegre.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bklvwyln.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2wnphtpzi.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2gwevlnjk.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2siqwxgdb.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2sjignagw.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2jrdbshyu.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2jjozzuer.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2rmaeldeb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2qlesxheu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2unzigrwr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2yzcjokqd.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2imkfreks.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ktmwijyc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2rnuszifj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2nnzutryh.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2vnoufidn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2byoaewsi.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2olcobejz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2wouflrsv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2teiqnvoj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2thoutqef.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2twwibfns.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2syaoupir.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ggtgguvw.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2pmdfejao.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mzlcsuzq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2domnntcr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2exrvrduh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2qxvkcxiq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2vkwpftza.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ydtwyxvb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wityihpt.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2claegdxn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ltvysgln.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ahjkximu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bwquirpv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2evrvrzjm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2qpjcnsxu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2wqcslgzt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2kziaqvhz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2mioaptnf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2myjozyzn.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2gtfjogzl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2qdicrajy.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iciwufho.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2zlgnicvp.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ohgwleze.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2elqtpvzm.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tvewafrn.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2owihsgjp.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2bdlbgndf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2rgczkdjb.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ousrgzjp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lafabnmt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rzarquub.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dkmjuedu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2eknidane.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2olftmyvs.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vberwnra.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2uimynswf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2vxdicudj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2yzhjkcyg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2bynrizso.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2nzogbzfw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kfsrzaxw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jdmmomfx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2xxdkxjuu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2rlkziqzg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ndrpmoql.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ecuggxfi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rhczqshf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2wcsmealh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dakphyir.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wyvikafw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yarknrjw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2osayigyk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2arjrakbp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zaxvjdvp.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2szjiwklc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2dcqlsjal.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2njmxxmon.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2cgycqydn.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2yriepcom.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ocxebzto.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2micsgrro.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2motewhgq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2awfkxysq.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2xntuamzk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rtqkadxc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2fmcutpgk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cijwhcmr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2undymnhk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2wymxtgiz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2rmrxxmpl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2rkxepzuj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2owxnbdxd.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xrxwddxd.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fsgzpvnd.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2opqnjpai.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2jqfpieal.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2bouwfoow.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bchkapdo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ojaaqxkq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2zxnomwkd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2tcidelig.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2cnyyrwaa.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2nhwvmaev.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2sxgagwhc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2aywmdmrb.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2tuwalvyp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jemeqcsh.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2oldxblbr.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2mjhrjhfr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hcysqcyu.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2wpevvixm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ojytidbw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2xdwbxnfq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2cjunpthk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2gzyfedwy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2umlxdrrk.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ixwuhaom.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2eeypylsi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ooqcxnhb.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2lxiuaaib.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ysfjtwuh.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zxnbydvq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2gamfoqkt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2srpyafhd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2dmmqbekh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2wgnfflbs.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2omaszxld.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2tidjhfnm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2vwsjpjye.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ohpgjgli.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tyuhgbxk.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pehndlqe.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hjdblaxn.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xhrnoaty.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2viylnmwh.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fcczaqzs.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hfcahgfg.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2rovwrirj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rkzxxyaa.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2uyncmabu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vodqbslm.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2vqhhjsoz.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xbyoqnik.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2kiharvar.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2lbqdgxgl.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qqvsmbks.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2qbqlhuam.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dvrcaxyl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2myeoboqr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vgcudniq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bqovsakp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2fywovurz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jjquwcqf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2dfbpkcip.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2glmaplwl.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2raqpjmxm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2opobbtej.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2oicgtgxf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lhrcbhrh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nciksknt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vzfpcbgs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2zjyjvvlg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uhnpsmez.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2lppzpcwh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2qxavjhek.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2evmxstbc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2cenuafjw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fcjpjisa.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2xgksxjrw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2oiqivngo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2rlwcfeem.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xnekxxkl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lypgcovi.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lzgedhng.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2kqvqjizg.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ufcrdisv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rvuoeoyg.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2uxkjwsgc.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qnvuqumz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2bhlbzhgi.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fpmvbkhd.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2lwasjdci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xoypolql.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2rzsvngmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qnsnavbm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jeztbtcy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2iftmybtc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pkkiiwfi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lhornkpo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qjqarghd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2lwrecfra.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2envfwfbe.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2hbtcrhfs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kwpjibac.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2xyqjmnqh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2flhcwcds.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ibloogsw.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jqztfsfk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gxzofewv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2miflpymh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hbzewbkm.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2nzkhrltx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2rnnoecnv.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mnizcliu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2wajarpqb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vshihvie.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gymcpkbm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rwmahynh.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cedgjvau.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2gocfqarp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ycqfvdrn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2opaxoaby.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2egtsfaaa.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2pgsvpzqg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2thphtzux.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2glgkzipr.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bzucfhpp.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2olpsffid.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2hffickjc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bsxefunh.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2regsxlmb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2vmzbvdop.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nauptlfg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2wcmwzxpl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2azhyxsqk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2zikephzv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zymnsqmp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2xuqechkh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2srwxxmic.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nltgvpdh.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2iugbsuan.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aqrhsitc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2edevhbcn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ibwmetnu.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mpvgxfrv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zhqrcjod.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dpzkaztj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zvtqwsor.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tlhhwxlh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2bqcnkzdy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2hrwnnnzv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eskdnrye.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2hbssbjcb.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fwtifqso.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2optmnuic.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fbvbpkcp.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2wggbdpbr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2rmehkwxs.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2nfuffzat.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2tpsfebtw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2bxbhcbwy.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hbiymsxz.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bmnzvucn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zrhugivr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2fhdurgez.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dtlhdmdg.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2mbylercn.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2eiccucfc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2isaywlah.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2vipqatld.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2sysuxfgl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2gaudlidn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2vtrtphbi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2hwckrzno.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2iztndhzz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2sqszrsyr.html


<!-- 参考信息 -->