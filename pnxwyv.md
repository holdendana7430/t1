代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.feifeiyinyue.top/gtebcymwok.html

[R50] awk 求和
来源：http://hz.sysykeji.top/gtmehxqcmo.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.havefunace.top/gtllyjpike.html

[R51] 排序去重取前几
来源：http://hz.jyoumei.cn/gtvofolkoc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.redwolf501.top/gtttmvkpgs.html

[R52] 统计行数
来源：http://hz.yuanzhike.top/gtkgatgilb.html

wc -l a.txt
来源：http://hz.yongpay.top/gtypgvjlec.html

[R53] 查看文件头与实时尾
来源：http://hz.ydjk.org.cn/gtkmlxczlw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cheryme.top/gtkagwiinh.html

[R54] 比较两个文件
来源：http://hz.yj20258.top/gtecemithy.html

diff a.txt b.txt
来源：http://hz.hywenlv.cn/gtjegxizrl.html

[R55] 压缩与解压
来源：http://hz.ywan-chungtsiang.top/gtsdqsnzej.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cucudq.cn/gtjtbiwgph.html

[R56] 远程拷贝
来源：http://hz.hongshengwenyu.top/gtpefqdwon.html

scp file user@host:/path/
来源：http://hz.ydzc1.top/gtwegcrppy.html

[R57] 远程执行命令
来源：http://hz.yangfankeji.com/gtomdgoklp.html

ssh user@host 'uptime'
来源：http://hz.ehwqpu.com/gtmtcnnldt.html

[R58] 下载文件
来源：http://hz.jqgfzy.top/gteahylvta.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hongshengwenyu.top/gtnanlyakv.html

[R59] 发 POST JSON
来源：http://hz.iojbl.cn/gtwvbhvotb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jyoumei.cn/gtghwbscmk.html

[R60] 只看 HTTP 状态码
来源：http://hz.shzxlz.cn/gtdxcsqpgq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.iojbl.cn/gtshdthrrn.html

[R61] 磁盘占用
来源：http://hz.yvedp.cn/gtjzvarkwz.html

df -h;  du -sh *
来源：http://hz.sweek.top/gtfzyimwsl.html

[R62] 找最占空间的文件
来源：http://hz.tian-w.cn/gtexaoufiz.html

du -ah . | sort -rh | head -10
来源：http://hz.zycfv.cn/gtopxatkdt.html

[R63] 内存与进程
来源：http://hz.nwbrower.top/gtprmjgpfk.html

free -h;  ps aux | grep nginx
来源：http://hz.jinqigfzy.top/gtzdrvybcu.html

[R64] 结束进程
来源：http://hz.havefunace.top/gtrruyllun.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yj202588.top/gtwridobbs.html

[R65] 查看端口占用
来源：http://hz.guowangkeji.top/gtalvslnas.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yangfankeji.com/gtdxpabmmv.html

[R66] 定时任务
来源：http://hz.andypj.xyz/gtbshjadqz.html

crontab -e;  crontab -l
来源：http://hz.fzhhl.top/gtbceajpnc.html

[R67] 生成随机十六进制串
来源：http://hz.yangfankeji.com/gtfddzhwnf.html

openssl rand -hex 16
来源：http://hz.jinqigufen.top/gtnhojcnwn.html

[R68] 计算文件校验值
来源：http://hz.cashguo.top/gtcofixjxy.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zycfv.cn/gtneppmfqz.html

[R69] 生成随机密码
来源：http://hz.cqqwz.cn/gtssxnwbgq.html

head -c 16 /dev/urandom | base64
来源：http://hz.svipenyu.cn/gtzizxnehp.html

[R70] 时间戳与互转
来源：http://hz.hywenlv.cn/gtgxgfzvgu.html

date +%s;  date -d @1700000000
来源：http://hz.hnxiangtu.top/gtrvswpmgr.html

[R71] 日期格式化
来源：http://hz.hnqzz.top/gtoaguqzrc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.birdmap.top/gtdybewpet.html

[R72] 等待端口就绪
来源：http://hz.cqqwz.cn/gtoezhhmup.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.nwbrower.top/gtytbkxevl.html

[R73] 分割大日志
来源：http://hz.zhixingplan.top/gtztmbvytt.html

split -l 1000 big.log part_
来源：http://hz.xinyue.icu/gtzsqlqkyr.html

[R74] 批量重命名
来源：http://hz.hnqzz.top/gtbgwhjfhm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hnxiangtu.top/gtjoumgatk.html

[R75] 导出环境变量
来源：http://hz.jinghuilouyu.cn/gtxzhtsbty.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.snrcjt.cn/gtfhubkujn.html

[R76] 使用临时文件
来源：http://hz.hongshengwenyu.top/gtfwtpmcaz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.pengpengdd.cyou/gtssmwxuwf.html

[R77] 读取用户输入
来源：http://hz.chenjidiqi.icu/gtvxicdgdy.html

read -rp "请输入: " ans
来源：http://hz.meibo888.top/gtozlcrhju.html

[R78] 交互式菜单
来源：http://hz.snrcjt.cn/gtmbnzbyfc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yangfankeji.com/gtxdcmmzcy.html

[R79] 解析命令行选项
来源：http://hz.zhijiandao.cn/gtbtkorxjv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ehwqpu.com/gtxieylfhq.html

[R80] 查看脚本执行耗时
来源：http://hz.hysaishi.cn/gtstykwrct.html

time ./run.sh
来源：http://hz.daria6918.cn/gtrmqjmjet.html

================================================================================
来源：http://hz.sweek.top/gtfvyfrwyb.html

S. C / C++ 专题
来源：http://hz.chenlongwang.top/gtuzswwstz.html

================================================================================
来源：http://hz.mhx1999.top/gtjfbkrgyr.html

[S01] C：Hello World
来源：http://hz.pycfn.com/gtgzmcbpwk.html

#include <stdio.h>
来源：http://hz.birdmap.top/gtgogekifk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xylfe.cn/gtkkwzzhty.html

[S02] C：变量与格式化输出
来源：http://hz.shangyingyoupin.top/gtsrrpfpzo.html

int a = 10; printf("%d\n", a);
来源：http://hz.redwolf501.top/gtxnmwvlnc.html

[S03] C：读入整数
来源：http://hz.xziqi.cn/gtakdlpleg.html

int x; scanf("%d", &x);
来源：http://hz.guowangkeji.top/gtlmqpqabl.html

[S04] C：字符串复制
来源：http://hz.shanyushiyangtech.top/gtoymiskrf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.quarkkingdee.top/gtukicfgpl.html

[S05] C：字符串长度
来源：http://hz.yj202588.top/gtrdrmjflm.html

strlen(s)
来源：http://hz.dashuyun.cn/gtslwfuosu.html

[S06] C：字符串比较
来源：http://hz.redwolf501.top/gtfzodfdkq.html

strcmp(a, b) == 0
来源：http://hz.zhiwuduotai.top/gtphinbwsv.html

[S07] C：数组遍历求和
来源：http://hz.xinyue.icu/gtqrzmvkvi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.svipenyu.cn/gtgsldniyc.html

[S08] C：动态内存分配与释放
来源：http://hz.jyoumei.cn/gtzxhkcupc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hnxiangtu.top/gtpihaqrgl.html

[S09] C：结构体定义与初始化
来源：http://hz.yonumen.top/gtmzuqmmco.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yj20258888.top/gtbmznojrm.html

[S10] C：指针与解引用
来源：http://hz.nanxinkj.top/gtsyvbjfaq.html

int *p = &a;  *p = 5;
来源：http://hz.c1oappe.top/gtcombkzsy.html

[S11] C：逐行读文件
来源：http://hz.yj202588.top/gtaehrztwa.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cqqwz.cn/gtabxacoed.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ybcxt.top/gtqewncbxv.html

fclose(f);
来源：http://hz.bjfxy.top/gtcuglkhsr.html

[S12] C：写文件
来源：http://hz.cdnleiting.top/gtqcrjvpsz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ywan-chungtsiang.top/gtkcftdyfe.html

[S13] C：宏定义
来源：http://hz.c1oappe.top/gtdjoqhxkh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.nwbrower.top/gtntklytbb.html

[S14] C：枚举
来源：http://hz.iojbl.cn/gtgjjmeujl.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.chenjidiqi.icu/gtsykudoto.html

[S15] C：类型转换
来源：http://hz.yongpay.top/gtkmwosfgj.html

(double) a / b
来源：http://hz.jqgfzy.top/gtwhnhpvmq.html

[S16] C：位操作置位
来源：http://hz.hnqzz.top/gtlwjqhcoz.html

x |= (1 << 3);
来源：http://hz.pengpengdd.cyou/gtwlrljzlq.html

[S17] C：安全拼接字符串
来源：http://hz.shuidangran.top/gtagnipcbt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xuanzx.com/gtfxhmucqb.html

[S18] C：命令行参数
来源：http://hz.0kj1m.cn/gtvzjykuap.html

int main(int argc, char **argv)
来源：http://hz.sxryk.cn/gtoevxpgqe.html

[S19] C：快速排序
来源：http://hz.hnxiangtu.top/gtemddrvii.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.vqdsnc.cn/gtroezcuii.html

[S20] C：二分查找
来源：http://hz.shzxlz.cn/gtcpywhoxa.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhijiandao.cn/gtkgtpqpap.html

[S21] C：字符类别判断
来源：http://hz.guowangkeji.top/gtpasfrsod.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.c1oappe.top/gtucvtypnf.html

[S22] C：字符串转数字
来源：http://hz.jqgfzy.top/gtvutffoup.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xingfuxueyuan.xyz/gtnjpvaxud.html

[S23] C：随机数
来源：http://hz.nanxinkj.top/gtrjzdrxis.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zycfv.cn/gtkphffooy.html

[S24] C：获取本地时间
来源：http://hz.smart0.xyz/gtrbmxpyfp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hywenlv.cn/gtxdliasmf.html

[S25] C：内存拷贝
来源：http://hz.cqqwz.cn/gtiozfafyf.html

memcpy(dst, src, n);
来源：http://hz.gzhubu.top/gthbdskjyp.html

[S26] C：内存清零
来源：http://hz.nwbrower.top/gtsmandtwt.html

memset(a, 0, sizeof a);
来源：http://hz.ydzc1.top/gtcxqnzofh.html

[S27] C：定义常量
来源：http://hz.mhx1999.top/gtztrulfuq.html

const double PI = 3.14159;
来源：http://hz.xuetiantiany.cn/gtfzdesmwm.html

[S28] C：静态变量
来源：http://hz.hongshengwenyu.top/gtrpetrnsj.html

static int counter = 0;
来源：http://hz.gotoacloud.top/gtxckvrfbu.html

[S29] C：变参函数
来源：http://hz.quarkkingdee.top/gtuuifqfna.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.aibaodan.cn/gtjyvdmdaw.html

[S30] C：头文件保护
来源：http://hz.gaohongyu789.top/gtkcvnffmm.html

#ifndef X_H
来源：http://hz.ydjk.org.cn/gtdmctmugx.html

#define X_H
来源：http://hz.jinyuanbaomall.cn/gtavracxvr.html

#endif
来源：http://hz.yj20258888.top/gtkgldvmvz.html

[S31] C++：Hello World
来源：http://hz.dashuyun.cn/gtsssoovew.html

#include <iostream>
来源：http://hz.c1oappe.top/gtrncduyuj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhengqikj.top/gtagqympag.html

[S32] C++：字符串
来源：http://hz.ywan-chungtsiang.top/gtatvybmbp.html

std::string s = "hi";  s += "!";
来源：http://hz.chenlongwang.top/gthuzhyyeq.html

[S33] C++：vector 增删
来源：http://hz.zhoulong.xyz/gtzkoqsocs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.aibaodan.cn/gtxmowoosy.html

[S34] C++：遍历 vector
来源：http://hz.cheryme.top/gtnobdikat.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.wangdashe.top/gtljoqimuf.html

[S35] C++：map
来源：http://hz.hnxiangtu.top/gtispkwmpp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nwbrower.top/gtzphqafet.html

[S36] C++：unordered_map
来源：http://hz.hnqzz.top/gtgoqoxkfz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hfpthk.cn/gthfmcqasn.html

[S37] C++：set
来源：http://hz.sweek.top/gtbmoxrtfl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.sxryk.cn/gtuftkrdrp.html

[S38] C++：排序
来源：http://hz.9152youxi.cn/gtvfbqkkdf.html

std::sort(v.begin(), v.end());
来源：http://hz.snrcjt.cn/gtxrxosfsg.html

[S39] C++：自定义比较器排序
来源：http://hz.sysykeji.top/gtmbxjwoii.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ywan-chungtsiang.top/gthnoauaih.html

[S40] C++：查找元素
来源：http://hz.gogol.net.cn/gtkotabqgz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.havefunace.top/gtcmxesapu.html

[S41] C++：类与构造函数
来源：http://hz.chenjidiqi.icu/gtprqiypci.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.bjfxy.top/gtexdbtjqo.html

[S42] C++：继承与虚函数
来源：http://hz.haohaochexian.top/gtsotcuevr.html

class B : public Base { public: void f() override {} };
来源：http://hz.zdqjudy.top/gtloodzeyn.html

[S43] C++：智能指针
来源：http://hz.yj20258888.top/gttfngkrdr.html

auto p = std::make_unique<int>(5);
来源：http://hz.jyoumei.cn/gtkpnoyjji.html

[S44] C++：引用传参
来源：http://hz.bjfxy.top/gtcknrarcn.html

void inc(int &x) { ++x; }
来源：http://hz.gogol.net.cn/gtqsrondzy.html

[S45] C++：lambda
来源：http://hz.cdnleiting.top/gtbyhzibap.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.dianchejie.cn/gtzeeljxjb.html

[S46] C++：函数模板
来源：http://hz.52xcode.cn/gtkbwqlleo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.meibo888.top/gtvnfchwsv.html

[S47] C++：结构化绑定遍历
来源：http://hz.chenzaomai.com/gtziqlemzk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.guannengcc.top/gtqhfuaezd.html

[S48] C++：逐行读文件
来源：http://hz.jinghuilouyu.cn/gtufhybsov.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.redwolf501.top/gtdhoqnnhg.html

while (std::getline(in, line)) { }
来源：http://hz.zhiwuduotai.top/gtjeknptdv.html

[S49] C++：写文件
来源：http://hz.chenzaomai.com/gtvuaabxia.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.sxryk.cn/gtpohvlrvt.html

[S50] C++：格式化数字
来源：http://hz.nanxuanxn.top/gtojebljiw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yangfankeji.com/gtwkpyutuv.html

[S51] C++：显式类型转换
来源：http://hz.zhengqikj.top/gtespbafbb.html

static_cast<double>(a) / b
来源：http://hz.gzhubu.top/gtvjedvowq.html

[S52] C++：const 与 noexcept
来源：http://hz.52xcode.cn/gtkmnsshea.html

int size() const noexcept { return n_; }
来源：http://hz.mhx1999.top/gtkgztgkpd.html

[S53] C++：移动语义
来源：http://hz.mhx1999.top/gtgorlrbch.html

std::vector<int> w = std::move(v);
来源：http://hz.ehwqpu.com/gtiocszlub.html

[S54] C++：异常处理
来源：http://hz.sweek.top/gtvsivdexv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cashguo.top/gtjqsmtmfh.html

[S55] C++：结构化绑定
来源：http://hz.cqqwz.cn/gtkvmgywnk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhixingplan.top/gtzwnchyuf.html

[S56] C++：optional
来源：http://hz.yongpay.top/gtdszsghnh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.wangdashe.top/gthrfskqii.html

[S57] C++：编译期常量
来源：http://hz.ppjwa.cn/gtuwonpxkf.html

constexpr int N = 10;
来源：http://hz.jiagoushi.top/gtedzapogu.html

[S58] C++：命名空间
来源：http://hz.jyoumei.cn/gtszlhlegc.html

namespace ns { int f() { return 1; } }
来源：http://hz.sufxvd.cn/gtnrevlxkp.html

[S59] C++：静态断言
来源：http://hz.vqdsnc.cn/gtfzwskkni.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hysaishi.cn/gtabtxojec.html

[S60] C++：遍历并删除元素
来源：http://hz.ivvv.top/gtebgcftnn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.9152youxi.cn/gtdvrelwmn.html

================================================================================
来源：http://hz.chenzaomai.com/gtjiycpkth.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shangyingyoupin.top/gtraksjxyy.html

================================================================================
来源：http://hz.cucudq.cn/gtheumfwod.html

[T01] Kotlin：Hello World
来源：http://hz.daxiang520.top/gtktmiosxd.html

println("Hello")
来源：http://hz.jinghuilouyu.cn/gtrvhdtpvl.html

[T02] Kotlin：变量
来源：http://hz.havefunace.top/gtunyxwpwc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jyoumei.cn/gtuvnenyba.html

[T03] Kotlin：字符串模板
来源：http://hz.aizwys.cn/gtyvykuzly.html

"值: $b"
来源：http://hz.ppjwa.cn/gtooqxrwqn.html

[T04] Kotlin：空安全
来源：http://hz.jlsjyb.cn/gtrfupsbtl.html

val n: String? = null;  n?.length
来源：http://hz.jyoumei.cn/gtilbndbdu.html

[T05] Kotlin：when 表达式
来源：http://hz.9152youxi.cn/gturwltijd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ydjk.org.cn/gtxihzbmcl.html

[T06] Kotlin：集合映射
来源：http://hz.andypj.xyz/gtwqertmjn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zycfv.cn/gtrpwguuui.html

[T07] Kotlin：集合过滤
来源：http://hz.fengsongda.top/gtcjkhbemd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jyoumei.cn/gtstogpudn.html

[T08] Kotlin：数据类
来源：http://hz.jiagoushi.top/gteuooslwc.html

data class User(val name: String, val age: Int)
来源：http://hz.nwbrower.top/gtspehkfkr.html

[T09] Kotlin：扩展函数
来源：http://hz.bjfxy.top/gthexeenjv.html

fun String.exclaim() = this + "!"
来源：http://hz.mhx1999.top/gtiefokjlf.html

[T10] Kotlin：默认参数
来源：http://hz.jinqigufen.top/gtbdmfsmlt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.sxryk.cn/gtgccgwjaf.html

[T11] Kotlin：协程
来源：http://hz.xinyue.icu/gtgghdoztu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.52xcode.cn/gtcueiclkp.html

[T12] Kotlin：解构声明
来源：http://hz.jqgufenzy.top/gtkezrshgv.html

val (a, b) = Pair(1, 2)
来源：http://hz.hongshengwenyu.top/gtjufzrblo.html

[T13] Kotlin：只读 Map
来源：http://hz.xylfe.cn/gtepsevdht.html

val m = mapOf("a" to 1)
来源：http://hz.jinyuanbaomall.cn/gtxoywvshr.html

[T14] Kotlin：循环
来源：http://hz.zhongyouzk.top/gtldasascs.html

for (i in 1..10) println(i)
来源：http://hz.cqqwz.cn/gtyrrbbthg.html

[T15] Kotlin：接口
来源：http://hz.chenjidiqi.icu/gtmmkwwhvs.html

interface Shape { fun area(): Double }
来源：http://hz.meibo888.top/gteolbporb.html

[T16] Swift：Hello World
来源：http://hz.ivvv.top/gtecnnbfra.html

print("Hello")
来源：http://hz.zhoulong.xyz/gtzsuixtcs.html

[T17] Swift：变量与常量
来源：http://hz.jinghuilouyu.cn/gtjqxhgkoq.html

var a = 1;  let b = 2
来源：http://hz.vqdsnc.cn/gtzrdeqiai.html

[T18] Swift：字符串插值
来源：http://hz.snrcjt.cn/gtrgxgfphy.html

"值: \(b)"
来源：http://hz.yvedp.cn/gtgxmayztg.html

[T19] Swift：可选绑定
来源：http://hz.jinqigfzy.top/gtnuceqszc.html

if let n = opt { print(n) }
来源：http://hz.dianchejie.cn/gtkrtcbgbz.html

[T20] Swift：数组操作
来源：http://hz.jinyuanbaomall.cn/gtztoxdmcd.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.daxiang520.top/gtolvecivd.html

[T21] Swift：遍历
来源：http://hz.meibo888.top/gteqpwnazv.html

for x in a { print(x) }
来源：http://hz.aizwys.cn/gtuuquxjfi.html

[T22] Swift：字典
来源：http://hz.aizwys.cn/gtofspbtpr.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.daxiang520.top/gtarmjaiyo.html

[T23] Swift：函数
来源：http://hz.zhongyouzk.top/gtzbsgchfb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.andypj.xyz/gtwymdiasb.html

[T24] Swift：闭包
来源：http://hz.316326.xyz/gtwxwzcphy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.snrcjt.cn/gtfiepelgh.html

[T25] Swift：结构体
来源：http://hz.smart0.xyz/gtbnqhaeug.html

struct P { var x: Int }
来源：http://hz.ybcxt.top/gtlvzzarkj.html

[T26] Swift：类与重写
来源：http://hz.yuanzhike.top/gtlcfigwam.html

class A: Base { override func f() {} }
来源：http://hz.bjfxy.top/gtnejapktw.html

[T27] Swift：错误处理
来源：http://hz.zhengqikj.top/gttxkrgxnw.html

do { try f() } catch { print(error) }
来源：http://hz.smart0.xyz/gtvsluudhm.html

[T28] Swift：枚举
来源：http://hz.svipenyu.cn/gtbtrckvvb.html

enum Color { case red, green }
来源：http://hz.xingfuxueyuan.xyz/gtmfpemwbp.html

[T29] Swift：guard 提前返回
来源：http://hz.jiagoushi.top/gtmxbnbrhn.html

guard let x = opt else { return }
来源：http://hz.cdnleiting.top/gtdihmbrlm.html

[T30] Swift：协议
来源：http://hz.yueranfly.top/gteqfoqybc.html

protocol Shape { func area() -> Double }
来源：http://hz.jinqigfzy.top/gtoivojewa.html

[T31] Lua：Hello World
来源：http://hz.yj20258.top/gtsbscpawb.html

print("Hello")
来源：http://hz.cdnleiting.top/gtflgyswex.html

[T32] Lua：局部变量
来源：http://hz.316326.xyz/gtrsiuqpzc.html

local a = 1
来源：http://hz.zycfv.cn/gtiyidsbdd.html

[T33] Lua：表（数组）
来源：http://hz.zhiwuduotai.top/gtlbyhpxbf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yueranfly.top/gttwohkpvp.html

[T34] Lua：遍历表
来源：http://hz.pengpengdd.cyou/gtdblezkrz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.52xcode.cn/gtwpqbqmch.html

[T35] Lua：字典表
来源：http://hz.ehwqpu.com/gtuzywkhkm.html

local d = { a = 1 };  d.b = 2
来源：http://hz.c1oappe.top/gtirblkyaa.html

[T36] Lua：函数
来源：http://hz.316326.xyz/gtqlorpsnv.html

function add(a, b) return a + b end
来源：http://hz.wangshuangyany.cn/gtjkbytacg.html

[T37] Lua：字符串拼接
来源：http://hz.andypj.xyz/gtdbujwvra.html

"a" .. "b"
来源：http://hz.nanxinkj.top/gthdbqvgjg.html

[T38] Lua：条件
来源：http://hz.hammf.cn/gtlcxyzjbe.html

if x > 0 then print("正") end
来源：http://hz.guowangkeji.top/gtrccxuanu.html

[T39] Lua：模式匹配
来源：http://hz.snrcjt.cn/gttkrmtnti.html

string.find(s, "%d+")
来源：http://hz.pycfn.com/gtmarjtqvr.html

[T40] Lua：元表
来源：http://hz.iojbl.cn/gtxxfadevd.html

setmetatable({}, { __index = base })
来源：http://hz.hammf.cn/gtyuyugnby.html

[T41] Perl：Hello World
来源：http://hz.yj20258888.top/gtxsrsbhvm.html

print "Hello\n";
来源：http://hz.shanyushiyangtech.top/gtptdeisow.html

[T42] Perl：变量类型
来源：http://hz.shanyushiyangkeji.top/gtsjylbwzk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yj20258.top/gtujezrmaj.html

[T43] Perl：字符串插值
来源：http://hz.gotoacloud.top/gtcskrnzdr.html

"值: $a"
来源：http://hz.birdmap.top/gtwxulmdrc.html

[T44] Perl：条件
来源：http://hz.xuetiantiany.cn/gtthwrouio.html

if ($a > 0) { print "正"; }
来源：http://hz.hongshengwenyu.top/gtsfbwednh.html

[T45] Perl：数组遍历
来源：http://hz.haohaochexian.top/gtieymuqpl.html

for my $x (@arr) { print $x; }
来源：http://hz.fengsongda.top/gtsrqmdvzn.html

[T46] Perl：哈希操作
来源：http://hz.hnqzz.top/gtwetscvkg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.fzhhl.top/gtmvqjnvkg.html

[T47] Perl：正则捕获
来源：http://hz.jyoumei.cn/gtvixvrgzc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yj20258888.top/gtsxfvnrlp.html

[T48] Perl：正则替换
来源：http://hz.svipenyu.cn/gtgqmjqmrk.html

$s =~ s/old/new/g;
来源：http://hz.tianlin.xyz/gtltezsypo.html

[T49] Perl：函数
来源：http://hz.yuxming.cn/gtxodbfehh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.nanxuanxn.top/gtqaewuuiw.html

[T50] Perl：逐行读文件
来源：http://hz.9152youxi.cn/gtdvsemobq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.tian-w.cn/gtjzavmmqb.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.feifeiyinyue.top/gtbqmxgmmv.html

[T51] Scala：Hello World
来源：http://hz.xinyue.icu/gtrwvhhiju.html

println("Hello")
来源：http://hz.jinqigfzy.top/gtcrgtjfvu.html

[T52] Scala：变量
来源：http://hz.ehwqpu.com/gttsafuoew.html


<!-- 参考信息 -->