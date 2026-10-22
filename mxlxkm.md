代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2zqszmqzy.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2eihytlew.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2pitqtvaf.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2xidjwyak.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2xzwktsxx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pswxcceb.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2idmulxku.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2fqkuuxln.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2pgyqhcar.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2qrxvsxym.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2tgoonsad.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ytnrlucj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2txfrenug.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vwzfndku.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ilbdupjm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxdviexc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aczjgdwr.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2anmldkuu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2kiozcobv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2zmumxwrs.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2lwuywdjb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ftmqxhxk.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hxclktvl.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2byrhpdka.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2anxrkfrv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2wgckihxk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2tbvvhcfm.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mvzddgpo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2fvzgfazo.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2vxpnaaml.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2dwkbyolm.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2cfxfkkaz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ghvflxdy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2jhdxiafe.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hprkssug.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ihjcdjgx.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2xrhcgkyc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ttmncrar.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2dhoxfjhv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2cvdyxtsw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2jzqgilku.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2pqdgyftt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2agjuqpdi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2vlfecbej.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ftyanets.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2vquyyrch.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2zsjoruie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iqcnsdkx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2gjyiwoaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bxqdwmxw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tjzzgkcp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2schbrsya.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2icxcugcz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2uohofhxm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2owainndz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2qgvkjrcj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2lxhvuusm.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2darqbvqo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2dsvqxwun.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2yiffiufy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2teruekmv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2hvkuponm.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jxkuqdpx.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gwymqtvd.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2njzyzame.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2uiuxvkpn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2vxkqooqb.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ggnootqy.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2jsyjutio.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2uzaezwuc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2capuamfc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2dotwnarc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sdwybgmd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nbbaxxjp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2gzqpiplz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2pzmmmwao.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ggfnhtxh.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2hjlnlfly.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2isvqjbah.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2xxtsliey.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2tlhduscd.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mfdbzocc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2qdvhfhif.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2eemrwnhw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jsmzncwu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2jhqrloyc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2arkktsnt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rbevfjwd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2yvckuxig.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zypazbqi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2qnubafpi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2vaoqmdnt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nkwcqwiw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fubljcuh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bkwkwoie.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2fhbhtkhq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2erssxvux.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2eiutetca.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2sxwczkrs.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ghcknmyg.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2mhuzlkgq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jvewegch.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2vkzfmtxs.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2mofolkry.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2bjwhifqj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2abopatdt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2htjfitlb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ckclilvj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mdlgoibp.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lbzxiecx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2wndqhfmu.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ycydmmcq.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2yoduvmjr.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2lnyqkyfn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2zktymicg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2owfrijah.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2sgsclono.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2bclupztq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2nakhgqvc.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2tqfyxzfs.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fzgerjcm.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kiuxpzmh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2oeqwsaky.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2qvdfobjz.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2wfrgyrkb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2vehedqsu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2suhnzdqj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2qwnoqhne.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2otwymiqe.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hjfbkpwa.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2oudpnlne.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2hsbibqbn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2rlpovqcj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2enkkjoxb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2cyhsluwo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uyeynqju.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2zsqavohd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2epdpfizf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2xrddvsmv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2gaydaphf.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2vddpjces.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2sxdedxnq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qakjprqi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2bpnrsogl.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ciwpnfos.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2wfhbcxmm.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2gwhlcifn.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2gkirhkmb.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2efajjoku.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2kkauauuw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2beowpsvp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rlxdrzwa.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wnyokdwn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2otfqlssx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2khatzfqo.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ezpuoysm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jqzdcrqe.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2rgcwpmvs.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2wqovzpnj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fcvueycq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2obmphnlb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2kvcuzqtv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ctridfoi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2irburhxv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2zxohhmfc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2bbsclgvq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ebytajbc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2hwcauyom.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2imknwjpa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2xdaspgol.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2deijeopc.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lnprhsjk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2huhvacmo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2yutmlhlc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ggezqpoc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jxqozlvy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2zgtntgom.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ctkxkwdu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pomzpbtu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2udzxpmid.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wbtsmzdz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2bicmznwg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2unpsfspv.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ubykbwil.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2zufgyydn.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2mvbhpoyc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jxjullhf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gjbikdvn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2imysewwq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oqkxddnj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2rgbbfnqs.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2mcgrcvcr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xrbrgrsd.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2dzgmhzqq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2frvradma.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2zfsjyzwg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2neywhtam.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2bqljpeib.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2vusornwj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2jxdicwjr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qoxedjkm.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2dfbrfrly.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2hwcgnrkw.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2qlygwdkl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2pxngaxac.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2bsvroojf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2rbqyfxkb.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2iqtupfro.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rcoybkkm.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2hjwtckos.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2vyeclfwq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xwwwumjo.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2omsxvcvu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2lkvtjxuf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2gvjdviqg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2pwqcalvy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2gmvplydr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2mmzfmenb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2mwlolbvk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2hdcarzdw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2gehjxgbt.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2fglwyiql.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2anikhfhe.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2sgxtmnyt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2hrwitrsp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zlyozinb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2hjranrql.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2dxantauw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2vustqicw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2rtcoqcvc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ixggztte.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2qboiuucn.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qagsrhzu.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nfykzrpf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ryqprwzc.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2izmwyjwc.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vnhymiiw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hncwrzsf.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gxqhywch.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2efmehdgf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wlwgcjuk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2wnxzuhkp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2xandnbox.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2xyqdzdna.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2dctmqzfx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2siayfuev.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2emuejmdc.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2gvdckoll.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2evnuvbsb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pqfczbsx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2wzuxvxoi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bmrsuclf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wtwnhcbj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2webduxzz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cqvazddz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2nhxotejz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2kdmqcdzh.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ifzixlgf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wuyueutk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dxsqqogf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vhdzfyew.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jaofqndi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2wxzvotet.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2uushjeru.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2fxvlqrns.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ajbppotd.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2hrdrtvsc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2uwrqxsok.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2fznzfjmm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2sdfebjwa.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2rnbbbpzi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2inbnyehq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2dhnvjgza.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cotjrlxo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2uwceqmmh.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2howwqtyc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wtqamxmp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2unlsktfn.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2exnjfoqe.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fbqrycwp.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2lkuwrmcy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2klkksgcq.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xhzbdura.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vvinbsua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2umzpfuhn.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2havmigww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqllkpdb.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hznioifn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2raiiahzf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mfrtxqzq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sskzxaei.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2injebznw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2bqlouuzx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2dhwjjxnz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2vgbbsivz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zpzjmmmx.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ioytezlb.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ezxtkphi.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fpcxzpta.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ixmqdodl.html


<!-- 参考信息 -->