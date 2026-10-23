代发 wailian999

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3xznszqfp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ivhcinxq.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3afxljwwk.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3nlrisesv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ilyiubst.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3bpkdifct.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3clfryamh.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3pjedllqt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3lbbdeffb.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ajqcfzgb.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3smkseiwt.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3xbeorvao.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ighzuwpz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3alycerxw.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3hdfhruek.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3fpwikaot.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ypdhbmar.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3rszssaoq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3udqwpkrk.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ftozmiax.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ozgplqal.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ddrybywc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dzzwjegq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3kkoqroqh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3mmayektk.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3crixlwwh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hvrdrxbx.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3tgwtkjpm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ihftnbxb.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3rtorkotx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3rumkdoff.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3yfyhsqnz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3wxqgxlyk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3hkrnahhg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3asveylbn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3yeqzshea.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3dykpteyx.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3yzceagmy.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3dvlawrgk.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3itzvzhon.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ocolvajm.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3vczvnemm.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3imyhsnrc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3hdcrkgpm.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3niccufbe.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3dzvxpkmd.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ivrnqtps.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3kyqnnusu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3rrclmigg.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3oyirvoro.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3klmityjq.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3wdwbuyrk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nseeeibo.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3rlbuvwba.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3spumrdlh.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3vjpeaanw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3neyronoq.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3whnkjned.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wunwlouj.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3gmkwooev.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3rufxixje.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3nrwuuxbs.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3joshhzmd.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3bbjnrpid.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3tfyqfcbx.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3yvpfbqpp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zgfjndje.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ttufyjoz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3lxaqriat.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3icgyyvfe.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3vxkdoawc.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3puvoiepe.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3jpvbjauk.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3yfafemyd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3lyzooscx.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3elgfggxm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3sekewqel.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3trfryapu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3jwwikuoh.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3fumsyvfe.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3sklnnicj.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3kromdwhw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3bcolyhbi.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3cihqytst.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3buahwkgs.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3fawttdnj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3kndrudpi.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3qruvwgxw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3stprbumq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3dfgjufvi.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3vorrvaxi.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3mzgpapyn.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3xvddavyk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3oqnrhxcw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nxrtnlcs.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3jezyqmgt.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3cbmimzso.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3fxfbuzmc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3tnywxesc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fowrazaf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3bciwiowe.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3kdoajcvd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3mauozfud.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3jlccfxdu.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3plvvidqf.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ixwyiwox.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ffkjbanc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ccvdxxwp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3igtvnqul.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3eesoazuh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3geursldi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3hzbgmmqo.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3nzygvakf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ynahbxjm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3mpwevnhu.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3hgepftbp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3cxrkrawd.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3dpkzuxab.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3bacmxxlr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cfqtwojt.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3posjmzoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wgzcgguz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ugmccwog.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3nqosiusr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3txbwmdnw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3vhefldmy.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3deevtgze.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3wcbnhqbs.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3vrxjonst.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3whucpdtz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pcfydgas.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zfufrsiz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wqljidce.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3yclboywj.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3qmdcgtzt.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3mpesjgah.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3wmniostf.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3jrrhygdr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3lrytjcrw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3dnlvclaf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3eoopdaxi.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3umirypyy.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3padabgvf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kjkyemkv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3zffreuyq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ansnyqdl.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3fpjsngey.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ymwepxph.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ctmwangg.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3cgymoupv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3qttzlcmc.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3utnluuyg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3vlvxsesb.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3lumrxyeq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ckugtnso.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3jmowwzxi.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3kfmmnbjf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bbkeiitk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3mqnotdny.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ykpohuzc.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3bgnvnqjd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3mwisbgej.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3oarcjlbf.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3cfzywcqr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jdspekec.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3hjjpqjsa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3qpiaxcwj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ronvdvfh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ebbschta.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ihwudoyl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3rdwvoxey.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ffvyhahz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3dcrhlxzp.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3kpjonroi.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3rzlpgjvv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3vfzgdxhw.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3kcewkken.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3fsfptzdo.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xhwcvwpn.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3xvhzdctx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3tiwmfhsw.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3pundpsju.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3hrglwqor.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3wfzprioz.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3zmqqhoob.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3czacyzjn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3rcyyjqeb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sjmflbrt.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3terbshmx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3thslldvq.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ricgppxt.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3coqybizl.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3maskpuhh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tzpogmpp.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3nlbcxpss.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqjstnfr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3jqcremxh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ptkajlyy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3akcerycf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iltqlnrq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3lnsyitwh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3mbtrqsee.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ifnxdqhw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ddmaegoj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3fngolugy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3tbbvcygu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3wyvmqesa.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3izmnodph.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3sxhqvehn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3uqtscjvo.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3pbfqubyc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3kglnvsfs.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3irvlmjso.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3iafdlrpp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3joctyptv.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3pctzunxs.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3psnogyls.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3kkygsswz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3dxywagln.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3jjuktivf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3zpyccdds.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnpaystw.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ixutzymn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3mjmmfons.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ncamguep.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3psdhfmoj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3vprxswez.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3iunvscjx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rdgnkngx.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3cbdpegam.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3bgawcraa.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3esjnzcoi.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ufpaihvd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3enfdixni.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3wxxmtomt.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3tprqdtfy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3onyrirbt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3creyiigw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3wqygxysr.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3movmlunx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ckofetkg.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3dplgpcth.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3lqrcsgcn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3gqlonstr.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3siqmkpnm.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3bzlhzuwh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3liwmmldz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3njmpjlgc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3yunfsnrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ncrhghmk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xqalvlvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jsiysamr.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3npoduluk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pqdsyjik.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3rknmwymc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ywzqhomq.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3rlftfirm.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3daqoeocn.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3btcpdiae.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3lxzttslo.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3nnuveolc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3xcjwbxhl.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3rxtdczpp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3oobwzrll.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3rqxlqako.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3canrpito.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3bgcxbvzi.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3plldqroa.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3sclqnvhd.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3veioedfv.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3gnbfpsaq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3kioalvys.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3ftseimbj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3jwpljgqy.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3zylwqyog.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3acmvoojf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3tztlreya.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3imnewmod.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zulqjyau.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nkwbtjtk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3tkepemkp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ncaksyxg.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mzkzluit.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vhakplbq.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3xjmhuqnj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rxqinuvt.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3urzehgmd.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ihtkuhbu.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3lzssftfm.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3otvdbnwv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ufiziopj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3duuavsgm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3habxdieu.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3mlybajuj.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3fyeepzkr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zelqphlg.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3nbkgjclv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3wwacrybk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zuwmyfpj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fxbleqei.html


<!-- 参考信息 -->