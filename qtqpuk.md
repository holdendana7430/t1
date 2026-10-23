代发 wailian999

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3avzajrgi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3wijycisd.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lbweonnk.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3thfymxqk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbthzwzr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3oplqzxci.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3kzafjiwg.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rmcfjpbe.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3nbpsrfvt.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3yaggusio.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3rjlloguw.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3cwkcymjl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3cfgyarhb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uzpnyttl.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gzywdnvj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zoxwhavl.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3cggttxis.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3vomumydh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ssevqrdh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mtnbqetc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ribilfwb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3dvolbuss.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3jvoqjqzz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgeaafuf.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3mfvkqdzs.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3eskytlck.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3zkogvfyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fkjdsuwq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3frjzditv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uujbxnmq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qprcluer.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3xpxmgdhz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3kzfwuzpx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tabaicon.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3exvdpvsv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3jfylrjzf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3bhjugxhf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ztozauid.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3lcfdxtud.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ivxijqje.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3nqkpbvil.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3dglgxkzv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3useuzzoc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3dbzlpvvi.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3qtbcxlrq.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3phdidbqz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3emrpoloi.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xalbywuc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3tyitgllg.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3datwhelt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3qgtqozbv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3prfqesoz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xvoybwvx.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ukfvcwup.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3frytuzyj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3fwjulxfk.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yiydtkjg.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3cybjhvgy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3mvmnfjml.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3jsimjtam.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3dfmmcqpk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xtzmggke.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jhljcgeg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3csdqnhxi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3nkesbesi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3bxrdfbro.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3rbwgvrsn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3opoqbzfc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fubdlzrk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3diecitdn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3xclkhocl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3jkibocut.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gqvvwqcm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xbhexggv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3niopdbbc.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xgsrdevi.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lbolauxs.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3clyehiza.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3yktbyjbo.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3tzlcznsm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3zvflgprf.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qbtjpwuz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ekgptjri.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3tuwcztpr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3vbktyfqy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3hmwlpcjp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jyvbspmt.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qwzgkvyp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rcghceco.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ytmdsxsi.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3friuydfs.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ptxhmisd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vusdaymt.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ubxoakqj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3lbxpcqpq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3lrizfdrt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3eoxmmvjl.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3giyqgeem.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ogxgogey.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3mgfarfbc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3xcbbnmft.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3budsahnn.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3feysitud.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xlxubodk.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3bzonpshf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3gqpymepc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3mjvxldui.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3lmenukih.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3alpaisid.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3uilnktpe.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3fwmqjiqh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3sapswzox.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3flwpfqcg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3msyylres.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3fdiljhvl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3vkwlkggr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3bkmankni.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3tqlgzvtl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ixlfvkrl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3rtwxcvfc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3qpdgcypu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3nlaqmyqi.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qdlboume.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3aawqoqwn.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3rulocrmx.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pvejvokg.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3xqqcmnij.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qjcnhxet.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3vxddkxth.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3bihpobwl.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3mxbapuca.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3sgkwfjsj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3pydruezb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jjkjakes.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3aixkzesp.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hajunzuf.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3mdmzkunv.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3liaikzcl.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3bplcpfdb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3pwnsxexo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vgfhzyqk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sfhltyue.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dyinqgdr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gylgpndm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3gsqogfld.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3exrppzox.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bztodgwr.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3gvaekxxf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ntpimndo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jpbewdfq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gpvifgas.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wnhpzlah.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pbbjyjoa.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3uunvlvqn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hkmonidj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zhdzjbfk.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3qdbfamvn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qnpgwzbi.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3llawqgux.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3oklotdyg.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3rdkhrwsu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3vegmrhiw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ltkwwbmn.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3potkkziv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mvfrenym.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3eapeotrf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xqvxfyyy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ncvhguup.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zmfomrfi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3lcnftimx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3vntutmnx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3hcourqmt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3cjssopib.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3isxlxcou.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gglcdwen.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vfufnvre.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3orofwmze.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3qbrxgviz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3helmtlvf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3hmejdsjy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dejcfilm.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ocpahljq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3wimahhln.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3zfkwljpj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ydzrrvlp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3qlkogybz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3rcxcxsaf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3sotcrdqp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3sfgwpxwe.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hzzfjgde.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ghqwypcs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nemwcjgu.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3dzykfodn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3yuqobvmn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3hmirnwej.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3iaykylsz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3xxkdqkgd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3jsmflzgd.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3azkqsdwv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3dqxbdsqk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3xrydevcz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hkktttbg.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3nywputhg.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3kpblsucb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3tlvrzgns.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3grobslid.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3iyibwwsw.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3nfswpfqa.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3hkfjjsbv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3empujjfz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3galvlqdp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3lypcomsi.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rxmkqwsh.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bvqtiylk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rglaxdeh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pexrhfzw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3krnwtgts.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ilyboiat.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ynyldpqb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3cfrncvwp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zjrtukqm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3uwcfakxy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3txynlyru.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3tcwyxpnv.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3txiqcksz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3snyqcypk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3gwphssdi.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3sxykkcrp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3vemvweyl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3dpdljnau.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3btbqtkav.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wybdiqad.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3icxcnlsq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3qojfcccv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3vkvyopwk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3zpyhupkv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ulzoniek.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3bclybjpr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3wskzikqi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3zfxqodhr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3boxzltsb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nxbzvgce.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3juabnqwp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3juxcmdri.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pkysrgex.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3qczgnyrj.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3arykdbng.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3fcbndrwl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3levedrli.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3njmcwahm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3juhtgwwc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3almznnbf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3lrfqxken.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3lkkdwxgq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3erzcjaxo.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mkjbuzzf.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nsfexqgv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3lgnuobdx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hzritxii.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ghoisrfg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3btgerqqt.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ysqemorp.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dsvndilb.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3dptmwuig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mlzadety.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3xrxlnbzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ecljdcxf.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hxgzhwqx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3wufiwqkd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3lcqvaypl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yycwmesr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3hyiahomp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3okdaehac.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ufmamoxd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ljvqidgy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tpmmzbcn.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mfftdejd.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3hjtszjtv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3jyqacqlw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wdboeyaf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3aqrszyxz.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vwiegdrp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ewyarfzt.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3jiyscqyn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wetlqdgj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jkrlevnh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3egqddukc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3eyrkznmt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cxklvhet.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wmsprdoi.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3oonukaxp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wfohumkk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3irrkknke.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3bdunjjzz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3dyqdguhn.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ygiqsdmx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3hkhgecif.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ierezjti.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ivjysdyt.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3imswgblq.html


<!-- 参考信息 -->