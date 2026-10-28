代发 wailian999

find . -name "*.tmp" -delete
来源：http://hz.ybcxt.top/gtlklrginj.html

[R46] 递归替换文件内容
来源：http://hz.yueranfly.top/gtovxdsscp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shzxlz.cn/gtxtbirkch.html

[R47] sed 单行替换
来源：http://hz.jinghuilouyu.cn/gtquyaautq.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.chenjidiqi.icu/gtzuvcvyji.html

[R48] awk 取指定列
来源：http://hz.jinqigufen.top/gtrzmqhenv.html

awk '{print $1, $3}' a.txt
来源：http://hz.gogol.net.cn/gtgzahjtqi.html

[R49] awk 带条件
来源：http://hz.zhongyouzk.top/gtubphavvm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.feifeiyinyue.top/gtdpinbwsf.html

[R50] awk 求和
来源：http://hz.kuanghao11.cn/gtcbyqghgs.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shzxlz.cn/gtgeuajyjr.html

[R51] 排序去重取前几
来源：http://hz.hysaishi.cn/gtfmgpokqn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hysaishi.cn/gtutescebq.html

[R52] 统计行数
来源：http://hz.zhoulong.xyz/gtmgmhjpfo.html

wc -l a.txt
来源：http://hz.aibaodan.cn/gtesmuyzto.html

[R53] 查看文件头与实时尾
来源：http://hz.gaohongyu789.top/gtqqiokvay.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yongpay.top/gtgesevzqz.html

[R54] 比较两个文件
来源：http://hz.meibo888.top/gtacbhxczw.html

diff a.txt b.txt
来源：http://hz.xinyue.icu/gtznfsgwst.html

[R55] 压缩与解压
来源：http://hz.yj202588.top/gtkknpzhia.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xuetiantiany.cn/gtxmnxdqpc.html

[R56] 远程拷贝
来源：http://hz.ydjk.org.cn/gtkdilqzpu.html

scp file user@host:/path/
来源：http://hz.ehwqpu.com/gtthcrfbpl.html

[R57] 远程执行命令
来源：http://hz.sysykeji.top/gtnfcztmhi.html

ssh user@host 'uptime'
来源：http://hz.xinyue.icu/gtgodjwtdv.html

[R58] 下载文件
来源：http://hz.ppjwa.cn/gtiqjzpisl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cucudq.cn/gtoaytzruv.html

[R59] 发 POST JSON
来源：http://hz.dashuyun.cn/gtmlelxrcp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.dashuyun.cn/gtldjpdhve.html

[R60] 只看 HTTP 状态码
来源：http://hz.jinqigufen.top/gtqmuavnop.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.aizwys.cn/gtxyzocuht.html

[R61] 磁盘占用
来源：http://hz.quarkkingdee.top/gtimcjkfmv.html

df -h;  du -sh *
来源：http://hz.snrcjt.cn/gtfzwvdnbt.html

[R62] 找最占空间的文件
来源：http://hz.yuxming.cn/gtntdlyjku.html

du -ah . | sort -rh | head -10
来源：http://hz.chenzaomai.com/gtjcauzrqo.html

[R63] 内存与进程
来源：http://hz.nanxinkj.top/gtyqbvawmj.html

free -h;  ps aux | grep nginx
来源：http://hz.zhoulong.xyz/gtjbxtyums.html

[R64] 结束进程
来源：http://hz.guannengcc.top/gtpbmwokkx.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yj20258888.top/gtezhpylyh.html

[R65] 查看端口占用
来源：http://hz.yueranfly.top/gtrmredjqw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.316326.xyz/gtaauftjmo.html

[R66] 定时任务
来源：http://hz.ybcxt.top/gtguqdhzvq.html

crontab -e;  crontab -l
来源：http://hz.gzhubu.top/gtbrfmyute.html

[R67] 生成随机十六进制串
来源：http://hz.chenzaomai.com/gtstbpxcjp.html

openssl rand -hex 16
来源：http://hz.yj20258.top/gtqgyzstxr.html

[R68] 计算文件校验值
来源：http://hz.ybcxt.top/gtaqqczbcv.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ybcxt.top/gtajqahbne.html

[R69] 生成随机密码
来源：http://hz.shanyushiyangtech.top/gtunnnddsi.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhijiandao.cn/gtjepmhbus.html

[R70] 时间戳与互转
来源：http://hz.wangdashe.top/gtqirkcvdt.html

date +%s;  date -d @1700000000
来源：http://hz.hysaishi.cn/gtkayrnyxn.html

[R71] 日期格式化
来源：http://hz.ppjwa.cn/gtswbddsry.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.aizwys.cn/gtvljdxwdz.html

[R72] 等待端口就绪
来源：http://hz.chenjidiqi.icu/gtlbvhtdcy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.redwolf501.top/gtkxghoiyd.html

[R73] 分割大日志
来源：http://hz.gotoacloud.top/gtzahhfyoj.html

split -l 1000 big.log part_
来源：http://hz.daria6918.cn/gtarpmheyh.html

[R74] 批量重命名
来源：http://hz.zhengqikj.top/gtgljaxpli.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shangyingyoupin.top/gtrcbfplnd.html

[R75] 导出环境变量
来源：http://hz.mhx1999.top/gtrtyxisll.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jyoumei.cn/gtlleqbmbt.html

[R76] 使用临时文件
来源：http://hz.yuanzhike.top/gtmfwhbiyw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.52xcode.cn/gtzuuzegkx.html

[R77] 读取用户输入
来源：http://hz.hnxiangtu.top/gtklnqdapd.html

read -rp "请输入: " ans
来源：http://hz.aibaodan.cn/gttlbgkvaf.html

[R78] 交互式菜单
来源：http://hz.dianchejie.cn/gtegrylzxe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hammf.cn/gtcydwbhxy.html

[R79] 解析命令行选项
来源：http://hz.shanyushiyangkeji.top/gtnvopmbvi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ehwqpu.com/gtfulepjir.html

[R80] 查看脚本执行耗时
来源：http://hz.cheryme.top/gtcmnfihnb.html

time ./run.sh
来源：http://hz.dianchejie.cn/gtnriugckj.html

================================================================================
来源：http://hz.sysykeji.top/gtdosdytgl.html

S. C / C++ 专题
来源：http://hz.zhixingplan.top/gtftnarxlf.html

================================================================================
来源：http://hz.sweek.top/gthchvjagu.html

[S01] C：Hello World
来源：http://hz.yueranfly.top/gtytizesqa.html

#include <stdio.h>
来源：http://hz.fengsongda.top/gtpuordcbd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.316326.xyz/gtrncsluwx.html

[S02] C：变量与格式化输出
来源：http://hz.ehwqpu.com/gtlnpsjlqn.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhiwuduotai.top/gtmbzcgtsy.html

[S03] C：读入整数
来源：http://hz.zdqjudy.top/gtzmscjymw.html

int x; scanf("%d", &x);
来源：http://hz.zhoulong.xyz/gtlsrniymn.html

[S04] C：字符串复制
来源：http://hz.fengsongda.top/gtzujwyatw.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.chenlongwang.top/gtsvuhwvxg.html

[S05] C：字符串长度
来源：http://hz.chenlongwang.top/gtegrijxft.html

strlen(s)
来源：http://hz.yvedp.cn/gtlhjzeumj.html

[S06] C：字符串比较
来源：http://hz.yangfankeji.com/gtgpctijpr.html

strcmp(a, b) == 0
来源：http://hz.jqgfzy.top/gtfdptpcpj.html

[S07] C：数组遍历求和
来源：http://hz.ywan-chungtsiang.top/gtydohgmhl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hnxiangtu.top/gtyxwkjmjp.html

[S08] C：动态内存分配与释放
来源：http://hz.redwolf501.top/gtsuzyhgrx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.quarkkingdee.top/gtmivkxdcd.html

[S09] C：结构体定义与初始化
来源：http://hz.jianghu66.top/gtorfkfufv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zdqjudy.top/gtundtyeve.html

[S10] C：指针与解引用
来源：http://hz.yongpay.top/gtwtyaqzuu.html

int *p = &a;  *p = 5;
来源：http://hz.nanxinkj.top/gtijpcfaft.html

[S11] C：逐行读文件
来源：http://hz.shzxlz.cn/gtpjdyrrdz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.c1oappe.top/gtuorynirb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.gogol.net.cn/gtjbczekuu.html

fclose(f);
来源：http://hz.snrcjt.cn/gtipyjtkze.html

[S12] C：写文件
来源：http://hz.shuidangran.top/gtjwephled.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.daxiang520.top/gtjactqmmb.html

[S13] C：宏定义
来源：http://hz.zhijiandao.cn/gtunfbqwbq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.guowangkeji.top/gtdzqabums.html

[S14] C：枚举
来源：http://hz.nanxinkj.top/gtywyzhuuy.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.nwbrower.top/gtpexepxth.html

[S15] C：类型转换
来源：http://hz.nwbrower.top/gtforewtyh.html

(double) a / b
来源：http://hz.cheryme.top/gtevacvumz.html

[S16] C：位操作置位
来源：http://hz.gzhubu.top/gtobnbbnsb.html

x |= (1 << 3);
来源：http://hz.9152youxi.cn/gtsdpcxrzt.html

[S17] C：安全拼接字符串
来源：http://hz.zycfv.cn/gthgdoeeap.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinghuilouyu.cn/gtextzyowe.html

[S18] C：命令行参数
来源：http://hz.hfpthk.cn/gtevcyacyf.html

int main(int argc, char **argv)
来源：http://hz.zhoulong.xyz/gthggokmtg.html

[S19] C：快速排序
来源：http://hz.gzhubu.top/gtjehbwvaw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.iojbl.cn/gtwzmkalck.html

[S20] C：二分查找
来源：http://hz.sweek.top/gttqelcpfy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yvedp.cn/gtbdqvykmt.html

[S21] C：字符类别判断
来源：http://hz.daria6918.cn/gtmqfxtcap.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.quarkkingdee.top/gtunscchec.html

[S22] C：字符串转数字
来源：http://hz.feifeiyinyue.top/gtmfjdfrto.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xylfe.cn/gtskmediyz.html

[S23] C：随机数
来源：http://hz.tanke756.top/gtnshbflbs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yangfankeji.com/gtnedljiyv.html

[S24] C：获取本地时间
来源：http://hz.shzxlz.cn/gtibzopxkg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hysaishi.cn/gtsgnsjdoa.html

[S25] C：内存拷贝
来源：http://hz.shuidangran.top/gtpiwlnzqy.html

memcpy(dst, src, n);
来源：http://hz.cdnleiting.top/gtsuaqlngt.html

[S26] C：内存清零
来源：http://hz.quarkkingdee.top/gtujqiyimz.html

memset(a, 0, sizeof a);
来源：http://hz.gzhubu.top/gtaehqwhal.html

[S27] C：定义常量
来源：http://hz.zhiwuduotai.top/gtorirmvmz.html

const double PI = 3.14159;
来源：http://hz.xuanzx.com/gtggtnesre.html

[S28] C：静态变量
来源：http://hz.xuanzx.com/gthalsncnm.html

static int counter = 0;
来源：http://hz.svipenyu.cn/gtwfvfsqyq.html

[S29] C：变参函数
来源：http://hz.zycfv.cn/gtckdkfpia.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shangyingyoupin.top/gtwjmbumxp.html

[S30] C：头文件保护
来源：http://hz.jqgufenzy.top/gtzhyphgvo.html

#ifndef X_H
来源：http://hz.sxryk.cn/gtbrfbubfa.html

#define X_H
来源：http://hz.sxryk.cn/gtspipkktq.html

#endif
来源：http://hz.cheryme.top/gtcxxkovhv.html

[S31] C++：Hello World
来源：http://hz.tian-w.cn/gtkgjhoihs.html

#include <iostream>
来源：http://hz.ywan-chungtsiang.top/gtoqzdavcc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jianghu66.top/gtyaaxvqjc.html

[S32] C++：字符串
来源：http://hz.yonumen.top/gteotgutyp.html

std::string s = "hi";  s += "!";
来源：http://hz.shzxlz.cn/gttbhlvcuh.html

[S33] C++：vector 增删
来源：http://hz.dashuyun.cn/gtovqxzjhl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xingfuxueyuan.xyz/gtgegenyse.html

[S34] C++：遍历 vector
来源：http://hz.cqqwz.cn/gtgxksyykz.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhixingplan.top/gthvkxxnzk.html

[S35] C++：map
来源：http://hz.svipenyu.cn/gtmxqqaoza.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xinyue.icu/gtelpxsrio.html

[S36] C++：unordered_map
来源：http://hz.yuxming.cn/gtxzhflfkh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.havefunace.top/gttdfvvhke.html

[S37] C++：set
来源：http://hz.yonumen.top/gtoaejccba.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cdnleiting.top/gtzxrwphdc.html

[S38] C++：排序
来源：http://hz.yj20258.top/gtxalirari.html

std::sort(v.begin(), v.end());
来源：http://hz.jqgfzy.top/gtaikkuaal.html

[S39] C++：自定义比较器排序
来源：http://hz.shzxlz.cn/gtefikrkul.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.dashuyun.cn/gtkzsmbyal.html

[S40] C++：查找元素
来源：http://hz.yj202588.top/gtadztimsz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xylfe.cn/gtcxvnvqeu.html

[S41] C++：类与构造函数
来源：http://hz.shuidangran.top/gtisvzsfga.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sweek.top/gtwnfpxfri.html

[S42] C++：继承与虚函数
来源：http://hz.jinqigfzy.top/gtxyisihmx.html

class B : public Base { public: void f() override {} };
来源：http://hz.shangyingyoupin.top/gtbvyxbncc.html

[S43] C++：智能指针
来源：http://hz.nanxinkj.top/gtyyntvxab.html

auto p = std::make_unique<int>(5);
来源：http://hz.shanyushiyangtech.top/gtbqrabhni.html

[S44] C++：引用传参
来源：http://hz.yueranfly.top/gtxwubogqu.html

void inc(int &x) { ++x; }
来源：http://hz.tian-w.cn/gtatliedsk.html

[S45] C++：lambda
来源：http://hz.tianlin.xyz/gtozccqalp.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yuxming.cn/gtrwuxuvnw.html

[S46] C++：函数模板
来源：http://hz.shzxlz.cn/gtvisllmow.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.nwbrower.top/gtrswmkscn.html

[S47] C++：结构化绑定遍历
来源：http://hz.cheryme.top/gtnybsztwp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.sufxvd.cn/gtwxytosjh.html

[S48] C++：逐行读文件
来源：http://hz.shanyushiyangtech.top/gtslpkhkqy.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.cashguo.top/gtgkzokhjq.html

while (std::getline(in, line)) { }
来源：http://hz.52xcode.cn/gtdwuvtbrk.html

[S49] C++：写文件
来源：http://hz.gaohongyu789.top/gtspgscqfb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.quarkkingdee.top/gtoanpkbjr.html

[S50] C++：格式化数字
来源：http://hz.zhongyouzk.top/gtdnxoerbl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.pengpengdd.cyou/gtkpsiidva.html

[S51] C++：显式类型转换
来源：http://hz.shanyushiyangkeji.top/gtpeuyzpue.html

static_cast<double>(a) / b
来源：http://hz.wangshuangyany.cn/gtibrnzldj.html

[S52] C++：const 与 noexcept
来源：http://hz.cucudq.cn/gtjcjexvug.html

int size() const noexcept { return n_; }
来源：http://hz.cqqwz.cn/gtwdalwwpz.html

[S53] C++：移动语义
来源：http://hz.sxryk.cn/gtoddrszwn.html

std::vector<int> w = std::move(v);
来源：http://hz.yuanzhike.top/gtztiwthsf.html

[S54] C++：异常处理
来源：http://hz.svipenyu.cn/gtpsnwhehx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.kuanghao11.cn/gtowuiucom.html

[S55] C++：结构化绑定
来源：http://hz.tanke756.top/gtwunjsrsf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhijiandao.cn/gtdetqsomz.html

[S56] C++：optional
来源：http://hz.zhiwuduotai.top/gtzuqctdci.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hfpthk.cn/gtjtlibeuo.html

[S57] C++：编译期常量
来源：http://hz.gogol.net.cn/gtevkmxyzf.html

constexpr int N = 10;
来源：http://hz.nwbrower.top/gtbtzmhzse.html

[S58] C++：命名空间
来源：http://hz.meibo888.top/gtsymntgly.html

namespace ns { int f() { return 1; } }
来源：http://hz.tianlin.xyz/gtcnpqqfdf.html

[S59] C++：静态断言
来源：http://hz.andypj.xyz/gtopntxglq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yj202588.top/gttdcyrkmz.html

[S60] C++：遍历并删除元素
来源：http://hz.ywan-chungtsiang.top/gtclaxprge.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.nanxuanxn.top/gtnyykkysx.html

================================================================================
来源：http://hz.yj202588.top/gtufwwahkd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.316326.xyz/gtefieaibp.html

================================================================================
来源：http://hz.tianlin.xyz/gtqolvhvkg.html

[T01] Kotlin：Hello World
来源：http://hz.cucudq.cn/gtnxkgblxy.html

println("Hello")
来源：http://hz.pycfn.com/gtvthaqrfg.html

[T02] Kotlin：变量
来源：http://hz.smart0.xyz/gtxenavasg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shuidangran.top/gtyhfndyiy.html

[T03] Kotlin：字符串模板
来源：http://hz.iojbl.cn/gtnmoqgloj.html

"值: $b"
来源：http://hz.xingfuxueyuan.xyz/gtmwslvjcw.html

[T04] Kotlin：空安全
来源：http://hz.gaohongyu789.top/gttwroiqfk.html

val n: String? = null;  n?.length
来源：http://hz.jinyuanbaomall.cn/gtmfndpzaz.html

[T05] Kotlin：when 表达式
来源：http://hz.daxiang520.top/gtmmtzzwty.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.haohaochexian.top/gtbzdvgygd.html

[T06] Kotlin：集合映射
来源：http://hz.316326.xyz/gtpuiesbmn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.316326.xyz/gtoywhgmzm.html

[T07] Kotlin：集合过滤
来源：http://hz.0kj1m.cn/gtkyibjeex.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hammf.cn/gtgdprcwxr.html

[T08] Kotlin：数据类
来源：http://hz.gzhubu.top/gtzxoukfmh.html

data class User(val name: String, val age: Int)
来源：http://hz.ehwqpu.com/gtsoswbeex.html

[T09] Kotlin：扩展函数
来源：http://hz.chenlongwang.top/gtcqtaehpz.html

fun String.exclaim() = this + "!"
来源：http://hz.ywan-chungtsiang.top/gtcgvxvtkj.html

[T10] Kotlin：默认参数
来源：http://hz.ybcxt.top/gtnzzmzela.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hywenlv.cn/gthbhripig.html

[T11] Kotlin：协程
来源：http://hz.dashuyun.cn/gtvtjnirrj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.fzhhl.top/gtzrkbecdq.html

[T12] Kotlin：解构声明
来源：http://hz.guannengcc.top/gtcihyhzgg.html

val (a, b) = Pair(1, 2)
来源：http://hz.yuxming.cn/gtiufvmroa.html

[T13] Kotlin：只读 Map
来源：http://hz.xylfe.cn/gtuxontguz.html

val m = mapOf("a" to 1)
来源：http://hz.tanke756.top/gtijfwppic.html

[T14] Kotlin：循环
来源：http://hz.yonumen.top/gtdmyfucyo.html

for (i in 1..10) println(i)
来源：http://hz.gotoacloud.top/gtnqhhacdv.html

[T15] Kotlin：接口
来源：http://hz.hongshengwenyu.top/gtjhfrluzb.html

interface Shape { fun area(): Double }
来源：http://hz.zhiwuduotai.top/gtxzaasavh.html

[T16] Swift：Hello World
来源：http://hz.ybcxt.top/gtuxmsoeyy.html

print("Hello")
来源：http://hz.jqgfzy.top/gtzekjdunz.html

[T17] Swift：变量与常量
来源：http://hz.jinqigfzy.top/gtuhlvvero.html

var a = 1;  let b = 2
来源：http://hz.jianghu66.top/gtqrcvmqzg.html

[T18] Swift：字符串插值
来源：http://hz.zhiwuduotai.top/gttliinrcr.html

"值: \(b)"
来源：http://hz.52xcode.cn/gtcnahpjre.html

[T19] Swift：可选绑定
来源：http://hz.vqdsnc.cn/gtukzsdziv.html

if let n = opt { print(n) }
来源：http://hz.yueranfly.top/gtvkphdfpy.html

[T20] Swift：数组操作
来源：http://hz.nanxinkj.top/gtkjpclzke.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zdqjudy.top/gtidqxpaiv.html

[T21] Swift：遍历
来源：http://hz.yangfankeji.com/gtwqicuxax.html

for x in a { print(x) }
来源：http://hz.jinqigfzy.top/gtjwkzqvcs.html

[T22] Swift：字典
来源：http://hz.redwolf501.top/gttlehjubl.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.iojbl.cn/gtjxyxdyye.html

[T23] Swift：函数
来源：http://hz.316326.xyz/gtxjdpfhba.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ivvv.top/gtpvllyxky.html

[T24] Swift：闭包
来源：http://hz.hfpthk.cn/gtdlrvnqjo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.mhx1999.top/gtsbiiichu.html

[T25] Swift：结构体
来源：http://hz.mhx1999.top/gttdwlhkaj.html

struct P { var x: Int }
来源：http://hz.xziqi.cn/gtvpjbtoay.html

[T26] Swift：类与重写
来源：http://hz.zhijiandao.cn/gtjfyogdmk.html

class A: Base { override func f() {} }
来源：http://hz.quarkkingdee.top/gtpyenjkwo.html

[T27] Swift：错误处理
来源：http://hz.hammf.cn/gtvpmaixma.html

do { try f() } catch { print(error) }
来源：http://hz.jianghu66.top/gtfttahmvh.html

[T28] Swift：枚举
来源：http://hz.hnqzz.top/gtescprgzv.html

enum Color { case red, green }
来源：http://hz.dianchejie.cn/gtltczmigv.html

[T29] Swift：guard 提前返回
来源：http://hz.yvedp.cn/gtjtyogemq.html

guard let x = opt else { return }
来源：http://hz.feifeiyinyue.top/gtfzlyhhju.html

[T30] Swift：协议
来源：http://hz.wangdashe.top/gtesbacbqf.html

protocol Shape { func area() -> Double }
来源：http://hz.wangshuangyany.cn/gtznlljicn.html

[T31] Lua：Hello World
来源：http://hz.sweek.top/gtjxfchyfg.html

print("Hello")
来源：http://hz.hywenlv.cn/gtcodfirit.html

[T32] Lua：局部变量
来源：http://hz.xingfuxueyuan.xyz/gtxqrydimr.html

local a = 1
来源：http://hz.hysaishi.cn/gtpxxjwlao.html

[T33] Lua：表（数组）
来源：http://hz.jyoumei.cn/gtkytkuhnz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yueranfly.top/gtjsriqrzy.html

[T34] Lua：遍历表
来源：http://hz.vqdsnc.cn/gtrxiaxeng.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.mhx1999.top/gtnvybcdkc.html

[T35] Lua：字典表
来源：http://hz.nwbrower.top/gtafofytel.html

local d = { a = 1 };  d.b = 2
来源：http://hz.andypj.xyz/gtefqmerwz.html

[T36] Lua：函数
来源：http://hz.redwolf501.top/gtirfzszza.html

function add(a, b) return a + b end
来源：http://hz.pycfn.com/gtrvotnxcn.html

[T37] Lua：字符串拼接
来源：http://hz.snrcjt.cn/gthiqkdbsq.html

"a" .. "b"
来源：http://hz.nanxuanxn.top/gtbtheufgb.html

[T38] Lua：条件
来源：http://hz.gzhubu.top/gtccbviscq.html

if x > 0 then print("正") end
来源：http://hz.jinyuanbaomall.cn/gtqyqhbgxo.html

[T39] Lua：模式匹配
来源：http://hz.daria6918.cn/gtnnsszrhl.html

string.find(s, "%d+")
来源：http://hz.hongshengwenyu.top/gtnpqpbzqy.html

[T40] Lua：元表
来源：http://hz.yuxming.cn/gttipeupay.html

setmetatable({}, { __index = base })
来源：http://hz.zhixingplan.top/gtmjqemzox.html

[T41] Perl：Hello World
来源：http://hz.smart0.xyz/gtwybmvxke.html

print "Hello\n";
来源：http://hz.jinqigfzy.top/gtlnvxguro.html

[T42] Perl：变量类型
来源：http://hz.nwbrower.top/gtvzrsxxij.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.mhx1999.top/gteqirkfzf.html

[T43] Perl：字符串插值
来源：http://hz.xingfuxueyuan.xyz/gtjmgcfnwu.html

"值: $a"
来源：http://hz.feifeiyinyue.top/gtvvxjsxoy.html

[T44] Perl：条件
来源：http://hz.c1oappe.top/gtfcutlkbb.html

if ($a > 0) { print "正"; }
来源：http://hz.sufxvd.cn/gtjkorbauw.html

[T45] Perl：数组遍历
来源：http://hz.yangfankeji.com/gtfilqhbcp.html

for my $x (@arr) { print $x; }
来源：http://hz.ivvv.top/gtzzpbprqo.html

[T46] Perl：哈希操作
来源：http://hz.yj20258888.top/gtxgccqpjc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.tanke756.top/gtnhniwoki.html

[T47] Perl：正则捕获
来源：http://hz.sxryk.cn/gtdcldjvzv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.chenzaomai.com/gteowocxpd.html

[T48] Perl：正则替换
来源：http://hz.ppjwa.cn/gthnxghtvi.html

$s =~ s/old/new/g;
来源：http://hz.aibaodan.cn/gtgmzcanox.html


<!-- 参考信息 -->