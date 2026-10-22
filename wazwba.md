代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2qbvqlrkl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nxwyqusx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ywmixgfn.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2yljhmwuu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2lipreqir.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2tpdvrpnq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2lnhsscha.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ljbtazkv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ezoowkxf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ojsaaetd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2esrqiqje.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ywzotamk.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2jfazunrf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2zsfufpdf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2lxqmrvhf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2knserjxh.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2mrdveshf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ofihpksj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2secyznyd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2jrfmpjsp.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2hvncxsqa.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2eqadnski.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2vaezmvol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mozezanl.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2sdkgpjur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2axbhhkwx.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ctzjkgri.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2prrwnkir.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lqlrbmro.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2tzhnvxjy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2yodlwddp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2zezkxpos.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2touvfdnr.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2tejatuyf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2tyucnuek.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2qwyifmdp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2kayuqkfg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2vuhidvkh.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ujqzgulh.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2clgolcro.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2mesjpgar.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ulbtsmfi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2yjrpmyee.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2kbtklvmu.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2icgtiakt.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ptfnvpif.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2xjqtupsm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2biyoihkz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2auxqebrj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mgcizjuq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2yunullbh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2xbividge.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dkyyvdza.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2aydzmcoj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gyybfwym.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2jguvkmto.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2pwlanyyx.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2lsxbpjhm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2hztlzdwv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2neylavry.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2thdsazku.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2dacwtfbq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2eomuqjes.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mdeugwrw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dwohduzb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rffobbik.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2nhqawvom.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2nkfpiqcb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vomnijqh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lptsohae.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mreamgsd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2beqmwxrm.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pmdhwhcj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2rtcrllli.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2jyoeheco.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zynyjcdw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2cufiqcpa.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hkoluthe.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zpumchts.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2sqiwvfsm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2hfvpydzb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ikvshixk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sberivcg.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2yrbdizwo.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hquqtqxw.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2efcrsyhc.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2snizrkbe.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2eldshqqs.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zzweyobh.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2rmjgfdgc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ephfozdf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2vflcyroc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2uohqhgfx.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2qwwdutqe.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2vtkaezya.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2eeldtapq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2mbjhfqfx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rjxelscu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2nareprry.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2yljnckjh.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2olcewlvp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2mgsvoufa.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2cwmaolrf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2fbjeqwkq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ugerattm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2oiknghpf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2qvkiqcth.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2xrwoocou.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2mfquakrf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2szikrghj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2nqcmtgiw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2wxarglzp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2xcejffzq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2jdsddxxl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ecixjnaq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2lainrwrt.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2zemdjwwz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2uaxtoynb.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2drghzivu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2dhebxrjc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gpfkazeq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hkpcbvul.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2udrjawqj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ayfserpm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2axnuegyu.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2bwmxwidw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2xuzsuhfa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2pmyktfcp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2itspvxue.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2szezycqo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2xwmfdyme.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wigmbypd.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2rwusmnzh.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2cubbugbm.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ardxudee.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2zsvbwjkk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2scrxqxqg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fqhwhqdz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jsuiurjn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2crzxclpa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2dhwgbddv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2uyerxirf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bsjtgibd.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2cxgormkv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2avdbzgjm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yksmweqp.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2onbxapic.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rkcfadlq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2whqawswx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2npvmnxad.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cxqbjpcf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zqswuond.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2jvbyrqgk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wyexlpri.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jpnpvnbb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tesixkki.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ckadsuiu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2vtbfgsqo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ymgglwje.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2gfxomlfz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2sytptanj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2trwzqsjr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2orjdpbdg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ojqkeobl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mxybzecs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2gmcvruge.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2eqbkaxfz.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2mbkfjrfk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2uwfrsrxm.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2glnlyuoo.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2vkvyiwny.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lnhnyscs.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2gmzqtomn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2otvpzail.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vyksqdps.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2eooprmvd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2fxmwzngb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2bwhiwamz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2fuhoeszg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ktmevdkx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2fmphdcov.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2rbhrotqu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2uxkafzbr.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2cajjizwi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2otihckwp.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2kjaxinpw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2tkkmtosc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2smrskqkv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2folfhczv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rshmiqko.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vfetjkhr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2onzazrtf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2rcjlspzl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2cgfaebnm.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2axnoqsks.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2flrnoyka.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2jqbukftf.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wtzxkynt.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2krxljwet.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nulryjzt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nzhugeno.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wbluoxqs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2fqlcheiy.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2fnolscfc.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2htmhetqj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2kmckxiqe.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2uxbvkwhl.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2kazgckgj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ucqrjkvr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2igifszmo.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xsbttbmw.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uimtqctz.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rfqazemi.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vgmzxewv.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2eabzqaka.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ejylvpmr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2taoirnsi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2sgbdbezt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qerbfowm.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2isiuiakh.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uebtpqso.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ltuotdgk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2jajiuqps.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2rtyrrdtq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2xluwqdai.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2pemsoiup.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2doqjuhob.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2exsuupeb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cqmduvpg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ixmetrpa.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2aohmcghw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2gzzjpwio.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2yqnrbiak.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2hqafbeas.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2sozdzfcn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2xpkmugmh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ldzudvxz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yfqikvoy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ajktjnlj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2vrihhhkm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2erjnyqsy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2xgkdbyif.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2johembnk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2atysfuwc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2zzeonosb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2qrrymrea.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2palugryy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kshcilpa.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2jvzupzay.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2vlpllezf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hzmdrzif.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2llwgraym.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2oootxnde.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jsekkuzk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ycfmypnh.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2maizbvnx.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qnalbgtb.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2fdlizkzb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2utunwcei.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wtthuvhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2msltakpe.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2bpgzoihh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gdeyibcw.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hjtnkxtw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2kphjqwnl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2xfwrtlxs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fywupzju.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2weqszcbm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2bxxlysos.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sgydnrqu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2sigepoxo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mcojwyqw.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2qyvlgupi.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2zyfmatdl.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2yzwoyqqq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fbqiulfp.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lswbxvns.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gxhlxmyr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2gziuhuwo.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2efgvakyp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2cavsmpnf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vysfobsf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2xbzsdahj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nallpqyr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dgtijdcb.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2olesvaos.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yhgtfnbe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ufzcbukx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2tpfzbadw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2wemqlhds.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2gyptqldg.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2nfzfhuet.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2bqafzzfj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2pxoarhsf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2okidhnnm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wibpbcux.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2brjwesvq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vnfyyspq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zudevgzh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2dymfmzbo.html


<!-- 参考信息 -->