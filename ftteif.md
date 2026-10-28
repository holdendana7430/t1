代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.pengpengdd.cyou/gtjvmvkamf.html

[R36] 并发执行多个任务
来源：http://hz.jinqigufen.top/gtzpixcjmi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.smart0.xyz/gtkhtitwmo.html

[R37] 把输出赋给变量
来源：http://hz.hfpthk.cn/gttexzclxg.html

files=$(ls -1)
来源：http://hz.hongshengwenyu.top/gttcfavmiw.html

[R38] 管道串联
来源：http://hz.mhx1999.top/gtqzbzlfbl.html

cat a.txt | grep -i error | wc -l
来源：http://hz.tianlin.xyz/gtypwwdtiy.html

[R39] 重定向标准输出与错误
来源：http://hz.shangyingyoupin.top/gtmdaccxcn.html

cmd > out.log 2>&1
来源：http://hz.meibo888.top/gtavngpklu.html

[R40] 追加写日志
来源：http://hz.jinqigufen.top/gthgmgscrt.html

echo "log" >> out.log
来源：http://hz.zhiwuduotai.top/gtqnlekwss.html

[R41] 丢弃输出
来源：http://hz.daria6918.cn/gtwpeaijmy.html

cmd >/dev/null 2>&1
来源：http://hz.ivvv.top/gtwqldmznu.html

[R42] 输入重定向
来源：http://hz.hnqzz.top/gtcxnhyheh.html

wc -l < a.txt
来源：http://hz.sufxvd.cn/gtgdghjjqt.html

[R43] 按名字查找文件
来源：http://hz.yvedp.cn/gttxhszfej.html

find . -name "*.log" -type f
来源：http://hz.sufxvd.cn/gtzlhdqwcv.html

[R44] 按修改时间查找
来源：http://hz.tian-w.cn/gtyccavolc.html

find . -mtime -7 -type f
来源：http://hz.xylfe.cn/gtchtnqdgs.html

[R45] 批量删除
来源：http://hz.hammf.cn/gtgscqgyax.html

find . -name "*.tmp" -delete
来源：http://hz.hfpthk.cn/gtnpelgyxq.html

[R46] 递归替换文件内容
来源：http://hz.xuanzx.com/gtohmczmpw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.9152youxi.cn/gtmbuydcqc.html

[R47] sed 单行替换
来源：http://hz.gogol.net.cn/gtbqcbldoj.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hongshengwenyu.top/gtdzxsemqx.html

[R48] awk 取指定列
来源：http://hz.nanxuanxn.top/gthptyffzd.html

awk '{print $1, $3}' a.txt
来源：http://hz.haohaochexian.top/gtehyqrhtf.html

[R49] awk 带条件
来源：http://hz.xinyue.icu/gtstpiople.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xinyue.icu/gtmyxwlvky.html

[R50] awk 求和
来源：http://hz.ydzc1.top/gtpwhopjbh.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cdnleiting.top/gtxjcyddke.html

[R51] 排序去重取前几
来源：http://hz.yj202588.top/gtusdijtmg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zycfv.cn/gthvbnwlyo.html

[R52] 统计行数
来源：http://hz.jqgfzy.top/gtaczpzfvl.html

wc -l a.txt
来源：http://hz.zhoulong.xyz/gtcleigfvj.html

[R53] 查看文件头与实时尾
来源：http://hz.ivvv.top/gtrwklepcw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jianghu66.top/gtcmjaoklo.html

[R54] 比较两个文件
来源：http://hz.ydzc1.top/gtqyjgyotv.html

diff a.txt b.txt
来源：http://hz.xylfe.cn/gtdnbappuj.html

[R55] 压缩与解压
来源：http://hz.jinyuanbaomall.cn/gtppjjdmwz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.guowangkeji.top/gttocwhnuj.html

[R56] 远程拷贝
来源：http://hz.shanyushiyangkeji.top/gtdrsbchak.html

scp file user@host:/path/
来源：http://hz.shanyushiyangkeji.top/gteveetnqf.html

[R57] 远程执行命令
来源：http://hz.guowangkeji.top/gtqqqkjgrp.html

ssh user@host 'uptime'
来源：http://hz.xuanzx.com/gtllwtzrah.html

[R58] 下载文件
来源：http://hz.zhijiandao.cn/gtvabgqres.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinyuanbaomall.cn/gtoofplgsn.html

[R59] 发 POST JSON
来源：http://hz.sweek.top/gtpijetzuk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinqigfzy.top/gtcfkpdfbg.html

[R60] 只看 HTTP 状态码
来源：http://hz.wangdashe.top/gtqkyjjwsy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.tian-w.cn/gtrinupqml.html

[R61] 磁盘占用
来源：http://hz.zhijiandao.cn/gtzcxqjpgm.html

df -h;  du -sh *
来源：http://hz.yongpay.top/gtjhfvrjbm.html

[R62] 找最占空间的文件
来源：http://hz.cdnleiting.top/gtbksplfyi.html

du -ah . | sort -rh | head -10
来源：http://hz.jinghuilouyu.cn/gtbspjramf.html

[R63] 内存与进程
来源：http://hz.shanyushiyangtech.top/gtlpkxqxpi.html

free -h;  ps aux | grep nginx
来源：http://hz.feifeiyinyue.top/gtmxkblacy.html

[R64] 结束进程
来源：http://hz.xziqi.cn/gtuhwjvqec.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shangyingyoupin.top/gtbbhteftl.html

[R65] 查看端口占用
来源：http://hz.cqqwz.cn/gtfhiabcze.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jiagoushi.top/gtkpcryaqh.html

[R66] 定时任务
来源：http://hz.jinghuilouyu.cn/gtjklufgeu.html

crontab -e;  crontab -l
来源：http://hz.yangfankeji.com/gtiaosbaua.html

[R67] 生成随机十六进制串
来源：http://hz.dashuyun.cn/gtweykibla.html

openssl rand -hex 16
来源：http://hz.daxiang520.top/gtoqprouqu.html

[R68] 计算文件校验值
来源：http://hz.jianghu66.top/gtwcrrytog.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.smart0.xyz/gtagltzjvl.html

[R69] 生成随机密码
来源：http://hz.fengsongda.top/gtxbpqoxdz.html

head -c 16 /dev/urandom | base64
来源：http://hz.c1oappe.top/gtnxnqemzl.html

[R70] 时间戳与互转
来源：http://hz.pengpengdd.cyou/gtfbmytcuc.html

date +%s;  date -d @1700000000
来源：http://hz.pengpengdd.cyou/gtydwoghhv.html

[R71] 日期格式化
来源：http://hz.gaohongyu789.top/gtwslpsemx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.316326.xyz/gtxcdczwwu.html

[R72] 等待端口就绪
来源：http://hz.jinghuilouyu.cn/gtjurwrjgh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.vqdsnc.cn/gtrihkwgok.html

[R73] 分割大日志
来源：http://hz.hywenlv.cn/gtecvzefrb.html

split -l 1000 big.log part_
来源：http://hz.guowangkeji.top/gtkptbffqd.html

[R74] 批量重命名
来源：http://hz.hnxiangtu.top/gtwsfmzkld.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xylfe.cn/gtguxztvsl.html

[R75] 导出环境变量
来源：http://hz.ivvv.top/gtiuaamkrw.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.tanke756.top/gtlyddnajo.html

[R76] 使用临时文件
来源：http://hz.tian-w.cn/gtbeotaesb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenlongwang.top/gtfcocaaoe.html

[R77] 读取用户输入
来源：http://hz.9152youxi.cn/gtkjpzgeoa.html

read -rp "请输入: " ans
来源：http://hz.pengpengdd.cyou/gtphgvnavh.html

[R78] 交互式菜单
来源：http://hz.tianlin.xyz/gttplqmego.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.daxiang520.top/gtsgbdsmib.html

[R79] 解析命令行选项
来源：http://hz.shanyushiyangkeji.top/gtfrijfjtx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sufxvd.cn/gtbswhsqwa.html

[R80] 查看脚本执行耗时
来源：http://hz.zhijiandao.cn/gtpffjtvqt.html

time ./run.sh
来源：http://hz.jyoumei.cn/gtmliqtmwx.html

================================================================================
来源：http://hz.dashuyun.cn/gttdadxeug.html

S. C / C++ 专题
来源：http://hz.xylfe.cn/gtojcdwgnm.html

================================================================================
来源：http://hz.gogol.net.cn/gtnrokhdkf.html

[S01] C：Hello World
来源：http://hz.hywenlv.cn/gtzbsyeiya.html

#include <stdio.h>
来源：http://hz.zhixingplan.top/gtqkzxtveg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.dianchejie.cn/gtgocmbtcx.html

[S02] C：变量与格式化输出
来源：http://hz.aibaodan.cn/gtyjokjqgn.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhongyouzk.top/gtzwajnqzb.html

[S03] C：读入整数
来源：http://hz.hnqzz.top/gttgxfwdrm.html

int x; scanf("%d", &x);
来源：http://hz.yangfankeji.com/gtwqgqhwch.html

[S04] C：字符串复制
来源：http://hz.ydjk.org.cn/gtsrvgmdzy.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yanxiufei.cn/gtsycghuei.html

[S05] C：字符串长度
来源：http://hz.nanxinkj.top/gtsymzgedg.html

strlen(s)
来源：http://hz.yj20258.top/gtlucjqoja.html

[S06] C：字符串比较
来源：http://hz.snrcjt.cn/gtptkleamd.html

strcmp(a, b) == 0
来源：http://hz.daria6918.cn/gteezlhrly.html

[S07] C：数组遍历求和
来源：http://hz.hammf.cn/gtonffuvof.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yongpay.top/gtzvdrxivu.html

[S08] C：动态内存分配与释放
来源：http://hz.cqqwz.cn/gturuztaas.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.guowangkeji.top/gtqzsusogz.html

[S09] C：结构体定义与初始化
来源：http://hz.ybcxt.top/gtxnzfwbzb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.daxiang520.top/gtqyqczslr.html

[S10] C：指针与解引用
来源：http://hz.wangshuangyany.cn/gtojzxpwkp.html

int *p = &a;  *p = 5;
来源：http://hz.c1oappe.top/gtdqvadmkr.html

[S11] C：逐行读文件
来源：http://hz.xylfe.cn/gtuzjbwhri.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xuanzx.com/gtashqhjbo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.c1oappe.top/gtkthygcnj.html

fclose(f);
来源：http://hz.ppjwa.cn/gtyemrexea.html

[S12] C：写文件
来源：http://hz.zhongyouzk.top/gtllklrrhu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xinyue.icu/gtppbbkgbb.html

[S13] C：宏定义
来源：http://hz.shzxlz.cn/gtvswjsqrv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yvedp.cn/gtvvuclujp.html

[S14] C：枚举
来源：http://hz.cqqwz.cn/gtfjntzldp.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.bjfxy.top/gtvjayvnhz.html

[S15] C：类型转换
来源：http://hz.bjfxy.top/gteseugeid.html

(double) a / b
来源：http://hz.jqgfzy.top/gtwpgwzxbm.html

[S16] C：位操作置位
来源：http://hz.mhx1999.top/gtxgewfylw.html

x |= (1 << 3);
来源：http://hz.jlsjyb.cn/gtcgasqoob.html

[S17] C：安全拼接字符串
来源：http://hz.316326.xyz/gtlltljbdl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yvedp.cn/gtkoscngxy.html

[S18] C：命令行参数
来源：http://hz.jianghu66.top/gtojalyrje.html

int main(int argc, char **argv)
来源：http://hz.jqgfzy.top/gtnyjgrtfi.html

[S19] C：快速排序
来源：http://hz.xziqi.cn/gtsaemhqdv.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.sxryk.cn/gtpubwuwbz.html

[S20] C：二分查找
来源：http://hz.yangfankeji.com/gtiypqnooh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.andypj.xyz/gtibdlhuvh.html

[S21] C：字符类别判断
来源：http://hz.cashguo.top/gtugigftlo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.nwbrower.top/gtpcfbwmxu.html

[S22] C：字符串转数字
来源：http://hz.chenlongwang.top/gtmuujmijf.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.sxryk.cn/gtvcoxayef.html

[S23] C：随机数
来源：http://hz.wangshuangyany.cn/gtvvnbvfwk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yanxiufei.cn/gtpcggltdv.html

[S24] C：获取本地时间
来源：http://hz.cucudq.cn/gtgiwjcggu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.sxryk.cn/gtskufrvsj.html

[S25] C：内存拷贝
来源：http://hz.jiagoushi.top/gtcisyljje.html

memcpy(dst, src, n);
来源：http://hz.cashguo.top/gtjcxhjpen.html

[S26] C：内存清零
来源：http://hz.316326.xyz/gtdztkqmny.html

memset(a, 0, sizeof a);
来源：http://hz.xuanzx.com/gtsthutqis.html

[S27] C：定义常量
来源：http://hz.yvedp.cn/gtiufnohhv.html

const double PI = 3.14159;
来源：http://hz.zhengqikj.top/gtozvwasim.html

[S28] C：静态变量
来源：http://hz.shzxlz.cn/gtqevelxui.html

static int counter = 0;
来源：http://hz.ybcxt.top/gthynsxsws.html

[S29] C：变参函数
来源：http://hz.fengsongda.top/gtglrufoho.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yonumen.top/gtcexpnxly.html

[S30] C：头文件保护
来源：http://hz.iojbl.cn/gtqxcgjrue.html

#ifndef X_H
来源：http://hz.yuxming.cn/gtqjzkrtbg.html

#define X_H
来源：http://hz.svipenyu.cn/gtafpzbzrz.html

#endif
来源：http://hz.cucudq.cn/gtiifkvgpd.html

[S31] C++：Hello World
来源：http://hz.9152youxi.cn/gtbjqbudll.html

#include <iostream>
来源：http://hz.quarkkingdee.top/gtqmoyhmxc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xuetiantiany.cn/gtplvwdius.html

[S32] C++：字符串
来源：http://hz.iojbl.cn/gtouqmcrrg.html

std::string s = "hi";  s += "!";
来源：http://hz.yvedp.cn/gtfndmuyvu.html

[S33] C++：vector 增删
来源：http://hz.chenzaomai.com/gtximzgdhd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yueranfly.top/gtpqpvqfzk.html

[S34] C++：遍历 vector
来源：http://hz.shanyushiyangtech.top/gtremceipp.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.gogol.net.cn/gtbceflsbd.html

[S35] C++：map
来源：http://hz.jinqigufen.top/gtjrtvtrkd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ybcxt.top/gtbqvxhwmc.html

[S36] C++：unordered_map
来源：http://hz.ywan-chungtsiang.top/gtkvxpyvbg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shzxlz.cn/gtfuzyxpsd.html

[S37] C++：set
来源：http://hz.ehwqpu.com/gtozwvtyfu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.nanxuanxn.top/gtfvryjlfd.html

[S38] C++：排序
来源：http://hz.ybcxt.top/gthncijmuo.html

std::sort(v.begin(), v.end());
来源：http://hz.guannengcc.top/gtvmfrhaaj.html

[S39] C++：自定义比较器排序
来源：http://hz.sufxvd.cn/gtzbdfnlsv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.daria6918.cn/gtuaikljqg.html

[S40] C++：查找元素
来源：http://hz.xziqi.cn/gtbupuyrrv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shuidangran.top/gtohktaxuy.html

[S41] C++：类与构造函数
来源：http://hz.9152youxi.cn/gtvlkpmvib.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.gotoacloud.top/gtlhccrsvo.html

[S42] C++：继承与虚函数
来源：http://hz.andypj.xyz/gtmpkqscoq.html

class B : public Base { public: void f() override {} };
来源：http://hz.birdmap.top/gtffrmhocd.html

[S43] C++：智能指针
来源：http://hz.hongshengwenyu.top/gtuijdhima.html

auto p = std::make_unique<int>(5);
来源：http://hz.pengpengdd.cyou/gtuerntivl.html

[S44] C++：引用传参
来源：http://hz.dashuyun.cn/gtsqhgnjun.html

void inc(int &x) { ++x; }
来源：http://hz.shanyushiyangkeji.top/gtinmpufvp.html

[S45] C++：lambda
来源：http://hz.316326.xyz/gtxrxqvuka.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.smart0.xyz/gtcjgztnwc.html

[S46] C++：函数模板
来源：http://hz.yuxming.cn/gttcckqflt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.9152youxi.cn/gtybdvpjoo.html

[S47] C++：结构化绑定遍历
来源：http://hz.andypj.xyz/gtwdxqjhbb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.sweek.top/gtleuazlan.html

[S48] C++：逐行读文件
来源：http://hz.ywan-chungtsiang.top/gtllvhnyji.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zycfv.cn/gtfczpffvt.html

while (std::getline(in, line)) { }
来源：http://hz.hywenlv.cn/gtshucnzdt.html

[S49] C++：写文件
来源：http://hz.ydjk.org.cn/gtnmefdnxy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.daxiang520.top/gtwhmcyapb.html

[S50] C++：格式化数字
来源：http://hz.chenjidiqi.icu/gtnstojmfl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhengqikj.top/gtvojxvvdu.html

[S51] C++：显式类型转换
来源：http://hz.xziqi.cn/gtwzldwudh.html

static_cast<double>(a) / b
来源：http://hz.gzhubu.top/gtxdprjujg.html

[S52] C++：const 与 noexcept
来源：http://hz.tianlin.xyz/gtitjzkpmv.html

int size() const noexcept { return n_; }
来源：http://hz.smart0.xyz/gtxxhgkncr.html

[S53] C++：移动语义
来源：http://hz.shangyingyoupin.top/gtllokqmxa.html

std::vector<int> w = std::move(v);
来源：http://hz.pycfn.com/gtorsajoux.html

[S54] C++：异常处理
来源：http://hz.jlsjyb.cn/gtpqtvsfms.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hongshengwenyu.top/gtrarhkmen.html

[S55] C++：结构化绑定
来源：http://hz.ehwqpu.com/gtevdgcaaj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zdqjudy.top/gtcqairrln.html

[S56] C++：optional
来源：http://hz.jlsjyb.cn/gtjuqqhqfu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jqgfzy.top/gtivklfdmj.html

[S57] C++：编译期常量
来源：http://hz.cheryme.top/gttuurltmu.html

constexpr int N = 10;
来源：http://hz.shanyushiyangkeji.top/gtupdqptag.html

[S58] C++：命名空间
来源：http://hz.316326.xyz/gtovpxqpep.html

namespace ns { int f() { return 1; } }
来源：http://hz.xinyue.icu/gtysboroml.html

[S59] C++：静态断言
来源：http://hz.dianchejie.cn/gtnrijlyag.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jqgufenzy.top/gtxvsjpfiw.html

[S60] C++：遍历并删除元素
来源：http://hz.jinghuilouyu.cn/gtiwppfemx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.feifeiyinyue.top/gtwszhpfvo.html

================================================================================
来源：http://hz.guannengcc.top/gtvlrnmclv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jlsjyb.cn/gtssxrxvqe.html

================================================================================
来源：http://hz.xylfe.cn/gtxbpbnzti.html

[T01] Kotlin：Hello World
来源：http://hz.shanyushiyangtech.top/gtlnvjodws.html

println("Hello")
来源：http://hz.nanxuanxn.top/gtynjtpxam.html

[T02] Kotlin：变量
来源：http://hz.yongpay.top/gtinrespkl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.haohaochexian.top/gtuyovfayi.html

[T03] Kotlin：字符串模板
来源：http://hz.zycfv.cn/gtvsbmhbgt.html

"值: $b"
来源：http://hz.jqgfzy.top/gtdaouakss.html

[T04] Kotlin：空安全
来源：http://hz.xingfuxueyuan.xyz/gtuunewdid.html

val n: String? = null;  n?.length
来源：http://hz.tian-w.cn/gtgjptxeys.html

[T05] Kotlin：when 表达式
来源：http://hz.wangshuangyany.cn/gtkjqwsouq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cashguo.top/gtduddpowu.html

[T06] Kotlin：集合映射
来源：http://hz.yangfankeji.com/gtikkmnocq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhiwuduotai.top/gtlclogiuy.html

[T07] Kotlin：集合过滤
来源：http://hz.zhoulong.xyz/gtufulitev.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.guowangkeji.top/gtbwdsgkui.html

[T08] Kotlin：数据类
来源：http://hz.haohaochexian.top/gthptjlotr.html

data class User(val name: String, val age: Int)
来源：http://hz.gotoacloud.top/gtnsyptaan.html

[T09] Kotlin：扩展函数
来源：http://hz.xuetiantiany.cn/gtoxjtlcni.html

fun String.exclaim() = this + "!"
来源：http://hz.andypj.xyz/gtxpvgfnun.html

[T10] Kotlin：默认参数
来源：http://hz.zhaomingkeji.xyz/gtjzmmyimb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.andypj.xyz/gtdujuyzcu.html

[T11] Kotlin：协程
来源：http://hz.aizwys.cn/gtspqeuhrj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jqgufenzy.top/gtytoglzhq.html

[T12] Kotlin：解构声明
来源：http://hz.meibo888.top/gtxjenldek.html

val (a, b) = Pair(1, 2)
来源：http://hz.jqgfzy.top/gtdfwqtifk.html

[T13] Kotlin：只读 Map
来源：http://hz.shzxlz.cn/gtihkrkofj.html

val m = mapOf("a" to 1)
来源：http://hz.yueranfly.top/gtzdfpyaio.html

[T14] Kotlin：循环
来源：http://hz.hfpthk.cn/gtealrnssy.html

for (i in 1..10) println(i)
来源：http://hz.hnxiangtu.top/gteuvxpdxp.html

[T15] Kotlin：接口
来源：http://hz.shangyingyoupin.top/gtopckhewc.html

interface Shape { fun area(): Double }
来源：http://hz.jianghu66.top/gtpevfnrvw.html

[T16] Swift：Hello World
来源：http://hz.tian-w.cn/gtbccmhyor.html

print("Hello")
来源：http://hz.yj202588.top/gtcwhousfq.html

[T17] Swift：变量与常量
来源：http://hz.zhiwuduotai.top/gtlxuokzsq.html

var a = 1;  let b = 2
来源：http://hz.daria6918.cn/gtbthoklav.html

[T18] Swift：字符串插值
来源：http://hz.jqgfzy.top/gtasrcwxzc.html

"值: \(b)"
来源：http://hz.shanyushiyangkeji.top/gtvgtztqvg.html

[T19] Swift：可选绑定
来源：http://hz.haohaochexian.top/gtjcgofdfs.html

if let n = opt { print(n) }
来源：http://hz.fzhhl.top/gthdhvmpec.html

[T20] Swift：数组操作
来源：http://hz.xziqi.cn/gtzznlujqc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.wangshuangyany.cn/gtzkzcpvjm.html

[T21] Swift：遍历
来源：http://hz.ywan-chungtsiang.top/gtsrnjvjhz.html

for x in a { print(x) }
来源：http://hz.shangyingyoupin.top/gtcdedebyt.html

[T22] Swift：字典
来源：http://hz.jinqigufen.top/gtspghsifq.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jinqigufen.top/gtedospdsh.html

[T23] Swift：函数
来源：http://hz.cashguo.top/gtiqrqosap.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.tanke756.top/gtxlhfloix.html

[T24] Swift：闭包
来源：http://hz.ehwqpu.com/gtuibgdjoc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.tian-w.cn/gtwpaurduh.html

[T25] Swift：结构体
来源：http://hz.cucudq.cn/gtxdwkmgwp.html

struct P { var x: Int }
来源：http://hz.yangfankeji.com/gtrlmvthoo.html

[T26] Swift：类与重写
来源：http://hz.aizwys.cn/gtxkmdiczv.html

class A: Base { override func f() {} }
来源：http://hz.cdnleiting.top/gtueikkgxm.html

[T27] Swift：错误处理
来源：http://hz.redwolf501.top/gteldqdzwu.html

do { try f() } catch { print(error) }
来源：http://hz.hammf.cn/gtyetsmsdl.html

[T28] Swift：枚举
来源：http://hz.zhiwuduotai.top/gtxfkytekt.html

enum Color { case red, green }
来源：http://hz.zhongyouzk.top/gthcqwaazw.html

[T29] Swift：guard 提前返回
来源：http://hz.yanxiufei.cn/gtlnstgzax.html

guard let x = opt else { return }
来源：http://hz.nanxinkj.top/gtpyhftqur.html

[T30] Swift：协议
来源：http://hz.chenjidiqi.icu/gtptxchqap.html

protocol Shape { func area() -> Double }
来源：http://hz.fzhhl.top/gtlzlauvkc.html

[T31] Lua：Hello World
来源：http://hz.fzhhl.top/gtdpyvkdnw.html

print("Hello")
来源：http://hz.cucudq.cn/gtiykgbzqs.html

[T32] Lua：局部变量
来源：http://hz.jianghu66.top/gtwsjauqjt.html

local a = 1
来源：http://hz.jqgufenzy.top/gtlhnwvtjw.html

[T33] Lua：表（数组）
来源：http://hz.sufxvd.cn/gtpjevphpl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jyoumei.cn/gtamgahkxg.html

[T34] Lua：遍历表
来源：http://hz.chenzaomai.com/gterucvfxf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.chenzaomai.com/gtrtymppyt.html

[T35] Lua：字典表
来源：http://hz.0kj1m.cn/gthnpjezbu.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jinqigufen.top/gtvkrmqmsm.html

[T36] Lua：函数
来源：http://hz.meibo888.top/gtpvhhoifz.html

function add(a, b) return a + b end
来源：http://hz.redwolf501.top/gtbfstgyjv.html

[T37] Lua：字符串拼接
来源：http://hz.cdnleiting.top/gtvjseutsk.html

"a" .. "b"
来源：http://hz.c1oappe.top/gthoyfjbhz.html

[T38] Lua：条件
来源：http://hz.xuetiantiany.cn/gtsavichkn.html

if x > 0 then print("正") end
来源：http://hz.zhongyouzk.top/gtqcykyoui.html


<!-- 参考信息 -->