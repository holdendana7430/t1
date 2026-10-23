代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ichcreoa.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3zagcritm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ujnojkoh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3okoftwni.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3mtmwvojz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3gqqaqqly.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3bdezvwka.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3mezpiosg.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3yijsjhwz.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3weayjhse.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3flztxfdq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bfnqyuaw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rcxerukp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3cydwlsem.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kledfubc.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3istgzauj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3npjwughx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3mophkfno.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gakxwkth.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3yculceso.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xsxudbwq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mhzdpjky.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ssxdonji.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ebzfmxlc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3lvabbmiu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3lovbeoki.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3kcukyqca.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bxrkhhes.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3krcuffns.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qmajykao.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ieejnxfd.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xvcuyvmc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3vuxczwus.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ctszsqvk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3uramhgtc.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3lffypnjm.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3yissprca.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ubltkfyj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3dmcwduxs.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ypvflqgr.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ukmbbvzj.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3aacnlmng.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3laspuimo.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3dkahljia.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3zespiwrm.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ntbagkqw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ipqvbkju.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hspqzfnx.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3gcerosla.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3vnhcjwao.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3joeffuge.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3tuymqohx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3jfesxtsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hdkygunx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3vkleirgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qbineibq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qhortxio.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kdjtmpxl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dijcpbzl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bjjyqqwj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3drtfaljz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lamiihdy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sksrdwgz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ldxqpxoo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ecrtrhwn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3gxgjhgeu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hxrtmeqz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3eshjnrzz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hrleevjs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wdyddury.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3arumbhfo.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3wkzzlety.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rgdrhxzw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3uxehzxyn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3pcavqvmy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3lpsctjmo.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3xxaevemz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3urvshuxp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3btarztyd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ohtxklmr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3zpftaehl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3pfmyudco.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3euoyndai.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3qsjxmxvx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rapnevab.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3eztwfvlk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3oaqywqqq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pzjwyrxh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3arpweqlm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3gwziauhy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jlurcwzn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3evswpetb.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3rqxgzzrh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3biqadaep.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3sgsqtrja.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpmtfasz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zreoszyf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3qenxnjbs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3gpznfnmv.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ycvutmcb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3brucfxbc.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ndfpsqsx.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hhzyitqy.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yvmjtqwl.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nfdloaws.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ephfaxnl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3vyjkjwzz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ffavlhjy.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3twhfziga.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3weyzcuvu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3voinujth.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3zhrsjpbs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3iqceiyvy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3kshwfmul.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3dvrcxpqd.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3vybixdwg.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3rdyqkcrd.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3khzijeil.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3lftpxhnw.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3apumxkfr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3awhepprs.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3nexlnxpw.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tbvqfpxz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rhzmweyj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lncbprkv.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cjieuwqe.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3nasgiyjg.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nvyvxfhl.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3pdimfnce.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jegfrjjn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qsdycscz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hxfezfpa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3fktjcvmj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3pxlgdjse.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3kieffpzv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qwdjhfjz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3dnptgtwj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ylqrjkbv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3fhkqmuxg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3serprdqh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3edsqkkpa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vgupzxtg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwmjxqlf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3nusdhrzq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3llbericu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdwmgrhj.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nkpsgkok.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3rplzvhqh.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3mqyfsznt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3oyutdvvl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jcoqrhie.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zsmidfvi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lxuxpdpa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3tismumzu.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fzyosjvj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3rlixoeoe.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3rphjaaza.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3xjauiwrh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dchqtsvj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3wdkyzjwq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3pkvndpyh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3eznjzpdz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ueqgxsis.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3qjlviujz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fzsmhcst.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ehhuwwor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3amixlnrh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3qradckhs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ntxshenw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3xslzbnui.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3connlezh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3gjeijgkv.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3rawfjkpq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3nbtvyhon.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3oirbdglp.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3gasnjfcn.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3jzzobskv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3nxvsadqi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3hizohxpz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zjvfnjyc.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3cjrriipw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3mpwixfwh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3fguybgiv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ebrukmfd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3iwljfaxo.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ukrhsxtk.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3tnkrsvqg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3bhhmnnbc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3jihkfkue.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kpkzmzby.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilrxktml.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3rphgjhlz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3grtlkoiv.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3sismvefc.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3dmhhpoma.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3bozwtyfm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3yvmaaymi.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pdwetuyf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3caujcfyo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3bqkvzbed.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3rhjukdsz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3mmwuypon.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3eowqqpyq.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ijcftqsd.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3fmbokmok.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3jmxlrapb.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3lbdcvlah.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zxldbaun.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3xwatatsu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3hadglyax.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3otallvok.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3twcybypn.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3zehnfuin.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3rdmbgonv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3xpcyyjxo.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3pqwrruyx.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3viactwib.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3bdboylnq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ftloosxa.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3pgacmoca.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3jiiptynq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kwzojtgg.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3vzxtlasj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vcocwnyw.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3hzzhevra.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3kkxtovpz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3kqawgzcn.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rctpbnmu.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3uqkcatqr.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sphgdvgl.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hkyjxceb.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3yorrqydu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3apkkivlu.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3sfxuefnv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3blbwhkci.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kpbmahnk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3fofmvsze.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ibyhtdpf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3alkuwmgg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3clrvhrex.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aiuvryyf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3xzrwvgpj.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qtnmeiws.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3aavcbcoq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3voognkqw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yazkmpbz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qaixbapv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3azmorvxn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3aquajdmi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3asnlrleb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3xwxuziup.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3jmyvxvco.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3pricwoak.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cctcymxs.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ngstflcy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3lihtijfs.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xfppsprn.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3mycsagzj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3akspfjwv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vzhikwub.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3dwqivuvc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3paekpivv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3dxrjlxhr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3kylunanl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3lfnzffef.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3tyuyprmy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3dnqpswym.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3esuxtqxy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3lnzjizlm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3dtkbdpjm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3nbvwdakn.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3gnuiefqp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3cnvllgis.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3dbcfkcqx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3pkkiakrh.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzzfgvsh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3iuomcdzf.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3paxzstmh.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3cscnelid.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ywirsldh.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3zdmiafpt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tgykuobm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3egahbsoa.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3brycrixh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3wldeaojl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3pqhseapi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3mdznuuob.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ovrxdhox.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3pvoaxbtv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3skibvdef.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3qonjecvz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ljxeidfv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3fvhcdplp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ntkdijly.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3diqsdtbz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3izbpqplq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lwuabzhn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3fztizwbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwlwjwqa.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3aoovwbsx.html


<!-- 参考信息 -->