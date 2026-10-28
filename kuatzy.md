代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.meibo888.top/gtfsxkjgpz.html

[R36] 并发执行多个任务
来源：http://hz.0kj1m.cn/gtxgqeebry.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.chenzaomai.com/gttkmlkgvz.html

[R37] 把输出赋给变量
来源：http://hz.gotoacloud.top/gtuszgcdfz.html

files=$(ls -1)
来源：http://hz.xuetiantiany.cn/gtxjnldold.html

[R38] 管道串联
来源：http://hz.wangshuangyany.cn/gtylpxzcho.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ehwqpu.com/gtllwgpyyo.html

[R39] 重定向标准输出与错误
来源：http://hz.yangfankeji.com/gtucbiitgh.html

cmd > out.log 2>&1
来源：http://hz.dashuyun.cn/gtnrhbvvjj.html

[R40] 追加写日志
来源：http://hz.cashguo.top/gtmhttuxbu.html

echo "log" >> out.log
来源：http://hz.jianghu66.top/gtjnwblamd.html

[R41] 丢弃输出
来源：http://hz.zhengqikj.top/gtnoslrcqu.html

cmd >/dev/null 2>&1
来源：http://hz.tian-w.cn/gtitljgjqd.html

[R42] 输入重定向
来源：http://hz.kuanghao11.cn/gtxrsvffti.html

wc -l < a.txt
来源：http://hz.fengsongda.top/gtzhcldpmv.html

[R43] 按名字查找文件
来源：http://hz.jlsjyb.cn/gtzisyyibs.html

find . -name "*.log" -type f
来源：http://hz.jinghuilouyu.cn/gtzhpgbuqv.html

[R44] 按修改时间查找
来源：http://hz.yonumen.top/gtybecsrcj.html

find . -mtime -7 -type f
来源：http://hz.xylfe.cn/gtjtkqzlok.html

[R45] 批量删除
来源：http://hz.cqqwz.cn/gtbceygiwn.html

find . -name "*.tmp" -delete
来源：http://hz.c1oappe.top/gtiblsqdqd.html

[R46] 递归替换文件内容
来源：http://hz.zhongyouzk.top/gtyfnjucxr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.havefunace.top/gtwwrqdbcj.html

[R47] sed 单行替换
来源：http://hz.xuanzx.com/gtgadjmpyd.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yj202588.top/gtlachjowh.html

[R48] awk 取指定列
来源：http://hz.hongshengwenyu.top/gthgnhfwru.html

awk '{print $1, $3}' a.txt
来源：http://hz.hnqzz.top/gtxwzfkkfs.html

[R49] awk 带条件
来源：http://hz.wangshuangyany.cn/gtzmkfnica.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xuanzx.com/gtbchzqbuo.html

[R50] awk 求和
来源：http://hz.fengsongda.top/gtenercpah.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xuanzx.com/gtjiaccgfp.html

[R51] 排序去重取前几
来源：http://hz.daria6918.cn/gtxfdcqgng.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cdnleiting.top/gtnwdjwjuj.html

[R52] 统计行数
来源：http://hz.fengsongda.top/gthhwsqhil.html

wc -l a.txt
来源：http://hz.ehwqpu.com/gtxrwykyvj.html

[R53] 查看文件头与实时尾
来源：http://hz.ydjk.org.cn/gtonhdklhi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shuidangran.top/gtkdjtuouo.html

[R54] 比较两个文件
来源：http://hz.pycfn.com/gtywneiewg.html

diff a.txt b.txt
来源：http://hz.meibo888.top/gtysyqlciw.html

[R55] 压缩与解压
来源：http://hz.tanke756.top/gtvsnvcyqq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.9152youxi.cn/gtebzlyzbn.html

[R56] 远程拷贝
来源：http://hz.0kj1m.cn/gtiktlrzxg.html

scp file user@host:/path/
来源：http://hz.zhoulong.xyz/gtyayvthaf.html

[R57] 远程执行命令
来源：http://hz.jinghuilouyu.cn/gttdmgcffu.html

ssh user@host 'uptime'
来源：http://hz.svipenyu.cn/gtgmtybmtr.html

[R58] 下载文件
来源：http://hz.andypj.xyz/gtnmzacqse.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yanxiufei.cn/gtlvlroesz.html

[R59] 发 POST JSON
来源：http://hz.dashuyun.cn/gtldmwamhv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yangfankeji.com/gtbeblmhad.html

[R60] 只看 HTTP 状态码
来源：http://hz.jinqigufen.top/gtzemxrhdy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yvedp.cn/gtknstifue.html

[R61] 磁盘占用
来源：http://hz.dianchejie.cn/gtiucfvsom.html

df -h;  du -sh *
来源：http://hz.ydzc1.top/gtbohntazg.html

[R62] 找最占空间的文件
来源：http://hz.yj20258.top/gtxbwzcjjp.html

du -ah . | sort -rh | head -10
来源：http://hz.pengpengdd.cyou/gtjxqvsugw.html

[R63] 内存与进程
来源：http://hz.meibo888.top/gtjhqbftiz.html

free -h;  ps aux | grep nginx
来源：http://hz.zhaomingkeji.xyz/gtjitjqdly.html

[R64] 结束进程
来源：http://hz.yonumen.top/gtvskvcavh.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhiwuduotai.top/gtcvpnpfau.html

[R65] 查看端口占用
来源：http://hz.jinghuilouyu.cn/gteqcnrbpz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jqgfzy.top/gtmtsazgga.html

[R66] 定时任务
来源：http://hz.guowangkeji.top/gtpoispepw.html

crontab -e;  crontab -l
来源：http://hz.yangfankeji.com/gtavkjdsmj.html

[R67] 生成随机十六进制串
来源：http://hz.iojbl.cn/gtgueabomp.html

openssl rand -hex 16
来源：http://hz.tanke756.top/gtxjtlxjiv.html

[R68] 计算文件校验值
来源：http://hz.ppjwa.cn/gtvudaihpk.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jqgfzy.top/gtpwgvpxnj.html

[R69] 生成随机密码
来源：http://hz.cashguo.top/gtcfcwojgr.html

head -c 16 /dev/urandom | base64
来源：http://hz.jinyuanbaomall.cn/gtudiadkkz.html

[R70] 时间戳与互转
来源：http://hz.vqdsnc.cn/gtbtctdvxk.html

date +%s;  date -d @1700000000
来源：http://hz.ivvv.top/gtuyufriuc.html

[R71] 日期格式化
来源：http://hz.tian-w.cn/gtmnnyjisr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jinqigufen.top/gtylataqhe.html

[R72] 等待端口就绪
来源：http://hz.hysaishi.cn/gtrocnttmk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.c1oappe.top/gtmujjkfoa.html

[R73] 分割大日志
来源：http://hz.daria6918.cn/gttpztrtxs.html

split -l 1000 big.log part_
来源：http://hz.xingfuxueyuan.xyz/gtcbwawbvx.html

[R74] 批量重命名
来源：http://hz.ydzc1.top/gthosxnsqk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shanyushiyangtech.top/gtaogokziv.html

[R75] 导出环境变量
来源：http://hz.yuxming.cn/gtdwczzgat.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ydjk.org.cn/gttlvqsyah.html

[R76] 使用临时文件
来源：http://hz.yueranfly.top/gtwlkjzazy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.wangdashe.top/gthicogokq.html

[R77] 读取用户输入
来源：http://hz.nanxinkj.top/gtsdzvduty.html

read -rp "请输入: " ans
来源：http://hz.hywenlv.cn/gtfrcuniee.html

[R78] 交互式菜单
来源：http://hz.yangfankeji.com/gtpixgkwyr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.bjfxy.top/gtvutoykgo.html

[R79] 解析命令行选项
来源：http://hz.ehwqpu.com/gtcwwuqutl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.feifeiyinyue.top/gtfpmabzip.html

[R80] 查看脚本执行耗时
来源：http://hz.ppjwa.cn/gtsanidwac.html

time ./run.sh
来源：http://hz.cucudq.cn/gtpqhrgzmb.html

================================================================================
来源：http://hz.ybcxt.top/gthkjccyis.html

S. C / C++ 专题
来源：http://hz.ybcxt.top/gtdmfxjwzs.html

================================================================================
来源：http://hz.ehwqpu.com/gthqlzosmq.html

[S01] C：Hello World
来源：http://hz.tanke756.top/gtxytvpkgu.html

#include <stdio.h>
来源：http://hz.aibaodan.cn/gthgminwha.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.chenjidiqi.icu/gtncberehf.html

[S02] C：变量与格式化输出
来源：http://hz.gogol.net.cn/gtzosqlewu.html

int a = 10; printf("%d\n", a);
来源：http://hz.ivvv.top/gtdhkvsjvg.html

[S03] C：读入整数
来源：http://hz.quarkkingdee.top/gtbgofkdcp.html

int x; scanf("%d", &x);
来源：http://hz.ydjk.org.cn/gtaggyivyl.html

[S04] C：字符串复制
来源：http://hz.jiagoushi.top/gtiuindeeq.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jqgfzy.top/gtwcbypznk.html

[S05] C：字符串长度
来源：http://hz.zhaomingkeji.xyz/gtcgozexpy.html

strlen(s)
来源：http://hz.vqdsnc.cn/gtesxgjiwg.html

[S06] C：字符串比较
来源：http://hz.9152youxi.cn/gtsyxtqaal.html

strcmp(a, b) == 0
来源：http://hz.yonumen.top/gtuzldwcei.html

[S07] C：数组遍历求和
来源：http://hz.jinqigufen.top/gthwiwacns.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yanxiufei.cn/gtxckbinox.html

[S08] C：动态内存分配与释放
来源：http://hz.jinqigfzy.top/gtyppxkjdy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.316326.xyz/gtglbnnobz.html

[S09] C：结构体定义与初始化
来源：http://hz.52xcode.cn/gtlszacxhn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yj20258888.top/gtzrsxdelo.html

[S10] C：指针与解引用
来源：http://hz.cashguo.top/gtiptdcmtl.html

int *p = &a;  *p = 5;
来源：http://hz.meibo888.top/gtefblpnpg.html

[S11] C：逐行读文件
来源：http://hz.sysykeji.top/gtyqafonwl.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xziqi.cn/gtexejmeql.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.svipenyu.cn/gtluufasfz.html

fclose(f);
来源：http://hz.shuidangran.top/gtgnwfjlsl.html

[S12] C：写文件
来源：http://hz.0kj1m.cn/gtlnfyrkls.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hnxiangtu.top/gtdstttxqr.html

[S13] C：宏定义
来源：http://hz.chenlongwang.top/gtcchlhcjb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.chenzaomai.com/gtegkpgees.html

[S14] C：枚举
来源：http://hz.sufxvd.cn/gtelvyabwu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.chenjidiqi.icu/gttvbpdrdv.html

[S15] C：类型转换
来源：http://hz.tanke756.top/gtjeiwmpvu.html

(double) a / b
来源：http://hz.smart0.xyz/gtevfzebve.html

[S16] C：位操作置位
来源：http://hz.9152youxi.cn/gtrxjdumvu.html

x |= (1 << 3);
来源：http://hz.gzhubu.top/gtqysblqlc.html

[S17] C：安全拼接字符串
来源：http://hz.kuanghao11.cn/gtihuefyus.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jqgfzy.top/gtcbwupjvz.html

[S18] C：命令行参数
来源：http://hz.ehwqpu.com/gtzneboovo.html

int main(int argc, char **argv)
来源：http://hz.daxiang520.top/gtlhcuxobu.html

[S19] C：快速排序
来源：http://hz.wangdashe.top/gtpffwynbf.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.aibaodan.cn/gtvjfhjohc.html

[S20] C：二分查找
来源：http://hz.hnqzz.top/gtlveiwpyl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.tian-w.cn/gtzvibkcqj.html

[S21] C：字符类别判断
来源：http://hz.hammf.cn/gtibwandlh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.gogol.net.cn/gtmdhwmaiv.html

[S22] C：字符串转数字
来源：http://hz.ydzc1.top/gtaoizibxe.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yj20258888.top/gtbvkshgkf.html

[S23] C：随机数
来源：http://hz.cashguo.top/gtbtzyzydy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.havefunace.top/gtejwitsik.html

[S24] C：获取本地时间
来源：http://hz.cqqwz.cn/gtsrvqtabl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.nanxinkj.top/gtiffpjgfa.html

[S25] C：内存拷贝
来源：http://hz.yj20258888.top/gtkjmkhagc.html

memcpy(dst, src, n);
来源：http://hz.yangfankeji.com/gtldvbfdfg.html

[S26] C：内存清零
来源：http://hz.bjfxy.top/gtiofrybyo.html

memset(a, 0, sizeof a);
来源：http://hz.ydzc1.top/gtjpchjzcw.html

[S27] C：定义常量
来源：http://hz.smart0.xyz/gtrqmdpmoq.html

const double PI = 3.14159;
来源：http://hz.jinqigfzy.top/gtllhsznug.html

[S28] C：静态变量
来源：http://hz.zhengqikj.top/gtubrmbhgu.html

static int counter = 0;
来源：http://hz.yueranfly.top/gtxflkbhqh.html

[S29] C：变参函数
来源：http://hz.yuanzhike.top/gtizueunfv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.smart0.xyz/gtiqgvpkfp.html

[S30] C：头文件保护
来源：http://hz.jqgfzy.top/gtlyqyveyt.html

#ifndef X_H
来源：http://hz.fzhhl.top/gtxpzymrwq.html

#define X_H
来源：http://hz.guannengcc.top/gtqnehejhj.html

#endif
来源：http://hz.ydzc1.top/gtmwmsxgcg.html

[S31] C++：Hello World
来源：http://hz.jinqigufen.top/gtxcfywaaw.html

#include <iostream>
来源：http://hz.xuanzx.com/gtamqiibdj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yongpay.top/gtkmtxcngg.html

[S32] C++：字符串
来源：http://hz.daria6918.cn/gtkytmiwfq.html

std::string s = "hi";  s += "!";
来源：http://hz.birdmap.top/gtcouhzwqo.html

[S33] C++：vector 增删
来源：http://hz.snrcjt.cn/gtkvhgdlng.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.9152youxi.cn/gtzigcfcig.html

[S34] C++：遍历 vector
来源：http://hz.c1oappe.top/gthsbflplf.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.tianlin.xyz/gtxuhkkyiz.html

[S35] C++：map
来源：http://hz.pengpengdd.cyou/gtanahrrxa.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.fzhhl.top/gtjkrmrtrz.html

[S36] C++：unordered_map
来源：http://hz.jinghuilouyu.cn/gtqiyqckek.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.wangshuangyany.cn/gtskmlrmyp.html

[S37] C++：set
来源：http://hz.yuxming.cn/gtecuclyvq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.meibo888.top/gtubzvjhar.html

[S38] C++：排序
来源：http://hz.zhengqikj.top/gtbvoosogx.html

std::sort(v.begin(), v.end());
来源：http://hz.meibo888.top/gtcrlebuoc.html

[S39] C++：自定义比较器排序
来源：http://hz.gaohongyu789.top/gtptpuswuq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.nwbrower.top/gtyysrrawh.html

[S40] C++：查找元素
来源：http://hz.ydjk.org.cn/gtgwyribrn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.wangdashe.top/gtajltbolh.html

[S41] C++：类与构造函数
来源：http://hz.ydjk.org.cn/gtbqlqgerc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.c1oappe.top/gtrfbbnpei.html

[S42] C++：继承与虚函数
来源：http://hz.cqqwz.cn/gtjoudwwwb.html

class B : public Base { public: void f() override {} };
来源：http://hz.yvedp.cn/gtypbhuifi.html

[S43] C++：智能指针
来源：http://hz.gogol.net.cn/gtrisncbsa.html

auto p = std::make_unique<int>(5);
来源：http://hz.xingfuxueyuan.xyz/gtlhuycndx.html

[S44] C++：引用传参
来源：http://hz.jinyuanbaomall.cn/gtlbpvsmiy.html

void inc(int &x) { ++x; }
来源：http://hz.cqqwz.cn/gtwmvgeefw.html

[S45] C++：lambda
来源：http://hz.chenjidiqi.icu/gtvtlrjdmk.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xylfe.cn/gtglnqjybu.html

[S46] C++：函数模板
来源：http://hz.tian-w.cn/gtenytdhhy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jiagoushi.top/gtcwlmdtaf.html

[S47] C++：结构化绑定遍历
来源：http://hz.smart0.xyz/gtsxxkfnjk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhiwuduotai.top/gtqnkarrxx.html

[S48] C++：逐行读文件
来源：http://hz.gotoacloud.top/gtxckvxkrh.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.pengpengdd.cyou/gtmzwssarn.html

while (std::getline(in, line)) { }
来源：http://hz.tian-w.cn/gttkygtish.html

[S49] C++：写文件
来源：http://hz.iojbl.cn/gtkdoqnzae.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jinghuilouyu.cn/gtmgjctzvk.html

[S50] C++：格式化数字
来源：http://hz.tian-w.cn/gtliliyffp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ydzc1.top/gtftsaoolw.html

[S51] C++：显式类型转换
来源：http://hz.wangdashe.top/gtcywqeecm.html

static_cast<double>(a) / b
来源：http://hz.guannengcc.top/gtcvwknmri.html

[S52] C++：const 与 noexcept
来源：http://hz.jinghuilouyu.cn/gtoadnkrbm.html

int size() const noexcept { return n_; }
来源：http://hz.yanxiufei.cn/gtskmewptv.html

[S53] C++：移动语义
来源：http://hz.dianchejie.cn/gtbssulguh.html

std::vector<int> w = std::move(v);
来源：http://hz.yanxiufei.cn/gttlsifxcc.html

[S54] C++：异常处理
来源：http://hz.xingfuxueyuan.xyz/gtuwbnjjsj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ivvv.top/gtmuxnhwzj.html

[S55] C++：结构化绑定
来源：http://hz.cucudq.cn/gtklgljlcb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.fzhhl.top/gtzgetbmfb.html

[S56] C++：optional
来源：http://hz.meibo888.top/gtxiaawrte.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xuetiantiany.cn/gtcgwybtbn.html

[S57] C++：编译期常量
来源：http://hz.hywenlv.cn/gtovsbpfer.html

constexpr int N = 10;
来源：http://hz.haohaochexian.top/gtuqxkthaa.html

[S58] C++：命名空间
来源：http://hz.hammf.cn/gtwlmpllsh.html

namespace ns { int f() { return 1; } }
来源：http://hz.shuidangran.top/gtcpqmghle.html

[S59] C++：静态断言
来源：http://hz.cheryme.top/gtnmrpxjht.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sweek.top/gtimbpcfin.html

[S60] C++：遍历并删除元素
来源：http://hz.chenjidiqi.icu/gtgvfjbewt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yvedp.cn/gthkfdussq.html

================================================================================
来源：http://hz.yj20258.top/gtpksmhatc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinyuanbaomall.cn/gthkcxxdon.html

================================================================================
来源：http://hz.cheryme.top/gtdzrbwtvs.html

[T01] Kotlin：Hello World
来源：http://hz.dianchejie.cn/gtiepltcuk.html

println("Hello")
来源：http://hz.dashuyun.cn/gtjgusqqmh.html

[T02] Kotlin：变量
来源：http://hz.cqqwz.cn/gtyuthpsuv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.sxryk.cn/gtabckfzbc.html

[T03] Kotlin：字符串模板
来源：http://hz.jianghu66.top/gtppkrpbup.html

"值: $b"
来源：http://hz.0kj1m.cn/gttufydwln.html

[T04] Kotlin：空安全
来源：http://hz.haohaochexian.top/gtphffobvx.html

val n: String? = null;  n?.length
来源：http://hz.havefunace.top/gtmoomyecc.html

[T05] Kotlin：when 表达式
来源：http://hz.nanxinkj.top/gtzrvjuurq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.pycfn.com/gtjefshajy.html

[T06] Kotlin：集合映射
来源：http://hz.quarkkingdee.top/gtbxdexzhn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhixingplan.top/gtjjmvtcpj.html

[T07] Kotlin：集合过滤
来源：http://hz.shanyushiyangkeji.top/gtivmtzrwe.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhixingplan.top/gtyffvepbl.html

[T08] Kotlin：数据类
来源：http://hz.hongshengwenyu.top/gtjfpkwkbd.html

data class User(val name: String, val age: Int)
来源：http://hz.yuanzhike.top/gtvdpeekdd.html

[T09] Kotlin：扩展函数
来源：http://hz.yonumen.top/gtovsljshq.html

fun String.exclaim() = this + "!"
来源：http://hz.yuanzhike.top/gtxqkaqaou.html

[T10] Kotlin：默认参数
来源：http://hz.wangshuangyany.cn/gtpkivxvjm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.aizwys.cn/gtpycwrnod.html

[T11] Kotlin：协程
来源：http://hz.chenzaomai.com/gtszclwzzr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.aibaodan.cn/gtcsflbvpu.html

[T12] Kotlin：解构声明
来源：http://hz.sweek.top/gtkenjqlik.html

val (a, b) = Pair(1, 2)
来源：http://hz.pycfn.com/gtkvvgquky.html

[T13] Kotlin：只读 Map
来源：http://hz.guowangkeji.top/gtxmndblea.html

val m = mapOf("a" to 1)
来源：http://hz.jianghu66.top/gtfehvlfrj.html

[T14] Kotlin：循环
来源：http://hz.gzhubu.top/gtlwnoraap.html

for (i in 1..10) println(i)
来源：http://hz.yvedp.cn/gtipkkeacq.html

[T15] Kotlin：接口
来源：http://hz.zhijiandao.cn/gtyxqjquhp.html

interface Shape { fun area(): Double }
来源：http://hz.cucudq.cn/gtlywwuqrr.html

[T16] Swift：Hello World
来源：http://hz.nwbrower.top/gtbuktbzlj.html

print("Hello")
来源：http://hz.birdmap.top/gtcsuplfvl.html

[T17] Swift：变量与常量
来源：http://hz.jinghuilouyu.cn/gtuxajjvkk.html

var a = 1;  let b = 2
来源：http://hz.havefunace.top/gtahvpfsqf.html

[T18] Swift：字符串插值
来源：http://hz.shanyushiyangkeji.top/gtrsobeeik.html

"值: \(b)"
来源：http://hz.xuanzx.com/gtjenhxuez.html

[T19] Swift：可选绑定
来源：http://hz.yj20258.top/gtybqbkpro.html

if let n = opt { print(n) }
来源：http://hz.andypj.xyz/gtkoermszv.html

[T20] Swift：数组操作
来源：http://hz.tanke756.top/gtopwupees.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.pengpengdd.cyou/gtynphxvys.html

[T21] Swift：遍历
来源：http://hz.zhongyouzk.top/gtgegzftzv.html

for x in a { print(x) }
来源：http://hz.xylfe.cn/gtztubkzsk.html

[T22] Swift：字典
来源：http://hz.zycfv.cn/gtifldcayw.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ywan-chungtsiang.top/gtxzbufnxt.html

[T23] Swift：函数
来源：http://hz.ydzc1.top/gtxrfpwaui.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yanxiufei.cn/gterqzpbna.html

[T24] Swift：闭包
来源：http://hz.jqgufenzy.top/gtonbvpsmn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.cheryme.top/gtqhcyggzc.html

[T25] Swift：结构体
来源：http://hz.wangdashe.top/gtlqcksiji.html

struct P { var x: Int }
来源：http://hz.yuanzhike.top/gtuzivaoiv.html

[T26] Swift：类与重写
来源：http://hz.yongpay.top/gtdxgscnah.html

class A: Base { override func f() {} }
来源：http://hz.hfpthk.cn/gtgzrjaoqz.html

[T27] Swift：错误处理
来源：http://hz.tanke756.top/gtfrgazsge.html

do { try f() } catch { print(error) }
来源：http://hz.cdnleiting.top/gtfwdjzsfv.html

[T28] Swift：枚举
来源：http://hz.hfpthk.cn/gtpdrtnkrw.html

enum Color { case red, green }
来源：http://hz.dianchejie.cn/gtwyhkdptc.html

[T29] Swift：guard 提前返回
来源：http://hz.daxiang520.top/gtyykhakhf.html

guard let x = opt else { return }
来源：http://hz.wangdashe.top/gtswzwduur.html

[T30] Swift：协议
来源：http://hz.jiagoushi.top/gtfvkwdcmp.html

protocol Shape { func area() -> Double }
来源：http://hz.shanyushiyangkeji.top/gtykyxwgyc.html

[T31] Lua：Hello World
来源：http://hz.hysaishi.cn/gtygiphyai.html

print("Hello")
来源：http://hz.nanxuanxn.top/gtxjrjtgzp.html

[T32] Lua：局部变量
来源：http://hz.tian-w.cn/gtnkzoizzg.html

local a = 1
来源：http://hz.daria6918.cn/gthfcovkzd.html

[T33] Lua：表（数组）
来源：http://hz.fengsongda.top/gtkofcqufn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yangfankeji.com/gtvtejhkme.html

[T34] Lua：遍历表
来源：http://hz.sufxvd.cn/gtghdjtfca.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.aibaodan.cn/gtoqoidvtl.html

[T35] Lua：字典表
来源：http://hz.redwolf501.top/gtymhyyqtu.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ehwqpu.com/gthnstclvw.html

[T36] Lua：函数
来源：http://hz.snrcjt.cn/gtapzkmord.html

function add(a, b) return a + b end
来源：http://hz.yuanzhike.top/gtwrkhxovi.html

[T37] Lua：字符串拼接
来源：http://hz.jinqigfzy.top/gtwmvgyaql.html

"a" .. "b"
来源：http://hz.0kj1m.cn/gtwcosuyho.html

[T38] Lua：条件
来源：http://hz.gotoacloud.top/gtueisfust.html

if x > 0 then print("正") end
来源：http://hz.jqgufenzy.top/gtccwvnoup.html


<!-- 参考信息 -->