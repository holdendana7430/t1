代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dttwauig.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2xnbeyvra.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vnidlhgr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2woshkzrr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2wbcqiogx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2gohzwsyu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2hbottavb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2fznboxhw.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2bgodotyw.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2qavcamcz.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2vemqcbod.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vefetbkw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2lvxhtgmb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2uspybaee.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2knxcotmc.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2yhbydytr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2lmogmujj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2wiafbvki.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nspkuqxv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xyesppin.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bkshqmep.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kkcruubj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lylitlvh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mvsqygnk.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2xvbsncbv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2newmjpqg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ibatfkkx.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2cvyhevls.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ixjebadq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xrzggeqc.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qcmyeqpi.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2frjzimkh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2evxfenbe.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2rzstmzev.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wpguvxie.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2vafwwkxm.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2jewbgmsm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ovfqijzt.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2epknijww.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2kuwqyaag.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2mwqnzqfv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2tkzhdazv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2lqbawhwy.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2mynqvwkq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2flcdnjxj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2djycgnor.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2aatbgzse.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2qapctqkt.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rqwyyciv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2puzffvdd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2jtwzuaso.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2bdkyalxf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2wapopddm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gjrafxla.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ruszyqna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kljcinft.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2dbhqtzah.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bhcopear.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fmvtxltv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rjmpvinw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wfsczsir.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ejdmoael.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uueguidn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2uqqvnigd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tkbrqzgs.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ppklxzml.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pazwfqbv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2opboygwi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tdfsfimj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2raidlfqa.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2mvanceng.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qahkrcnx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2amqwehwg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2piphiqck.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2qlmbmnzp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2wbworhfo.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2wxuhryuw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rdfiojku.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rlayuang.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xtxopbne.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2fdiijgdo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2qgagexhn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2umfxtubz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2cwflrrnc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sglsdnbb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2jofpnwjr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2dorwmwly.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qumjkssc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2jjvxceuh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2uopsrojg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uiivfyix.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iaksraui.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2wztflwtb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nwwxdssk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddfklgvd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tevzgrjr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkudrwow.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2nvkmphtp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2udiibvso.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vfrneqxa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2bxheswbd.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2nnjjceqh.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rbqvxgoq.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pzqwdjnz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fflrcnej.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gukfhrek.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2zafyllxj.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2lfqzjatd.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2zfkoxtzd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2asxbeblz.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2rizzlmqb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2zbhbylit.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2nrvllrxm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2kcydywbm.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2mehwkpzz.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2cezfqunj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2tonszfze.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2zzmfsqcf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2iajyaefv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2dvthvscn.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2tchdkffl.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2layobipi.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xrsuqrlx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kjucepan.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ntqqbeyw.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2raictbxf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wjarjdlk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lojjnpdq.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2eivxsjnp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2gsckdpea.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2udrfgdwx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mumwsdji.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2yyrxxeli.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2stpbllcc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2iucgccux.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ztcjytgy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2dlrfbkda.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2pvtiqbxn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2anlpsasb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckbltfkw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2wprebmsy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2bfwytiqk.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksurpolm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2bvjiajkv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2yxvopqhf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2gujllolf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yklxewqc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ebwyprun.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2tpswtfzz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ixewylst.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xsqaozma.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pfmdcuvi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2uzaomoiz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2comakqmw.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2roigfbex.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2txvzvwby.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2nzhuguwg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2jlhrvmbq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2sbshhnbp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ifmrbjax.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2uhqkrpiq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2mjphqjng.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2axvicute.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2qfhgstwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gblvghjr.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2rdokkpgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pandnwgm.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2lqbhbvzc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2bgzvtnhf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2xsfikhaa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2nepemsho.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qzjosmut.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2uerrdqim.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2mrejalii.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2neqabxuv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2frutecax.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2urhswuof.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2hwmloewj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ofgrlqjz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2liimiaob.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mldrvmut.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2qsiofffc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2kmwdtmty.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ylsyykxv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2bskovhbr.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2etkbhcuj.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2qemtubsq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2umgvcnci.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2chifbhjs.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rekewfak.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2lkugawat.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2psrfatsv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2koyjrads.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqsemvee.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2canjdsot.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2amcwndiu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2kbxafyeu.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dydjohyq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2swuordhe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2zqqjsffl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2sliuqclz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2njfxqryo.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2srbdabpl.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2vpehrfwa.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2xevpsrol.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2azivxdba.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2prksyswu.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tmnimtuz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ucdwyavz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2mhphkobb.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2hnktsjeb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2cfrphmmn.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2usekzkxl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2tdalnofy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2uzvjozej.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ovqdjbsy.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rhvaveky.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2qqwlzegm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2wqdoszsv.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ofgcgmjd.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2eejmaxro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rswisdmx.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2pvhezsbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ldkmnbeo.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2yfktcbff.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2rabubfnv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2wxjvqbqb.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2gwfvypoy.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2qxxfmrkd.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nvgazuuq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nufemjtf.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2gfwgmwka.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ylfvohcs.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2ybggkldm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ecjzljtf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ozhvocur.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2rpywwpbc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2zthbzbsx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zpfywbum.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2fbgvjbyl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2hpcxaqbt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2kczcgyeb.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2upuebibf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2djsuxshr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2tntiyijv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2xjgvsobk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ovlmdabx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2cecmuznr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2zsaokoqc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2qgfeupvx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ubcfvyxg.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2qhfeogek.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2dscwpgrs.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lhzerova.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2qngetgsk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ygsujlol.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2gavrmuku.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2hzdalxni.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ggibcjsw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2mkvfdyjk.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2hpqjpvbx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2jwqfirtc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2wvgaxbmq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2beuugqua.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bshamkeg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2heevhkur.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cpxbffvg.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2lujiymdm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2oytvactm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2killhavm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2znjqdedi.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uabjzmzz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2nyfjfslk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2dsepuytv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2boyprajv.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2lawszizt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2tpbvqvdy.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2xjhzdagw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2vytzlrvw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2mnulxail.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2lcnsyknp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2iupeypmg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2imndietf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zmdnrmkj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2apwvshxl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hiwquozs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2imptcjdy.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2cgsfgazt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2aexnckvd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zmcbjigk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2fydrfnol.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2begghrme.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2lxxqjhlw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2cujricst.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2extqkvnb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2vnbnhgtc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otoijqfh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2nsdubsyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lbwdyfwr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2irtwhuow.html


<!-- 参考信息 -->