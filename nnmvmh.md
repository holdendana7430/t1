代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yanxiufei.cn/gtccmlpwsp.html

[R52] 统计行数
来源：http://hz.gzhubu.top/gtkaozwjoq.html

wc -l a.txt
来源：http://hz.havefunace.top/gtbnstzbvt.html

[R53] 查看文件头与实时尾
来源：http://hz.9152youxi.cn/gtqpclznvj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.sweek.top/gtukcrwpfr.html

[R54] 比较两个文件
来源：http://hz.gzhubu.top/gtxppfdlsy.html

diff a.txt b.txt
来源：http://hz.snrcjt.cn/gtovtnakcx.html

[R55] 压缩与解压
来源：http://hz.smart0.xyz/gtytjdcnvi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cqqwz.cn/gtckwxhoga.html

[R56] 远程拷贝
来源：http://hz.iojbl.cn/gtalthjzoe.html

scp file user@host:/path/
来源：http://hz.sweek.top/gtzxftfkcu.html

[R57] 远程执行命令
来源：http://hz.tian-w.cn/gtmkglixyr.html

ssh user@host 'uptime'
来源：http://hz.mhx1999.top/gtrsdwmqcr.html

[R58] 下载文件
来源：http://hz.xylfe.cn/gtjpahauxb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.nanxinkj.top/gtqkxjpdgi.html

[R59] 发 POST JSON
来源：http://hz.hysaishi.cn/gtkrashjgf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhengqikj.top/gtmrgrgivw.html

[R60] 只看 HTTP 状态码
来源：http://hz.dashuyun.cn/gtfmhvkblm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jinqigfzy.top/gtqmpfnvst.html

[R61] 磁盘占用
来源：http://hz.shanyushiyangtech.top/gtchmkyugw.html

df -h;  du -sh *
来源：http://hz.sxryk.cn/gtgyqeixjt.html

[R62] 找最占空间的文件
来源：http://hz.jinghuilouyu.cn/gtqxrpcydu.html

du -ah . | sort -rh | head -10
来源：http://hz.gaohongyu789.top/gtxfnahhys.html

[R63] 内存与进程
来源：http://hz.yanxiufei.cn/gtfnwqplka.html

free -h;  ps aux | grep nginx
来源：http://hz.wangshuangyany.cn/gtvzogjrhf.html

[R64] 结束进程
来源：http://hz.xziqi.cn/gtjdtrgtym.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shzxlz.cn/gtdelirxam.html

[R65] 查看端口占用
来源：http://hz.tianlin.xyz/gtlnemtvus.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jlsjyb.cn/gtgpeccbbj.html

[R66] 定时任务
来源：http://hz.0kj1m.cn/gtuopbjqoc.html

crontab -e;  crontab -l
来源：http://hz.havefunace.top/gtxisjowyu.html

[R67] 生成随机十六进制串
来源：http://hz.hongshengwenyu.top/gtqncjfkvt.html

openssl rand -hex 16
来源：http://hz.dashuyun.cn/gtnkpkghyr.html

[R68] 计算文件校验值
来源：http://hz.shzxlz.cn/gtztxbepel.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.smart0.xyz/gtxgpdmflx.html

[R69] 生成随机密码
来源：http://hz.ybcxt.top/gtwhigaqyi.html

head -c 16 /dev/urandom | base64
来源：http://hz.shangyingyoupin.top/gtuclbmouq.html

[R70] 时间戳与互转
来源：http://hz.ppjwa.cn/gtrmclpofj.html

date +%s;  date -d @1700000000
来源：http://hz.hnxiangtu.top/gtjiomjaav.html

[R71] 日期格式化
来源：http://hz.jinqigfzy.top/gtmribkrpp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yueranfly.top/gtnypokoda.html

[R72] 等待端口就绪
来源：http://hz.haohaochexian.top/gtkfkyyfkb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hfpthk.cn/gtlopcakmn.html

[R73] 分割大日志
来源：http://hz.xuetiantiany.cn/gtesiurzcf.html

split -l 1000 big.log part_
来源：http://hz.havefunace.top/gtaunqjdko.html

[R74] 批量重命名
来源：http://hz.xuanzx.com/gtvbjdjlao.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.sxryk.cn/gtieoyoipi.html

[R75] 导出环境变量
来源：http://hz.gzhubu.top/gtlocrfwed.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.haohaochexian.top/gtjbhponpn.html

[R76] 使用临时文件
来源：http://hz.hfpthk.cn/gtehfzzyhb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhiwuduotai.top/gtjeubnvmq.html

[R77] 读取用户输入
来源：http://hz.52xcode.cn/gtrwteznpn.html

read -rp "请输入: " ans
来源：http://hz.hfpthk.cn/gtlmspudfe.html

[R78] 交互式菜单
来源：http://hz.hnqzz.top/gtedrugcon.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ydjk.org.cn/gtawxcmzkj.html

[R79] 解析命令行选项
来源：http://hz.shuidangran.top/gtvkyoiswc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.redwolf501.top/gtnrxtygzt.html

[R80] 查看脚本执行耗时
来源：http://hz.shuidangran.top/gtdzxxugoe.html

time ./run.sh
来源：http://hz.sysykeji.top/gtnwdviswx.html

================================================================================
来源：http://hz.guannengcc.top/gtebxarlay.html

S. C / C++ 专题
来源：http://hz.chenzaomai.com/gtfnbtvefc.html

================================================================================
来源：http://hz.yuanzhike.top/gtizsyezkc.html

[S01] C：Hello World
来源：http://hz.cdnleiting.top/gtirsvzgox.html

#include <stdio.h>
来源：http://hz.0kj1m.cn/gtdpvcynjf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.daria6918.cn/gtktahpfrz.html

[S02] C：变量与格式化输出
来源：http://hz.pycfn.com/gtenbklepn.html

int a = 10; printf("%d\n", a);
来源：http://hz.ydjk.org.cn/gtvqvwhexw.html

[S03] C：读入整数
来源：http://hz.c1oappe.top/gthqeqsqzv.html

int x; scanf("%d", &x);
来源：http://hz.wangshuangyany.cn/gtqptpibjx.html

[S04] C：字符串复制
来源：http://hz.chenzaomai.com/gtlrchvmym.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yongpay.top/gtvbdnhglm.html

[S05] C：字符串长度
来源：http://hz.jqgufenzy.top/gtxmipuzib.html

strlen(s)
来源：http://hz.gotoacloud.top/gtolvozqls.html

[S06] C：字符串比较
来源：http://hz.shzxlz.cn/gtlqautgsd.html

strcmp(a, b) == 0
来源：http://hz.tanke756.top/gtejnlyxug.html

[S07] C：数组遍历求和
来源：http://hz.andypj.xyz/gtoxfdivkb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.quarkkingdee.top/gtdbqnuzlz.html

[S08] C：动态内存分配与释放
来源：http://hz.shzxlz.cn/gtiweugvpv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.snrcjt.cn/gtitlajunp.html

[S09] C：结构体定义与初始化
来源：http://hz.jinqigufen.top/gtkutwsqwn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.redwolf501.top/gtjmtrdxkz.html

[S10] C：指针与解引用
来源：http://hz.ydjk.org.cn/gtpuuwypyt.html

int *p = &a;  *p = 5;
来源：http://hz.shangyingyoupin.top/gtdmuucawr.html

[S11] C：逐行读文件
来源：http://hz.cashguo.top/gtpoytsevi.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hongshengwenyu.top/gtncfaypeo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.andypj.xyz/gtwdrjmadm.html

fclose(f);
来源：http://hz.ydjk.org.cn/gtlhfdifbw.html

[S12] C：写文件
来源：http://hz.gaohongyu789.top/gtxyajnvhv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.chenjidiqi.icu/gttmdxlzaw.html

[S13] C：宏定义
来源：http://hz.shuidangran.top/gthkwbdzqb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhoulong.xyz/gtdmlyegii.html

[S14] C：枚举
来源：http://hz.dashuyun.cn/gtdudwfqhv.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.gogol.net.cn/gtelyszyfy.html

[S15] C：类型转换
来源：http://hz.zhoulong.xyz/gtbevxxrpr.html

(double) a / b
来源：http://hz.sufxvd.cn/gtpserufiy.html

[S16] C：位操作置位
来源：http://hz.shangyingyoupin.top/gtyvzferuk.html

x |= (1 << 3);
来源：http://hz.sysykeji.top/gtuturzqct.html

[S17] C：安全拼接字符串
来源：http://hz.9152youxi.cn/gtzeqcimyi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sxryk.cn/gtulufiqzf.html

[S18] C：命令行参数
来源：http://hz.dianchejie.cn/gthtedaldx.html

int main(int argc, char **argv)
来源：http://hz.yj20258.top/gtupddujns.html

[S19] C：快速排序
来源：http://hz.yanxiufei.cn/gtyhfiukai.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yj202588.top/gtnylzexon.html

[S20] C：二分查找
来源：http://hz.jinqigfzy.top/gtwntylniz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yonumen.top/gtlpiqxett.html

[S21] C：字符类别判断
来源：http://hz.cheryme.top/gtuopabvbc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.gogol.net.cn/gtorhqeotd.html

[S22] C：字符串转数字
来源：http://hz.yj202588.top/gtvudpannf.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.daxiang520.top/gtbiyrcmuj.html

[S23] C：随机数
来源：http://hz.havefunace.top/gtjacmkfqw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hnxiangtu.top/gtvedyjjvw.html

[S24] C：获取本地时间
来源：http://hz.zycfv.cn/gtyuywcndc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cqqwz.cn/gtyoskjgzh.html

[S25] C：内存拷贝
来源：http://hz.daria6918.cn/gtxjkxmblf.html

memcpy(dst, src, n);
来源：http://hz.ehwqpu.com/gtvbnaowcn.html

[S26] C：内存清零
来源：http://hz.cheryme.top/gtgchvnvzi.html

memset(a, 0, sizeof a);
来源：http://hz.vqdsnc.cn/gtkzkmulhz.html

[S27] C：定义常量
来源：http://hz.andypj.xyz/gtuwytfzas.html

const double PI = 3.14159;
来源：http://hz.xingfuxueyuan.xyz/gtqtsfgfll.html

[S28] C：静态变量
来源：http://hz.gogol.net.cn/gtndwffsvd.html

static int counter = 0;
来源：http://hz.dashuyun.cn/gtfbfgfnmr.html

[S29] C：变参函数
来源：http://hz.shzxlz.cn/gthwbtdwbx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zycfv.cn/gtipcabptx.html

[S30] C：头文件保护
来源：http://hz.jinqigfzy.top/gtxpjcpyjk.html

#ifndef X_H
来源：http://hz.nanxuanxn.top/gtlazcbzzf.html

#define X_H
来源：http://hz.ybcxt.top/gtfzpfnqhb.html

#endif
来源：http://hz.9152youxi.cn/gtxrlmcviv.html

[S31] C++：Hello World
来源：http://hz.cucudq.cn/gtmopoqbmu.html

#include <iostream>
来源：http://hz.ydjk.org.cn/gtuyeuybje.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.daria6918.cn/gtxxvlnzsf.html

[S32] C++：字符串
来源：http://hz.shangyingyoupin.top/gtoxrbpkve.html

std::string s = "hi";  s += "!";
来源：http://hz.xuanzx.com/gtpqokrhtf.html

[S33] C++：vector 增删
来源：http://hz.tianlin.xyz/gtveeplbtl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yueranfly.top/gtmldjupto.html

[S34] C++：遍历 vector
来源：http://hz.jiagoushi.top/gtapioxtdr.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.52xcode.cn/gtomwvgtql.html

[S35] C++：map
来源：http://hz.cqqwz.cn/gthvnapmfl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yanxiufei.cn/gtpisohfdr.html

[S36] C++：unordered_map
来源：http://hz.hnqzz.top/gtjlgwzops.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinyuanbaomall.cn/gtrjnhdmdd.html

[S37] C++：set
来源：http://hz.vqdsnc.cn/gtlfhmpqzi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.sufxvd.cn/gtiznpcbrf.html

[S38] C++：排序
来源：http://hz.jianghu66.top/gticexsheg.html

std::sort(v.begin(), v.end());
来源：http://hz.dashuyun.cn/gtftwsjlya.html

[S39] C++：自定义比较器排序
来源：http://hz.shanyushiyangtech.top/gtmaqzvcee.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jqgfzy.top/gtsntvjcny.html

[S40] C++：查找元素
来源：http://hz.mhx1999.top/gtadeawlbg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yj202588.top/gtafacmbkz.html

[S41] C++：类与构造函数
来源：http://hz.aibaodan.cn/gtpyeekeiz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.fzhhl.top/gtvlomfsnt.html

[S42] C++：继承与虚函数
来源：http://hz.fengsongda.top/gtzbesejtl.html

class B : public Base { public: void f() override {} };
来源：http://hz.fengsongda.top/gtcmssmnhy.html

[S43] C++：智能指针
来源：http://hz.zhongyouzk.top/gtluxannfr.html

auto p = std::make_unique<int>(5);
来源：http://hz.zycfv.cn/gtnspteyyp.html

[S44] C++：引用传参
来源：http://hz.xingfuxueyuan.xyz/gtmjzfhqxs.html

void inc(int &x) { ++x; }
来源：http://hz.ywan-chungtsiang.top/gtwwclbgrc.html

[S45] C++：lambda
来源：http://hz.wangshuangyany.cn/gtzmhdrrre.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.guannengcc.top/gtxwxzxdaa.html

[S46] C++：函数模板
来源：http://hz.cashguo.top/gtcdduizhj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.guannengcc.top/gtjebkkmjx.html

[S47] C++：结构化绑定遍历
来源：http://hz.cdnleiting.top/gtpwdkcpaz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.svipenyu.cn/gthhocowca.html

[S48] C++：逐行读文件
来源：http://hz.redwolf501.top/gtrtsfjwng.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.snrcjt.cn/gtgdulygkv.html

while (std::getline(in, line)) { }
来源：http://hz.zhengqikj.top/gtihpgmjry.html

[S49] C++：写文件
来源：http://hz.nwbrower.top/gtcmdlzqqh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.tian-w.cn/gthervxhir.html

[S50] C++：格式化数字
来源：http://hz.dashuyun.cn/gthtajutyk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.tanke756.top/gtfyanfaxm.html

[S51] C++：显式类型转换
来源：http://hz.zdqjudy.top/gttxxdlell.html

static_cast<double>(a) / b
来源：http://hz.yueranfly.top/gtbaudbizz.html

[S52] C++：const 与 noexcept
来源：http://hz.chenzaomai.com/gtgmqecjbx.html

int size() const noexcept { return n_; }
来源：http://hz.yanxiufei.cn/gtrlbricwo.html

[S53] C++：移动语义
来源：http://hz.fengsongda.top/gtxconpgkn.html

std::vector<int> w = std::move(v);
来源：http://hz.gaohongyu789.top/gtviudqztp.html

[S54] C++：异常处理
来源：http://hz.hnxiangtu.top/gtprggmxfg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.birdmap.top/gtwkgqssxs.html

[S55] C++：结构化绑定
来源：http://hz.jlsjyb.cn/gtwaxcqxkp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.svipenyu.cn/gtazuzskud.html

[S56] C++：optional
来源：http://hz.xziqi.cn/gtpqjhlimk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.tian-w.cn/gtklbmkevn.html

[S57] C++：编译期常量
来源：http://hz.jinyuanbaomall.cn/gtyoaxqnke.html

constexpr int N = 10;
来源：http://hz.svipenyu.cn/gtjxedsgcg.html

[S58] C++：命名空间
来源：http://hz.shuidangran.top/gteacpgbsq.html

namespace ns { int f() { return 1; } }
来源：http://hz.aibaodan.cn/gtnlisbggt.html

[S59] C++：静态断言
来源：http://hz.zhixingplan.top/gtlypileyd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.chenlongwang.top/gtfgsgfsth.html

[S60] C++：遍历并删除元素
来源：http://hz.sweek.top/gthjxoxkna.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ydjk.org.cn/gtobipjgwc.html

================================================================================
来源：http://hz.tanke756.top/gtxrbvcpfh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xziqi.cn/gtspuuepej.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtdrzukjxe.html

[T01] Kotlin：Hello World
来源：http://hz.pengpengdd.cyou/gtqezazsum.html

println("Hello")
来源：http://hz.zhijiandao.cn/gtgsrfmfly.html

[T02] Kotlin：变量
来源：http://hz.svipenyu.cn/gtsnnxbqdz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhaomingkeji.xyz/gtjvdogiqo.html

[T03] Kotlin：字符串模板
来源：http://hz.xziqi.cn/gtmshrwozf.html

"值: $b"
来源：http://hz.yj202588.top/gtdzzsghqw.html

[T04] Kotlin：空安全
来源：http://hz.sweek.top/gtgubbvgog.html

val n: String? = null;  n?.length
来源：http://hz.birdmap.top/gtpdebfrjz.html

[T05] Kotlin：when 表达式
来源：http://hz.yuxming.cn/gtbczksqen.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ydjk.org.cn/gtnjhzkwhs.html

[T06] Kotlin：集合映射
来源：http://hz.gzhubu.top/gtgzkaafaa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.52xcode.cn/gtqkklrlfm.html

[T07] Kotlin：集合过滤
来源：http://hz.yongpay.top/gtnchqqfxi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xziqi.cn/gtsjdothkn.html

[T08] Kotlin：数据类
来源：http://hz.xuanzx.com/gtuksoangv.html

data class User(val name: String, val age: Int)
来源：http://hz.0kj1m.cn/gtarzrpghc.html

[T09] Kotlin：扩展函数
来源：http://hz.tanke756.top/gtxqwjcnqb.html

fun String.exclaim() = this + "!"
来源：http://hz.yonumen.top/gtshausnrb.html

[T10] Kotlin：默认参数
来源：http://hz.snrcjt.cn/gtedmrqjfh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.c1oappe.top/gtmdititpp.html

[T11] Kotlin：协程
来源：http://hz.sufxvd.cn/gtjofduzuu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yonumen.top/gtzuvqgoyg.html

[T12] Kotlin：解构声明
来源：http://hz.ybcxt.top/gtaiyocnup.html

val (a, b) = Pair(1, 2)
来源：http://hz.yueranfly.top/gtgrmqkxks.html

[T13] Kotlin：只读 Map
来源：http://hz.xuetiantiany.cn/gtugrnlyxv.html

val m = mapOf("a" to 1)
来源：http://hz.daxiang520.top/gtwlckglgs.html

[T14] Kotlin：循环
来源：http://hz.dashuyun.cn/gtpdhakrdn.html

for (i in 1..10) println(i)
来源：http://hz.tianlin.xyz/gtkvllhlrm.html

[T15] Kotlin：接口
来源：http://hz.meibo888.top/gtmpfczsva.html

interface Shape { fun area(): Double }
来源：http://hz.svipenyu.cn/gturfuizdg.html

[T16] Swift：Hello World
来源：http://hz.shuidangran.top/gtnizybqrm.html

print("Hello")
来源：http://hz.jiagoushi.top/gtknlyjzfm.html

[T17] Swift：变量与常量
来源：http://hz.zhaomingkeji.xyz/gtazpbmbvj.html

var a = 1;  let b = 2
来源：http://hz.sxryk.cn/gtxsjuqqhn.html

[T18] Swift：字符串插值
来源：http://hz.shzxlz.cn/gtzmdhrdai.html

"值: \(b)"
来源：http://hz.daria6918.cn/gtubfpulsy.html

[T19] Swift：可选绑定
来源：http://hz.nwbrower.top/gtozorcwtr.html

if let n = opt { print(n) }
来源：http://hz.aizwys.cn/gtpgxfylel.html

[T20] Swift：数组操作
来源：http://hz.jinyuanbaomall.cn/gtindsvxyj.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.pengpengdd.cyou/gtonjwkivn.html

[T21] Swift：遍历
来源：http://hz.316326.xyz/gtvnzehkht.html

for x in a { print(x) }
来源：http://hz.jyoumei.cn/gtsswhertl.html

[T22] Swift：字典
来源：http://hz.cheryme.top/gtpsmmliwb.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.guowangkeji.top/gtahuozpyv.html

[T23] Swift：函数
来源：http://hz.yuxming.cn/gtzqfcthpp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.guowangkeji.top/gtqvrryfab.html

[T24] Swift：闭包
来源：http://hz.ydjk.org.cn/gtynggyqer.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.quarkkingdee.top/gthcmjjlgl.html

[T25] Swift：结构体
来源：http://hz.aizwys.cn/gtjikvrarr.html

struct P { var x: Int }
来源：http://hz.sufxvd.cn/gttvwbnqxo.html

[T26] Swift：类与重写
来源：http://hz.daria6918.cn/gtwwvubtec.html

class A: Base { override func f() {} }
来源：http://hz.ydzc1.top/gtkyndtplt.html

[T27] Swift：错误处理
来源：http://hz.hysaishi.cn/gturdutrap.html

do { try f() } catch { print(error) }
来源：http://hz.xuanzx.com/gtzcvtjdvf.html

[T28] Swift：枚举
来源：http://hz.dashuyun.cn/gtkkonbqou.html

enum Color { case red, green }
来源：http://hz.zhongyouzk.top/gthnlsugke.html

[T29] Swift：guard 提前返回
来源：http://hz.tanke756.top/gtkpaxrtit.html

guard let x = opt else { return }
来源：http://hz.xuetiantiany.cn/gtubhbjest.html

[T30] Swift：协议
来源：http://hz.yongpay.top/gtxvyqfsjj.html

protocol Shape { func area() -> Double }
来源：http://hz.yj202588.top/gtravgjour.html

[T31] Lua：Hello World
来源：http://hz.yj20258888.top/gtrytxvoxg.html

print("Hello")
来源：http://hz.gogol.net.cn/gtgpegudkc.html

[T32] Lua：局部变量
来源：http://hz.nwbrower.top/gtkrgnoznv.html

local a = 1
来源：http://hz.pengpengdd.cyou/gtldraisac.html

[T33] Lua：表（数组）
来源：http://hz.hywenlv.cn/gtmgcjggfz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.gzhubu.top/gtioimvwrl.html

[T34] Lua：遍历表
来源：http://hz.sweek.top/gtmkgqedcq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.havefunace.top/gtdvhxaypy.html

[T35] Lua：字典表
来源：http://hz.meibo888.top/gtkgzsvrtf.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xingfuxueyuan.xyz/gtkbqjdxdk.html

[T36] Lua：函数
来源：http://hz.yj20258.top/gtqepfxmlg.html

function add(a, b) return a + b end
来源：http://hz.chenlongwang.top/gtejufurbk.html

[T37] Lua：字符串拼接
来源：http://hz.tanke756.top/gtzgmgqslj.html

"a" .. "b"
来源：http://hz.pengpengdd.cyou/gtinydrlnj.html

[T38] Lua：条件
来源：http://hz.yvedp.cn/gtcehwfmlo.html

if x > 0 then print("正") end
来源：http://hz.jinqigufen.top/gtkhibmqqh.html

[T39] Lua：模式匹配
来源：http://hz.xylfe.cn/gtkdkzoygv.html

string.find(s, "%d+")
来源：http://hz.andypj.xyz/gtvmhrnmqp.html

[T40] Lua：元表
来源：http://hz.yonumen.top/gttwzxezde.html

setmetatable({}, { __index = base })
来源：http://hz.jqgufenzy.top/gtuqhmnuns.html

[T41] Perl：Hello World
来源：http://hz.mhx1999.top/gtlmjvtuus.html

print "Hello\n";
来源：http://hz.zdqjudy.top/gtmkrgbtji.html

[T42] Perl：变量类型
来源：http://hz.gzhubu.top/gtdnfibbjj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jlsjyb.cn/gtlzrdrspd.html

[T43] Perl：字符串插值
来源：http://hz.svipenyu.cn/gtzekjnwxs.html

"值: $a"
来源：http://hz.yj20258888.top/gtnzzabywc.html

[T44] Perl：条件
来源：http://hz.havefunace.top/gtjkidwfxj.html

if ($a > 0) { print "正"; }
来源：http://hz.yj20258.top/gtsweyzfsm.html

[T45] Perl：数组遍历
来源：http://hz.kuanghao11.cn/gtlkvxttet.html

for my $x (@arr) { print $x; }
来源：http://hz.jinyuanbaomall.cn/gtotuwiovr.html

[T46] Perl：哈希操作
来源：http://hz.yonumen.top/gtzlfrqfwe.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.snrcjt.cn/gtfuqokuzv.html

[T47] Perl：正则捕获
来源：http://hz.jiagoushi.top/gtsbgjujyk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zdqjudy.top/gthncnxiat.html

[T48] Perl：正则替换
来源：http://hz.dashuyun.cn/gtwiallrwb.html

$s =~ s/old/new/g;
来源：http://hz.nanxuanxn.top/gtenhatcfb.html

[T49] Perl：函数
来源：http://hz.haohaochexian.top/gtfliezrdu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.guannengcc.top/gtnmwrqpin.html

[T50] Perl：逐行读文件
来源：http://hz.nanxinkj.top/gtyusikfzg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.shanyushiyangkeji.top/gttigelzuo.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yuanzhike.top/gtjdadnhyo.html

[T51] Scala：Hello World
来源：http://hz.pengpengdd.cyou/gteatafpse.html

println("Hello")
来源：http://hz.yuanzhike.top/gtqnqwxbpe.html

[T52] Scala：变量
来源：http://hz.fzhhl.top/gtumbjmlek.html

val a = 1;  var b = 2
来源：http://hz.shuidangran.top/gtnltrigca.html

[T53] Scala：字符串插值
来源：http://hz.redwolf501.top/gtroigcsbo.html

s"值: $b"
来源：http://hz.gzhubu.top/gthzpscnun.html

[T54] Scala：集合映射
来源：http://hz.xuetiantiany.cn/gtygakpxjq.html


<!-- 参考信息 -->