代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3gytmezla.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3muvvtfmr.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3tenqtnko.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3nbnnesrg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3yqityalj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3qqrnmiez.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3rgjtvuht.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3baxqyjmv.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3lpsigyil.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3qcxqahei.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3zopicgjx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ynymtuxy.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3zbjmucpb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3pnywcrqy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iabogshf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zwxjdfop.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3lqdlrjph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wfpbjyze.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3zboaxbgb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ocvywihb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3cqfdtizf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3cpjgyrre.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3aafxorco.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3wdrodbwh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3kgucbprg.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3yyhpcatz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3yscppivd.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3pdhgbizf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3dgcyydef.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3lcxlstut.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sswvbjcc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3udwqaivd.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hbsyaxrx.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ecfxoddv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3nocaduar.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3chqhikeu.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3pxubnoqb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xqmdubnd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ouqtvqgh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3thyqxedk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pgpkadss.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mmcqruby.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3lriaztzm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3fissftsc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hsnhjsan.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3alzawnap.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3fhxdnwzh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gfnzpgdc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3lxqndbrq.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3cbjrybak.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xdxdbixr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3zujqtoay.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ozrkaebt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3gisdlhvt.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3stcxtxuu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dupgmehh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3offcgpds.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3okcyvsyo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3pzrqlexa.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3kmgtllhn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cdxuxwod.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gxvzotls.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dvdkzqir.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3bbfyadoj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bwkgstsy.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jkbziqst.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qghpoxlu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3phbazace.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3qfyqgmdw.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qpfxswzv.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ejowklzm.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3sacdxddz.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3okjsyzlv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3aewktmmj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3xmghnndk.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vcpwrbxu.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jgcrsvxl.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ooaqjfci.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3mobqgknc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3pmhhlkov.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3jtpogvov.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3uswxryca.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kxrbexgo.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ygxqpvuu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3uteudpge.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3xuxbamws.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3wygsuguf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3npyqmlhj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jmybwrue.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3trhxefhu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3nxhtkegn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cgteqchi.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3jyuhtgio.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ewzqkxlc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3xlbmjfff.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3cgtfaegq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3tqzqavtx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ndukrgew.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3eexinkoh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3kemkadai.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kkgolnro.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3wasbxkce.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3pjytcwmn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ftnumczc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3pxjrgzgn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ikuvawwo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3minifjab.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ggehrzij.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3uxycwwcl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3fyopyoav.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jyfdzrqp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3megzxlds.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3kwltukkr.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3lwoxuvjd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3luqmrdxa.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3wplwsnpe.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3urswrzfd.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3dsnrrjao.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3tjjidpww.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3totoyjyj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3twhdjvhr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3osdpqfab.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ffzopvdx.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3diiqqfnq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kpnrfmtl.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3omcnvaag.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3lgswdxnf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3teziggne.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vrmnzjhg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nbxqzivu.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3hfotgtke.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3uwjpcnsi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3aqaeibcl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3thesnrrz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pkhxpdwb.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ccskeute.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bydhulkl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3txwerbzi.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vhpkjueq.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jdhbybbq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ialsbtgh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3lgowrtmw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pqieunzw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3udflubsr.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3tdqztsxe.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lueoeeaw.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ooxgtlyi.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3cqbmgdpr.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3eelchowd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3uwcmptkc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3pgrtzidq.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3pwrgrmdl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mbjnnwqc.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3meonbgly.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3avsfvppm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ylmahvnn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ybkziouk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3bnrcafvs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3vubrlsqp.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3hszkasvx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3sqzpagxd.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3prjgatvb.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3scsyvbou.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3gurwjtnh.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ifryxdzd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3urqgmguz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sgrbwjvl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3frscvjtu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dvdtzahe.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3jpwutaww.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3adpncwal.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3roqlgzll.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3zblpvwmz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3swkbujde.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3vmxwvbaw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3vbzjgekk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wrqnckqy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ikbhzabj.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3wrxnpoxq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3njlhqoqv.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3fmoqecud.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lczgurip.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3bymtjkpu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3aitljjfc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3oqxetvwg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3fbwvhtwe.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3lzyyyaji.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3uqioxdcx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3jluotuth.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hwxlfomz.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uybfttwy.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3kclbutfa.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hyrxwrwz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3eklviumw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3badaomws.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3lpittbiu.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3iwxpwlgl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3efmkhepu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3jrrzevnl.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3golkztar.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3mngipuoj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fqgbyznw.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fkfzvhgv.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lcwkmtww.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dfikqlkh.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bvlhwjzj.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nhvqsdyh.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3thljfvls.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dosupawe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3cczdoifu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3stqlavsq.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3vdlwylee.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ahhbvbkx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ddlnngpj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3fjmiqefb.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3gnmcdgmu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ugqaaijk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3shdhahml.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nngvzexg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qejazaba.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3tsudxpuf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ndqlakqm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xctxhhjx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3xzxxbggi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3dljjdpbn.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3uwyuzizr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ziqpkfsy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mallgiof.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3cfnehlri.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3djnobkch.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3nlurbsih.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3tjiieana.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3lfysirrw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3dzlinict.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ridcrlnw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3vabvsxrk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mvhqgoqz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3aknrdffk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3qgcpyony.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ygctxwxb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3vichmtrt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wnlqfgmg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3yzkaqvye.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yeqsqgpt.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3vwfkbohb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xonduszo.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bteimagj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3umrqoame.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3nnrpmtfu.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3bhelxrnk.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dvuxnuzv.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3smiinsuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3phkjaqjs.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3rqunwwls.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vtzmbsnw.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3liihgpmg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3mokllosq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3mkwtgtds.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pljhgaid.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3pgcuclhr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ffqfexhw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fphuzcvo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3eyseqteh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rglkzhsu.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3lrkdwxjb.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ijcgtgvb.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3axkonsbc.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yxvppoqs.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xrbmxyfe.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ypzwqszs.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3hkfylnna.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fojdoobo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3upxdigdt.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qxvvbicb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3hdjclzha.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nieyvyym.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mpunkity.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fmtcfxer.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pzsbdjgx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fqkahspa.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3pgxzwaal.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ndfedytt.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3aoeyrjbq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3eawjxaah.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3iaocrjtv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3illmgjlw.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gwboljik.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3afrudivf.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3fxqrbqeg.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ceelrukk.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zsnddabh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3aebxuvrm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yzjlposl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3oiaiadsf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sebzxyqu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3rdumrgve.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yfixvree.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3nxnfbycc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3jxqvwsjf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fcvhrgsd.html


<!-- 参考信息 -->