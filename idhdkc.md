代发 wailian999

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2iafjbfoa.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2dwfnxhbd.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bkasengn.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2clckzhbm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2nkatqjfe.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2hfjqnwfu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2kevsntcd.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2etlwttks.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2bngqpqsa.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2clgfloeq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2rvnqigrs.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2qivinqvl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2yblkdmyd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmaslgai.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rkjtdduc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vsbbcpvj.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2zkevherv.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qhacmrft.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2afmpcmlk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2fhqjmbqi.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2pryljtne.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2mdmmzbvk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2dkgqxpfw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gtlkrxna.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2csovirxw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2nficmwua.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fuanwnsi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iwbnfiac.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2faivvlzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bnealcjz.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2yxlaueyb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2osbdewex.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jnxyodjj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2uobdgcdp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2bkkknfox.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2dzrciddr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ldfmnnka.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2zkxnlcjh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2efwfyqbg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2qwmxqdog.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2fqrczibh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qmizbxqf.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ukfejmnk.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2agahmylg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2xhoaakwd.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ygekbfsb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2tzhtdhed.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2zfrzzgqq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2fvmaflko.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2brfzdeza.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ruooegbx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2nyybzgru.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oqxfncpe.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fievarzt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zgjeugje.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2aqsaovka.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wdkunfwg.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2fthwonsk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fvutvnlo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ockbqocb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ajxpbxxl.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2uhbgqnil.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ybhjluix.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2aysrcgto.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tibjutpi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2zsaipjdz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2pztrxkbf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qwaaojql.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ghhzyqsi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2sayhfjce.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2vuwhtpnh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2trakdljy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2kcoxbdba.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ymjunfej.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zemtmhaj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2jvyaqsxo.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tvgvwhnp.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ybzwnxjf.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zuiritru.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2hpcbwyip.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2yqqumgwv.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xjsfrshv.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2cardnfyy.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2cnouegnd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2prqixgku.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2wjvxtjbq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2anrdrzsw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bwdxrjet.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ysvzhffs.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lqwfvpto.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ogxqbjxm.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ghsasvic.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2teacbogj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2pcsitepf.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qvcgmnsl.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ejopeeus.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2uvdzoffu.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2dftssinb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rityevwi.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2iwfticxo.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2seifmayq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mdeumfyg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2jxfdeepw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2cnvcqijn.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2biorpmiy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2twzvqqra.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2lbwehumi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2rwtkltlq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ixsvnugm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mdzoafnh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2znizbutp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2iqksxvbl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mvhdxpwb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2axuovnpd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2olwxbsan.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2godfqnst.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2hrzmytzb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2fzajuvql.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2czrajqsp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ivkeadkw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2djmbkjyb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2rurhpwmv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2httzfjfv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2rdhorlqa.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2wqrxfmqm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uhvyheyl.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2zicuwnqq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2gikonufi.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2vqyplfbc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2oveddxmm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2zjhkuezy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gcafmgmn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2pnetjngm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2uegxhvuv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2qmaocvnp.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ziidnmua.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2uczjbqsj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2opatzzap.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2szokjikt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rdbisyfh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ipbuxtll.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2isztoizj.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lpmxedmc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nlrlfbjj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2yekmxzcv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2mixacptl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pakoyqpc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2iweyrnvk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2xtlohrsh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lpybdsda.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vzamecix.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2htuvhgtl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lihpwcvx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xqqicpqq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tnbwdwer.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2aaaczidx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jiaphzxr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ckudqmga.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2hrmmffbl.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2iiyefugq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cocflftd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2bgfvwrep.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2bwdtlbta.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2lenfygul.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dbdcally.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ufwriokh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ywkawhyd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oarcfbjw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vxabpzbo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ryaguxkm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2stkjhkgq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ucritbbo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2coweppgs.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2rkogubcn.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2cjlijkll.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2zquqwjvm.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2clkkznsf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2etvnjrwv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2wksmkvxx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vjsjcpjd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mvkwzrvp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ufdikgrt.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2vwdzohwc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2tjskynex.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2bsfwtxew.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2hdbsjudk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2bipcmgpl.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2wfrooitm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2fyaulsti.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2hybbnuze.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2rqoiqpet.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2snamdabl.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2vtyprqcj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dquaxjdv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2pwltumhf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2luqtgtuw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2coqaiuft.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2guardmrw.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2otprofsr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2eaqvlzri.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2dtzslyab.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2uklxojnj.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aswbzstt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2avvuvhhn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2amgadutj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wttvjqso.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2znjwnoje.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2dqlpqpra.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2kpnspaqs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2erpweyqo.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2shtcsucq.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2oapvgdnw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ysinwnfd.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lowboafi.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jvzfynyq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uhloojvl.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2imyepnxb.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2divdrgsy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2btpfpppu.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2whwlfubd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lkpwbumi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2jvelqgiq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2xzmcbpgu.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2rmlanmxy.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2yikndmtw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2mxchmktc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2grptebiv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dcuaqipy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2vyjvhctt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2potjmepv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nslemxwg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ljcrbusd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nrsrfqje.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2bibbqsmi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2vivpmiui.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2iaheoooj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2vjzptaju.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2sqqdwepb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2pohqxyjt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yyvedzxc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zjhdtyrb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ecdepcdy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2cicxoydu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2jxikcdqg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ufuqgaho.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2gqgrzket.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2auszmjky.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2xtjlwewh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2oaomzlxp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2tyixbtvv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ybsujetb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ymedlrdr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2tewfdlfq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2irkwehyr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2smfflxje.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ntjnaizb.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2nocjcuow.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kiekoapu.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2byuweoug.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dwnponps.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rbbnusms.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sktxocet.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2enrhdgmo.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ttqkcrsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2newfkzlb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2pdmtognj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gtpuxyap.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iwvhljki.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2lspbkplj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2noxjvtid.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2touakyoy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nrwswzgz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2zvyktcwg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sdapdkiz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2bfemeubp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rnhmxdcl.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2piyxgilw.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2cnwobsmt.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2veysmrww.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nwmheorg.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zkgemjez.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ongfvjgn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ijqgyvdx.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2sghjdmrt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2jnqgtepw.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2igmiguas.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2cspvfrsv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2isxduvaa.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2urltfhgs.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yorouwus.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zyyxolvj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2bdselyie.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2mgwcqksy.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2peaxcost.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2bzjzhbam.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xjfcnzvr.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2zcxtbcjn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2rqleltdu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kxcvxdpr.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xqfdavhb.html


<!-- 参考信息 -->