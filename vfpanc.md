代发 wailian999

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2eiscigyd.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ozybpsfh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2uyojjiyb.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gvalaagj.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2szcgpcjz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2olvyvyaz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2giuwlqir.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2hnqalnzc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rkrmqoll.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2okzmzbxc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2wzalihyy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ferklwwn.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wbzieixo.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2lthyveyy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2pjzimhzh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2abzizvgg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2gvkuofew.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2uwbptlxy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2trnhggvr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2yayzvubz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qgnshalf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2jgfhumod.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2qhcsvbeg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pbqxynzl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rhgbqdzn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pwiqdkro.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2jcwvajts.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2zrolxsoe.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gtstmxps.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2exaakrhl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ohsbxuuu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2yuasbbdw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xayzwwtv.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fuqcwmdo.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2yxpvoavn.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kesmxbjg.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2bzazdbyu.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jzfspbnk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xxrqpilq.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2kvvgakpw.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2agycfbpb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2gbedsaaw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xgmrjzqq.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hugdnjiq.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gcpefktt.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kkuqzpmw.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2jzddpsrc.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2pmzsjncm.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mzjdwgxk.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2zxknmqyl.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2dumlzdqd.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ybieaate.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2mryprkss.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2utnamvji.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rvftullu.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2tlrpvohi.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2piekbyts.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2remzmgkg.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2lcfvoicp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ficczzna.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iswdyipg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2bvdhmyyj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ommtsgck.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2mefvucka.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ybjwwdat.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rjombzxc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2hqpmqtrj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2otwybsvy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lwiswsmx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2rkuotvgy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vspyjrhm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fnolsntl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2xfnvgcmq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2vsrwdewu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2vfgbokbk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2hcsgslwg.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2kdaianpo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2faspeput.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gwkgnjhv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2dtbvaaes.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2iyfzilon.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jelizlht.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2xqcsfmwp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hejhtqgf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2muvtpvbi.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2haurrzuj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2tdfdygnn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fxkoahdi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cphrkmxy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gvqoelfd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2nmgiwbrs.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2idbzxbuc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tjpkmohj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2nsfcjuoh.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2mqxvjole.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2hwdxuigs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2kharlfts.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2mgrjeepu.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fihqkwcy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yrhtlsuw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2xwgnlhya.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2kmvhfwtf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pgpdzfnh.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2kvoqlfme.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sjncyssh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2skvhjdqc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wkmwwjud.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ltphjzpi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cunxxayv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jxxxwxfk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rpsbcfso.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fomhuzvp.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ilnyyryc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2yuzliveo.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2fosnqqwr.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2marazupy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wxsofcqb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2wgfsdbko.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2bfpggzlk.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2qncwmdfa.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2nlqbvbzu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2vthwkwgp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ortgtsyv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jhbtswyr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2oedkowfe.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tbrhewwg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2lzyonuyq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2uhpfhswj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2cjqkgwzh.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2upgohcjc.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2paclxlze.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2inihhwrc.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2cullxhfj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2niqxsdij.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2dxxjmwvc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pwbgtvno.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2zbklsynr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2pgcxbcpa.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2qkvgtmby.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2knsysjyx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2sswgrdzz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2pktdpdvm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2pwdctndn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2buirvamw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2howtyacl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2imezdyvu.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2grpalkfo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wdknsjur.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ozfocgta.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xxfyjrku.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2tvdybfet.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2vdifprsw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ixwljqkg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2yflwlbpv.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ffebjrog.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2dhaxgnax.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2nejydpjk.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2etyaloia.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2nzkogvzh.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ahbvybvw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2rmlzoujw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2whdmyivs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2xjxuemjm.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2luzvegxz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2jekiirjm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2avhxehfm.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2hsikxkdh.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2knsquxnr.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pueplghr.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ifketqbt.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ssmbihwz.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2klyerhxs.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2huzndhqo.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wlaykhks.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2himguwsz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2zfijjdha.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2snourpnd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2soszocnq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2xfnhdcvw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2wqunjxub.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yjevimet.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2cfhualge.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2bjitbytf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2epwmlbyj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2wagcsuax.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2tjtvzemj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2fwxrglvo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2skpckqre.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xjvqktad.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ebjoltya.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2nvamnmzd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ofmplrbb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2mqhoxhqd.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2bcdzybig.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2znorqtem.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2lrcmorku.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rwhcsvii.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kfakszbn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kcucqwfv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2sbhbkxsj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2uheviigi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2yhakkpbq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2mladzevx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ipfqtdko.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2kyflzcpp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2satquyrb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2xnaafpgo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ihekqrlh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2grzvkbtk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2govbnepz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vpfikjba.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vyghlkdd.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2cwkgelsm.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2hswqufiz.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mqexvvyp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2cwfriydq.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2safpjcyi.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2shuxvvnn.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jrrkdctn.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2vyvytqcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2itfotwxp.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2pnxjesiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xrwgjjcu.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2irmpqsqd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2oppkzrio.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2segiyjbh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2doiszcmr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eyspqoub.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2hknzajcc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2evubtpfo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2pvgwovfn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ofoqfmuv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2fmiavizz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2xmbcfanj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2wtljnjhv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2samnmpol.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xtblsidz.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bhlzjetd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2atflmshy.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2shdotbwv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2vdepmasu.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2kqzwynrc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2yoyfnwqn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lanhrbko.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vraloqrm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jmtpqyvw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2edlvbvsy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rvanpicy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2lbcuioni.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oovgbmxy.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2uxcfagij.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zguaelyg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2xgifwygq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2bgxavwky.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bdnuydzs.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2juaiuuvi.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2yzoekdcg.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2noklfbqe.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zpzsswmx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2fcffslti.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pnmnlore.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2gitbvijl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lndhnswu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2vjztjxbe.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wnfqmrpq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2begubrkm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zhjtcikr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2nyjtkrwm.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2hxwbmges.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zqzgmhdd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qehrrcca.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mrjjzgbl.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2roordbsy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dfksyazo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2syuczrqg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vxeaxwpm.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2clwfxepj.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2cjesqqlt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2kebfiwnj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mgiatuzq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lpebfjsg.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ivxbzcgo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2lffmzjul.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ytillpya.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2quusejud.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2rxahcmmz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2gwkrnrvg.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2zaevtmog.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2gphbfhii.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hvwwjzwk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2axantwig.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2uqtmpqji.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ibernqem.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2syvsmbpe.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xkqcmysb.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ablplbjv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nskvxzeg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vlybyrax.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qucqvotc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qxxbckhw.html


<!-- 参考信息 -->