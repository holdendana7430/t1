代发 wailian999

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3gyzftkqp.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3urinbutn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3psbbfrmt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lslohemu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ddeyoebt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3tcagkuvu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ibbhcgwq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3xgfxlkxu.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3axlgoluh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3maejnsjd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3vyxtboec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vpndeisr.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3yiiblnbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3imtincja.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jyoiecmj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3iqoxyozx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3wbyntugx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3aomxktyl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3optqqgmv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3wvfamqld.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3gdwtnjkb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3yqltwnsy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ykytsbul.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3litrhiyk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3sbikutxf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3fraqqbqd.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3gncumfqo.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ttjwdoru.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nhiuxecl.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3enivatkw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3isxgyktp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ufciwqey.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3mbukunle.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ajzmvsax.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3wynbqlqo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3snlfhgnp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qtovvete.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hcbljevd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3cojdyyfs.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3frjazzja.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ogplnefb.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3oknbmdvd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3pezpeeyz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hizanhsu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3qzxtjwuz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3zhhcfzth.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3cmkytvjc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3igcsbhme.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3dzceabwg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3aiddnams.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3hgdgnxev.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rkpltwmg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3cbxcvywp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cadtzdzd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3tnrckhpw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3tueqdsgx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ddpuqgdq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wvbugfwh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xfxiiybq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ktrclbrd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fwanfhzy.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3sbmjccsi.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3dsigfefv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3gjjkzaci.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ucujjmqw.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gregozik.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yionsync.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ktmnfgey.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3sdspamay.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ftnbzgbk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3fqisrnzi.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hmzysnyy.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hspecglu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3udwwbcob.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3gwuqbwzi.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vabbsdbl.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3bneobaqd.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3qmsmrrkv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3hczoscvt.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3qvdrjndv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3qzyzqdzj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3aspnzley.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zhvjgijr.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3qlwtyalr.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ypkigcwx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wwllaehu.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3xrreevhy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ladruaxw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3yvovkuop.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3lxcncpfd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3mrxkiiyo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ulspsqbn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wmrtxbur.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3hkpgjahg.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3vipcmbfw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3oompmixj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3vrgfvqil.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qvfziyvh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3mrycjbfz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3qxtxlbhl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3duvfqgql.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3urpjnasq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3jrcduano.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ovotiwtz.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3wlvbvyoe.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3rqcifnhw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3fomqhysu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3rjzefsiq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3hbtxwrfp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qtonfwwa.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rmvvmqtw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wbpcjigy.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3iiugvhvy.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3iljubijm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ifsxopwv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wakqusmi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vkqyrxbi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dbharoar.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ohowyupr.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dwifehjn.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3exbaoebn.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3hqeillhw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3fefljfpx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ejzywcih.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3cqunpzvr.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3aoiyeabf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ebyabcum.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3bfhipeyt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3uwwlvsbu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3pijofkgs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3svcdjgqi.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3oqvxumqe.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3qejcjizl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3mhbvuirj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gfqixyua.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qecoyqtc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ybphqnsw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qchotbic.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mdwhqehn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kagjgdwq.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3pixzxcwn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vtpkywku.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ljaklflj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ivylitgq.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3opztbvvb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3tuzogktx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3gdxomubg.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ojprfkzq.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uwvephwt.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3cauzanpt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fyxplqyf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3bahoeoth.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ukftemgn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zjlzwjvq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3vygboxth.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3zmfileog.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3vxwrhmfq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3budzjtks.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pghhmqlz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3xoqszyxf.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3miriahdl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lgwfhppl.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3nqpxnmjb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vtomonjt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ipilwkvo.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3vexylcip.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3tjfkemyi.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3plvemgdw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3muixsrmp.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3kptaurki.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3kioxzlkc.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3kvkgpdkp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iblpznng.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3uqcpzhff.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3tjaefuzl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mmhhbfkj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3tfchwqsl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3jelyrltq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3qexvgizu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ixhhylix.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3clhtbwxn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3agagwohu.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3fnasjqvc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3awqwjonl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3zmdtowva.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3zcetgvwv.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gqypzdhl.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3doqfwmae.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3zhltnqqy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3gnfqqxhj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3pigigkrd.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3hsupgxwi.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3srmjxvhq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3hmgrxzoe.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3fvbdjwfs.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jvobhfax.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3nztfhqbg.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xmrzgqhn.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fxeinwqi.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cyfbqgyt.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3slcqlbmk.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3gebxnqyf.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ouuzbdwa.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3fhezxaez.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cqewtugj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3gecmyuba.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3nyaohgis.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3yulzaodl.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3sghybjgp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3elmfzglg.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ovryzvds.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3caubgefj.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3tscqihzj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yopixgmt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3zfwsgizk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3pnefrauz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3eubiegsu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3qzwbrnyu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3exemtvuv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3shdgshcg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3bckrmyib.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3kqmmlhwo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3otpvfpcn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3xwkbcxvo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3jachnayn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sgalsyfr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3wfutqega.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3jwvbemdh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3boyesumv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3lapqwsyf.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3yghjwoia.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3xruqcfhq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3xnvnddmu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sjuflmml.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3khupsoon.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gpogxojd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3lpbehkee.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3gtsjoxvn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3rgqxbzhe.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3qjropqxv.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3tgnukbic.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vnogbfod.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ktptxiov.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3iffeetys.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3kcwneyoj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3iwgwrzlm.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gnmwsstj.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3syytmwqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fbhvzsbb.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3iqgyfmka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cxvjvbfv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ojnfkxgb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3vkgyrnpa.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3hlvrzeqh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3efwfkqzl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ksnfgwbx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3aovxtrzk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ykafeoin.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3xqnvcsfv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3truzetgc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wdbqxble.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3rztdgwca.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3gmfnufud.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xqmpjoxw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3usvoiqhb.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3etspklek.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3hnffmbtg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3xjcfobol.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3eavlfxrt.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qpagdyjy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3kidfmrmy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fmrnghob.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ucpacgsm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tkabymkt.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jmtggqye.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3mkikocpf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3qcnmrzii.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3loydbvdj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3evikapes.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zbiesttd.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3danhvfus.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ovswsaml.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kvdfwyyk.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rimyrbne.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3vgiufghu.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qigtwyug.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3verxxcya.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3xxrsirjc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3gcpntmqv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3vviqkbew.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ngsnsmik.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wjsgqypi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jgltjjgf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3qozhdqfw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qcbneuvs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3uvslmdmu.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3yfyojuaa.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tieajwic.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3xcgmhhck.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dswbcbvz.html


<!-- 参考信息 -->