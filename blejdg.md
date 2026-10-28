代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hfpthk.cn/gtjsetifrk.html

[R50] awk 求和
来源：http://hz.vqdsnc.cn/gtcyitvwfb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.gzhubu.top/gtiwfwtaaj.html

[R51] 排序去重取前几
来源：http://hz.yonumen.top/gtanzbvfhz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gzhubu.top/gtvdeaphww.html

[R52] 统计行数
来源：http://hz.ybcxt.top/gtqveihuqt.html

wc -l a.txt
来源：http://hz.havefunace.top/gtroltepnn.html

[R53] 查看文件头与实时尾
来源：http://hz.iojbl.cn/gtuzfbvdcf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.daria6918.cn/gtmxwsqhsj.html

[R54] 比较两个文件
来源：http://hz.shanyushiyangtech.top/gtyxqvtajz.html

diff a.txt b.txt
来源：http://hz.aibaodan.cn/gtgtkicvaq.html

[R55] 压缩与解压
来源：http://hz.shzxlz.cn/gtstxhaabk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.andypj.xyz/gtlnvvozda.html

[R56] 远程拷贝
来源：http://hz.nanxuanxn.top/gtejgacxdd.html

scp file user@host:/path/
来源：http://hz.daxiang520.top/gtplkkqnzy.html

[R57] 远程执行命令
来源：http://hz.jlsjyb.cn/gtbqwuiwtb.html

ssh user@host 'uptime'
来源：http://hz.jyoumei.cn/gthtrrzfus.html

[R58] 下载文件
来源：http://hz.kuanghao11.cn/gtmyvyepik.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinyuanbaomall.cn/gtmopmamon.html

[R59] 发 POST JSON
来源：http://hz.shangyingyoupin.top/gtbyipcxlo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinqigufen.top/gtfuyfyugi.html

[R60] 只看 HTTP 状态码
来源：http://hz.hywenlv.cn/gtuaimsxun.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhiwuduotai.top/gtlwgcglsk.html

[R61] 磁盘占用
来源：http://hz.xuanzx.com/gtgfyxakqc.html

df -h;  du -sh *
来源：http://hz.yuxming.cn/gteoiwmvku.html

[R62] 找最占空间的文件
来源：http://hz.hywenlv.cn/gtitmcmanv.html

du -ah . | sort -rh | head -10
来源：http://hz.zhengqikj.top/gtvvrsqces.html

[R63] 内存与进程
来源：http://hz.chenlongwang.top/gtawuaobey.html

free -h;  ps aux | grep nginx
来源：http://hz.sweek.top/gthrdnyzdy.html

[R64] 结束进程
来源：http://hz.daxiang520.top/gtflmrgjez.html

kill -9 $(pgrep -f app.py)
来源：http://hz.daxiang520.top/gteaqizufy.html

[R65] 查看端口占用
来源：http://hz.cucudq.cn/gtbxpihavt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.pengpengdd.cyou/gtffcuugoq.html

[R66] 定时任务
来源：http://hz.jlsjyb.cn/gtvsbvgorb.html

crontab -e;  crontab -l
来源：http://hz.smart0.xyz/gtxylcbppu.html

[R67] 生成随机十六进制串
来源：http://hz.birdmap.top/gtejtcnkcz.html

openssl rand -hex 16
来源：http://hz.guannengcc.top/gtxdrfyfpy.html

[R68] 计算文件校验值
来源：http://hz.fengsongda.top/gtanxdckgu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.c1oappe.top/gtumcujrcw.html

[R69] 生成随机密码
来源：http://hz.kuanghao11.cn/gtbdowqtqs.html

head -c 16 /dev/urandom | base64
来源：http://hz.cdnleiting.top/gtpzilxcxv.html

[R70] 时间戳与互转
来源：http://hz.zhaomingkeji.xyz/gtxypyyvkm.html

date +%s;  date -d @1700000000
来源：http://hz.birdmap.top/gtneicnybh.html

[R71] 日期格式化
来源：http://hz.feifeiyinyue.top/gtpkisvuzy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.fengsongda.top/gtilzfkbvw.html

[R72] 等待端口就绪
来源：http://hz.chenjidiqi.icu/gthatavlby.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhixingplan.top/gtuwediecu.html

[R73] 分割大日志
来源：http://hz.jqgufenzy.top/gthmedazov.html

split -l 1000 big.log part_
来源：http://hz.shzxlz.cn/gttqoiflpt.html

[R74] 批量重命名
来源：http://hz.jinqigfzy.top/gtqbyhvcyt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.c1oappe.top/gtqspfdqao.html

[R75] 导出环境变量
来源：http://hz.gaohongyu789.top/gtnfmovdtu.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.nanxuanxn.top/gtobbctafq.html

[R76] 使用临时文件
来源：http://hz.0kj1m.cn/gtnxvttfxf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hammf.cn/gtmgeflexj.html

[R77] 读取用户输入
来源：http://hz.tianlin.xyz/gtapvahagb.html

read -rp "请输入: " ans
来源：http://hz.gotoacloud.top/gteuzkrynd.html

[R78] 交互式菜单
来源：http://hz.sysykeji.top/gtedytxalj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zdqjudy.top/gtzrloidbo.html

[R79] 解析命令行选项
来源：http://hz.vqdsnc.cn/gtzjgpvhmp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ywan-chungtsiang.top/gttsnctgoz.html

[R80] 查看脚本执行耗时
来源：http://hz.redwolf501.top/gtdytjacpj.html

time ./run.sh
来源：http://hz.cdnleiting.top/gtpbsoeiff.html

================================================================================
来源：http://hz.yj20258888.top/gtojgutyeb.html

S. C / C++ 专题
来源：http://hz.sxryk.cn/gttaouxgct.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtbzwgudmm.html

[S01] C：Hello World
来源：http://hz.jinqigfzy.top/gtoxhewkvu.html

#include <stdio.h>
来源：http://hz.wangdashe.top/gttyddgntu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.c1oappe.top/gteyurnwyl.html

[S02] C：变量与格式化输出
来源：http://hz.shanyushiyangkeji.top/gtvuyflumt.html

int a = 10; printf("%d\n", a);
来源：http://hz.smart0.xyz/gtsyawzrdr.html

[S03] C：读入整数
来源：http://hz.tianlin.xyz/gtzemzfbhu.html

int x; scanf("%d", &x);
来源：http://hz.hywenlv.cn/gtococqwpl.html

[S04] C：字符串复制
来源：http://hz.tian-w.cn/gthmzsgows.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jianghu66.top/gtnzlxjfxu.html

[S05] C：字符串长度
来源：http://hz.hnxiangtu.top/gtsvzcvtti.html

strlen(s)
来源：http://hz.jianghu66.top/gtwpkthoor.html

[S06] C：字符串比较
来源：http://hz.zhijiandao.cn/gtnzvnbxdh.html

strcmp(a, b) == 0
来源：http://hz.kuanghao11.cn/gtftmmeqas.html

[S07] C：数组遍历求和
来源：http://hz.0kj1m.cn/gtjstkxvnl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zycfv.cn/gtrkgdvkbg.html

[S08] C：动态内存分配与释放
来源：http://hz.jinqigfzy.top/gtoqwebhhb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hnxiangtu.top/gtcyvynnac.html

[S09] C：结构体定义与初始化
来源：http://hz.dashuyun.cn/gtdekzbmcv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yanxiufei.cn/gtapaetulg.html

[S10] C：指针与解引用
来源：http://hz.cqqwz.cn/gtwmvbyiih.html

int *p = &a;  *p = 5;
来源：http://hz.shuidangran.top/gtbcugiasq.html

[S11] C：逐行读文件
来源：http://hz.mhx1999.top/gtmnkcdzjo.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sysykeji.top/gtfirdipmk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yongpay.top/gtlkjqppyb.html

fclose(f);
来源：http://hz.jlsjyb.cn/gtomdjwehn.html

[S12] C：写文件
来源：http://hz.hammf.cn/gtgjlyeaqv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hongshengwenyu.top/gtxemneyxg.html

[S13] C：宏定义
来源：http://hz.daxiang520.top/gtvgrrsoih.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.316326.xyz/gtsrlgjnso.html

[S14] C：枚举
来源：http://hz.jqgfzy.top/gtfwrilsdq.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.havefunace.top/gtagljpzjt.html

[S15] C：类型转换
来源：http://hz.xziqi.cn/gtpjklxonu.html

(double) a / b
来源：http://hz.mhx1999.top/gtmaqojwms.html

[S16] C：位操作置位
来源：http://hz.chenjidiqi.icu/gtdlbmapto.html

x |= (1 << 3);
来源：http://hz.svipenyu.cn/gtlybywbiq.html

[S17] C：安全拼接字符串
来源：http://hz.ydzc1.top/gtufyxnvri.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.aizwys.cn/gtvgxtpmis.html

[S18] C：命令行参数
来源：http://hz.yvedp.cn/gtbztzfxoo.html

int main(int argc, char **argv)
来源：http://hz.hammf.cn/gtwtdapzob.html

[S19] C：快速排序
来源：http://hz.ydjk.org.cn/gtxxzxinrg.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xuetiantiany.cn/gtugvwfrde.html

[S20] C：二分查找
来源：http://hz.0kj1m.cn/gtdvwwwyot.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ywan-chungtsiang.top/gtheaxojle.html

[S21] C：字符类别判断
来源：http://hz.ydzc1.top/gtovticvru.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.316326.xyz/gthmcnratz.html

[S22] C：字符串转数字
来源：http://hz.ywan-chungtsiang.top/gthiljafhq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shuidangran.top/gtszjlzrkh.html

[S23] C：随机数
来源：http://hz.xziqi.cn/gtseffslbe.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yueranfly.top/gtdipkgoeh.html

[S24] C：获取本地时间
来源：http://hz.xingfuxueyuan.xyz/gtgjqtzypy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zdqjudy.top/gtkkaxnqxp.html

[S25] C：内存拷贝
来源：http://hz.shuidangran.top/gtmqydajzp.html

memcpy(dst, src, n);
来源：http://hz.haohaochexian.top/gthvkqraiw.html

[S26] C：内存清零
来源：http://hz.hammf.cn/gtfiuxqjhp.html

memset(a, 0, sizeof a);
来源：http://hz.pengpengdd.cyou/gtawcprubx.html

[S27] C：定义常量
来源：http://hz.zhoulong.xyz/gtaodbapnl.html

const double PI = 3.14159;
来源：http://hz.daxiang520.top/gtkdxufvyf.html

[S28] C：静态变量
来源：http://hz.ydjk.org.cn/gtbkdtbedc.html

static int counter = 0;
来源：http://hz.zhiwuduotai.top/gtkqidgspu.html

[S29] C：变参函数
来源：http://hz.wangdashe.top/gtiqwoahoq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shanyushiyangkeji.top/gtwdqgelfd.html

[S30] C：头文件保护
来源：http://hz.zhijiandao.cn/gttqrxctsz.html

#ifndef X_H
来源：http://hz.iojbl.cn/gtuytuocvq.html

#define X_H
来源：http://hz.yuxming.cn/gthcxktwop.html

#endif
来源：http://hz.shanyushiyangkeji.top/gtedkzpvha.html

[S31] C++：Hello World
来源：http://hz.chenzaomai.com/gthewjpwzs.html

#include <iostream>
来源：http://hz.zhoulong.xyz/gtaildgfjl.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jlsjyb.cn/gtkhnrmhtr.html

[S32] C++：字符串
来源：http://hz.shanyushiyangtech.top/gtqiglvprc.html

std::string s = "hi";  s += "!";
来源：http://hz.shzxlz.cn/gtzsjhsfgn.html

[S33] C++：vector 增删
来源：http://hz.tanke756.top/gtbpccwpjt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zdqjudy.top/gtzsdvmpgl.html

[S34] C++：遍历 vector
来源：http://hz.ywan-chungtsiang.top/gtffiqdkfq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.gogol.net.cn/gtcswbfebn.html

[S35] C++：map
来源：http://hz.jyoumei.cn/gtpbqrdmsu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yanxiufei.cn/gteklkkucq.html

[S36] C++：unordered_map
来源：http://hz.birdmap.top/gtzeevsocl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hnqzz.top/gtwsmpwvpd.html

[S37] C++：set
来源：http://hz.guannengcc.top/gtsipsohft.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zdqjudy.top/gtnhhvhqmc.html

[S38] C++：排序
来源：http://hz.yueranfly.top/gtawmgwvhc.html

std::sort(v.begin(), v.end());
来源：http://hz.sxryk.cn/gtsujpzbpb.html

[S39] C++：自定义比较器排序
来源：http://hz.shangyingyoupin.top/gtnobbnbgu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.nanxinkj.top/gtnfqeeuth.html

[S40] C++：查找元素
来源：http://hz.andypj.xyz/gtfyodzawf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cashguo.top/gtnvfzoxrl.html

[S41] C++：类与构造函数
来源：http://hz.ybcxt.top/gtsisuwrpp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.haohaochexian.top/gtvjddsjto.html

[S42] C++：继承与虚函数
来源：http://hz.tanke756.top/gtveiiggme.html

class B : public Base { public: void f() override {} };
来源：http://hz.kuanghao11.cn/gtujfvzzmz.html

[S43] C++：智能指针
来源：http://hz.xziqi.cn/gtmwcbexfg.html

auto p = std::make_unique<int>(5);
来源：http://hz.shanyushiyangtech.top/gtahhugnvq.html

[S44] C++：引用传参
来源：http://hz.jqgufenzy.top/gtewbtwvcw.html

void inc(int &x) { ++x; }
来源：http://hz.nwbrower.top/gttxogfcvc.html

[S45] C++：lambda
来源：http://hz.shanyushiyangkeji.top/gtkmymcpoj.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yj20258888.top/gtorhrelue.html

[S46] C++：函数模板
来源：http://hz.jinqigufen.top/gtvzlzwyny.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jianghu66.top/gtykfifvrs.html

[S47] C++：结构化绑定遍历
来源：http://hz.nwbrower.top/gtidypezmk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.bjfxy.top/gttzimnopa.html

[S48] C++：逐行读文件
来源：http://hz.shzxlz.cn/gtklvqilie.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shuidangran.top/gticimxxdm.html

while (std::getline(in, line)) { }
来源：http://hz.ehwqpu.com/gtybtshrac.html

[S49] C++：写文件
来源：http://hz.dashuyun.cn/gtvxfekkoc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jinqigfzy.top/gtmllzpcau.html

[S50] C++：格式化数字
来源：http://hz.vqdsnc.cn/gtjykooech.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.daria6918.cn/gtirvbffaw.html

[S51] C++：显式类型转换
来源：http://hz.daria6918.cn/gtjytwefec.html

static_cast<double>(a) / b
来源：http://hz.zhengqikj.top/gtlkwdfdgh.html

[S52] C++：const 与 noexcept
来源：http://hz.nwbrower.top/gtxttkpkrk.html

int size() const noexcept { return n_; }
来源：http://hz.chenzaomai.com/gthyeyqwng.html

[S53] C++：移动语义
来源：http://hz.gogol.net.cn/gtvrbmordg.html

std::vector<int> w = std::move(v);
来源：http://hz.sweek.top/gtclmzarrv.html

[S54] C++：异常处理
来源：http://hz.xinyue.icu/gtpwlxjyoh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ywan-chungtsiang.top/gtdgqzqddt.html

[S55] C++：结构化绑定
来源：http://hz.iojbl.cn/gtkowlldnt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cucudq.cn/gtsycesdzn.html

[S56] C++：optional
来源：http://hz.gotoacloud.top/gtiaupttao.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ppjwa.cn/gtujowtrcn.html

[S57] C++：编译期常量
来源：http://hz.fengsongda.top/gtlwoegrbf.html

constexpr int N = 10;
来源：http://hz.kuanghao11.cn/gtveryhpfm.html

[S58] C++：命名空间
来源：http://hz.nwbrower.top/gtfeoopzws.html

namespace ns { int f() { return 1; } }
来源：http://hz.shzxlz.cn/gtamtvuhzi.html

[S59] C++：静态断言
来源：http://hz.gzhubu.top/gtzykfvsok.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.feifeiyinyue.top/gtcziespre.html

[S60] C++：遍历并删除元素
来源：http://hz.cashguo.top/gtyajjxulm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.gzhubu.top/gtpqdptmsn.html

================================================================================
来源：http://hz.ehwqpu.com/gtzelqvrgi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jqgfzy.top/gturrlghmc.html

================================================================================
来源：http://hz.yj202588.top/gtntgmhvjk.html

[T01] Kotlin：Hello World
来源：http://hz.cdnleiting.top/gthrxbjrhe.html

println("Hello")
来源：http://hz.ydzc1.top/gtwbmpsxwx.html

[T02] Kotlin：变量
来源：http://hz.jinghuilouyu.cn/gtckyzotew.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jinyuanbaomall.cn/gtrvyxnxma.html

[T03] Kotlin：字符串模板
来源：http://hz.cashguo.top/gtdzbfbhry.html

"值: $b"
来源：http://hz.pycfn.com/gtmmsnbgqc.html

[T04] Kotlin：空安全
来源：http://hz.wangshuangyany.cn/gtmhakyrze.html

val n: String? = null;  n?.length
来源：http://hz.cucudq.cn/gtzqmpotrb.html

[T05] Kotlin：when 表达式
来源：http://hz.jinyuanbaomall.cn/gtwxhodwfd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.sweek.top/gttptzydmt.html

[T06] Kotlin：集合映射
来源：http://hz.ppjwa.cn/gtfsdwtwbd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ywan-chungtsiang.top/gtrtedogsw.html

[T07] Kotlin：集合过滤
来源：http://hz.guowangkeji.top/gtfstzqllg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hfpthk.cn/gtbteqahjv.html

[T08] Kotlin：数据类
来源：http://hz.yuxming.cn/gthubxcowo.html

data class User(val name: String, val age: Int)
来源：http://hz.shuidangran.top/gtbkhilzmn.html

[T09] Kotlin：扩展函数
来源：http://hz.sufxvd.cn/gtosrghgkg.html

fun String.exclaim() = this + "!"
来源：http://hz.cashguo.top/gtzspcjjmp.html

[T10] Kotlin：默认参数
来源：http://hz.vqdsnc.cn/gtoofcfocr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.316326.xyz/gtjocfkfcq.html

[T11] Kotlin：协程
来源：http://hz.iojbl.cn/gtqpaxvmsy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinghuilouyu.cn/gtyxpmtfyb.html

[T12] Kotlin：解构声明
来源：http://hz.meibo888.top/gtkywjileb.html

val (a, b) = Pair(1, 2)
来源：http://hz.hammf.cn/gtkxzqkrwo.html

[T13] Kotlin：只读 Map
来源：http://hz.hammf.cn/gtsqrkyffi.html

val m = mapOf("a" to 1)
来源：http://hz.hysaishi.cn/gtgnwuxbji.html

[T14] Kotlin：循环
来源：http://hz.zhongyouzk.top/gtgacscnml.html

for (i in 1..10) println(i)
来源：http://hz.yj20258.top/gtlkkvvxgl.html

[T15] Kotlin：接口
来源：http://hz.aibaodan.cn/gtbfzgykfg.html

interface Shape { fun area(): Double }
来源：http://hz.ehwqpu.com/gtljwhzeqv.html

[T16] Swift：Hello World
来源：http://hz.dashuyun.cn/gtdmpdxplk.html

print("Hello")
来源：http://hz.jqgfzy.top/gttobzxbmg.html

[T17] Swift：变量与常量
来源：http://hz.nanxinkj.top/gtwlsrlwrd.html

var a = 1;  let b = 2
来源：http://hz.havefunace.top/gtsgygutgp.html

[T18] Swift：字符串插值
来源：http://hz.9152youxi.cn/gtewvdvljx.html

"值: \(b)"
来源：http://hz.shanyushiyangkeji.top/gtekxoxdfz.html

[T19] Swift：可选绑定
来源：http://hz.aibaodan.cn/gtuarhrdux.html

if let n = opt { print(n) }
来源：http://hz.ydjk.org.cn/gtvvmrbohr.html

[T20] Swift：数组操作
来源：http://hz.yuxming.cn/gtbgvolnpa.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.dashuyun.cn/gtzpitdthf.html

[T21] Swift：遍历
来源：http://hz.tian-w.cn/gtihrvsobw.html

for x in a { print(x) }
来源：http://hz.gogol.net.cn/gtktslbkfc.html

[T22] Swift：字典
来源：http://hz.guowangkeji.top/gtxtfkbjlw.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.iojbl.cn/gtiiqnpfyp.html

[T23] Swift：函数
来源：http://hz.xingfuxueyuan.xyz/gtaexwekvp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zdqjudy.top/gtusyfgjto.html

[T24] Swift：闭包
来源：http://hz.hywenlv.cn/gtileklaub.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jinghuilouyu.cn/gtawgjfgvd.html

[T25] Swift：结构体
来源：http://hz.52xcode.cn/gtbrukvkmy.html

struct P { var x: Int }
来源：http://hz.hnxiangtu.top/gtqsayqrmb.html

[T26] Swift：类与重写
来源：http://hz.mhx1999.top/gtrjcgpyro.html

class A: Base { override func f() {} }
来源：http://hz.hywenlv.cn/gtmcbyrsjo.html

[T27] Swift：错误处理
来源：http://hz.nanxinkj.top/gtqjdleqct.html

do { try f() } catch { print(error) }
来源：http://hz.cucudq.cn/gtvazctton.html

[T28] Swift：枚举
来源：http://hz.zdqjudy.top/gtrwuliuge.html

enum Color { case red, green }
来源：http://hz.jinyuanbaomall.cn/gtqllmxcwq.html

[T29] Swift：guard 提前返回
来源：http://hz.sxryk.cn/gtmykzqoyj.html

guard let x = opt else { return }
来源：http://hz.zhongyouzk.top/gtktbbnasp.html

[T30] Swift：协议
来源：http://hz.quarkkingdee.top/gtqrayqfzj.html

protocol Shape { func area() -> Double }
来源：http://hz.snrcjt.cn/gtenatxjpr.html

[T31] Lua：Hello World
来源：http://hz.sxryk.cn/gtcnhbfubp.html

print("Hello")
来源：http://hz.zdqjudy.top/gtxpmbwvse.html

[T32] Lua：局部变量
来源：http://hz.316326.xyz/gtjyrluqfk.html

local a = 1
来源：http://hz.hongshengwenyu.top/gtqznttqeq.html

[T33] Lua：表（数组）
来源：http://hz.shanyushiyangtech.top/gtiplovbtg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.gogol.net.cn/gtyebpijga.html

[T34] Lua：遍历表
来源：http://hz.smart0.xyz/gtuoxtvmqg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zycfv.cn/gtrpmagnxf.html

[T35] Lua：字典表
来源：http://hz.havefunace.top/gtavsuniyl.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zhixingplan.top/gtdnzepcye.html

[T36] Lua：函数
来源：http://hz.smart0.xyz/gtomklslgc.html

function add(a, b) return a + b end
来源：http://hz.feifeiyinyue.top/gtogrkcicv.html

[T37] Lua：字符串拼接
来源：http://hz.52xcode.cn/gtslaieowj.html

"a" .. "b"
来源：http://hz.pengpengdd.cyou/gtjwztsfpp.html

[T38] Lua：条件
来源：http://hz.aibaodan.cn/gtshiccpas.html

if x > 0 then print("正") end
来源：http://hz.guannengcc.top/gthpiaergy.html

[T39] Lua：模式匹配
来源：http://hz.gotoacloud.top/gttuukbvde.html

string.find(s, "%d+")
来源：http://hz.jlsjyb.cn/gtgordwcfz.html

[T40] Lua：元表
来源：http://hz.zhijiandao.cn/gtjfhsuljc.html

setmetatable({}, { __index = base })
来源：http://hz.aibaodan.cn/gtqxmyycrd.html

[T41] Perl：Hello World
来源：http://hz.zhoulong.xyz/gtefkrowgy.html

print "Hello\n";
来源：http://hz.chenjidiqi.icu/gtpydnhvyi.html

[T42] Perl：变量类型
来源：http://hz.yongpay.top/gtllgzoufa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.ehwqpu.com/gtonqdfmng.html

[T43] Perl：字符串插值
来源：http://hz.gzhubu.top/gtjlsemnkv.html

"值: $a"
来源：http://hz.yongpay.top/gtvpfanktf.html

[T44] Perl：条件
来源：http://hz.sufxvd.cn/gtxzoimhfv.html

if ($a > 0) { print "正"; }
来源：http://hz.ydzc1.top/gtyemfiqgc.html

[T45] Perl：数组遍历
来源：http://hz.yuanzhike.top/gttfhuyarv.html

for my $x (@arr) { print $x; }
来源：http://hz.yongpay.top/gtmmfclybi.html

[T46] Perl：哈希操作
来源：http://hz.yueranfly.top/gtlhcmaoiw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.aibaodan.cn/gtoecugbla.html

[T47] Perl：正则捕获
来源：http://hz.jyoumei.cn/gtbvxdvgnc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.cheryme.top/gtixfurnya.html

[T48] Perl：正则替换
来源：http://hz.shangyingyoupin.top/gtvmelrkcw.html

$s =~ s/old/new/g;
来源：http://hz.chenzaomai.com/gtrgabyxfz.html

[T49] Perl：函数
来源：http://hz.hysaishi.cn/gtlphxqjeu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jiagoushi.top/gtxvxkhjnt.html

[T50] Perl：逐行读文件
来源：http://hz.hysaishi.cn/gtvpbclcru.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.shuidangran.top/gthfdqzkhu.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.birdmap.top/gtaaiewviu.html

[T51] Scala：Hello World
来源：http://hz.jlsjyb.cn/gttonrwzwl.html

println("Hello")
来源：http://hz.yvedp.cn/gtwduafjit.html

[T52] Scala：变量
来源：http://hz.c1oappe.top/gtzrplnwop.html


<!-- 参考信息 -->