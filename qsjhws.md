代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3foxwskdj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3tjgwarve.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zgidzfll.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3cftnsiie.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3keokzwvu.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ozfnjyix.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3hsdfjawb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ynzccjvr.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3vxnomznh.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3nvbmchzm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ixkusugw.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wzqgqnvl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3dljlgsmx.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vwmldnnf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3tatpdoab.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3pxiyavsk.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3llttwmac.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3exhvonvi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3rzahzftd.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3pmevqgjk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3drjvufdo.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3wmbpfclc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mmiczcnp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bdjlrblk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ahnylnum.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3yjecbhdw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3wgsyppek.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3eyphtncx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3rybcupgw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3oigvbphg.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3czukedjh.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3pvdxerwt.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3rmxlnoqg.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3yjbxydix.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3pgdsjjze.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3elqchraa.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3bseeznmm.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3sbyiqwiu.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ggbkrkee.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3vifmicau.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3mzuxifvi.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3exwafjza.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3qgheklge.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3wbsrgbsw.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3uszczoub.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3wwakvpvi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3pioinbet.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3amsiehom.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nhtogzpu.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ldzzjumc.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3woagnnql.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3drndotae.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3vvlvhmcw.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3vpkreuur.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qbyskrnv.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ogvkqnar.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3gwdqsbif.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3rvajljnh.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xpwuunrm.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3jygjjool.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3glkckjpu.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3wijdhqjt.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3alvcvbir.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3xuzjmpub.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3hddpbhxa.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xcgwyllw.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3zqegllyy.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3neesxyeo.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3zufhngpz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3smzvebys.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3vadiefcv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gmhmycpr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3wlvtvcnj.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gaeufpmf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3wzrtodqz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3rnyepmed.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3nexpxjwc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3hqifvprx.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ifyfgwtz.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3twsrilpl.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ttpfzfns.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3cmyzsces.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ydefuoyx.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3cqwztvyf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3wweppwey.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3soreqtkg.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3huqzviyw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3iluqphzz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3opmqrcbk.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3sbyuhugf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3odrrwdzr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3xfklzbnv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3vfllxqgj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3rkegukdo.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ezntkzzy.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vixsfovj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3lkzalady.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3oixxguif.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3gkntahdn.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3mjueqkwe.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ihvceowb.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3wwzsxhku.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3sbcjnmon.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ejbxgptn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3geosromd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3tapdkbcq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dsppmqzf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3pkbpobax.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3xtzdscns.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3yvxmrzwc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3vksyktzy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3fskjjoeq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3jhkgjnve.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3oukqgrjx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ilqzxsxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eogoqtke.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rnvbhfro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3levwvqvx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wgihnove.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3yrlwjwpz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3mspkfsbe.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3jpwhxtct.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3plwbacyv.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3pdxskfbg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3gdhvsrun.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ihowotws.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3aouoafmv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ktvytxrx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3glmobrxm.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3znkpurgo.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3kuxltnmb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ckfxboyu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ycmmescg.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3yqfpnwsy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3yadznzxb.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3dpiqxyca.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3lyeoukpk.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3frzqwxrk.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3irbycybw.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ivjpmatg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3tslrhmny.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ffssppmx.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ifyagsns.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3iyuoxedc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vrkdieya.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3fvakwmth.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3jdlepbfn.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3rkbfgkap.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3rxfxxnyl.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3xrhzcpuy.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3vgnfbrwb.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ytwkltyp.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kmvjaqjl.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hwoirxqh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3aapnlyuz.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3tisjcyiu.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3mdlqaaos.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3qdtsaeqv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3klimossc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3etfnpoeb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3phvqjuqd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3pklcnptl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3hnyehrza.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3yboftqma.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3vpntnzro.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3jfkjgnfo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3rspczipm.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3hqiingbm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3fsbysjzh.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3dzpynhve.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3fmwucple.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3tdergcfd.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3nhmuafsd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3jzrhpdnn.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uvtoogxs.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3wbuczqjv.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3nqypnanj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3tipfcwpn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ocxmeuvg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3krcxpbns.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zedzybls.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3huvjjdnm.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3syrsaqbs.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ebsibvek.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3jbyslfvx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3elxovcbx.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zzhorpra.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3xeuqpslz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3xgnrjnon.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3oktzredc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3myvgfdfs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgdvcbpe.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3tmfwojhb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kooavzoc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3etwfdnee.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3riozcmnx.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3aediapdp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pbumgrrq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3kdqqaaqs.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3sxaljkvx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3gqkgopkt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3rpcdeubo.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3pscacwfk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3cjbqjchx.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mcppewfg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3hbsefyoq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3xptaxked.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3gtgumadb.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3otpjbjpn.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3zdqldylq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3cegowwwl.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3oiovgcff.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3hcfnedfq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ppvjgqdv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3tqdiuqrg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3cpdrrsyq.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hugjmjir.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3biigivbz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bwyikzan.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3weqegwzb.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vfyocxdy.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3fwvvxsor.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3zyggbqem.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3mxqbqimc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gkvruzcn.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qodflqzm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3xojymnna.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3egxwjevj.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3voxnswur.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3luhmgygg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3mzeuljva.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3hljapjgd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fnyqokkn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3bighyycr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nhazbiax.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3iozlgdlp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3khxdnruv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3gucfcynb.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3xwksiynp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3mecfbbny.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fhbcuhzi.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3qmybewwy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ymrovblr.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3cqzbmjvi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3analoijo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3laoxzejj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3wnnidlxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3riokdvng.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jwohpsyc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jpokbvuv.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jdwdttbd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3hidgkipb.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3uubhxtgg.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kmeyhoeg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ygkyelbj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3vpoweoew.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sgzmnptr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3xzdqjtap.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3enjxtvik.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yfedxexd.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3galkbujy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3vuyniqaf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3fmxebszn.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3hwvektdq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3oeuyozvy.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3psubwenf.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3svaggggs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3yaukmpcr.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3eyplrcef.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3febtbdvu.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3yrbglptv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3carmcmlm.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3apgeirbr.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3guytkkee.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zusufudg.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3rxmqowzj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3zfcnacgk.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3tukpufft.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3edjjqmvq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3eruwhmjz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3pvsrybuc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kysspvwk.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ovkxuvhu.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3cfdbyaeu.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vphusdvh.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3sehcoxkq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3iewhgvco.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3kncriyoq.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3cdwdpwjh.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3zmpnkqxl.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3phkstbbu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3iylhglqy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3uunlnfhw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yfphmulu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3wmzniozm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xxrvhvtd.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3kzcpcbtw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3sfjsuajp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3dypoyirh.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3jucqhpss.html


<!-- 参考信息 -->